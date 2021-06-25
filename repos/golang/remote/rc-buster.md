## `golang:rc-buster`

```console
$ docker pull golang@sha256:2a421895b1ab160983a23da98a4f3760bfdf37606d48ee4b67391de84dfbba76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `golang:rc-buster` - linux; amd64

```console
$ docker pull golang@sha256:c26ec125649d0bdeb0510a5cb21f7ae8d2d701eb37b36c1728e92c3cc27f7993
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.3 MB (323327614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52ab75730fc871b2603f201fbb5020bf32523b8c67780843ca2238c3a7666fb5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:25 GMT
ADD file:a232795a746e5842d1a864a00462be6bd86543aeed8d06d2830dd955a4c1b3fc in / 
# Wed, 23 Jun 2021 00:20:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:52:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:53:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:53:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 00:29:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 00:29:13 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 00:29:14 GMT
ENV GOLANG_VERSION=1.17beta1
# Thu, 24 Jun 2021 00:29:26 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.17beta1.linux-amd64.tar.gz'; 			sha256='a479681705b65971f9db079bfce53c4393bfa241d952eb09de88fb40677d3c4c'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17beta1.linux-armv6l.tar.gz'; 			sha256='f4ab69c75a1f9e43b07ca9a0bfdf68ca1e2b0b51d4ebfb8c79f60ed14629f4e6'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17beta1.linux-arm64.tar.gz'; 			sha256='ede56f79c5061146929ab4a128e8ee7bc713d141e87b3df4e0aa670938e128b3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17beta1.linux-386.tar.gz'; 			sha256='cebbf75985ba7e6f1a5b137916a6019685d52ecf36c262092ffc3f714cd85974'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17beta1.linux-ppc64le.tar.gz'; 			sha256='0a6e5034fcbd4b38642b56841a042135aec1e87f61258d2d70aafc0a667bdd11'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17beta1.linux-s390x.tar.gz'; 			sha256='3501d139a9433775001730f1d9c3fb60d7b93b969fe16bd80fc7387a3d5259b1'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17beta1.src.tar.gz'; 		sha256='02b8973725f9bc545955865576e8c8f6ca672312f69fd9e5549c25b0ce1d75f0'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 24 Jun 2021 00:29:27 GMT
ENV GOPATH=/go
# Thu, 24 Jun 2021 00:29:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 00:29:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 24 Jun 2021 00:29:29 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:0bc3020d05f1e08b41f1c5d54650a157b1690cde7fedb1fafbc9cda70ee2ec5c`  
		Last Modified: Wed, 23 Jun 2021 00:25:08 GMT  
		Size: 50.4 MB (50435617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a110e58716600c199fc95f633b30735c33a25b5adcfb16d1d7edbcb78a3f1b62`  
		Last Modified: Wed, 23 Jun 2021 01:01:46 GMT  
		Size: 7.8 MB (7832997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d3c0fa203acbade733bff627daa75b84c97f9d0553bcdf967a3f1d37471277`  
		Last Modified: Wed, 23 Jun 2021 01:01:47 GMT  
		Size: 10.0 MB (9997255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fd09c11b021b756b7a92a4f70a3d444ce7e63a1c24e5749d236dc2c6e68514`  
		Last Modified: Wed, 23 Jun 2021 01:02:12 GMT  
		Size: 51.8 MB (51841560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78287c648ba24843d09e43253bb28f9020904cf5874e292918bba071c6c42564`  
		Last Modified: Thu, 24 Jun 2021 00:34:11 GMT  
		Size: 68.7 MB (68749808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44c5933c431e13e6e336b95d5de62ce390c606b00f574ccb92dbe61f8f8c6f0`  
		Last Modified: Thu, 24 Jun 2021 00:34:22 GMT  
		Size: 134.5 MB (134470222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ddbc615b742d94c22900f9a7768628648cf7b074623864029fa0731b35664c3`  
		Last Modified: Thu, 24 Jun 2021 00:34:00 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; arm variant v5

```console
$ docker pull golang@sha256:9868d294d5a8e1e6b467c5818749a9f465f64ee6ec3664c5ed33b1388ca11377
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.2 MB (272163228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2002342de29dd560014d50eac187764c365ce8cf1fa66da3c05b27a28e4faf9e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:38 GMT
ADD file:cbb86580a65f84ec39691b126a21ef374bc4f2f2fe5c27979134aa940d6326f6 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:39:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:39:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 05:40:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 21:47:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 21:47:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Jun 2021 21:47:55 GMT
ENV GOLANG_VERSION=1.17beta1
# Wed, 23 Jun 2021 21:51:32 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.17beta1.linux-amd64.tar.gz'; 			sha256='a479681705b65971f9db079bfce53c4393bfa241d952eb09de88fb40677d3c4c'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17beta1.linux-armv6l.tar.gz'; 			sha256='f4ab69c75a1f9e43b07ca9a0bfdf68ca1e2b0b51d4ebfb8c79f60ed14629f4e6'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17beta1.linux-arm64.tar.gz'; 			sha256='ede56f79c5061146929ab4a128e8ee7bc713d141e87b3df4e0aa670938e128b3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17beta1.linux-386.tar.gz'; 			sha256='cebbf75985ba7e6f1a5b137916a6019685d52ecf36c262092ffc3f714cd85974'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17beta1.linux-ppc64le.tar.gz'; 			sha256='0a6e5034fcbd4b38642b56841a042135aec1e87f61258d2d70aafc0a667bdd11'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17beta1.linux-s390x.tar.gz'; 			sha256='3501d139a9433775001730f1d9c3fb60d7b93b969fe16bd80fc7387a3d5259b1'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17beta1.src.tar.gz'; 		sha256='02b8973725f9bc545955865576e8c8f6ca672312f69fd9e5549c25b0ce1d75f0'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 23 Jun 2021 21:51:34 GMT
ENV GOPATH=/go
# Wed, 23 Jun 2021 21:51:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Jun 2021 21:51:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 23 Jun 2021 21:51:36 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:3b0b1347a8a3d1156e417fffc79192d014d9cc985fa5e55a49cf67c21e7a81da`  
		Last Modified: Wed, 23 Jun 2021 00:00:57 GMT  
		Size: 48.2 MB (48153698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516d9fa44d74100e5f41bad5b510ea489670072286500cb3e7ec282353be3fd6`  
		Last Modified: Wed, 23 Jun 2021 05:57:15 GMT  
		Size: 7.4 MB (7376607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0bd36c0872a5d6227f9c9a854165764990cd8c08f66f8fb948836745f04edb`  
		Last Modified: Wed, 23 Jun 2021 05:57:16 GMT  
		Size: 9.7 MB (9687536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d18936e3f6729a8b31c3c99ef11f98a03ae427bed6603c8e52901cdd5f90a40`  
		Last Modified: Wed, 23 Jun 2021 05:58:10 GMT  
		Size: 49.6 MB (49575238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d80a8aabd73c0fd3bfcd31a1ec149455d5c8a0c26d262e8450625326f70a15`  
		Last Modified: Wed, 23 Jun 2021 22:00:11 GMT  
		Size: 52.1 MB (52056617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b013ceed6354a5cd733af45dc930416cbc8a35bc6bf0768a49bf3e738d4735b`  
		Last Modified: Wed, 23 Jun 2021 22:00:49 GMT  
		Size: 105.3 MB (105313376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f586d9bb391afa4aead12d5820923522dd22cd5d47d4b980238f9dbcf22b8d9`  
		Last Modified: Wed, 23 Jun 2021 21:59:36 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; arm variant v7

```console
$ docker pull golang@sha256:ba29fb94c70daf7abdec59c2f54ac66ed790dfc16729bf861b3fa2b4cea4fe44
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.0 MB (265963231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e26bc64e19fd694e4122f438a68ddd00cb04f50032e56ff2f564f3ceca07ca85`
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
# Thu, 24 Jun 2021 17:35:57 GMT
ENV GOLANG_VERSION=1.17beta1
# Thu, 24 Jun 2021 17:36:27 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.17beta1.linux-amd64.tar.gz'; 			sha256='a479681705b65971f9db079bfce53c4393bfa241d952eb09de88fb40677d3c4c'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17beta1.linux-armv6l.tar.gz'; 			sha256='f4ab69c75a1f9e43b07ca9a0bfdf68ca1e2b0b51d4ebfb8c79f60ed14629f4e6'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17beta1.linux-arm64.tar.gz'; 			sha256='ede56f79c5061146929ab4a128e8ee7bc713d141e87b3df4e0aa670938e128b3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17beta1.linux-386.tar.gz'; 			sha256='cebbf75985ba7e6f1a5b137916a6019685d52ecf36c262092ffc3f714cd85974'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17beta1.linux-ppc64le.tar.gz'; 			sha256='0a6e5034fcbd4b38642b56841a042135aec1e87f61258d2d70aafc0a667bdd11'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17beta1.linux-s390x.tar.gz'; 			sha256='3501d139a9433775001730f1d9c3fb60d7b93b969fe16bd80fc7387a3d5259b1'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17beta1.src.tar.gz'; 		sha256='02b8973725f9bc545955865576e8c8f6ca672312f69fd9e5549c25b0ce1d75f0'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 24 Jun 2021 17:36:29 GMT
ENV GOPATH=/go
# Thu, 24 Jun 2021 17:36:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 17:36:31 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 24 Jun 2021 17:36:31 GMT
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
	-	`sha256:e4435dad9171f80492791f394e203021902c1be9ca81e5f0e7aa8a9d6c355dcb`  
		Last Modified: Thu, 24 Jun 2021 17:56:55 GMT  
		Size: 103.0 MB (102997750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d558089b14ae573fc24fd96750a6557853e86206eeba9b411e166d65f993d021`  
		Last Modified: Thu, 24 Jun 2021 17:55:44 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:d972cfb8ad9c5f1aba288df92e7993e21c55eeb559392c7a4bff0d0fed374a3c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.2 MB (284214595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e72aacad20948023cb4483f7e19862b0e6eed28e5e94478000bcbc2813956046`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:24 GMT
ADD file:bc9eebfc439e3fbf9db01c98dc2448d9bededd394b893e397661227b81859dea in / 
# Tue, 22 Jun 2021 23:49:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:24:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:24:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:25:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:53:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:53:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Jun 2021 12:53:20 GMT
ENV GOLANG_VERSION=1.17beta1
# Wed, 23 Jun 2021 12:53:31 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.17beta1.linux-amd64.tar.gz'; 			sha256='a479681705b65971f9db079bfce53c4393bfa241d952eb09de88fb40677d3c4c'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17beta1.linux-armv6l.tar.gz'; 			sha256='f4ab69c75a1f9e43b07ca9a0bfdf68ca1e2b0b51d4ebfb8c79f60ed14629f4e6'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17beta1.linux-arm64.tar.gz'; 			sha256='ede56f79c5061146929ab4a128e8ee7bc713d141e87b3df4e0aa670938e128b3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17beta1.linux-386.tar.gz'; 			sha256='cebbf75985ba7e6f1a5b137916a6019685d52ecf36c262092ffc3f714cd85974'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17beta1.linux-ppc64le.tar.gz'; 			sha256='0a6e5034fcbd4b38642b56841a042135aec1e87f61258d2d70aafc0a667bdd11'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17beta1.linux-s390x.tar.gz'; 			sha256='3501d139a9433775001730f1d9c3fb60d7b93b969fe16bd80fc7387a3d5259b1'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17beta1.src.tar.gz'; 		sha256='02b8973725f9bc545955865576e8c8f6ca672312f69fd9e5549c25b0ce1d75f0'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 23 Jun 2021 12:53:32 GMT
ENV GOPATH=/go
# Wed, 23 Jun 2021 12:53:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Jun 2021 12:53:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 23 Jun 2021 12:53:33 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:310b368da98207b4fd030cc969461bfba1ea7c73fc5da1f015e05570d3eb2510`  
		Last Modified: Tue, 22 Jun 2021 23:54:51 GMT  
		Size: 49.2 MB (49221986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86422c44ee005c4d5ccb0e2fa32685229207b712728cd4b8c0ef97174f079df7`  
		Last Modified: Wed, 23 Jun 2021 00:33:16 GMT  
		Size: 7.7 MB (7694715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9137877e0c26a439a8954003b21876b6059de852c839631e8cf6fda5bd36434c`  
		Last Modified: Wed, 23 Jun 2021 00:33:17 GMT  
		Size: 10.0 MB (9984281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785171b903c4d81c5b7539417a7b05f4a9bc6a35840595233bf4e369d8aee387`  
		Last Modified: Wed, 23 Jun 2021 00:33:41 GMT  
		Size: 52.2 MB (52165169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31a19a8a6841af41513223b2701373734838fc000bd6928b9c55613c3c79d53`  
		Last Modified: Wed, 23 Jun 2021 12:58:51 GMT  
		Size: 62.6 MB (62615492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a908954429f10403d9153b8b7ef4f8b94609e5f330c9f74c817cfe0d553c5b1`  
		Last Modified: Wed, 23 Jun 2021 12:58:58 GMT  
		Size: 102.5 MB (102532797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57128cde34583b9c0e1645dea5427eb4ed24ec3d5fcb3ac30a0ce73c6588dbd0`  
		Last Modified: Wed, 23 Jun 2021 12:58:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; 386

```console
$ docker pull golang@sha256:5c3ec7cf353dbc8f1b7b94c13c5a11cbc9992d684ee62b2ece444c3e32a072b0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.1 MB (302126082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a19973fc695d77139daf7c76aa6e3150b819257625290123265ccb44561c33a6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:18 GMT
ADD file:e69bc1dee51190c812075d4b4e8ba1e67f67250af9f2ddbaecaf2c9316a07bbd in / 
# Tue, 22 Jun 2021 23:39:18 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:09:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:09:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:09:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 17:06:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 17:06:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Jun 2021 17:06:41 GMT
ENV GOLANG_VERSION=1.17beta1
# Wed, 23 Jun 2021 17:07:03 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.17beta1.linux-amd64.tar.gz'; 			sha256='a479681705b65971f9db079bfce53c4393bfa241d952eb09de88fb40677d3c4c'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17beta1.linux-armv6l.tar.gz'; 			sha256='f4ab69c75a1f9e43b07ca9a0bfdf68ca1e2b0b51d4ebfb8c79f60ed14629f4e6'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17beta1.linux-arm64.tar.gz'; 			sha256='ede56f79c5061146929ab4a128e8ee7bc713d141e87b3df4e0aa670938e128b3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17beta1.linux-386.tar.gz'; 			sha256='cebbf75985ba7e6f1a5b137916a6019685d52ecf36c262092ffc3f714cd85974'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17beta1.linux-ppc64le.tar.gz'; 			sha256='0a6e5034fcbd4b38642b56841a042135aec1e87f61258d2d70aafc0a667bdd11'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17beta1.linux-s390x.tar.gz'; 			sha256='3501d139a9433775001730f1d9c3fb60d7b93b969fe16bd80fc7387a3d5259b1'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17beta1.src.tar.gz'; 		sha256='02b8973725f9bc545955865576e8c8f6ca672312f69fd9e5549c25b0ce1d75f0'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 23 Jun 2021 17:07:05 GMT
ENV GOPATH=/go
# Wed, 23 Jun 2021 17:07:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Jun 2021 17:07:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 23 Jun 2021 17:07:07 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:c4109247a8f9a72ed1435270480f72d6db8d6f038c6941d86a94f4dd0be8f789`  
		Last Modified: Tue, 22 Jun 2021 23:45:45 GMT  
		Size: 51.2 MB (51207098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823a83541e8a9ed59943f9915ac65a73f57137e829772a16bc0bca5031a8cc07`  
		Last Modified: Wed, 23 Jun 2021 00:17:58 GMT  
		Size: 8.0 MB (7998521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7455379cfe2e69e9290d3b103e5889bee3e1c03187bb9e2a454325fd6a7f1a`  
		Last Modified: Wed, 23 Jun 2021 00:17:58 GMT  
		Size: 10.3 MB (10339805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295349fcd02216e45784e329283de2e5811af98fafed9195ab2cf24bf58febe2`  
		Last Modified: Wed, 23 Jun 2021 00:18:25 GMT  
		Size: 53.4 MB (53436615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4006490c7f6243af4cf35efc741f2a30a00b10892a7cd5b7e601bf35bb27f69`  
		Last Modified: Wed, 23 Jun 2021 17:14:57 GMT  
		Size: 73.6 MB (73617257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ee9bf8e11941b2897d5580717dba9c3d24de8837026e36c88f8e90d654cb31`  
		Last Modified: Wed, 23 Jun 2021 17:15:04 GMT  
		Size: 105.5 MB (105526629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b6f5ec64f5e70d7806f7d3549b1b09e2e6f05a0e26a88791b02ba74adad032`  
		Last Modified: Wed, 23 Jun 2021 17:14:38 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; mips64le

```console
$ docker pull golang@sha256:eebb683d2367837e755b07bbeff965a6588fa657d9a8265377fcc57fb03d4d5e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.4 MB (274413028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9e82c38653798c12a8e084ab924e9d8634141005d12403316dd3ae22b7fc70a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:09:06 GMT
ADD file:4673ab387e5a746227250295a00343ac2d03d6aafdc28d019a9bdf26bb97c8c8 in / 
# Wed, 23 Jun 2021 00:09:07 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:42:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:42:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:43:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 18:05:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 18:05:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Jun 2021 18:05:04 GMT
ENV GOLANG_VERSION=1.17beta1
# Wed, 23 Jun 2021 18:14:57 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.17beta1.linux-amd64.tar.gz'; 			sha256='a479681705b65971f9db079bfce53c4393bfa241d952eb09de88fb40677d3c4c'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17beta1.linux-armv6l.tar.gz'; 			sha256='f4ab69c75a1f9e43b07ca9a0bfdf68ca1e2b0b51d4ebfb8c79f60ed14629f4e6'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17beta1.linux-arm64.tar.gz'; 			sha256='ede56f79c5061146929ab4a128e8ee7bc713d141e87b3df4e0aa670938e128b3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17beta1.linux-386.tar.gz'; 			sha256='cebbf75985ba7e6f1a5b137916a6019685d52ecf36c262092ffc3f714cd85974'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17beta1.linux-ppc64le.tar.gz'; 			sha256='0a6e5034fcbd4b38642b56841a042135aec1e87f61258d2d70aafc0a667bdd11'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17beta1.linux-s390x.tar.gz'; 			sha256='3501d139a9433775001730f1d9c3fb60d7b93b969fe16bd80fc7387a3d5259b1'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17beta1.src.tar.gz'; 		sha256='02b8973725f9bc545955865576e8c8f6ca672312f69fd9e5549c25b0ce1d75f0'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 23 Jun 2021 18:14:58 GMT
ENV GOPATH=/go
# Wed, 23 Jun 2021 18:14:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Jun 2021 18:15:01 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 23 Jun 2021 18:15:01 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:e3f0127f2925aa298e3074daa756fb98cf945e5aa11c7dd3cb6d66cc3ba2c7ac`  
		Last Modified: Wed, 23 Jun 2021 00:15:06 GMT  
		Size: 49.1 MB (49080336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92573df8c3dcb8e821060f2830e027ebc52f7da05600cbb49cfdbb39aedcce5e`  
		Last Modified: Wed, 23 Jun 2021 00:53:52 GMT  
		Size: 7.3 MB (7252466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857f80da49549480363cca077bae713c30796f17d3a33620cdfca3a75e0cd160`  
		Last Modified: Wed, 23 Jun 2021 00:53:53 GMT  
		Size: 10.0 MB (10016316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5c2138b0b86fd417cc80da35fb6cccb87f7266d2be62853e3611c28a601c32`  
		Last Modified: Wed, 23 Jun 2021 00:54:42 GMT  
		Size: 50.8 MB (50844925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2c2a73fb7dd82c837752786e34918eaaa17ad8febefbd91afc6e2e1a34ea0f`  
		Last Modified: Wed, 23 Jun 2021 18:31:55 GMT  
		Size: 54.7 MB (54669152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723bd093417adbee887f10f063c9f4e054b24b7b54ef917fd981c76feb958e1e`  
		Last Modified: Wed, 23 Jun 2021 18:32:27 GMT  
		Size: 102.5 MB (102549707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d11b163c73562c017fbbe96e0388cd5c0633d3996e720f7bfcfd00013fa9d0a`  
		Last Modified: Wed, 23 Jun 2021 18:31:13 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; ppc64le

```console
$ docker pull golang@sha256:52cb5c93db704fccde859a004005634f355351c3893470188b5c85ea9658eced
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.2 MB (305237852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02a011eb35a3af8ec3214b3a8c5059171939dfa9fe15f3981b4da1438e4ac6dd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:30:05 GMT
ADD file:b73f8d66b8be6103349949991124c7d82e38589b2db6212e920cb3b6d5ceefef in / 
# Wed, 23 Jun 2021 00:30:13 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 02:33:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 02:34:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 02:38:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 02:32:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 02:32:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 02:32:52 GMT
ENV GOLANG_VERSION=1.17beta1
# Thu, 24 Jun 2021 02:33:53 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.17beta1.linux-amd64.tar.gz'; 			sha256='a479681705b65971f9db079bfce53c4393bfa241d952eb09de88fb40677d3c4c'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17beta1.linux-armv6l.tar.gz'; 			sha256='f4ab69c75a1f9e43b07ca9a0bfdf68ca1e2b0b51d4ebfb8c79f60ed14629f4e6'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17beta1.linux-arm64.tar.gz'; 			sha256='ede56f79c5061146929ab4a128e8ee7bc713d141e87b3df4e0aa670938e128b3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17beta1.linux-386.tar.gz'; 			sha256='cebbf75985ba7e6f1a5b137916a6019685d52ecf36c262092ffc3f714cd85974'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17beta1.linux-ppc64le.tar.gz'; 			sha256='0a6e5034fcbd4b38642b56841a042135aec1e87f61258d2d70aafc0a667bdd11'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17beta1.linux-s390x.tar.gz'; 			sha256='3501d139a9433775001730f1d9c3fb60d7b93b969fe16bd80fc7387a3d5259b1'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17beta1.src.tar.gz'; 		sha256='02b8973725f9bc545955865576e8c8f6ca672312f69fd9e5549c25b0ce1d75f0'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 24 Jun 2021 02:34:26 GMT
ENV GOPATH=/go
# Thu, 24 Jun 2021 02:34:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 02:35:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 24 Jun 2021 02:35:31 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:83f72610ec8bc58c0c3a70f0bdf9d866e8d0156845a9aa24bc0ed2fdaf0fd8b4`  
		Last Modified: Wed, 23 Jun 2021 00:36:35 GMT  
		Size: 54.2 MB (54182463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cdd4a29fac3f4917f56dc5f262d8365826de2b3fb72d6188dc15aa46e8e6d6`  
		Last Modified: Wed, 23 Jun 2021 03:13:08 GMT  
		Size: 8.3 MB (8271984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de85832cf44484bc526bc3e5af3698f3f1b7e753c47e9be91655ca62e7d3abd3`  
		Last Modified: Wed, 23 Jun 2021 03:13:09 GMT  
		Size: 10.7 MB (10727812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8657fc4cb7f4239ffd0cc0698de0121b50102bdc97b4c558bf496726505f2962`  
		Last Modified: Wed, 23 Jun 2021 03:13:34 GMT  
		Size: 57.5 MB (57457627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f24f115b5797938b90fd83181a3e4820b4bb477a507c5003d1630f229698bf`  
		Last Modified: Thu, 24 Jun 2021 02:49:40 GMT  
		Size: 73.7 MB (73660453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae820c6d8450665b818ce4815e6967343d6f357180e6003ff511ea3f83ec6bdd`  
		Last Modified: Thu, 24 Jun 2021 02:49:45 GMT  
		Size: 100.9 MB (100937358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb41c6ceeae66baad15006539dbae854954adae689feb97368e34e4eb9afd06d`  
		Last Modified: Thu, 24 Jun 2021 02:49:26 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-buster` - linux; s390x

```console
$ docker pull golang@sha256:866290130ec723f37e57782812db7a453046347f4b8786452c3d1cf6eccdf3cd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.2 MB (280164065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeb0cbf3e91bc0d49983aa453ab2b4e5f38aa67d60f315f8cb9fc4ab04ffe26a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:42:13 GMT
ADD file:b935574081a3fbceb534880a35e5245e10c52a3b9d70224811e221b4c6254cfe in / 
# Tue, 22 Jun 2021 23:42:16 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:05:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:06:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:06:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:22:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 		pkg-config 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:22:43 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Jun 2021 12:22:43 GMT
ENV GOLANG_VERSION=1.17beta1
# Wed, 23 Jun 2021 12:23:01 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.17beta1.linux-amd64.tar.gz'; 			sha256='a479681705b65971f9db079bfce53c4393bfa241d952eb09de88fb40677d3c4c'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.17beta1.linux-armv6l.tar.gz'; 			sha256='f4ab69c75a1f9e43b07ca9a0bfdf68ca1e2b0b51d4ebfb8c79f60ed14629f4e6'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.17beta1.linux-arm64.tar.gz'; 			sha256='ede56f79c5061146929ab4a128e8ee7bc713d141e87b3df4e0aa670938e128b3'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.17beta1.linux-386.tar.gz'; 			sha256='cebbf75985ba7e6f1a5b137916a6019685d52ecf36c262092ffc3f714cd85974'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.17beta1.linux-ppc64le.tar.gz'; 			sha256='0a6e5034fcbd4b38642b56841a042135aec1e87f61258d2d70aafc0a667bdd11'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.17beta1.linux-s390x.tar.gz'; 			sha256='3501d139a9433775001730f1d9c3fb60d7b93b969fe16bd80fc7387a3d5259b1'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17beta1.src.tar.gz'; 		sha256='02b8973725f9bc545955865576e8c8f6ca672312f69fd9e5549c25b0ce1d75f0'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 23 Jun 2021 12:23:07 GMT
ENV GOPATH=/go
# Wed, 23 Jun 2021 12:23:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Jun 2021 12:23:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 23 Jun 2021 12:23:08 GMT
WORKDIR /go
```

-	Layers:
	-	`sha256:2b8d113de06cefaa0768df3e10da0c3b8272e15922e18ea75b0bb4dee23b551d`  
		Last Modified: Tue, 22 Jun 2021 23:45:28 GMT  
		Size: 49.0 MB (49003924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de1b6d51a91a64482d6eabf778b8c4e433f7dc198440476d01d0dbb31aee4fe`  
		Last Modified: Wed, 23 Jun 2021 00:12:08 GMT  
		Size: 7.4 MB (7400480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64019084b252c52592ff8cab3bf20be9bab2801ea36e88025071f901f1cb38e`  
		Last Modified: Wed, 23 Jun 2021 00:12:08 GMT  
		Size: 9.9 MB (9882902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481cb3d9acd652b3fd56e606ff28a1bb48aa89be3365577a33d2cd35c908d867`  
		Last Modified: Wed, 23 Jun 2021 00:12:24 GMT  
		Size: 51.4 MB (51380256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bed2826325580193e1f03df87cd7d0c20d5a324c45056157542eaec1654b5b8`  
		Last Modified: Wed, 23 Jun 2021 12:27:41 GMT  
		Size: 56.8 MB (56817772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470e345c468c1d07867d437681e7db2209f5578b714116d75f9c136a548233f7`  
		Last Modified: Wed, 23 Jun 2021 12:27:47 GMT  
		Size: 105.7 MB (105678575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc7cfd464ebed356c8ec0d28c07160238860f048d1b27aa14b180d46b2f19a1`  
		Last Modified: Wed, 23 Jun 2021 12:27:33 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
