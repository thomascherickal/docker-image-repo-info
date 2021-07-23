## `golang:1-buster`

```console
$ docker pull golang@sha256:4ff67e6e860bd4bf09aa3c66dad45db6a624fccc8172a30ae7e983938fd4c6d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `golang:1-buster` - linux; amd64

```console
$ docker pull golang@sha256:60d87036a5ef3cd02b3a7acf1dce82071716a84e03e94ee0b544e566e14a2aef
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.9 MB (317908035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:028d102f774acfd5d9a17d60dc321add40bea5cc6f06e0a84fd3aca1bb4c2b12`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 01:12:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:01:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:01:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 02:02:35 GMT
ENV GOLANG_VERSION=1.16.6
# Fri, 23 Jul 2021 02:02:50 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.16.6.linux-amd64.tar.gz'; 			sha256='be333ef18b3016e9d7cb7b1ff1fdb0cac800ca0be4cf2290fe613b3d069dfe0d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.16.6.linux-armv6l.tar.gz'; 			sha256='b1ca342e81897da3f25da4e75ae29b267db1674fe7222d9bfc4c666bcf6fce69'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.16.6.linux-arm64.tar.gz'; 			sha256='9e38047463da6daecab9017cd0599f33f84991e68263752cfab49253bbc98c30'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.16.6.linux-386.tar.gz'; 			sha256='33d028b6d2a4abeb74cccd55024500ae49d5edfb08a30665db0b49cd1052c37e'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.16.6.linux-ppc64le.tar.gz'; 			sha256='62b5e9bb9440b7166241e5b7d5f49c7372b36429c8308a8456ee46fc1397a0fe'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.16.6.linux-s390x.tar.gz'; 			sha256='f07de592165539b3e9fbc6d067affea930b33d54cff5b5d3630d82b8682d3c3f'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 		sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Fri, 23 Jul 2021 02:02:51 GMT
ENV GOPATH=/go
# Fri, 23 Jul 2021 02:02:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 02:02:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 23 Jul 2021 02:02:52 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf76209566d0c8d78df205b09e6e5b52ff7f10cb4e1c03d9336ed7dd2decd919`  
		Last Modified: Thu, 22 Jul 2021 01:20:16 GMT  
		Size: 51.8 MB (51841203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6182a456504bb119011b721ede5d1e6cf4d0621447465d80cc1d4e53c0ef95e6`  
		Last Modified: Fri, 23 Jul 2021 02:05:30 GMT  
		Size: 68.7 MB (68749967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc29a487638239fd8dbd95edec35e479575d7da115cd3e7ce6d107766384980a`  
		Last Modified: Fri, 23 Jul 2021 02:06:58 GMT  
		Size: 129.1 MB (129050918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff36ba4656980ea99a067c8a9b39f210a4da82badccaa2bae27317e711985668`  
		Last Modified: Fri, 23 Jul 2021 02:06:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm variant v5

```console
$ docker pull golang@sha256:d06714cbbc9812e0a44bf5714770ac5a2fb0b029d75143d4c60d738c9bea6378
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.4 MB (269403515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acb4e173d352b747621b0c902f246f90cc831593a03e18114f766be2c4c64355`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:49:34 GMT
ADD file:4a4158b5432e31cd686b7b2874c22d86a381ac71c3146fe6746501db3d216b41 in / 
# Thu, 22 Jul 2021 00:49:35 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:03:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 02:03:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 02:04:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 16:11:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 16:11:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 16:15:28 GMT
ENV GOLANG_VERSION=1.16.6
# Thu, 22 Jul 2021 16:18:28 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.16.6.linux-amd64.tar.gz'; 			sha256='be333ef18b3016e9d7cb7b1ff1fdb0cac800ca0be4cf2290fe613b3d069dfe0d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.16.6.linux-armv6l.tar.gz'; 			sha256='b1ca342e81897da3f25da4e75ae29b267db1674fe7222d9bfc4c666bcf6fce69'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.16.6.linux-arm64.tar.gz'; 			sha256='9e38047463da6daecab9017cd0599f33f84991e68263752cfab49253bbc98c30'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.16.6.linux-386.tar.gz'; 			sha256='33d028b6d2a4abeb74cccd55024500ae49d5edfb08a30665db0b49cd1052c37e'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.16.6.linux-ppc64le.tar.gz'; 			sha256='62b5e9bb9440b7166241e5b7d5f49c7372b36429c8308a8456ee46fc1397a0fe'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.16.6.linux-s390x.tar.gz'; 			sha256='f07de592165539b3e9fbc6d067affea930b33d54cff5b5d3630d82b8682d3c3f'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 		sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 22 Jul 2021 16:18:30 GMT
ENV GOPATH=/go
# Thu, 22 Jul 2021 16:18:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 16:18:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Jul 2021 16:18:33 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:cd9bc325fb9e2673d4a4f97499e5ac67f82d24eef19ed2cb8d13af9c9256d20c`  
		Last Modified: Thu, 22 Jul 2021 01:01:22 GMT  
		Size: 48.2 MB (48153246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ac5ad14f3066e98bd031f59bcd25af51c46975f1f67aa9e984aae49997f855`  
		Last Modified: Thu, 22 Jul 2021 02:21:02 GMT  
		Size: 7.4 MB (7376533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3538b6814e6bbc64643ef42ffb80c592cecc6833f8c77baa213b7d572de2f060`  
		Last Modified: Thu, 22 Jul 2021 02:21:02 GMT  
		Size: 9.7 MB (9687577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98fc7d7506f4cd2a0d1ab64ad0e0a5e9863175a5bcadf61c19a25091d861d34`  
		Last Modified: Thu, 22 Jul 2021 02:21:56 GMT  
		Size: 49.6 MB (49575389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0603fa664f95d8074de109c383370a08008de46caf8d285bdc49edb42461b128`  
		Last Modified: Thu, 22 Jul 2021 16:23:47 GMT  
		Size: 52.1 MB (52056868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68302f1b133e5efe4858e61ebb06f83af90aa9fb8c281838c0b1be00d9a05c62`  
		Last Modified: Thu, 22 Jul 2021 16:25:34 GMT  
		Size: 102.6 MB (102553746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2228a31e2bde73fc7e42406509211f508e5b94aea152d4e25c435ccbb38a5d9`  
		Last Modified: Thu, 22 Jul 2021 16:24:27 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm variant v7

```console
$ docker pull golang@sha256:b697bf37e05703bf9734528d193c1e5a42e186867c3c031e44f275db31f1dbb4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.2 MB (263246829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00df7a502309d1461884428b75fe2b367bfe68fd8ec37371d847088e6de1f2a2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:01 GMT
ADD file:3edc1a2322b55593b3cd8e935ca6d837e7618bcaaab27a09c9822728f8272ce0 in / 
# Wed, 23 Jun 2021 00:20:02 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:46:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:46:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 05:47:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 17:35:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 17:35:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 06:03:01 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 06:03:36 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.16.6.linux-amd64.tar.gz'; 			sha256='be333ef18b3016e9d7cb7b1ff1fdb0cac800ca0be4cf2290fe613b3d069dfe0d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.16.6.linux-armv6l.tar.gz'; 			sha256='b1ca342e81897da3f25da4e75ae29b267db1674fe7222d9bfc4c666bcf6fce69'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.16.6.linux-arm64.tar.gz'; 			sha256='9e38047463da6daecab9017cd0599f33f84991e68263752cfab49253bbc98c30'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.16.6.linux-386.tar.gz'; 			sha256='33d028b6d2a4abeb74cccd55024500ae49d5edfb08a30665db0b49cd1052c37e'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.16.6.linux-ppc64le.tar.gz'; 			sha256='62b5e9bb9440b7166241e5b7d5f49c7372b36429c8308a8456ee46fc1397a0fe'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.16.6.linux-s390x.tar.gz'; 			sha256='f07de592165539b3e9fbc6d067affea930b33d54cff5b5d3630d82b8682d3c3f'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 		sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 13 Jul 2021 06:03:38 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 06:03:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 06:03:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 06:03:41 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:a3ac2852d9d20585eb4d19973a45b69522d16832456ea5b52f0298b2937afc09`  
		Last Modified: Wed, 23 Jun 2021 00:31:04 GMT  
		Size: 45.9 MB (45917482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d59952ec0a1da3155a9d9a84f07fc99163c3b5429cae2d6d37e9de664191d9d`  
		Last Modified: Wed, 23 Jun 2021 06:18:36 GMT  
		Size: 7.1 MB (7124226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac8017b9330d1a833e533de62b0525c9033b03c74f0d5c3b28b478231b03803`  
		Last Modified: Wed, 23 Jun 2021 06:18:37 GMT  
		Size: 9.3 MB (9343805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e065f215c483cb5ee70970d3a4708cdce964e110f4d6e1c6f19ff783e71842fb`  
		Last Modified: Wed, 23 Jun 2021 06:19:26 GMT  
		Size: 47.4 MB (47357244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c88433545097560ca93a4ae36d8df5d579b3c96306ad2ec247ebfee64b9c6dc`  
		Last Modified: Thu, 24 Jun 2021 17:56:15 GMT  
		Size: 53.2 MB (53222568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a62336912364cf0cd59510d4a118b97f7e47e47873412ccc4a58a1f1e11fd7`  
		Last Modified: Tue, 13 Jul 2021 06:28:04 GMT  
		Size: 100.3 MB (100281348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e024f18d76793870b61cb20d8ee744797d287ef0c5bad0c6dd214045bf020963`  
		Last Modified: Tue, 13 Jul 2021 06:26:56 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:0ac15cdd282b5a0552c54f61ebb609bd2a4e64007e6de9cb198bad2a8a36a6b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.3 MB (281311379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fab6a1960e25c07b81544cad9507a35768eb4271db31d8355add99a8fa002758`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:59 GMT
ADD file:3e8e075f08a6b727602af05c539f43648a48663cbb3a88eeba310cfc32c01d78 in / 
# Thu, 22 Jul 2021 00:40:00 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:15:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:16:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 01:16:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:32:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:32:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:33:17 GMT
ENV GOLANG_VERSION=1.16.6
# Thu, 22 Jul 2021 13:33:25 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.16.6.linux-amd64.tar.gz'; 			sha256='be333ef18b3016e9d7cb7b1ff1fdb0cac800ca0be4cf2290fe613b3d069dfe0d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.16.6.linux-armv6l.tar.gz'; 			sha256='b1ca342e81897da3f25da4e75ae29b267db1674fe7222d9bfc4c666bcf6fce69'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.16.6.linux-arm64.tar.gz'; 			sha256='9e38047463da6daecab9017cd0599f33f84991e68263752cfab49253bbc98c30'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.16.6.linux-386.tar.gz'; 			sha256='33d028b6d2a4abeb74cccd55024500ae49d5edfb08a30665db0b49cd1052c37e'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.16.6.linux-ppc64le.tar.gz'; 			sha256='62b5e9bb9440b7166241e5b7d5f49c7372b36429c8308a8456ee46fc1397a0fe'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.16.6.linux-s390x.tar.gz'; 			sha256='f07de592165539b3e9fbc6d067affea930b33d54cff5b5d3630d82b8682d3c3f'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 		sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 22 Jul 2021 13:33:26 GMT
ENV GOPATH=/go
# Thu, 22 Jul 2021 13:33:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:33:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Jul 2021 13:33:27 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:d272b0d8f7c4fd0caf0ef022ce544cfe3800e349a73b585f82837e6526a4247e`  
		Last Modified: Thu, 22 Jul 2021 00:45:18 GMT  
		Size: 49.2 MB (49222109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fabd82f026fa10e0e0341fa3d6d3112de04413ea6c46e72bcc1dca40d924aa`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 7.7 MB (7694906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0193c0cdceae23cd0e13721651d74f409440171fe8a1c8b521616b6ed29db6e1`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 10.0 MB (9984335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967a8f1385966af47c9f250997e3158c319d498adc004c91570f770ceac5045a`  
		Last Modified: Thu, 22 Jul 2021 01:25:24 GMT  
		Size: 52.2 MB (52167528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f10b34911491399aa2caeb545e897b4fd44568636b77f650887a40f2e08e4e1`  
		Last Modified: Thu, 22 Jul 2021 13:36:49 GMT  
		Size: 62.6 MB (62616191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fbd834000c96d1474c9ee97c2deec7e76ac0ca6e3534c5304a47fdbdc41133`  
		Last Modified: Thu, 22 Jul 2021 13:38:06 GMT  
		Size: 99.6 MB (99626155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3745b9acab91baf35f9796791de76f7107e828789d6587afc76de73c9887cdd0`  
		Last Modified: Thu, 22 Jul 2021 13:37:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; 386

```console
$ docker pull golang@sha256:0cc7239c49d17a892fd1469620868ab5028fec00d9aa9789599832b8858f8e4d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.7 MB (299699008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44ff1fdf29723ba63086e8b805f590c27956ddf7fdead325675760d57f3e5920`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:33 GMT
ADD file:574afb2f0b9121fa552563f323a2edd9a3aa71fc927a280c3eb9cbbf944a12ff in / 
# Thu, 22 Jul 2021 00:39:34 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:05:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:05:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 04:05:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 17:28:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 17:28:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 17:29:26 GMT
ENV GOLANG_VERSION=1.16.6
# Thu, 22 Jul 2021 17:29:49 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.16.6.linux-amd64.tar.gz'; 			sha256='be333ef18b3016e9d7cb7b1ff1fdb0cac800ca0be4cf2290fe613b3d069dfe0d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.16.6.linux-armv6l.tar.gz'; 			sha256='b1ca342e81897da3f25da4e75ae29b267db1674fe7222d9bfc4c666bcf6fce69'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.16.6.linux-arm64.tar.gz'; 			sha256='9e38047463da6daecab9017cd0599f33f84991e68263752cfab49253bbc98c30'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.16.6.linux-386.tar.gz'; 			sha256='33d028b6d2a4abeb74cccd55024500ae49d5edfb08a30665db0b49cd1052c37e'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.16.6.linux-ppc64le.tar.gz'; 			sha256='62b5e9bb9440b7166241e5b7d5f49c7372b36429c8308a8456ee46fc1397a0fe'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.16.6.linux-s390x.tar.gz'; 			sha256='f07de592165539b3e9fbc6d067affea930b33d54cff5b5d3630d82b8682d3c3f'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 		sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 22 Jul 2021 17:29:50 GMT
ENV GOPATH=/go
# Thu, 22 Jul 2021 17:29:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 17:29:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Jul 2021 17:29:53 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:276c935c592dc1b2a80709bfb684b8cadd019d62fed321da14653e74bc260bd2`  
		Last Modified: Thu, 22 Jul 2021 00:45:59 GMT  
		Size: 51.2 MB (51206749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74777b942e5ddcca1441a21360061ce9f880ebd5f5020bd1f8480c09ec3c9a1`  
		Last Modified: Thu, 22 Jul 2021 04:15:32 GMT  
		Size: 8.0 MB (7998524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f821b4d53bda0dd46941c09587233f0b5d34c76bd3efb4d2d0766dddea8f99`  
		Last Modified: Thu, 22 Jul 2021 04:15:33 GMT  
		Size: 10.3 MB (10339898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b349e22a93ae2ec7a8fb4830b9b80b272c758fbff384a0410f5c834c9c26a681`  
		Last Modified: Thu, 22 Jul 2021 04:16:00 GMT  
		Size: 53.4 MB (53437923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479946c45602f49688fd89ae011dcae1ef8315e2d84dc6e4c3e2df15ea1f2534`  
		Last Modified: Thu, 22 Jul 2021 17:34:54 GMT  
		Size: 73.6 MB (73617644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea7d952b14bc06f68bd26906f96e7e7ee9858137ba0842d4537e433d672ffe2`  
		Last Modified: Thu, 22 Jul 2021 17:37:02 GMT  
		Size: 103.1 MB (103098113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2856e89c1151ca86a82bba24d56a2803e7a99840f6873d07cc2dff7dd67fd56`  
		Last Modified: Thu, 22 Jul 2021 17:36:43 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; mips64le

```console
$ docker pull golang@sha256:b0918c322750851e4356f3483e6af0b6a3204b77c95c36e2468f27c6992b43c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.5 MB (271471405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76da0e8bb77a621090f7e9427e1ac9d61067aa97ddd0e6d3fbb4237a19e6c4c5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:09:22 GMT
ADD file:1a6aa3d9fc5224e35958d4109d5bcb3afa5948beb85e45b91f46655fe8fadb2f in / 
# Thu, 22 Jul 2021 00:09:23 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:42:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 00:42:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 00:43:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 18:36:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 18:36:27 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 18:46:23 GMT
ENV GOLANG_VERSION=1.16.6
# Thu, 22 Jul 2021 18:54:16 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.16.6.linux-amd64.tar.gz'; 			sha256='be333ef18b3016e9d7cb7b1ff1fdb0cac800ca0be4cf2290fe613b3d069dfe0d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.16.6.linux-armv6l.tar.gz'; 			sha256='b1ca342e81897da3f25da4e75ae29b267db1674fe7222d9bfc4c666bcf6fce69'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.16.6.linux-arm64.tar.gz'; 			sha256='9e38047463da6daecab9017cd0599f33f84991e68263752cfab49253bbc98c30'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.16.6.linux-386.tar.gz'; 			sha256='33d028b6d2a4abeb74cccd55024500ae49d5edfb08a30665db0b49cd1052c37e'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.16.6.linux-ppc64le.tar.gz'; 			sha256='62b5e9bb9440b7166241e5b7d5f49c7372b36429c8308a8456ee46fc1397a0fe'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.16.6.linux-s390x.tar.gz'; 			sha256='f07de592165539b3e9fbc6d067affea930b33d54cff5b5d3630d82b8682d3c3f'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 		sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 22 Jul 2021 18:54:18 GMT
ENV GOPATH=/go
# Thu, 22 Jul 2021 18:54:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 18:54:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Jul 2021 18:54:21 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:dfc6cf8967b24f7ad8c4469c3140cf3967000ae27e3b40b7c72fb89755953841`  
		Last Modified: Thu, 22 Jul 2021 00:15:25 GMT  
		Size: 49.1 MB (49080577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c97f1ec44468b6cf3c95775fd68ad34176e3f3f5b114e01ef45fda232435a0ee`  
		Last Modified: Thu, 22 Jul 2021 00:54:11 GMT  
		Size: 7.3 MB (7252390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5a98fef30417ecbf0d84d2f4e0a5d8c4c745505f4453d9d128eaabe85f0caa`  
		Last Modified: Thu, 22 Jul 2021 00:54:11 GMT  
		Size: 10.0 MB (10016296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d36b0ec1b127ef255da5d2ac89935eebf1177a48ee713fa2c190f0357961a9c`  
		Last Modified: Thu, 22 Jul 2021 00:55:01 GMT  
		Size: 50.8 MB (50844871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4efd8c3e0917726909d66a1120a3edfe62a1786d35c564dec6a6af02454cda92`  
		Last Modified: Thu, 22 Jul 2021 19:03:17 GMT  
		Size: 54.7 MB (54668722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc7ec6b033fef303cf2a5c49c89e7eaebc327caf11431be8fc5329568b1a08e`  
		Last Modified: Thu, 22 Jul 2021 19:05:10 GMT  
		Size: 99.6 MB (99608423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e330bf3a3ee0f771fd816baf7530a73af5414b0642ec07c8059e96ab6232b638`  
		Last Modified: Thu, 22 Jul 2021 19:04:02 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; ppc64le

```console
$ docker pull golang@sha256:0e0d355f168850cfc3d7cdb13a347bf0e019f8a8c4acbddf79fb3745b7a7893a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.4 MB (302391597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5aff0a200ab3d854ef86104d305f1bf1844074675ae51c0a12b2097598998d8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Jul 2021 15:57:37 GMT
ADD file:b73f8d66b8be6103349949991124c7d82e38589b2db6212e920cb3b6d5ceefef in / 
# Fri, 09 Jul 2021 15:57:40 GMT
CMD ["bash"]
# Sat, 10 Jul 2021 06:21:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Jul 2021 06:22:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Jul 2021 06:25:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 11 Jul 2021 04:34:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Sun, 11 Jul 2021 04:34:37 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 02:38:01 GMT
ENV GOLANG_VERSION=1.16.6
# Tue, 13 Jul 2021 02:38:53 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.16.6.linux-amd64.tar.gz'; 			sha256='be333ef18b3016e9d7cb7b1ff1fdb0cac800ca0be4cf2290fe613b3d069dfe0d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.16.6.linux-armv6l.tar.gz'; 			sha256='b1ca342e81897da3f25da4e75ae29b267db1674fe7222d9bfc4c666bcf6fce69'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.16.6.linux-arm64.tar.gz'; 			sha256='9e38047463da6daecab9017cd0599f33f84991e68263752cfab49253bbc98c30'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.16.6.linux-386.tar.gz'; 			sha256='33d028b6d2a4abeb74cccd55024500ae49d5edfb08a30665db0b49cd1052c37e'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.16.6.linux-ppc64le.tar.gz'; 			sha256='62b5e9bb9440b7166241e5b7d5f49c7372b36429c8308a8456ee46fc1397a0fe'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.16.6.linux-s390x.tar.gz'; 			sha256='f07de592165539b3e9fbc6d067affea930b33d54cff5b5d3630d82b8682d3c3f'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 		sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Tue, 13 Jul 2021 02:39:06 GMT
ENV GOPATH=/go
# Tue, 13 Jul 2021 02:39:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jul 2021 02:39:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 13 Jul 2021 02:39:29 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:83f72610ec8bc58c0c3a70f0bdf9d866e8d0156845a9aa24bc0ed2fdaf0fd8b4`  
		Last Modified: Wed, 23 Jun 2021 00:36:35 GMT  
		Size: 54.2 MB (54182463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ba02bc6289674c1f1edb2ead79c9223d07b7bbb36fbf1ad389ee06ea3cb2fa`  
		Last Modified: Sat, 10 Jul 2021 07:06:15 GMT  
		Size: 8.3 MB (8271883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6dd9fe5e0862c666475fcf95f93e2e378b2463bf5bc4da89adc0d524db7b85`  
		Last Modified: Sat, 10 Jul 2021 07:06:15 GMT  
		Size: 10.7 MB (10727750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616ea7685f787e68800f7e4498c98c228e037fd71fc274a2a23d5efd0274d00f`  
		Last Modified: Sat, 10 Jul 2021 07:06:47 GMT  
		Size: 57.5 MB (57457148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f358e08bf439d0c96d303f551d53f3635d578c74afc7201b78eb3da8937300`  
		Last Modified: Sun, 11 Jul 2021 04:48:01 GMT  
		Size: 73.7 MB (73659977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bd00db6852e0fe75eab112e92252847dfe2a318825241bfea71a81b410c825`  
		Last Modified: Tue, 13 Jul 2021 02:54:12 GMT  
		Size: 98.1 MB (98092221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9d4efe4b0bb126cd5759e0a3f4e6264e4644c42255f479dd30af7e901909f5`  
		Last Modified: Tue, 13 Jul 2021 02:53:53 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-buster` - linux; s390x

```console
$ docker pull golang@sha256:4516c60e1ec5e24ef54f299c1eb711c9d0f49213e7bcd740e5cd261181a3653b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.7 MB (277742420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dd4a74aec0e69dc61dfd30ab55720c6a04e61c18260bf9f0ccc02b6a7854b6b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:21 GMT
ADD file:0862dc2e420958057c0edfbacc39968850751ffdec84962ab8577b7787c5296f in / 
# Thu, 22 Jul 2021 00:42:26 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:11:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:11:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 01:12:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 21:21:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 21:21:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 21:23:37 GMT
ENV GOLANG_VERSION=1.16.6
# Thu, 22 Jul 2021 21:23:56 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.16.6.linux-amd64.tar.gz'; 			sha256='be333ef18b3016e9d7cb7b1ff1fdb0cac800ca0be4cf2290fe613b3d069dfe0d'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.16.6.linux-armv6l.tar.gz'; 			sha256='b1ca342e81897da3f25da4e75ae29b267db1674fe7222d9bfc4c666bcf6fce69'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.16.6.linux-arm64.tar.gz'; 			sha256='9e38047463da6daecab9017cd0599f33f84991e68263752cfab49253bbc98c30'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.16.6.linux-386.tar.gz'; 			sha256='33d028b6d2a4abeb74cccd55024500ae49d5edfb08a30665db0b49cd1052c37e'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.16.6.linux-ppc64le.tar.gz'; 			sha256='62b5e9bb9440b7166241e5b7d5f49c7372b36429c8308a8456ee46fc1397a0fe'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.16.6.linux-s390x.tar.gz'; 			sha256='f07de592165539b3e9fbc6d067affea930b33d54cff5b5d3630d82b8682d3c3f'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.16.6.src.tar.gz'; 		sha256='a3a5d4bc401b51db065e4f93b523347a4d343ae0c0b08a65c3423b05a138037d'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 22 Jul 2021 21:24:01 GMT
ENV GOPATH=/go
# Thu, 22 Jul 2021 21:24:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 21:24:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 22 Jul 2021 21:24:03 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:8776c37054ddd28ba8fe526b8dbc08bf7b521ae9ddb8eacd008d05185571cde0`  
		Last Modified: Thu, 22 Jul 2021 00:47:50 GMT  
		Size: 49.0 MB (49003783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c06f635d71fe906f56e25278d5659aa940f095c1ecf199e41436e197534383a`  
		Last Modified: Thu, 22 Jul 2021 01:27:40 GMT  
		Size: 7.4 MB (7400582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f57129f34059279bed7373d2b35f16c94df2418b85c5ae20dc715f2e1999498`  
		Last Modified: Thu, 22 Jul 2021 01:27:41 GMT  
		Size: 9.9 MB (9883324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f6521600d1dbe8e9e84511427b15a7cb2dd42039504bb9679b6ed7e7ee0dca`  
		Last Modified: Thu, 22 Jul 2021 01:28:00 GMT  
		Size: 51.4 MB (51380867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1228c41a068ba9c3aca67ff810dadc0c8a62694a090ea82e610e8728cfbbb031`  
		Last Modified: Thu, 22 Jul 2021 21:28:50 GMT  
		Size: 56.8 MB (56817857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ba4fcbcd4e630855e817bd37651f8d004d7a51fcb8775a4168cfb48efef18d`  
		Last Modified: Thu, 22 Jul 2021 21:29:22 GMT  
		Size: 103.3 MB (103255850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692381f36adecab2f5d947fd7dc35a5b0bc6441d68017bc04f49ee39ae890193`  
		Last Modified: Thu, 22 Jul 2021 21:29:09 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
