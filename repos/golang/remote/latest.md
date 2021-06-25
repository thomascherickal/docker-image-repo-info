## `golang:latest`

```console
$ docker pull golang@sha256:2e4c37697fc00ea0b40e03360946cf1434f504f03836540ab0209687d920076c
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
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `golang:latest` - linux; amd64

```console
$ docker pull golang@sha256:be99fa59acd78bb22a41bbc1e15ebfab2262498ee0c2e28c3d09bc44d51d1774
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.9 MB (317909765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee23292e282684136ded9a63f7f96b3aea50e19e9a5cec684aa7d107d6e1cc30`
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
# Thu, 24 Jun 2021 00:30:53 GMT
ENV GOLANG_VERSION=1.16.5
# Thu, 24 Jun 2021 00:31:03 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.16.5.linux-amd64.tar.gz'; 			sha256='b12c23023b68de22f74c0524f10b753e7b08b1504cb7e417eccebdd3fae49061'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.16.5.linux-armv6l.tar.gz'; 			sha256='93cacacfbe87e3106b5bf5821de106f0f0a43c8bd1029826d44445c15df795a5'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.16.5.linux-arm64.tar.gz'; 			sha256='d5446b46ef6f36fdffa852f73dfbbe78c1ddf010b99fa4964944b9ae8b4d6799'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.16.5.linux-386.tar.gz'; 			sha256='a37c6b71d0b673fe8dfeb2a8b3de78824f05d680ad32b7ac6b58c573fa6695de'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.16.5.linux-ppc64le.tar.gz'; 			sha256='fad2da6c86ede8448d2d0e66e1776e2f0ae9169714eade29b9ffbbdede7fc6cc'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.16.5.linux-s390x.tar.gz'; 			sha256='21085f6a3568fae639edf383cce78bcb00d8f415e5e3d7feb04b6124e8e9efc1'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 		sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 24 Jun 2021 00:31:04 GMT
ENV GOPATH=/go
# Thu, 24 Jun 2021 00:31:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 00:31:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 24 Jun 2021 00:31:06 GMT
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
	-	`sha256:f37c08d9a1e12991cd7504e83d694672027bfadf3a773e4be3252350bec7ade0`  
		Last Modified: Thu, 24 Jun 2021 00:35:31 GMT  
		Size: 129.1 MB (129052373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f10b5e5b99b6f0217b6bd63c2b7d84de88f6c349460a05b6fb0a01957ad18a0`  
		Last Modified: Thu, 24 Jun 2021 00:35:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm variant v5

```console
$ docker pull golang@sha256:f033f8aa3b9f08a770a46474937a63dc684b6ff14e7dcb4e63f287bc5a707928
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.4 MB (269405284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4d401058a4b2d36da3d6de8a0f49d3c33ee18bad7fe777f69c7acc8b7548c32`
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
# Wed, 23 Jun 2021 21:51:51 GMT
ENV GOLANG_VERSION=1.16.5
# Wed, 23 Jun 2021 21:54:49 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.16.5.linux-amd64.tar.gz'; 			sha256='b12c23023b68de22f74c0524f10b753e7b08b1504cb7e417eccebdd3fae49061'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.16.5.linux-armv6l.tar.gz'; 			sha256='93cacacfbe87e3106b5bf5821de106f0f0a43c8bd1029826d44445c15df795a5'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.16.5.linux-arm64.tar.gz'; 			sha256='d5446b46ef6f36fdffa852f73dfbbe78c1ddf010b99fa4964944b9ae8b4d6799'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.16.5.linux-386.tar.gz'; 			sha256='a37c6b71d0b673fe8dfeb2a8b3de78824f05d680ad32b7ac6b58c573fa6695de'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.16.5.linux-ppc64le.tar.gz'; 			sha256='fad2da6c86ede8448d2d0e66e1776e2f0ae9169714eade29b9ffbbdede7fc6cc'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.16.5.linux-s390x.tar.gz'; 			sha256='21085f6a3568fae639edf383cce78bcb00d8f415e5e3d7feb04b6124e8e9efc1'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 		sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 23 Jun 2021 21:54:51 GMT
ENV GOPATH=/go
# Wed, 23 Jun 2021 21:54:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Jun 2021 21:54:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 23 Jun 2021 21:54:54 GMT
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
	-	`sha256:108f6032cb25c64c1e9ab17666b1ffc8af1a304368f757bc01ffad3b3928e10a`  
		Last Modified: Wed, 23 Jun 2021 22:02:16 GMT  
		Size: 102.6 MB (102555433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815da6e8ea9828fa64a9c724410a4be9d1f4368ea756cdc652a0b19aade9999d`  
		Last Modified: Wed, 23 Jun 2021 22:01:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm variant v7

```console
$ docker pull golang@sha256:b05b4e9cb2d06227985165ff43c35d6d5876fcb3424d16414d82732e6f2922ab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.3 MB (263256993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f321ae45faa81cfab8d652197a3ec6da341f8b49de62f04e530dabf8e1e6b017`
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
# Thu, 24 Jun 2021 17:42:43 GMT
ENV GOLANG_VERSION=1.16.5
# Thu, 24 Jun 2021 17:43:10 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.16.5.linux-amd64.tar.gz'; 			sha256='b12c23023b68de22f74c0524f10b753e7b08b1504cb7e417eccebdd3fae49061'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.16.5.linux-armv6l.tar.gz'; 			sha256='93cacacfbe87e3106b5bf5821de106f0f0a43c8bd1029826d44445c15df795a5'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.16.5.linux-arm64.tar.gz'; 			sha256='d5446b46ef6f36fdffa852f73dfbbe78c1ddf010b99fa4964944b9ae8b4d6799'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.16.5.linux-386.tar.gz'; 			sha256='a37c6b71d0b673fe8dfeb2a8b3de78824f05d680ad32b7ac6b58c573fa6695de'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.16.5.linux-ppc64le.tar.gz'; 			sha256='fad2da6c86ede8448d2d0e66e1776e2f0ae9169714eade29b9ffbbdede7fc6cc'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.16.5.linux-s390x.tar.gz'; 			sha256='21085f6a3568fae639edf383cce78bcb00d8f415e5e3d7feb04b6124e8e9efc1'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 		sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 24 Jun 2021 17:43:12 GMT
ENV GOPATH=/go
# Thu, 24 Jun 2021 17:43:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 17:43:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 24 Jun 2021 17:43:14 GMT
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
	-	`sha256:a9687670e4aaa20dd5b1ddc52cc76fc06f4c8cf7bb59466653fe3c1a6c28100b`  
		Last Modified: Thu, 24 Jun 2021 18:01:23 GMT  
		Size: 100.3 MB (100291513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920a66464b01c0d127b0fc799c35c9eabacd2a64612a8ce3c3b44d2b97fc7b7d`  
		Last Modified: Thu, 24 Jun 2021 18:00:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; arm64 variant v8

```console
$ docker pull golang@sha256:d302623e7c93ddd20ff89fa0d3f44bf16d0218e236fc384778e0e8c4d6ffe894
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.3 MB (281318456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4116d705e71f6e56422736aeafb577b66743200ee27b1454e81b99acb922aa8`
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
# Wed, 23 Jun 2021 12:54:53 GMT
ENV GOLANG_VERSION=1.16.5
# Wed, 23 Jun 2021 12:55:01 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.16.5.linux-amd64.tar.gz'; 			sha256='b12c23023b68de22f74c0524f10b753e7b08b1504cb7e417eccebdd3fae49061'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.16.5.linux-armv6l.tar.gz'; 			sha256='93cacacfbe87e3106b5bf5821de106f0f0a43c8bd1029826d44445c15df795a5'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.16.5.linux-arm64.tar.gz'; 			sha256='d5446b46ef6f36fdffa852f73dfbbe78c1ddf010b99fa4964944b9ae8b4d6799'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.16.5.linux-386.tar.gz'; 			sha256='a37c6b71d0b673fe8dfeb2a8b3de78824f05d680ad32b7ac6b58c573fa6695de'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.16.5.linux-ppc64le.tar.gz'; 			sha256='fad2da6c86ede8448d2d0e66e1776e2f0ae9169714eade29b9ffbbdede7fc6cc'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.16.5.linux-s390x.tar.gz'; 			sha256='21085f6a3568fae639edf383cce78bcb00d8f415e5e3d7feb04b6124e8e9efc1'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 		sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 23 Jun 2021 12:55:02 GMT
ENV GOPATH=/go
# Wed, 23 Jun 2021 12:55:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Jun 2021 12:55:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 23 Jun 2021 12:55:03 GMT
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
	-	`sha256:8248e431fd7e628bbe6f99c96c1605d6ccaee4904b9c2a1e78e0bab8e2c62a3e`  
		Last Modified: Wed, 23 Jun 2021 13:00:09 GMT  
		Size: 99.6 MB (99636658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf39eafd2cc6a63cac074f0f72e7f0c22d81bbdfa7cbb22bf525bcc33a07ed9`  
		Last Modified: Wed, 23 Jun 2021 12:59:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; 386

```console
$ docker pull golang@sha256:04fe552b39189ee95c78d52471b2dadbe31e8677668798d896565464a11c6480
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.7 MB (299698805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dec77205da479fbaeb11a947ac7af5e577548915866b17614e305c3c9ed62d28`
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
# Wed, 23 Jun 2021 17:09:00 GMT
ENV GOLANG_VERSION=1.16.5
# Wed, 23 Jun 2021 17:09:20 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.16.5.linux-amd64.tar.gz'; 			sha256='b12c23023b68de22f74c0524f10b753e7b08b1504cb7e417eccebdd3fae49061'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.16.5.linux-armv6l.tar.gz'; 			sha256='93cacacfbe87e3106b5bf5821de106f0f0a43c8bd1029826d44445c15df795a5'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.16.5.linux-arm64.tar.gz'; 			sha256='d5446b46ef6f36fdffa852f73dfbbe78c1ddf010b99fa4964944b9ae8b4d6799'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.16.5.linux-386.tar.gz'; 			sha256='a37c6b71d0b673fe8dfeb2a8b3de78824f05d680ad32b7ac6b58c573fa6695de'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.16.5.linux-ppc64le.tar.gz'; 			sha256='fad2da6c86ede8448d2d0e66e1776e2f0ae9169714eade29b9ffbbdede7fc6cc'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.16.5.linux-s390x.tar.gz'; 			sha256='21085f6a3568fae639edf383cce78bcb00d8f415e5e3d7feb04b6124e8e9efc1'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 		sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 23 Jun 2021 17:09:21 GMT
ENV GOPATH=/go
# Wed, 23 Jun 2021 17:09:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Jun 2021 17:09:23 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 23 Jun 2021 17:09:23 GMT
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
	-	`sha256:84f12ad4201247ff6b3f4a116d6f9f03375324542ba77362575d18672940d18a`  
		Last Modified: Wed, 23 Jun 2021 17:16:54 GMT  
		Size: 103.1 MB (103099352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be305b84b133a7560e55b08a294809c187f618596ca73b3b1e9a41421737229`  
		Last Modified: Wed, 23 Jun 2021 17:16:25 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; mips64le

```console
$ docker pull golang@sha256:8f7966a42733de832de158c7602ce6e291a1376d1924e4c66016dfae85ccd9ed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.5 MB (271483331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75940e1b1c4a43faa3a8c480afc0c8659804e4f7b2fc75dea4b21aabfe50b235`
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
# Wed, 23 Jun 2021 18:15:15 GMT
ENV GOLANG_VERSION=1.16.5
# Wed, 23 Jun 2021 18:23:06 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.16.5.linux-amd64.tar.gz'; 			sha256='b12c23023b68de22f74c0524f10b753e7b08b1504cb7e417eccebdd3fae49061'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.16.5.linux-armv6l.tar.gz'; 			sha256='93cacacfbe87e3106b5bf5821de106f0f0a43c8bd1029826d44445c15df795a5'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.16.5.linux-arm64.tar.gz'; 			sha256='d5446b46ef6f36fdffa852f73dfbbe78c1ddf010b99fa4964944b9ae8b4d6799'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.16.5.linux-386.tar.gz'; 			sha256='a37c6b71d0b673fe8dfeb2a8b3de78824f05d680ad32b7ac6b58c573fa6695de'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.16.5.linux-ppc64le.tar.gz'; 			sha256='fad2da6c86ede8448d2d0e66e1776e2f0ae9169714eade29b9ffbbdede7fc6cc'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.16.5.linux-s390x.tar.gz'; 			sha256='21085f6a3568fae639edf383cce78bcb00d8f415e5e3d7feb04b6124e8e9efc1'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 		sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 23 Jun 2021 18:23:07 GMT
ENV GOPATH=/go
# Wed, 23 Jun 2021 18:23:08 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Jun 2021 18:23:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 23 Jun 2021 18:23:10 GMT
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
	-	`sha256:9c73295f9de7e9243b9c3afcac9745eead817e0d42c1e1ebdc391f8db28ac36a`  
		Last Modified: Wed, 23 Jun 2021 18:33:50 GMT  
		Size: 99.6 MB (99620011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4610a7fc5b6d58bc4b1c00ce97f4cc1040bfc25c36472fc3c450b7a605793327`  
		Last Modified: Wed, 23 Jun 2021 18:32:41 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; ppc64le

```console
$ docker pull golang@sha256:69d91de130503af6f05740673a4ce37690e662b39690384685f400d56b8e8e94
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.4 MB (302396335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6430aaf77fd7b97ebc432d72115c35862a86432239ccdc3747ade17989d93e7`
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
# Thu, 24 Jun 2021 02:39:06 GMT
ENV GOLANG_VERSION=1.16.5
# Thu, 24 Jun 2021 02:40:06 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.16.5.linux-amd64.tar.gz'; 			sha256='b12c23023b68de22f74c0524f10b753e7b08b1504cb7e417eccebdd3fae49061'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.16.5.linux-armv6l.tar.gz'; 			sha256='93cacacfbe87e3106b5bf5821de106f0f0a43c8bd1029826d44445c15df795a5'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.16.5.linux-arm64.tar.gz'; 			sha256='d5446b46ef6f36fdffa852f73dfbbe78c1ddf010b99fa4964944b9ae8b4d6799'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.16.5.linux-386.tar.gz'; 			sha256='a37c6b71d0b673fe8dfeb2a8b3de78824f05d680ad32b7ac6b58c573fa6695de'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.16.5.linux-ppc64le.tar.gz'; 			sha256='fad2da6c86ede8448d2d0e66e1776e2f0ae9169714eade29b9ffbbdede7fc6cc'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.16.5.linux-s390x.tar.gz'; 			sha256='21085f6a3568fae639edf383cce78bcb00d8f415e5e3d7feb04b6124e8e9efc1'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 		sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Thu, 24 Jun 2021 02:40:36 GMT
ENV GOPATH=/go
# Thu, 24 Jun 2021 02:40:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 02:41:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 24 Jun 2021 02:41:19 GMT
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
	-	`sha256:1931ca9279f616ca03d8b486df23379121967a135e0f43915209e182ad64d5d3`  
		Last Modified: Thu, 24 Jun 2021 02:50:21 GMT  
		Size: 98.1 MB (98095841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2a0fb3bd858ef74293304da536ad656f1a61cfd8d9313d950cd140fc181c63`  
		Last Modified: Thu, 24 Jun 2021 02:50:02 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - linux; s390x

```console
$ docker pull golang@sha256:5dfe2c80155527d49152e93c27b7e4a67aa42f3a7cff70b85be28b87a9c24331
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.7 MB (277729239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40467f1aa293039ae263de0fd8812b7bc9582ac3c0b3d0510a07661905c09372`
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
# Wed, 23 Jun 2021 12:24:18 GMT
ENV GOLANG_VERSION=1.16.5
# Wed, 23 Jun 2021 12:24:31 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	url=; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://dl.google.com/go/go1.16.5.linux-amd64.tar.gz'; 			sha256='b12c23023b68de22f74c0524f10b753e7b08b1504cb7e417eccebdd3fae49061'; 			;; 		'armel') 			export GOARCH='arm' GOARM='5' GOOS='linux'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.16.5.linux-armv6l.tar.gz'; 			sha256='93cacacfbe87e3106b5bf5821de106f0f0a43c8bd1029826d44445c15df795a5'; 			;; 		'arm64') 			url='https://dl.google.com/go/go1.16.5.linux-arm64.tar.gz'; 			sha256='d5446b46ef6f36fdffa852f73dfbbe78c1ddf010b99fa4964944b9ae8b4d6799'; 			;; 		'i386') 			url='https://dl.google.com/go/go1.16.5.linux-386.tar.gz'; 			sha256='a37c6b71d0b673fe8dfeb2a8b3de78824f05d680ad32b7ac6b58c573fa6695de'; 			;; 		'mips64el') 			export GOARCH='mips64le' GOOS='linux'; 			;; 		'ppc64el') 			url='https://dl.google.com/go/go1.16.5.linux-ppc64le.tar.gz'; 			sha256='fad2da6c86ede8448d2d0e66e1776e2f0ae9169714eade29b9ffbbdede7fc6cc'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.16.5.linux-s390x.tar.gz'; 			sha256='21085f6a3568fae639edf383cce78bcb00d8f415e5e3d7feb04b6124e8e9efc1'; 			;; 		*) echo >&2 "error: unsupported architecture '$dpkgArch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 		sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		echo >&2; 		echo >&2 "warning: current architecture ($dpkgArch) does not have a corresponding Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc" --progress=dot:giga; 	wget -O go.tgz "$url" --progress=dot:giga; 	echo "$sha256 *go.tgz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends golang-go; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apt-mark auto '.*' > /dev/null; 		apt-mark manual $savedAptMark > /dev/null; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		rm -rf /var/lib/apt/lists/*; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		go version
# Wed, 23 Jun 2021 12:24:35 GMT
ENV GOPATH=/go
# Wed, 23 Jun 2021 12:24:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Jun 2021 12:24:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 23 Jun 2021 12:24:37 GMT
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
	-	`sha256:7bd78c33e704ab3812cca7604e20971d72b4e18817fdb1e185f9cdbb70225d67`  
		Last Modified: Wed, 23 Jun 2021 12:28:10 GMT  
		Size: 103.2 MB (103243750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de67e1da7689d80295c42c6c594f57c60d33d0d83aad8a44a9ae3c8eb076c7f5`  
		Last Modified: Wed, 23 Jun 2021 12:27:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - windows version 10.0.17763.1999; amd64

```console
$ docker pull golang@sha256:f91a779a254fa569ac64f0f9ec590d5b905f54f840d1482ce5d5530415788b9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2806711674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dd98a92940373457cbb9edbd5e7a807db841abb4f907b1934e4560635d6080f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 12:10:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 12:37:22 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Jun 2021 12:37:25 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Jun 2021 12:37:29 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Jun 2021 12:37:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Jun 2021 12:38:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:38:25 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Jun 2021 12:38:51 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Jun 2021 12:38:53 GMT
ENV GOLANG_VERSION=1.16.5
# Wed, 09 Jun 2021 12:41:22 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:41:27 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7863ef96846d497ea06fe442ea13dcecaf5c248ce238c69800475281a4fa848e`  
		Last Modified: Wed, 09 Jun 2021 12:20:41 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f985a0b4390580a94aa3cbc8ecb01fc33805bb3304c4217dc5ec9fb6626011ca`  
		Last Modified: Wed, 09 Jun 2021 13:03:26 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5adf5cc2989b1cf730e7993bd088f778b31b33bac78f6d9c133226f7bcf4a6`  
		Last Modified: Wed, 09 Jun 2021 13:03:24 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480b981517ab26b6ee7e090e51d040995ac5a6a55410880ea3f0c8255dada3bc`  
		Last Modified: Wed, 09 Jun 2021 13:03:24 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a372a8dcfb8f1152565f4b8c928c202db247ddc21fd9a35838a2278c65ff6f`  
		Last Modified: Wed, 09 Jun 2021 13:03:23 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97090ffba94bc8afc85a54e404c8aca13253969fe01c8b0ac1f8ce3a0b909953`  
		Last Modified: Wed, 09 Jun 2021 13:03:53 GMT  
		Size: 25.4 MB (25445694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb1c026791860f230531a960e59a35d86f3ae617c5b6ad60155718694ed3720`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fca536252ace3ea8e08bcd38a313ad63d7d308f4a1d24734c324d191b65647`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 314.6 KB (314587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3865edd5ab3e6e2858d35fea90d96f24eb95579b3bb7f95674954df09b428a8e`  
		Last Modified: Wed, 09 Jun 2021 13:03:20 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424a1b81819edd902af8893d485a39318ee4023db4db6f9c73ebb8470a5c2310`  
		Last Modified: Wed, 09 Jun 2021 13:03:58 GMT  
		Size: 139.4 MB (139355479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f54cc4fcf8b7300908d2cb4aa6dbfe433cc614c35c200ca655b96d576a40412`  
		Last Modified: Wed, 09 Jun 2021 13:03:21 GMT  
		Size: 1.6 KB (1596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:latest` - windows version 10.0.14393.4467; amd64

```console
$ docker pull golang@sha256:a9608105254b4b35b86146a400e935309ca131dd84cd6577153e59da54977ce7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6435308964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff707bfc54244fb7de17bd3f874d1fcdc2c67e28495454b0241db504bac3b13a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 12:41:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 12:41:40 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Jun 2021 12:41:43 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Jun 2021 12:41:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Jun 2021 12:41:49 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Jun 2021 12:44:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:44:27 GMT
ENV GOPATH=C:\gopath
# Wed, 09 Jun 2021 12:45:49 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Jun 2021 12:45:51 GMT
ENV GOLANG_VERSION=1.16.5
# Wed, 09 Jun 2021 12:49:20 GMT
RUN $url = 'https://dl.google.com/go/go1.16.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '0a3fa279ae5b91bc8c88017198c8f1ba5d9925eb6e5d7571316e567c73add39d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 12:49:24 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c82e82e95dbad4ccc260b42e03767eb07222e2f00ec57a69b3c87b17da1d2fd3`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a881968e28f8c2900b00800a0de406d0e98740558d9564ad738d053e63d9a1e`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab71df915cf7ac4c559039a917269e11faab2d0e6862a01408431df7fb40362f`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82ce560dcbc3235ed87d6c938aa761616dbd299188ae53a51a266eb37f381f6`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bee5ea2f89fe3f3e514b8dfcd823da340447b633c6048e00773d1c30fbbc0e9`  
		Last Modified: Wed, 09 Jun 2021 13:04:22 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad71deb840b73610184070ebc7c566bd1dac9cc309d53679460697243bab7640`  
		Last Modified: Wed, 09 Jun 2021 13:04:50 GMT  
		Size: 25.4 MB (25441204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16f2a89ed7a230471eb96b67829deb255795564010b0ff2de47179cdfdec1d0`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cc755175ec255452c16e1e41cc78a8cd719d65f70221e7d128c1dc18eec8f2`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 307.7 KB (307689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d153904f724dbfda646a6c5ccdc1eed2545cf7777c8650461abdedafe75bc693`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ec88320a2e6bf1cfef8856b9271f7d2fa4d2ae8e0eb5b9a44175d04a725631`  
		Last Modified: Wed, 09 Jun 2021 13:04:58 GMT  
		Size: 143.8 MB (143821249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419b516d300f276d9a3f98a1d2c47394abb00b15edeaadcb2f5d0ecee3380f14`  
		Last Modified: Wed, 09 Jun 2021 13:04:19 GMT  
		Size: 1.6 KB (1576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
