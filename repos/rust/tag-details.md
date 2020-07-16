<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `rust`

-	[`rust:1`](#rust1)
-	[`rust:1.45`](#rust145)
-	[`rust:1.45.0`](#rust1450)
-	[`rust:1.45.0-alpine`](#rust1450-alpine)
-	[`rust:1.45.0-alpine3.11`](#rust1450-alpine311)
-	[`rust:1.45.0-alpine3.12`](#rust1450-alpine312)
-	[`rust:1.45.0-buster`](#rust1450-buster)
-	[`rust:1.45.0-slim`](#rust1450-slim)
-	[`rust:1.45.0-slim-buster`](#rust1450-slim-buster)
-	[`rust:1.45.0-slim-stretch`](#rust1450-slim-stretch)
-	[`rust:1.45.0-stretch`](#rust1450-stretch)
-	[`rust:1.45-alpine`](#rust145-alpine)
-	[`rust:1.45-alpine3.11`](#rust145-alpine311)
-	[`rust:1.45-alpine3.12`](#rust145-alpine312)
-	[`rust:1.45-buster`](#rust145-buster)
-	[`rust:1.45-slim`](#rust145-slim)
-	[`rust:1.45-slim-buster`](#rust145-slim-buster)
-	[`rust:1.45-slim-stretch`](#rust145-slim-stretch)
-	[`rust:1.45-stretch`](#rust145-stretch)
-	[`rust:1-alpine`](#rust1-alpine)
-	[`rust:1-alpine3.11`](#rust1-alpine311)
-	[`rust:1-alpine3.12`](#rust1-alpine312)
-	[`rust:1-buster`](#rust1-buster)
-	[`rust:1-slim`](#rust1-slim)
-	[`rust:1-slim-buster`](#rust1-slim-buster)
-	[`rust:1-slim-stretch`](#rust1-slim-stretch)
-	[`rust:1-stretch`](#rust1-stretch)
-	[`rust:alpine`](#rustalpine)
-	[`rust:alpine3.11`](#rustalpine311)
-	[`rust:alpine3.12`](#rustalpine312)
-	[`rust:buster`](#rustbuster)
-	[`rust:latest`](#rustlatest)
-	[`rust:slim`](#rustslim)
-	[`rust:slim-buster`](#rustslim-buster)
-	[`rust:slim-stretch`](#rustslim-stretch)
-	[`rust:stretch`](#ruststretch)

## `rust:1`

```console
$ docker pull rust@sha256:ee8f52372784746235500f9ee80685337a61dcde5e0d028a2aa955d15b6defc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1` - linux; amd64

```console
$ docker pull rust@sha256:b2fd2fcc9d28c1a6dc59c3b0b37913fd9a326c8e457e50617e1156fc1ad51e34
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **447.5 MB (447532458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be36dd54f964afeab7f33a72c583e81294fa2deab3fa05f73453209d3d57e199`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:39 GMT
ADD file:1ab357efe422cfed5e37af2dc60d07ccfd4bdee4d4a0c00838b5d68f19ff20c7 in / 
# Tue, 09 Jun 2020 01:20:39 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:47:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:48:00 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Jun 2020 19:21:04 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:21:18 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:e9afc4f90ab09248d75c8081b6dfba749a7f7efdac704ced7e0ceb506e02fa4a`  
		Last Modified: Tue, 09 Jun 2020 01:25:37 GMT  
		Size: 50.4 MB (50389504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e6b19a265d6b8b7934e7ddd7dc07f6e2fc945b3a28dda9b8aecb12cdb30e0`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 7.8 MB (7811709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14b6c2f8785723bceb5964c5dec1f0489b7750e9d4ec671e49bfba15d80a39`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 10.0 MB (9996168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5573c4b3094956931fd68c310ae92c9eb1a787f0c77ac2730be9d16cce172d5e`  
		Last Modified: Tue, 09 Jun 2020 02:00:08 GMT  
		Size: 51.8 MB (51827493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a88e76431345b48525c4e4d58d497810019f4bafdb5e2bd56dc34a05e09cc3`  
		Last Modified: Tue, 09 Jun 2020 02:00:47 GMT  
		Size: 192.2 MB (192214313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2afbc28d89df4b6fb2dc20541f4233efb213257aafdcfa2b4bb4290983e3ec6`  
		Last Modified: Thu, 18 Jun 2020 19:24:24 GMT  
		Size: 135.3 MB (135293271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1` - linux; arm variant v7

```console
$ docker pull rust@sha256:2a52a967c9b16f19fcc004490f7837ac612a0bb8da50858670f725e0796b4bc9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.4 MB (426430312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3e404c4c716a199bea9faa5dbdd48d89dac55e6b5496c8b944755a6f013054c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:00:40 GMT
ADD file:35073a186411c4b773a9d4d540ec0693ced845cb847b43d8465f9579174cd2b0 in / 
# Tue, 09 Jun 2020 01:00:45 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:48:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:52:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Jun 2020 19:13:13 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:13:42 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:cff0731da2e4f4a0ae8329840eb7fed7ea6aac11aecbfa15c6e684caec03920d`  
		Last Modified: Tue, 09 Jun 2020 01:09:57 GMT  
		Size: 45.9 MB (45868949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbeb0ded58d68be17265763fda36a4e1a520234a291d66f370d98a3e0d6e591`  
		Last Modified: Tue, 09 Jun 2020 02:11:21 GMT  
		Size: 7.1 MB (7097860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6159fbed770bb99a219eae06828da55caaa649879843c0b9df18ddda9b698b3`  
		Last Modified: Tue, 09 Jun 2020 02:11:20 GMT  
		Size: 9.3 MB (9343524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba732bafeb6b1467fd6908c64c6e8d10ffb27e44e3a25ab4c6c38e8f753baa5`  
		Last Modified: Tue, 09 Jun 2020 02:11:43 GMT  
		Size: 47.4 MB (47356467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d84f63917d0e3fb79c2b4c16f4595b8db444749589cfd28a57ef31188ab110`  
		Last Modified: Tue, 09 Jun 2020 02:12:32 GMT  
		Size: 168.4 MB (168420423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a94607ffab11c3cf1fb6f417882b1d8edc34360eb1e13530cb3170ab34cb57`  
		Last Modified: Thu, 18 Jun 2020 19:19:31 GMT  
		Size: 148.3 MB (148343089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:623732a5a57084e4da5db6732e4bc7578a425b95e6ffbbb59f0d5bdbd76433b4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **447.7 MB (447665351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddb6fcb343548fe6b5044b7778f1c7c05867e46be852e56f8c39cbbcd38754bb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:51:33 GMT
ADD file:73f1cc6ac15b24788e78ae41cd6c89cb5211d64baf491accbd95b6fe9718f17f in / 
# Tue, 09 Jun 2020 01:51:36 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:31:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:32:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:32:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:35:00 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 19 Jun 2020 00:04:43 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Fri, 19 Jun 2020 00:04:59 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:1db90d3d3b6598d485690f804e96153fb632e7434251d334e9a0c49b773855c9`  
		Last Modified: Tue, 09 Jun 2020 01:57:52 GMT  
		Size: 49.2 MB (49167914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e848fd373270c8ed6d276649dd8a5860d188f7d0ff306e91e4e3e092e541d99`  
		Last Modified: Tue, 09 Jun 2020 02:47:16 GMT  
		Size: 7.7 MB (7681351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c85f14a5d8064020366c03aa05ec1c8b0f731e0966bb9788960d27258634aef`  
		Last Modified: Tue, 09 Jun 2020 02:47:16 GMT  
		Size: 10.0 MB (9983910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334e38f2d6fff7c08f4ad1b38ec441d2cf963b761b5d85983396a75ff6d0c08f`  
		Last Modified: Tue, 09 Jun 2020 02:47:41 GMT  
		Size: 52.2 MB (52156256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326561827fde74d56d06dce7035ef6653dbf62a27a5dc35416ba6f00293a09b8`  
		Last Modified: Tue, 09 Jun 2020 02:48:39 GMT  
		Size: 183.7 MB (183744170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef821eade6b1f26263a9104496d7c6527232a00c8ecfa0aab6868fc10d480c9`  
		Last Modified: Fri, 19 Jun 2020 00:08:45 GMT  
		Size: 144.9 MB (144931750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1` - linux; 386

```console
$ docker pull rust@sha256:3f45b9475ee12ddc57e3de3a547e246e4441144975e665c9cfce651ba4bf1138
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **472.8 MB (472818538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f861e1f7ab671dcb926e2bd5fcacc831bcc72d0c99ecaf10f37719aae3f3a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:39:33 GMT
ADD file:f95fda6e1e7823d93ca50dd67a1ab99bdc8a7dea372ef27426915702500d54a2 in / 
# Tue, 09 Jun 2020 01:39:33 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:11:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:11:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:12:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:13:11 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Jun 2020 20:10:36 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 20:10:55 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:ca172633df711443e1bcc46650b24074efa097045feee542ecbb4934ae3ae01b`  
		Last Modified: Tue, 09 Jun 2020 01:44:44 GMT  
		Size: 51.2 MB (51156157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e4e2e742db8627ba5d7e0f076114e90c4fea4407cedd3599355e4c00828543`  
		Last Modified: Tue, 09 Jun 2020 02:32:03 GMT  
		Size: 8.0 MB (7981054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ba43d083b56bb094a5bac45d723e9bec0fe65d033950b3c4dc392e890c7e41`  
		Last Modified: Tue, 09 Jun 2020 02:32:03 GMT  
		Size: 10.3 MB (10338453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2391b0310a0be022e7ac6e202273ea7cc0ac5f16e862e5cb19c43c5db30b5b`  
		Last Modified: Tue, 09 Jun 2020 02:32:24 GMT  
		Size: 53.4 MB (53429728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3e805e55983a46c901632f289542625edb04ff470dc6dd9217466a3788d608`  
		Last Modified: Tue, 09 Jun 2020 02:33:23 GMT  
		Size: 198.8 MB (198755099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbce41824f90111fafebb16091199a32fe6de31d201a9cb9384f485fe5fb5de`  
		Last Modified: Thu, 18 Jun 2020 20:13:59 GMT  
		Size: 151.2 MB (151158047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.45`

**does not exist** (yet?)

## `rust:1.45.0`

**does not exist** (yet?)

## `rust:1.45.0-alpine`

**does not exist** (yet?)

## `rust:1.45.0-alpine3.11`

**does not exist** (yet?)

## `rust:1.45.0-alpine3.12`

**does not exist** (yet?)

## `rust:1.45.0-buster`

**does not exist** (yet?)

## `rust:1.45.0-slim`

**does not exist** (yet?)

## `rust:1.45.0-slim-buster`

**does not exist** (yet?)

## `rust:1.45.0-slim-stretch`

**does not exist** (yet?)

## `rust:1.45.0-stretch`

**does not exist** (yet?)

## `rust:1.45-alpine`

**does not exist** (yet?)

## `rust:1.45-alpine3.11`

**does not exist** (yet?)

## `rust:1.45-alpine3.12`

**does not exist** (yet?)

## `rust:1.45-buster`

**does not exist** (yet?)

## `rust:1.45-slim`

**does not exist** (yet?)

## `rust:1.45-slim-buster`

**does not exist** (yet?)

## `rust:1.45-slim-stretch`

**does not exist** (yet?)

## `rust:1.45-stretch`

**does not exist** (yet?)

## `rust:1-alpine`

```console
$ docker pull rust@sha256:544a9764c44b5a8f9de47dd3309151551b504e5b738579050d228a4e106dd594
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1-alpine` - linux; amd64

```console
$ docker pull rust@sha256:84783d5b9c9de0f38943e74d83eac5006728f5f3238ae73710ee519841629353
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175116033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15e5444ace0262a28b8594d6fe6d83da28d1b602294896c7ed70626a1c4d7331`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 18 Jun 2020 19:22:19 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 18 Jun 2020 19:22:19 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:22:35 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.21.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "0c86d467982bdf5c4b8d844bf8c3f7fc602cc4ac30b29262b8941d6d8b363d7e *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e80d17ab1e216ced34af8e4c92cbdcb53881599ae0a364b0de54ceafa10317`  
		Last Modified: Thu, 18 Jun 2020 19:25:47 GMT  
		Size: 47.6 MB (47612931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b07be5d9c15bd4c659d1629e62e614764cba4806aa02a7a078fbbae6b5b5ff`  
		Last Modified: Thu, 18 Jun 2020 19:25:59 GMT  
		Size: 124.7 MB (124705561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-alpine3.11`

```console
$ docker pull rust@sha256:5c6ea80f0383c487c27f483c63a322692095c7edc3a68626d2c6dbedb6f5f124
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1-alpine3.11` - linux; amd64

```console
$ docker pull rust@sha256:1968d4f2160449e0030099a7b638d1245a16247a54751166f4391b38d9da9a09
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.9 MB (163935516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7908f9163e8ad9f810645513206893baf01c00fd82a1de93205d685ded00b43`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:43:51 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 18 Jun 2020 19:21:59 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:22:11 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.21.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "0c86d467982bdf5c4b8d844bf8c3f7fc602cc4ac30b29262b8941d6d8b363d7e *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5d358e115edba184c114de906d7594bdb0932b1e9b313cbe6e692e3ed53edd`  
		Last Modified: Fri, 24 Apr 2020 12:45:08 GMT  
		Size: 36.4 MB (36416643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68834f533d5ab3bf8086d4400cc42d8eb1c89b5fa06b12992639159963581165`  
		Last Modified: Thu, 18 Jun 2020 19:25:31 GMT  
		Size: 124.7 MB (124705557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-alpine3.12`

```console
$ docker pull rust@sha256:544a9764c44b5a8f9de47dd3309151551b504e5b738579050d228a4e106dd594
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1-alpine3.12` - linux; amd64

```console
$ docker pull rust@sha256:84783d5b9c9de0f38943e74d83eac5006728f5f3238ae73710ee519841629353
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175116033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15e5444ace0262a28b8594d6fe6d83da28d1b602294896c7ed70626a1c4d7331`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 18 Jun 2020 19:22:19 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 18 Jun 2020 19:22:19 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:22:35 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.21.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "0c86d467982bdf5c4b8d844bf8c3f7fc602cc4ac30b29262b8941d6d8b363d7e *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e80d17ab1e216ced34af8e4c92cbdcb53881599ae0a364b0de54ceafa10317`  
		Last Modified: Thu, 18 Jun 2020 19:25:47 GMT  
		Size: 47.6 MB (47612931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b07be5d9c15bd4c659d1629e62e614764cba4806aa02a7a078fbbae6b5b5ff`  
		Last Modified: Thu, 18 Jun 2020 19:25:59 GMT  
		Size: 124.7 MB (124705561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-buster`

```console
$ docker pull rust@sha256:ee8f52372784746235500f9ee80685337a61dcde5e0d028a2aa955d15b6defc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-buster` - linux; amd64

```console
$ docker pull rust@sha256:b2fd2fcc9d28c1a6dc59c3b0b37913fd9a326c8e457e50617e1156fc1ad51e34
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **447.5 MB (447532458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be36dd54f964afeab7f33a72c583e81294fa2deab3fa05f73453209d3d57e199`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:39 GMT
ADD file:1ab357efe422cfed5e37af2dc60d07ccfd4bdee4d4a0c00838b5d68f19ff20c7 in / 
# Tue, 09 Jun 2020 01:20:39 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:47:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:48:00 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Jun 2020 19:21:04 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:21:18 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:e9afc4f90ab09248d75c8081b6dfba749a7f7efdac704ced7e0ceb506e02fa4a`  
		Last Modified: Tue, 09 Jun 2020 01:25:37 GMT  
		Size: 50.4 MB (50389504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e6b19a265d6b8b7934e7ddd7dc07f6e2fc945b3a28dda9b8aecb12cdb30e0`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 7.8 MB (7811709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14b6c2f8785723bceb5964c5dec1f0489b7750e9d4ec671e49bfba15d80a39`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 10.0 MB (9996168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5573c4b3094956931fd68c310ae92c9eb1a787f0c77ac2730be9d16cce172d5e`  
		Last Modified: Tue, 09 Jun 2020 02:00:08 GMT  
		Size: 51.8 MB (51827493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a88e76431345b48525c4e4d58d497810019f4bafdb5e2bd56dc34a05e09cc3`  
		Last Modified: Tue, 09 Jun 2020 02:00:47 GMT  
		Size: 192.2 MB (192214313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2afbc28d89df4b6fb2dc20541f4233efb213257aafdcfa2b4bb4290983e3ec6`  
		Last Modified: Thu, 18 Jun 2020 19:24:24 GMT  
		Size: 135.3 MB (135293271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:2a52a967c9b16f19fcc004490f7837ac612a0bb8da50858670f725e0796b4bc9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.4 MB (426430312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3e404c4c716a199bea9faa5dbdd48d89dac55e6b5496c8b944755a6f013054c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:00:40 GMT
ADD file:35073a186411c4b773a9d4d540ec0693ced845cb847b43d8465f9579174cd2b0 in / 
# Tue, 09 Jun 2020 01:00:45 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:48:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:52:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Jun 2020 19:13:13 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:13:42 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:cff0731da2e4f4a0ae8329840eb7fed7ea6aac11aecbfa15c6e684caec03920d`  
		Last Modified: Tue, 09 Jun 2020 01:09:57 GMT  
		Size: 45.9 MB (45868949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbeb0ded58d68be17265763fda36a4e1a520234a291d66f370d98a3e0d6e591`  
		Last Modified: Tue, 09 Jun 2020 02:11:21 GMT  
		Size: 7.1 MB (7097860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6159fbed770bb99a219eae06828da55caaa649879843c0b9df18ddda9b698b3`  
		Last Modified: Tue, 09 Jun 2020 02:11:20 GMT  
		Size: 9.3 MB (9343524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba732bafeb6b1467fd6908c64c6e8d10ffb27e44e3a25ab4c6c38e8f753baa5`  
		Last Modified: Tue, 09 Jun 2020 02:11:43 GMT  
		Size: 47.4 MB (47356467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d84f63917d0e3fb79c2b4c16f4595b8db444749589cfd28a57ef31188ab110`  
		Last Modified: Tue, 09 Jun 2020 02:12:32 GMT  
		Size: 168.4 MB (168420423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a94607ffab11c3cf1fb6f417882b1d8edc34360eb1e13530cb3170ab34cb57`  
		Last Modified: Thu, 18 Jun 2020 19:19:31 GMT  
		Size: 148.3 MB (148343089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:623732a5a57084e4da5db6732e4bc7578a425b95e6ffbbb59f0d5bdbd76433b4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **447.7 MB (447665351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddb6fcb343548fe6b5044b7778f1c7c05867e46be852e56f8c39cbbcd38754bb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:51:33 GMT
ADD file:73f1cc6ac15b24788e78ae41cd6c89cb5211d64baf491accbd95b6fe9718f17f in / 
# Tue, 09 Jun 2020 01:51:36 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:31:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:32:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:32:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:35:00 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 19 Jun 2020 00:04:43 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Fri, 19 Jun 2020 00:04:59 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:1db90d3d3b6598d485690f804e96153fb632e7434251d334e9a0c49b773855c9`  
		Last Modified: Tue, 09 Jun 2020 01:57:52 GMT  
		Size: 49.2 MB (49167914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e848fd373270c8ed6d276649dd8a5860d188f7d0ff306e91e4e3e092e541d99`  
		Last Modified: Tue, 09 Jun 2020 02:47:16 GMT  
		Size: 7.7 MB (7681351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c85f14a5d8064020366c03aa05ec1c8b0f731e0966bb9788960d27258634aef`  
		Last Modified: Tue, 09 Jun 2020 02:47:16 GMT  
		Size: 10.0 MB (9983910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334e38f2d6fff7c08f4ad1b38ec441d2cf963b761b5d85983396a75ff6d0c08f`  
		Last Modified: Tue, 09 Jun 2020 02:47:41 GMT  
		Size: 52.2 MB (52156256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326561827fde74d56d06dce7035ef6653dbf62a27a5dc35416ba6f00293a09b8`  
		Last Modified: Tue, 09 Jun 2020 02:48:39 GMT  
		Size: 183.7 MB (183744170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef821eade6b1f26263a9104496d7c6527232a00c8ecfa0aab6868fc10d480c9`  
		Last Modified: Fri, 19 Jun 2020 00:08:45 GMT  
		Size: 144.9 MB (144931750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-buster` - linux; 386

```console
$ docker pull rust@sha256:3f45b9475ee12ddc57e3de3a547e246e4441144975e665c9cfce651ba4bf1138
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **472.8 MB (472818538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f861e1f7ab671dcb926e2bd5fcacc831bcc72d0c99ecaf10f37719aae3f3a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:39:33 GMT
ADD file:f95fda6e1e7823d93ca50dd67a1ab99bdc8a7dea372ef27426915702500d54a2 in / 
# Tue, 09 Jun 2020 01:39:33 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:11:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:11:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:12:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:13:11 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Jun 2020 20:10:36 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 20:10:55 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:ca172633df711443e1bcc46650b24074efa097045feee542ecbb4934ae3ae01b`  
		Last Modified: Tue, 09 Jun 2020 01:44:44 GMT  
		Size: 51.2 MB (51156157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e4e2e742db8627ba5d7e0f076114e90c4fea4407cedd3599355e4c00828543`  
		Last Modified: Tue, 09 Jun 2020 02:32:03 GMT  
		Size: 8.0 MB (7981054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ba43d083b56bb094a5bac45d723e9bec0fe65d033950b3c4dc392e890c7e41`  
		Last Modified: Tue, 09 Jun 2020 02:32:03 GMT  
		Size: 10.3 MB (10338453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2391b0310a0be022e7ac6e202273ea7cc0ac5f16e862e5cb19c43c5db30b5b`  
		Last Modified: Tue, 09 Jun 2020 02:32:24 GMT  
		Size: 53.4 MB (53429728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3e805e55983a46c901632f289542625edb04ff470dc6dd9217466a3788d608`  
		Last Modified: Tue, 09 Jun 2020 02:33:23 GMT  
		Size: 198.8 MB (198755099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbce41824f90111fafebb16091199a32fe6de31d201a9cb9384f485fe5fb5de`  
		Last Modified: Thu, 18 Jun 2020 20:13:59 GMT  
		Size: 151.2 MB (151158047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-slim`

```console
$ docker pull rust@sha256:523456288f840fff23dcb1c29b3b8e646f71692d7f1c87bdd3f46b238621564b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-slim` - linux; amd64

```console
$ docker pull rust@sha256:354b345047ce24c3b879e4427ab1662f608c6a0f6c6ac08ef22a971dfdc3056e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.8 MB (207775593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a62af5c181f94d6dab0a455f90ff60d89533df670387ad05da3efcbd05604cf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:56 GMT
ADD file:4d35f6c8bbbe6801cc5f44989730fb6d349a644ecb36eca481e7df25842d6321 in / 
# Tue, 09 Jun 2020 01:20:56 GMT
CMD ["bash"]
# Thu, 18 Jun 2020 19:21:25 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:21:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:8559a31e96f442f2c7b6da49d6c84705f98a39d8be10b3f5f14821d0ee8417df`  
		Last Modified: Tue, 09 Jun 2020 01:25:50 GMT  
		Size: 27.1 MB (27098265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7d2123b96d6ae88d4ff7f4877c9979291967c9fe883cf38e086eeecc005131`  
		Last Modified: Thu, 18 Jun 2020 19:25:01 GMT  
		Size: 180.7 MB (180677328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim` - linux; arm variant v7

```console
$ docker pull rust@sha256:aef5e2e31a2962e3bc789b16a201df05f3891c8b6351e479ca235de0130fe842
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.9 MB (203947983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd3f2aae154d9d951d006d68c69e2e23d2588da7fd7787f948786f80f7f28d65`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:01:24 GMT
ADD file:a35ca31d2a743d6a1738b1652f4f06c789abbca314d120f0e7e748311ac09ed2 in / 
# Tue, 09 Jun 2020 01:01:30 GMT
CMD ["bash"]
# Thu, 18 Jun 2020 19:13:55 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:15:12 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:2dd003996c9ab82cac8112be0a4c04068e666e7a5d0cce3c65fb8f064de284e7`  
		Last Modified: Tue, 09 Jun 2020 01:10:25 GMT  
		Size: 22.7 MB (22705913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2123881e25542ae72b234649c763a7dfd2fd2058718602a4c9607ac6d57f7f`  
		Last Modified: Thu, 18 Jun 2020 19:20:33 GMT  
		Size: 181.2 MB (181242070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:92e0980cc684e652780a18ff7c064d5ef48775c46bff3dc22cc2d0e246568104
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.0 MB (210995124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1c0f5b7156a169a8083b7ea19ca95d8524073d7e526d8a2e478344adfcf5df9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:52:01 GMT
ADD file:98823648634dfc3af50862b1e2da1028b23996a37adf43b1b0c3c5b29e94b9c7 in / 
# Tue, 09 Jun 2020 01:52:04 GMT
CMD ["bash"]
# Fri, 19 Jun 2020 00:05:08 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Fri, 19 Jun 2020 00:05:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:33cc09c9b190539635d7c971301f623d94fda5b4b5647966c6c240902119009f`  
		Last Modified: Tue, 09 Jun 2020 01:58:14 GMT  
		Size: 25.9 MB (25857704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d4ea274349b38ba3d5b60affc7a3766710f53401f8d9a79792d5be308d6796`  
		Last Modified: Fri, 19 Jun 2020 00:09:47 GMT  
		Size: 185.1 MB (185137420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim` - linux; 386

```console
$ docker pull rust@sha256:6a71e80ff8fa21bb1a5acfee60e064f9a7d5632b257e4b8fee5d8a4dac7ca3d1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.9 MB (228879583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:145755b52ab3753e5762ce9454078790ae2ab87eb619ea2b58da393ea2601505`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:39:49 GMT
ADD file:9fb8fd8bf970c4134f555964fe485a3baa84f1d4c91c5aa35276c24404de9d5d in / 
# Tue, 09 Jun 2020 01:39:49 GMT
CMD ["bash"]
# Thu, 18 Jun 2020 20:11:06 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 20:11:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:860f8957d8be856e2235a28e49fc4dca17254951e0eb67d760769755656f5cad`  
		Last Modified: Tue, 09 Jun 2020 01:45:01 GMT  
		Size: 27.8 MB (27754909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8cbd90acddf34fb55f7c0859346ae57ddea6a96ace0a02fdca617f1a997879`  
		Last Modified: Thu, 18 Jun 2020 20:14:52 GMT  
		Size: 201.1 MB (201124674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-slim-buster`

```console
$ docker pull rust@sha256:523456288f840fff23dcb1c29b3b8e646f71692d7f1c87bdd3f46b238621564b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-slim-buster` - linux; amd64

```console
$ docker pull rust@sha256:354b345047ce24c3b879e4427ab1662f608c6a0f6c6ac08ef22a971dfdc3056e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.8 MB (207775593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a62af5c181f94d6dab0a455f90ff60d89533df670387ad05da3efcbd05604cf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:56 GMT
ADD file:4d35f6c8bbbe6801cc5f44989730fb6d349a644ecb36eca481e7df25842d6321 in / 
# Tue, 09 Jun 2020 01:20:56 GMT
CMD ["bash"]
# Thu, 18 Jun 2020 19:21:25 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:21:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:8559a31e96f442f2c7b6da49d6c84705f98a39d8be10b3f5f14821d0ee8417df`  
		Last Modified: Tue, 09 Jun 2020 01:25:50 GMT  
		Size: 27.1 MB (27098265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7d2123b96d6ae88d4ff7f4877c9979291967c9fe883cf38e086eeecc005131`  
		Last Modified: Thu, 18 Jun 2020 19:25:01 GMT  
		Size: 180.7 MB (180677328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:aef5e2e31a2962e3bc789b16a201df05f3891c8b6351e479ca235de0130fe842
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.9 MB (203947983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd3f2aae154d9d951d006d68c69e2e23d2588da7fd7787f948786f80f7f28d65`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:01:24 GMT
ADD file:a35ca31d2a743d6a1738b1652f4f06c789abbca314d120f0e7e748311ac09ed2 in / 
# Tue, 09 Jun 2020 01:01:30 GMT
CMD ["bash"]
# Thu, 18 Jun 2020 19:13:55 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:15:12 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:2dd003996c9ab82cac8112be0a4c04068e666e7a5d0cce3c65fb8f064de284e7`  
		Last Modified: Tue, 09 Jun 2020 01:10:25 GMT  
		Size: 22.7 MB (22705913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2123881e25542ae72b234649c763a7dfd2fd2058718602a4c9607ac6d57f7f`  
		Last Modified: Thu, 18 Jun 2020 19:20:33 GMT  
		Size: 181.2 MB (181242070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:92e0980cc684e652780a18ff7c064d5ef48775c46bff3dc22cc2d0e246568104
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.0 MB (210995124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1c0f5b7156a169a8083b7ea19ca95d8524073d7e526d8a2e478344adfcf5df9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:52:01 GMT
ADD file:98823648634dfc3af50862b1e2da1028b23996a37adf43b1b0c3c5b29e94b9c7 in / 
# Tue, 09 Jun 2020 01:52:04 GMT
CMD ["bash"]
# Fri, 19 Jun 2020 00:05:08 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Fri, 19 Jun 2020 00:05:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:33cc09c9b190539635d7c971301f623d94fda5b4b5647966c6c240902119009f`  
		Last Modified: Tue, 09 Jun 2020 01:58:14 GMT  
		Size: 25.9 MB (25857704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d4ea274349b38ba3d5b60affc7a3766710f53401f8d9a79792d5be308d6796`  
		Last Modified: Fri, 19 Jun 2020 00:09:47 GMT  
		Size: 185.1 MB (185137420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-buster` - linux; 386

```console
$ docker pull rust@sha256:6a71e80ff8fa21bb1a5acfee60e064f9a7d5632b257e4b8fee5d8a4dac7ca3d1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.9 MB (228879583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:145755b52ab3753e5762ce9454078790ae2ab87eb619ea2b58da393ea2601505`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:39:49 GMT
ADD file:9fb8fd8bf970c4134f555964fe485a3baa84f1d4c91c5aa35276c24404de9d5d in / 
# Tue, 09 Jun 2020 01:39:49 GMT
CMD ["bash"]
# Thu, 18 Jun 2020 20:11:06 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 20:11:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:860f8957d8be856e2235a28e49fc4dca17254951e0eb67d760769755656f5cad`  
		Last Modified: Tue, 09 Jun 2020 01:45:01 GMT  
		Size: 27.8 MB (27754909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8cbd90acddf34fb55f7c0859346ae57ddea6a96ace0a02fdca617f1a997879`  
		Last Modified: Thu, 18 Jun 2020 20:14:52 GMT  
		Size: 201.1 MB (201124674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-slim-stretch`

```console
$ docker pull rust@sha256:66456b3359fa48c9741ea86ba14effb5da705ce0fb4403015106ae8081ea5f5b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-slim-stretch` - linux; amd64

```console
$ docker pull rust@sha256:61df4b3040afc761017728188a9652bb6474b6205c7c34e8cd57a09d8dfe2c72
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.6 MB (195632258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9439f1d88c5c7b12b9806640caf78d6d530161280c3a2d5f578e85d74d0d2bbb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:35 GMT
ADD file:57b431451a292755d0f13673f5f3bea9f62aea36c7a1b59d34d7d200ba134fea in / 
# Tue, 09 Jun 2020 01:23:35 GMT
CMD ["bash"]
# Thu, 18 Jun 2020 19:20:27 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:20:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:7d2977b12acb33f192e3f20b7e15a467cc8f3f5124a15d975a6d4afe5fa3d258`  
		Last Modified: Tue, 09 Jun 2020 01:28:13 GMT  
		Size: 22.5 MB (22519600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f7ede80e96e0566399789a2786eecfb4c5f9c3604a881b446a32db6f01ec91`  
		Last Modified: Thu, 18 Jun 2020 19:23:53 GMT  
		Size: 173.1 MB (173112658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-stretch` - linux; arm variant v7

```console
$ docker pull rust@sha256:f79d863d88d0ff84fc76d7221f47420ee810de67430a30ad93d8b359e32d1214
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.7 MB (195669366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeaf868781e3933ea7563493f08a9248af68cb49350a0de81a2b2264c54d9c25`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:35 GMT
ADD file:4a0a863669948b35130fcf8cdb52999c49f7b3ee0620a1eef5f1a2e850a42f05 in / 
# Tue, 09 Jun 2020 01:06:37 GMT
CMD ["bash"]
# Thu, 18 Jun 2020 18:58:54 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:12:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:c439312a9c212b64af3c38cb326bb5fbe14bcf4a622115d59d44985e949bee82`  
		Last Modified: Tue, 09 Jun 2020 01:13:51 GMT  
		Size: 19.3 MB (19304370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353546c552425fb49ffeef7c3895693859ba33fa54bfcac5c3d4bd6952341b98`  
		Last Modified: Thu, 18 Jun 2020 19:18:33 GMT  
		Size: 176.4 MB (176364996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-stretch` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:efc8bfaf58df25ef6432a6e9312dc1807c3e00716205c72d00e4cfc57f18626c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.9 MB (195882477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6b524283c8151ca7dcd99551a7e271f36d232e5c65e97ce914344589814f324`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:49 GMT
ADD file:c85d28567b6123deb660b71c8b60d92378b5ba15ba5dcf495d9388817dc3aa44 in / 
# Tue, 09 Jun 2020 01:54:52 GMT
CMD ["bash"]
# Fri, 19 Jun 2020 00:03:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Fri, 19 Jun 2020 00:04:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:622dc742b82743ebf5607b215a65869096390ee41b0a61b5532f859fb94590b1`  
		Last Modified: Tue, 09 Jun 2020 02:00:28 GMT  
		Size: 20.4 MB (20375150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08568b0762f6b468d5d9fafe63b44e4f986a3dd82e31e85c68555345a0e146a2`  
		Last Modified: Fri, 19 Jun 2020 00:07:57 GMT  
		Size: 175.5 MB (175507327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-stretch` - linux; 386

```console
$ docker pull rust@sha256:9fc333d7b32f1389d3e066f162a4fa9dc6bb38537b0fab187906ff352d6bac27
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.1 MB (216130114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9ea2784f298048053574227bbc7d3fcb3c814eb375848e38be19f7f561450cd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:33 GMT
ADD file:8ef252685ffefc58654053bf145c830928a2cf423a6c757180649df772f1523d in / 
# Tue, 09 Jun 2020 01:42:34 GMT
CMD ["bash"]
# Thu, 18 Jun 2020 20:09:57 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 20:10:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:4ffbd6ec7974e514763a8d7d9fcf5e86e9440e2280e6e9561ea373b4bc50588e`  
		Last Modified: Tue, 09 Jun 2020 01:48:28 GMT  
		Size: 23.1 MB (23147892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff582d7ea58b49b27d3241c60c89aa592dde236d70e301e5099469f2a5fb6c54`  
		Last Modified: Thu, 18 Jun 2020 20:13:21 GMT  
		Size: 193.0 MB (192982222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-stretch`

```console
$ docker pull rust@sha256:07afa12e396109dd20c19193c6ced45a8988437fdfc6a084877b77af0a5aaef3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-stretch` - linux; amd64

```console
$ docker pull rust@sha256:cd0d96614c172237a7b782fc090733f3c12922fb29e3c064e8fe34453ac01b99
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **460.7 MB (460749631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de3ffe48a60a6c9bed849ef957b32f4172727e445e52eb24b7ece05596362a98`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:20 GMT
ADD file:6e16bc9cf28c19a1fb1fb516411643e33cbd2bdb7b6c2ce2468c6583c89871a2 in / 
# Tue, 09 Jun 2020 01:23:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:56:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:56:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:56:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:57:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Jun 2020 19:20:08 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:20:21 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:81fc1918191541a2ffb6ed1cd8386ef8302aea1b0613ebc768a00e76c1f34bb9`  
		Last Modified: Tue, 09 Jun 2020 01:27:59 GMT  
		Size: 45.4 MB (45375796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee49ee6a23d1c7e6b8b574c905dcd4a53efb869a539a957d3e47bc3698f01dc8`  
		Last Modified: Tue, 09 Jun 2020 02:02:39 GMT  
		Size: 10.7 MB (10749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82851092453815ec861754ded7101fcfa3b648d09a0818ced17ea80478f179a3`  
		Last Modified: Tue, 09 Jun 2020 02:02:38 GMT  
		Size: 4.3 MB (4339890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8f58c4fcca04f9622e97db77618075b618c24a58cce6c6860ca54c9a887745b`  
		Last Modified: Tue, 09 Jun 2020 02:02:52 GMT  
		Size: 50.1 MB (50082718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33699d7df21edc5ded5b679bc283e5890ed92c5bf20e53b48edcd9096c8a5962`  
		Last Modified: Tue, 09 Jun 2020 02:03:29 GMT  
		Size: 214.9 MB (214908336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baab346e84a2b6df78d07068567a9ebce0a2a15654279dcf576eec30d4a65367`  
		Last Modified: Thu, 18 Jun 2020 19:23:17 GMT  
		Size: 135.3 MB (135293871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-stretch` - linux; arm variant v7

```console
$ docker pull rust@sha256:3931004840e50e226b226a792a3255f4521ff543189500f17c31e6bc57d10725
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **445.8 MB (445787888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f9d65523682d96797f6e5ee80817988c61149f89eb4aedb09ee5dfec099d287`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:07 GMT
ADD file:c0b9ed1244ec0acfc9054c7cb80c768878e3da99740f981ba3a82bdd854305db in / 
# Tue, 09 Jun 2020 01:06:09 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:02:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:02:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:03:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:06:20 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Jun 2020 18:58:22 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 18:58:47 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:2566ca784846d2d0d4f9105084d94d68d8ea1a82a06a76c5bcd991ce5a10cda1`  
		Last Modified: Tue, 09 Jun 2020 01:13:35 GMT  
		Size: 42.1 MB (42102504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f976b5a12722f5e6e115157695654d36452b713c7fa64a860f8c9e14859402`  
		Last Modified: Tue, 09 Jun 2020 02:15:15 GMT  
		Size: 9.4 MB (9443335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35142ef6ea6c722cd0397799ab151e5da354eabc784b3acef29def7fa34e9bc`  
		Last Modified: Tue, 09 Jun 2020 02:15:13 GMT  
		Size: 3.9 MB (3918433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7773eda6b7a8801a6f09bd4ce443b7e88397ed16265ecd37f55af57db56c4658`  
		Last Modified: Tue, 09 Jun 2020 02:15:36 GMT  
		Size: 46.4 MB (46412697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf8c80047f39ca1669cf85bbab477a59e35f498d269e058afe91bf9850b7c52`  
		Last Modified: Tue, 09 Jun 2020 02:16:37 GMT  
		Size: 195.6 MB (195567505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74835fe8def5171fad1b8ae2b6f7d7c9051db5b7ba498e5c87bd601fcd4041e6`  
		Last Modified: Thu, 18 Jun 2020 19:16:16 GMT  
		Size: 148.3 MB (148343414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-stretch` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:ec2aae4f393360361384ad0e9abfc76a04f45f4415697265f80bd20fb7260d0c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **452.2 MB (452205272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1953029c1c941d34c706d21c87d82b81ce8b88ec5a840e0bcca3073f08436f52`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:22 GMT
ADD file:5cbf00485aed776e940988cadfad6853c640c13635ae54fb2b00aafccfe81a73 in / 
# Tue, 09 Jun 2020 01:54:25 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:39:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:40:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:43:35 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 19 Jun 2020 00:02:56 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Fri, 19 Jun 2020 00:03:15 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:4c4f692ec920eecb1f30d9ef8e50125217decc872d7ada6eeccc36c6dcb49e4d`  
		Last Modified: Tue, 09 Jun 2020 02:00:09 GMT  
		Size: 43.2 MB (43160923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0990c417a21ef9e268cc0822cd23968c4b17cded8170cce0c4d8f7e020e6fd`  
		Last Modified: Tue, 09 Jun 2020 02:50:17 GMT  
		Size: 9.7 MB (9699635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6b83fd41426d182f67fdac882a6bfcd3aad22d7226a653ae58d3046bd46b5e`  
		Last Modified: Tue, 09 Jun 2020 02:50:15 GMT  
		Size: 4.1 MB (4094104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2de3ad924e80f0d130d0bd9ed8ea866eefeb610874bce14fd8347d032772220`  
		Last Modified: Tue, 09 Jun 2020 02:50:36 GMT  
		Size: 48.0 MB (48034909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2720149da5321de7d3e31500696a088aae1c37ededd1680245aec1602c17c5`  
		Last Modified: Tue, 09 Jun 2020 02:51:32 GMT  
		Size: 202.3 MB (202283682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbefd35906cd779827ad7f0c9e26f349577d819f8d6901f51bf43e7cb8028b38`  
		Last Modified: Fri, 19 Jun 2020 00:06:57 GMT  
		Size: 144.9 MB (144932019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-stretch` - linux; 386

```console
$ docker pull rust@sha256:fb7764674949cf00a03a2b2cffd76e9757fed14e6d19c81ddb2d22e58e51e59f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.2 MB (484164275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0330c79b62c3998719e33191ce6cbdef2a0cbfe312f93af6145ec9bddde4aff0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:17 GMT
ADD file:6bbeeb0773b96fccb4cd5ba81dd19ec3580f8d8a3cdd3f1d6a3d2b514fbd6eb1 in / 
# Tue, 09 Jun 2020 01:42:18 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:26:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:26:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:27:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:28:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Jun 2020 20:09:35 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 20:09:53 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9e88f215fab896e3a7d1d2ce75c0d79960b236066e9033b97e76ca7f01ff2fdc`  
		Last Modified: Tue, 09 Jun 2020 01:48:12 GMT  
		Size: 46.1 MB (46094854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1130784446f3179c75741e18b159e7bca5d46db60bb1f9f57d67953023a50899`  
		Last Modified: Tue, 09 Jun 2020 02:37:03 GMT  
		Size: 10.8 MB (10772863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e32fbc0a9c533b460544bce821a796b4f02dd4da61100073a18fba329807ae`  
		Last Modified: Tue, 09 Jun 2020 02:37:01 GMT  
		Size: 4.6 MB (4561121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e9df71276e8af2305be9b32aca4dd788168bd7fe3c6029ddd8e4e8057f7d33`  
		Last Modified: Tue, 09 Jun 2020 02:37:31 GMT  
		Size: 51.6 MB (51615859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c496d702f58d364bb0ec81531f18a35844eb95f0f9e0dff097b6588eaa8fb7`  
		Last Modified: Tue, 09 Jun 2020 02:38:54 GMT  
		Size: 220.0 MB (219960753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399d9f86bb9f3cf9ef83ed8d3c204b9f1b9283c169ed9e53a8f4fa399cd3c571`  
		Last Modified: Thu, 18 Jun 2020 20:12:29 GMT  
		Size: 151.2 MB (151158825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:alpine`

```console
$ docker pull rust@sha256:544a9764c44b5a8f9de47dd3309151551b504e5b738579050d228a4e106dd594
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:alpine` - linux; amd64

```console
$ docker pull rust@sha256:84783d5b9c9de0f38943e74d83eac5006728f5f3238ae73710ee519841629353
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175116033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15e5444ace0262a28b8594d6fe6d83da28d1b602294896c7ed70626a1c4d7331`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 18 Jun 2020 19:22:19 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 18 Jun 2020 19:22:19 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:22:35 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.21.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "0c86d467982bdf5c4b8d844bf8c3f7fc602cc4ac30b29262b8941d6d8b363d7e *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e80d17ab1e216ced34af8e4c92cbdcb53881599ae0a364b0de54ceafa10317`  
		Last Modified: Thu, 18 Jun 2020 19:25:47 GMT  
		Size: 47.6 MB (47612931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b07be5d9c15bd4c659d1629e62e614764cba4806aa02a7a078fbbae6b5b5ff`  
		Last Modified: Thu, 18 Jun 2020 19:25:59 GMT  
		Size: 124.7 MB (124705561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:alpine3.11`

```console
$ docker pull rust@sha256:5c6ea80f0383c487c27f483c63a322692095c7edc3a68626d2c6dbedb6f5f124
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:alpine3.11` - linux; amd64

```console
$ docker pull rust@sha256:1968d4f2160449e0030099a7b638d1245a16247a54751166f4391b38d9da9a09
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.9 MB (163935516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7908f9163e8ad9f810645513206893baf01c00fd82a1de93205d685ded00b43`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:43:51 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 18 Jun 2020 19:21:59 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:22:11 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.21.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "0c86d467982bdf5c4b8d844bf8c3f7fc602cc4ac30b29262b8941d6d8b363d7e *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5d358e115edba184c114de906d7594bdb0932b1e9b313cbe6e692e3ed53edd`  
		Last Modified: Fri, 24 Apr 2020 12:45:08 GMT  
		Size: 36.4 MB (36416643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68834f533d5ab3bf8086d4400cc42d8eb1c89b5fa06b12992639159963581165`  
		Last Modified: Thu, 18 Jun 2020 19:25:31 GMT  
		Size: 124.7 MB (124705557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:alpine3.12`

```console
$ docker pull rust@sha256:544a9764c44b5a8f9de47dd3309151551b504e5b738579050d228a4e106dd594
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:alpine3.12` - linux; amd64

```console
$ docker pull rust@sha256:84783d5b9c9de0f38943e74d83eac5006728f5f3238ae73710ee519841629353
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175116033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15e5444ace0262a28b8594d6fe6d83da28d1b602294896c7ed70626a1c4d7331`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 18 Jun 2020 19:22:19 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 18 Jun 2020 19:22:19 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:22:35 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.21.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "0c86d467982bdf5c4b8d844bf8c3f7fc602cc4ac30b29262b8941d6d8b363d7e *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e80d17ab1e216ced34af8e4c92cbdcb53881599ae0a364b0de54ceafa10317`  
		Last Modified: Thu, 18 Jun 2020 19:25:47 GMT  
		Size: 47.6 MB (47612931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b07be5d9c15bd4c659d1629e62e614764cba4806aa02a7a078fbbae6b5b5ff`  
		Last Modified: Thu, 18 Jun 2020 19:25:59 GMT  
		Size: 124.7 MB (124705561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:buster`

```console
$ docker pull rust@sha256:ee8f52372784746235500f9ee80685337a61dcde5e0d028a2aa955d15b6defc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:buster` - linux; amd64

```console
$ docker pull rust@sha256:b2fd2fcc9d28c1a6dc59c3b0b37913fd9a326c8e457e50617e1156fc1ad51e34
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **447.5 MB (447532458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be36dd54f964afeab7f33a72c583e81294fa2deab3fa05f73453209d3d57e199`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:39 GMT
ADD file:1ab357efe422cfed5e37af2dc60d07ccfd4bdee4d4a0c00838b5d68f19ff20c7 in / 
# Tue, 09 Jun 2020 01:20:39 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:47:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:48:00 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Jun 2020 19:21:04 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:21:18 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:e9afc4f90ab09248d75c8081b6dfba749a7f7efdac704ced7e0ceb506e02fa4a`  
		Last Modified: Tue, 09 Jun 2020 01:25:37 GMT  
		Size: 50.4 MB (50389504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e6b19a265d6b8b7934e7ddd7dc07f6e2fc945b3a28dda9b8aecb12cdb30e0`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 7.8 MB (7811709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14b6c2f8785723bceb5964c5dec1f0489b7750e9d4ec671e49bfba15d80a39`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 10.0 MB (9996168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5573c4b3094956931fd68c310ae92c9eb1a787f0c77ac2730be9d16cce172d5e`  
		Last Modified: Tue, 09 Jun 2020 02:00:08 GMT  
		Size: 51.8 MB (51827493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a88e76431345b48525c4e4d58d497810019f4bafdb5e2bd56dc34a05e09cc3`  
		Last Modified: Tue, 09 Jun 2020 02:00:47 GMT  
		Size: 192.2 MB (192214313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2afbc28d89df4b6fb2dc20541f4233efb213257aafdcfa2b4bb4290983e3ec6`  
		Last Modified: Thu, 18 Jun 2020 19:24:24 GMT  
		Size: 135.3 MB (135293271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:2a52a967c9b16f19fcc004490f7837ac612a0bb8da50858670f725e0796b4bc9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.4 MB (426430312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3e404c4c716a199bea9faa5dbdd48d89dac55e6b5496c8b944755a6f013054c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:00:40 GMT
ADD file:35073a186411c4b773a9d4d540ec0693ced845cb847b43d8465f9579174cd2b0 in / 
# Tue, 09 Jun 2020 01:00:45 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:48:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:52:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Jun 2020 19:13:13 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:13:42 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:cff0731da2e4f4a0ae8329840eb7fed7ea6aac11aecbfa15c6e684caec03920d`  
		Last Modified: Tue, 09 Jun 2020 01:09:57 GMT  
		Size: 45.9 MB (45868949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbeb0ded58d68be17265763fda36a4e1a520234a291d66f370d98a3e0d6e591`  
		Last Modified: Tue, 09 Jun 2020 02:11:21 GMT  
		Size: 7.1 MB (7097860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6159fbed770bb99a219eae06828da55caaa649879843c0b9df18ddda9b698b3`  
		Last Modified: Tue, 09 Jun 2020 02:11:20 GMT  
		Size: 9.3 MB (9343524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba732bafeb6b1467fd6908c64c6e8d10ffb27e44e3a25ab4c6c38e8f753baa5`  
		Last Modified: Tue, 09 Jun 2020 02:11:43 GMT  
		Size: 47.4 MB (47356467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d84f63917d0e3fb79c2b4c16f4595b8db444749589cfd28a57ef31188ab110`  
		Last Modified: Tue, 09 Jun 2020 02:12:32 GMT  
		Size: 168.4 MB (168420423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a94607ffab11c3cf1fb6f417882b1d8edc34360eb1e13530cb3170ab34cb57`  
		Last Modified: Thu, 18 Jun 2020 19:19:31 GMT  
		Size: 148.3 MB (148343089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:623732a5a57084e4da5db6732e4bc7578a425b95e6ffbbb59f0d5bdbd76433b4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **447.7 MB (447665351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddb6fcb343548fe6b5044b7778f1c7c05867e46be852e56f8c39cbbcd38754bb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:51:33 GMT
ADD file:73f1cc6ac15b24788e78ae41cd6c89cb5211d64baf491accbd95b6fe9718f17f in / 
# Tue, 09 Jun 2020 01:51:36 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:31:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:32:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:32:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:35:00 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 19 Jun 2020 00:04:43 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Fri, 19 Jun 2020 00:04:59 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:1db90d3d3b6598d485690f804e96153fb632e7434251d334e9a0c49b773855c9`  
		Last Modified: Tue, 09 Jun 2020 01:57:52 GMT  
		Size: 49.2 MB (49167914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e848fd373270c8ed6d276649dd8a5860d188f7d0ff306e91e4e3e092e541d99`  
		Last Modified: Tue, 09 Jun 2020 02:47:16 GMT  
		Size: 7.7 MB (7681351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c85f14a5d8064020366c03aa05ec1c8b0f731e0966bb9788960d27258634aef`  
		Last Modified: Tue, 09 Jun 2020 02:47:16 GMT  
		Size: 10.0 MB (9983910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334e38f2d6fff7c08f4ad1b38ec441d2cf963b761b5d85983396a75ff6d0c08f`  
		Last Modified: Tue, 09 Jun 2020 02:47:41 GMT  
		Size: 52.2 MB (52156256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326561827fde74d56d06dce7035ef6653dbf62a27a5dc35416ba6f00293a09b8`  
		Last Modified: Tue, 09 Jun 2020 02:48:39 GMT  
		Size: 183.7 MB (183744170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef821eade6b1f26263a9104496d7c6527232a00c8ecfa0aab6868fc10d480c9`  
		Last Modified: Fri, 19 Jun 2020 00:08:45 GMT  
		Size: 144.9 MB (144931750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:buster` - linux; 386

```console
$ docker pull rust@sha256:3f45b9475ee12ddc57e3de3a547e246e4441144975e665c9cfce651ba4bf1138
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **472.8 MB (472818538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f861e1f7ab671dcb926e2bd5fcacc831bcc72d0c99ecaf10f37719aae3f3a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:39:33 GMT
ADD file:f95fda6e1e7823d93ca50dd67a1ab99bdc8a7dea372ef27426915702500d54a2 in / 
# Tue, 09 Jun 2020 01:39:33 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:11:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:11:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:12:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:13:11 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Jun 2020 20:10:36 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 20:10:55 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:ca172633df711443e1bcc46650b24074efa097045feee542ecbb4934ae3ae01b`  
		Last Modified: Tue, 09 Jun 2020 01:44:44 GMT  
		Size: 51.2 MB (51156157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e4e2e742db8627ba5d7e0f076114e90c4fea4407cedd3599355e4c00828543`  
		Last Modified: Tue, 09 Jun 2020 02:32:03 GMT  
		Size: 8.0 MB (7981054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ba43d083b56bb094a5bac45d723e9bec0fe65d033950b3c4dc392e890c7e41`  
		Last Modified: Tue, 09 Jun 2020 02:32:03 GMT  
		Size: 10.3 MB (10338453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2391b0310a0be022e7ac6e202273ea7cc0ac5f16e862e5cb19c43c5db30b5b`  
		Last Modified: Tue, 09 Jun 2020 02:32:24 GMT  
		Size: 53.4 MB (53429728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3e805e55983a46c901632f289542625edb04ff470dc6dd9217466a3788d608`  
		Last Modified: Tue, 09 Jun 2020 02:33:23 GMT  
		Size: 198.8 MB (198755099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbce41824f90111fafebb16091199a32fe6de31d201a9cb9384f485fe5fb5de`  
		Last Modified: Thu, 18 Jun 2020 20:13:59 GMT  
		Size: 151.2 MB (151158047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:latest`

```console
$ docker pull rust@sha256:ee8f52372784746235500f9ee80685337a61dcde5e0d028a2aa955d15b6defc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:latest` - linux; amd64

```console
$ docker pull rust@sha256:b2fd2fcc9d28c1a6dc59c3b0b37913fd9a326c8e457e50617e1156fc1ad51e34
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **447.5 MB (447532458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be36dd54f964afeab7f33a72c583e81294fa2deab3fa05f73453209d3d57e199`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:39 GMT
ADD file:1ab357efe422cfed5e37af2dc60d07ccfd4bdee4d4a0c00838b5d68f19ff20c7 in / 
# Tue, 09 Jun 2020 01:20:39 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:47:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:48:00 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Jun 2020 19:21:04 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:21:18 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:e9afc4f90ab09248d75c8081b6dfba749a7f7efdac704ced7e0ceb506e02fa4a`  
		Last Modified: Tue, 09 Jun 2020 01:25:37 GMT  
		Size: 50.4 MB (50389504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989e6b19a265d6b8b7934e7ddd7dc07f6e2fc945b3a28dda9b8aecb12cdb30e0`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 7.8 MB (7811709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14b6c2f8785723bceb5964c5dec1f0489b7750e9d4ec671e49bfba15d80a39`  
		Last Modified: Tue, 09 Jun 2020 01:59:52 GMT  
		Size: 10.0 MB (9996168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5573c4b3094956931fd68c310ae92c9eb1a787f0c77ac2730be9d16cce172d5e`  
		Last Modified: Tue, 09 Jun 2020 02:00:08 GMT  
		Size: 51.8 MB (51827493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a88e76431345b48525c4e4d58d497810019f4bafdb5e2bd56dc34a05e09cc3`  
		Last Modified: Tue, 09 Jun 2020 02:00:47 GMT  
		Size: 192.2 MB (192214313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2afbc28d89df4b6fb2dc20541f4233efb213257aafdcfa2b4bb4290983e3ec6`  
		Last Modified: Thu, 18 Jun 2020 19:24:24 GMT  
		Size: 135.3 MB (135293271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:latest` - linux; arm variant v7

```console
$ docker pull rust@sha256:2a52a967c9b16f19fcc004490f7837ac612a0bb8da50858670f725e0796b4bc9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.4 MB (426430312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3e404c4c716a199bea9faa5dbdd48d89dac55e6b5496c8b944755a6f013054c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:00:40 GMT
ADD file:35073a186411c4b773a9d4d540ec0693ced845cb847b43d8465f9579174cd2b0 in / 
# Tue, 09 Jun 2020 01:00:45 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:48:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:52:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Jun 2020 19:13:13 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:13:42 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:cff0731da2e4f4a0ae8329840eb7fed7ea6aac11aecbfa15c6e684caec03920d`  
		Last Modified: Tue, 09 Jun 2020 01:09:57 GMT  
		Size: 45.9 MB (45868949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbeb0ded58d68be17265763fda36a4e1a520234a291d66f370d98a3e0d6e591`  
		Last Modified: Tue, 09 Jun 2020 02:11:21 GMT  
		Size: 7.1 MB (7097860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6159fbed770bb99a219eae06828da55caaa649879843c0b9df18ddda9b698b3`  
		Last Modified: Tue, 09 Jun 2020 02:11:20 GMT  
		Size: 9.3 MB (9343524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba732bafeb6b1467fd6908c64c6e8d10ffb27e44e3a25ab4c6c38e8f753baa5`  
		Last Modified: Tue, 09 Jun 2020 02:11:43 GMT  
		Size: 47.4 MB (47356467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d84f63917d0e3fb79c2b4c16f4595b8db444749589cfd28a57ef31188ab110`  
		Last Modified: Tue, 09 Jun 2020 02:12:32 GMT  
		Size: 168.4 MB (168420423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a94607ffab11c3cf1fb6f417882b1d8edc34360eb1e13530cb3170ab34cb57`  
		Last Modified: Thu, 18 Jun 2020 19:19:31 GMT  
		Size: 148.3 MB (148343089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:latest` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:623732a5a57084e4da5db6732e4bc7578a425b95e6ffbbb59f0d5bdbd76433b4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **447.7 MB (447665351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddb6fcb343548fe6b5044b7778f1c7c05867e46be852e56f8c39cbbcd38754bb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:51:33 GMT
ADD file:73f1cc6ac15b24788e78ae41cd6c89cb5211d64baf491accbd95b6fe9718f17f in / 
# Tue, 09 Jun 2020 01:51:36 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:31:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:32:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:32:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:35:00 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 19 Jun 2020 00:04:43 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Fri, 19 Jun 2020 00:04:59 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:1db90d3d3b6598d485690f804e96153fb632e7434251d334e9a0c49b773855c9`  
		Last Modified: Tue, 09 Jun 2020 01:57:52 GMT  
		Size: 49.2 MB (49167914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e848fd373270c8ed6d276649dd8a5860d188f7d0ff306e91e4e3e092e541d99`  
		Last Modified: Tue, 09 Jun 2020 02:47:16 GMT  
		Size: 7.7 MB (7681351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c85f14a5d8064020366c03aa05ec1c8b0f731e0966bb9788960d27258634aef`  
		Last Modified: Tue, 09 Jun 2020 02:47:16 GMT  
		Size: 10.0 MB (9983910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334e38f2d6fff7c08f4ad1b38ec441d2cf963b761b5d85983396a75ff6d0c08f`  
		Last Modified: Tue, 09 Jun 2020 02:47:41 GMT  
		Size: 52.2 MB (52156256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326561827fde74d56d06dce7035ef6653dbf62a27a5dc35416ba6f00293a09b8`  
		Last Modified: Tue, 09 Jun 2020 02:48:39 GMT  
		Size: 183.7 MB (183744170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef821eade6b1f26263a9104496d7c6527232a00c8ecfa0aab6868fc10d480c9`  
		Last Modified: Fri, 19 Jun 2020 00:08:45 GMT  
		Size: 144.9 MB (144931750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:latest` - linux; 386

```console
$ docker pull rust@sha256:3f45b9475ee12ddc57e3de3a547e246e4441144975e665c9cfce651ba4bf1138
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **472.8 MB (472818538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f861e1f7ab671dcb926e2bd5fcacc831bcc72d0c99ecaf10f37719aae3f3a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:39:33 GMT
ADD file:f95fda6e1e7823d93ca50dd67a1ab99bdc8a7dea372ef27426915702500d54a2 in / 
# Tue, 09 Jun 2020 01:39:33 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:11:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:11:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:12:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:13:11 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Jun 2020 20:10:36 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 20:10:55 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:ca172633df711443e1bcc46650b24074efa097045feee542ecbb4934ae3ae01b`  
		Last Modified: Tue, 09 Jun 2020 01:44:44 GMT  
		Size: 51.2 MB (51156157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e4e2e742db8627ba5d7e0f076114e90c4fea4407cedd3599355e4c00828543`  
		Last Modified: Tue, 09 Jun 2020 02:32:03 GMT  
		Size: 8.0 MB (7981054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ba43d083b56bb094a5bac45d723e9bec0fe65d033950b3c4dc392e890c7e41`  
		Last Modified: Tue, 09 Jun 2020 02:32:03 GMT  
		Size: 10.3 MB (10338453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2391b0310a0be022e7ac6e202273ea7cc0ac5f16e862e5cb19c43c5db30b5b`  
		Last Modified: Tue, 09 Jun 2020 02:32:24 GMT  
		Size: 53.4 MB (53429728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3e805e55983a46c901632f289542625edb04ff470dc6dd9217466a3788d608`  
		Last Modified: Tue, 09 Jun 2020 02:33:23 GMT  
		Size: 198.8 MB (198755099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbce41824f90111fafebb16091199a32fe6de31d201a9cb9384f485fe5fb5de`  
		Last Modified: Thu, 18 Jun 2020 20:13:59 GMT  
		Size: 151.2 MB (151158047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:slim`

```console
$ docker pull rust@sha256:523456288f840fff23dcb1c29b3b8e646f71692d7f1c87bdd3f46b238621564b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:slim` - linux; amd64

```console
$ docker pull rust@sha256:354b345047ce24c3b879e4427ab1662f608c6a0f6c6ac08ef22a971dfdc3056e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.8 MB (207775593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a62af5c181f94d6dab0a455f90ff60d89533df670387ad05da3efcbd05604cf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:56 GMT
ADD file:4d35f6c8bbbe6801cc5f44989730fb6d349a644ecb36eca481e7df25842d6321 in / 
# Tue, 09 Jun 2020 01:20:56 GMT
CMD ["bash"]
# Thu, 18 Jun 2020 19:21:25 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:21:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:8559a31e96f442f2c7b6da49d6c84705f98a39d8be10b3f5f14821d0ee8417df`  
		Last Modified: Tue, 09 Jun 2020 01:25:50 GMT  
		Size: 27.1 MB (27098265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7d2123b96d6ae88d4ff7f4877c9979291967c9fe883cf38e086eeecc005131`  
		Last Modified: Thu, 18 Jun 2020 19:25:01 GMT  
		Size: 180.7 MB (180677328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim` - linux; arm variant v7

```console
$ docker pull rust@sha256:aef5e2e31a2962e3bc789b16a201df05f3891c8b6351e479ca235de0130fe842
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.9 MB (203947983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd3f2aae154d9d951d006d68c69e2e23d2588da7fd7787f948786f80f7f28d65`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:01:24 GMT
ADD file:a35ca31d2a743d6a1738b1652f4f06c789abbca314d120f0e7e748311ac09ed2 in / 
# Tue, 09 Jun 2020 01:01:30 GMT
CMD ["bash"]
# Thu, 18 Jun 2020 19:13:55 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:15:12 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:2dd003996c9ab82cac8112be0a4c04068e666e7a5d0cce3c65fb8f064de284e7`  
		Last Modified: Tue, 09 Jun 2020 01:10:25 GMT  
		Size: 22.7 MB (22705913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2123881e25542ae72b234649c763a7dfd2fd2058718602a4c9607ac6d57f7f`  
		Last Modified: Thu, 18 Jun 2020 19:20:33 GMT  
		Size: 181.2 MB (181242070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:92e0980cc684e652780a18ff7c064d5ef48775c46bff3dc22cc2d0e246568104
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.0 MB (210995124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1c0f5b7156a169a8083b7ea19ca95d8524073d7e526d8a2e478344adfcf5df9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:52:01 GMT
ADD file:98823648634dfc3af50862b1e2da1028b23996a37adf43b1b0c3c5b29e94b9c7 in / 
# Tue, 09 Jun 2020 01:52:04 GMT
CMD ["bash"]
# Fri, 19 Jun 2020 00:05:08 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Fri, 19 Jun 2020 00:05:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:33cc09c9b190539635d7c971301f623d94fda5b4b5647966c6c240902119009f`  
		Last Modified: Tue, 09 Jun 2020 01:58:14 GMT  
		Size: 25.9 MB (25857704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d4ea274349b38ba3d5b60affc7a3766710f53401f8d9a79792d5be308d6796`  
		Last Modified: Fri, 19 Jun 2020 00:09:47 GMT  
		Size: 185.1 MB (185137420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim` - linux; 386

```console
$ docker pull rust@sha256:6a71e80ff8fa21bb1a5acfee60e064f9a7d5632b257e4b8fee5d8a4dac7ca3d1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.9 MB (228879583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:145755b52ab3753e5762ce9454078790ae2ab87eb619ea2b58da393ea2601505`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:39:49 GMT
ADD file:9fb8fd8bf970c4134f555964fe485a3baa84f1d4c91c5aa35276c24404de9d5d in / 
# Tue, 09 Jun 2020 01:39:49 GMT
CMD ["bash"]
# Thu, 18 Jun 2020 20:11:06 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 20:11:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:860f8957d8be856e2235a28e49fc4dca17254951e0eb67d760769755656f5cad`  
		Last Modified: Tue, 09 Jun 2020 01:45:01 GMT  
		Size: 27.8 MB (27754909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8cbd90acddf34fb55f7c0859346ae57ddea6a96ace0a02fdca617f1a997879`  
		Last Modified: Thu, 18 Jun 2020 20:14:52 GMT  
		Size: 201.1 MB (201124674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:slim-buster`

```console
$ docker pull rust@sha256:523456288f840fff23dcb1c29b3b8e646f71692d7f1c87bdd3f46b238621564b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:slim-buster` - linux; amd64

```console
$ docker pull rust@sha256:354b345047ce24c3b879e4427ab1662f608c6a0f6c6ac08ef22a971dfdc3056e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.8 MB (207775593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a62af5c181f94d6dab0a455f90ff60d89533df670387ad05da3efcbd05604cf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:56 GMT
ADD file:4d35f6c8bbbe6801cc5f44989730fb6d349a644ecb36eca481e7df25842d6321 in / 
# Tue, 09 Jun 2020 01:20:56 GMT
CMD ["bash"]
# Thu, 18 Jun 2020 19:21:25 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:21:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:8559a31e96f442f2c7b6da49d6c84705f98a39d8be10b3f5f14821d0ee8417df`  
		Last Modified: Tue, 09 Jun 2020 01:25:50 GMT  
		Size: 27.1 MB (27098265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7d2123b96d6ae88d4ff7f4877c9979291967c9fe883cf38e086eeecc005131`  
		Last Modified: Thu, 18 Jun 2020 19:25:01 GMT  
		Size: 180.7 MB (180677328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:aef5e2e31a2962e3bc789b16a201df05f3891c8b6351e479ca235de0130fe842
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.9 MB (203947983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd3f2aae154d9d951d006d68c69e2e23d2588da7fd7787f948786f80f7f28d65`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:01:24 GMT
ADD file:a35ca31d2a743d6a1738b1652f4f06c789abbca314d120f0e7e748311ac09ed2 in / 
# Tue, 09 Jun 2020 01:01:30 GMT
CMD ["bash"]
# Thu, 18 Jun 2020 19:13:55 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:15:12 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:2dd003996c9ab82cac8112be0a4c04068e666e7a5d0cce3c65fb8f064de284e7`  
		Last Modified: Tue, 09 Jun 2020 01:10:25 GMT  
		Size: 22.7 MB (22705913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2123881e25542ae72b234649c763a7dfd2fd2058718602a4c9607ac6d57f7f`  
		Last Modified: Thu, 18 Jun 2020 19:20:33 GMT  
		Size: 181.2 MB (181242070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:92e0980cc684e652780a18ff7c064d5ef48775c46bff3dc22cc2d0e246568104
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.0 MB (210995124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1c0f5b7156a169a8083b7ea19ca95d8524073d7e526d8a2e478344adfcf5df9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:52:01 GMT
ADD file:98823648634dfc3af50862b1e2da1028b23996a37adf43b1b0c3c5b29e94b9c7 in / 
# Tue, 09 Jun 2020 01:52:04 GMT
CMD ["bash"]
# Fri, 19 Jun 2020 00:05:08 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Fri, 19 Jun 2020 00:05:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:33cc09c9b190539635d7c971301f623d94fda5b4b5647966c6c240902119009f`  
		Last Modified: Tue, 09 Jun 2020 01:58:14 GMT  
		Size: 25.9 MB (25857704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d4ea274349b38ba3d5b60affc7a3766710f53401f8d9a79792d5be308d6796`  
		Last Modified: Fri, 19 Jun 2020 00:09:47 GMT  
		Size: 185.1 MB (185137420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-buster` - linux; 386

```console
$ docker pull rust@sha256:6a71e80ff8fa21bb1a5acfee60e064f9a7d5632b257e4b8fee5d8a4dac7ca3d1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.9 MB (228879583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:145755b52ab3753e5762ce9454078790ae2ab87eb619ea2b58da393ea2601505`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:39:49 GMT
ADD file:9fb8fd8bf970c4134f555964fe485a3baa84f1d4c91c5aa35276c24404de9d5d in / 
# Tue, 09 Jun 2020 01:39:49 GMT
CMD ["bash"]
# Thu, 18 Jun 2020 20:11:06 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 20:11:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:860f8957d8be856e2235a28e49fc4dca17254951e0eb67d760769755656f5cad`  
		Last Modified: Tue, 09 Jun 2020 01:45:01 GMT  
		Size: 27.8 MB (27754909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8cbd90acddf34fb55f7c0859346ae57ddea6a96ace0a02fdca617f1a997879`  
		Last Modified: Thu, 18 Jun 2020 20:14:52 GMT  
		Size: 201.1 MB (201124674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:slim-stretch`

```console
$ docker pull rust@sha256:66456b3359fa48c9741ea86ba14effb5da705ce0fb4403015106ae8081ea5f5b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:slim-stretch` - linux; amd64

```console
$ docker pull rust@sha256:61df4b3040afc761017728188a9652bb6474b6205c7c34e8cd57a09d8dfe2c72
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.6 MB (195632258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9439f1d88c5c7b12b9806640caf78d6d530161280c3a2d5f578e85d74d0d2bbb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:35 GMT
ADD file:57b431451a292755d0f13673f5f3bea9f62aea36c7a1b59d34d7d200ba134fea in / 
# Tue, 09 Jun 2020 01:23:35 GMT
CMD ["bash"]
# Thu, 18 Jun 2020 19:20:27 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:20:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:7d2977b12acb33f192e3f20b7e15a467cc8f3f5124a15d975a6d4afe5fa3d258`  
		Last Modified: Tue, 09 Jun 2020 01:28:13 GMT  
		Size: 22.5 MB (22519600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f7ede80e96e0566399789a2786eecfb4c5f9c3604a881b446a32db6f01ec91`  
		Last Modified: Thu, 18 Jun 2020 19:23:53 GMT  
		Size: 173.1 MB (173112658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-stretch` - linux; arm variant v7

```console
$ docker pull rust@sha256:f79d863d88d0ff84fc76d7221f47420ee810de67430a30ad93d8b359e32d1214
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.7 MB (195669366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeaf868781e3933ea7563493f08a9248af68cb49350a0de81a2b2264c54d9c25`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:35 GMT
ADD file:4a0a863669948b35130fcf8cdb52999c49f7b3ee0620a1eef5f1a2e850a42f05 in / 
# Tue, 09 Jun 2020 01:06:37 GMT
CMD ["bash"]
# Thu, 18 Jun 2020 18:58:54 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:12:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:c439312a9c212b64af3c38cb326bb5fbe14bcf4a622115d59d44985e949bee82`  
		Last Modified: Tue, 09 Jun 2020 01:13:51 GMT  
		Size: 19.3 MB (19304370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353546c552425fb49ffeef7c3895693859ba33fa54bfcac5c3d4bd6952341b98`  
		Last Modified: Thu, 18 Jun 2020 19:18:33 GMT  
		Size: 176.4 MB (176364996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-stretch` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:efc8bfaf58df25ef6432a6e9312dc1807c3e00716205c72d00e4cfc57f18626c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.9 MB (195882477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6b524283c8151ca7dcd99551a7e271f36d232e5c65e97ce914344589814f324`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:49 GMT
ADD file:c85d28567b6123deb660b71c8b60d92378b5ba15ba5dcf495d9388817dc3aa44 in / 
# Tue, 09 Jun 2020 01:54:52 GMT
CMD ["bash"]
# Fri, 19 Jun 2020 00:03:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Fri, 19 Jun 2020 00:04:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:622dc742b82743ebf5607b215a65869096390ee41b0a61b5532f859fb94590b1`  
		Last Modified: Tue, 09 Jun 2020 02:00:28 GMT  
		Size: 20.4 MB (20375150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08568b0762f6b468d5d9fafe63b44e4f986a3dd82e31e85c68555345a0e146a2`  
		Last Modified: Fri, 19 Jun 2020 00:07:57 GMT  
		Size: 175.5 MB (175507327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-stretch` - linux; 386

```console
$ docker pull rust@sha256:9fc333d7b32f1389d3e066f162a4fa9dc6bb38537b0fab187906ff352d6bac27
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.1 MB (216130114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9ea2784f298048053574227bbc7d3fcb3c814eb375848e38be19f7f561450cd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:33 GMT
ADD file:8ef252685ffefc58654053bf145c830928a2cf423a6c757180649df772f1523d in / 
# Tue, 09 Jun 2020 01:42:34 GMT
CMD ["bash"]
# Thu, 18 Jun 2020 20:09:57 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 20:10:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:4ffbd6ec7974e514763a8d7d9fcf5e86e9440e2280e6e9561ea373b4bc50588e`  
		Last Modified: Tue, 09 Jun 2020 01:48:28 GMT  
		Size: 23.1 MB (23147892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff582d7ea58b49b27d3241c60c89aa592dde236d70e301e5099469f2a5fb6c54`  
		Last Modified: Thu, 18 Jun 2020 20:13:21 GMT  
		Size: 193.0 MB (192982222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:stretch`

```console
$ docker pull rust@sha256:07afa12e396109dd20c19193c6ced45a8988437fdfc6a084877b77af0a5aaef3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:stretch` - linux; amd64

```console
$ docker pull rust@sha256:cd0d96614c172237a7b782fc090733f3c12922fb29e3c064e8fe34453ac01b99
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **460.7 MB (460749631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de3ffe48a60a6c9bed849ef957b32f4172727e445e52eb24b7ece05596362a98`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:20 GMT
ADD file:6e16bc9cf28c19a1fb1fb516411643e33cbd2bdb7b6c2ce2468c6583c89871a2 in / 
# Tue, 09 Jun 2020 01:23:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:56:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:56:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:56:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:57:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Jun 2020 19:20:08 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 19:20:21 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:81fc1918191541a2ffb6ed1cd8386ef8302aea1b0613ebc768a00e76c1f34bb9`  
		Last Modified: Tue, 09 Jun 2020 01:27:59 GMT  
		Size: 45.4 MB (45375796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee49ee6a23d1c7e6b8b574c905dcd4a53efb869a539a957d3e47bc3698f01dc8`  
		Last Modified: Tue, 09 Jun 2020 02:02:39 GMT  
		Size: 10.7 MB (10749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82851092453815ec861754ded7101fcfa3b648d09a0818ced17ea80478f179a3`  
		Last Modified: Tue, 09 Jun 2020 02:02:38 GMT  
		Size: 4.3 MB (4339890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8f58c4fcca04f9622e97db77618075b618c24a58cce6c6860ca54c9a887745b`  
		Last Modified: Tue, 09 Jun 2020 02:02:52 GMT  
		Size: 50.1 MB (50082718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33699d7df21edc5ded5b679bc283e5890ed92c5bf20e53b48edcd9096c8a5962`  
		Last Modified: Tue, 09 Jun 2020 02:03:29 GMT  
		Size: 214.9 MB (214908336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baab346e84a2b6df78d07068567a9ebce0a2a15654279dcf576eec30d4a65367`  
		Last Modified: Thu, 18 Jun 2020 19:23:17 GMT  
		Size: 135.3 MB (135293871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:stretch` - linux; arm variant v7

```console
$ docker pull rust@sha256:3931004840e50e226b226a792a3255f4521ff543189500f17c31e6bc57d10725
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **445.8 MB (445787888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f9d65523682d96797f6e5ee80817988c61149f89eb4aedb09ee5dfec099d287`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:07 GMT
ADD file:c0b9ed1244ec0acfc9054c7cb80c768878e3da99740f981ba3a82bdd854305db in / 
# Tue, 09 Jun 2020 01:06:09 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:02:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:02:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:03:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:06:20 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Jun 2020 18:58:22 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 18:58:47 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:2566ca784846d2d0d4f9105084d94d68d8ea1a82a06a76c5bcd991ce5a10cda1`  
		Last Modified: Tue, 09 Jun 2020 01:13:35 GMT  
		Size: 42.1 MB (42102504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f976b5a12722f5e6e115157695654d36452b713c7fa64a860f8c9e14859402`  
		Last Modified: Tue, 09 Jun 2020 02:15:15 GMT  
		Size: 9.4 MB (9443335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35142ef6ea6c722cd0397799ab151e5da354eabc784b3acef29def7fa34e9bc`  
		Last Modified: Tue, 09 Jun 2020 02:15:13 GMT  
		Size: 3.9 MB (3918433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7773eda6b7a8801a6f09bd4ce443b7e88397ed16265ecd37f55af57db56c4658`  
		Last Modified: Tue, 09 Jun 2020 02:15:36 GMT  
		Size: 46.4 MB (46412697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf8c80047f39ca1669cf85bbab477a59e35f498d269e058afe91bf9850b7c52`  
		Last Modified: Tue, 09 Jun 2020 02:16:37 GMT  
		Size: 195.6 MB (195567505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74835fe8def5171fad1b8ae2b6f7d7c9051db5b7ba498e5c87bd601fcd4041e6`  
		Last Modified: Thu, 18 Jun 2020 19:16:16 GMT  
		Size: 148.3 MB (148343414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:stretch` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:ec2aae4f393360361384ad0e9abfc76a04f45f4415697265f80bd20fb7260d0c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **452.2 MB (452205272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1953029c1c941d34c706d21c87d82b81ce8b88ec5a840e0bcca3073f08436f52`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:22 GMT
ADD file:5cbf00485aed776e940988cadfad6853c640c13635ae54fb2b00aafccfe81a73 in / 
# Tue, 09 Jun 2020 01:54:25 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:39:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:40:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:43:35 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 19 Jun 2020 00:02:56 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Fri, 19 Jun 2020 00:03:15 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:4c4f692ec920eecb1f30d9ef8e50125217decc872d7ada6eeccc36c6dcb49e4d`  
		Last Modified: Tue, 09 Jun 2020 02:00:09 GMT  
		Size: 43.2 MB (43160923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0990c417a21ef9e268cc0822cd23968c4b17cded8170cce0c4d8f7e020e6fd`  
		Last Modified: Tue, 09 Jun 2020 02:50:17 GMT  
		Size: 9.7 MB (9699635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6b83fd41426d182f67fdac882a6bfcd3aad22d7226a653ae58d3046bd46b5e`  
		Last Modified: Tue, 09 Jun 2020 02:50:15 GMT  
		Size: 4.1 MB (4094104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2de3ad924e80f0d130d0bd9ed8ea866eefeb610874bce14fd8347d032772220`  
		Last Modified: Tue, 09 Jun 2020 02:50:36 GMT  
		Size: 48.0 MB (48034909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2720149da5321de7d3e31500696a088aae1c37ededd1680245aec1602c17c5`  
		Last Modified: Tue, 09 Jun 2020 02:51:32 GMT  
		Size: 202.3 MB (202283682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbefd35906cd779827ad7f0c9e26f349577d819f8d6901f51bf43e7cb8028b38`  
		Last Modified: Fri, 19 Jun 2020 00:06:57 GMT  
		Size: 144.9 MB (144932019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:stretch` - linux; 386

```console
$ docker pull rust@sha256:fb7764674949cf00a03a2b2cffd76e9757fed14e6d19c81ddb2d22e58e51e59f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.2 MB (484164275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0330c79b62c3998719e33191ce6cbdef2a0cbfe312f93af6145ec9bddde4aff0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:17 GMT
ADD file:6bbeeb0773b96fccb4cd5ba81dd19ec3580f8d8a3cdd3f1d6a3d2b514fbd6eb1 in / 
# Tue, 09 Jun 2020 01:42:18 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:26:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:26:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:27:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:28:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Jun 2020 20:09:35 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.44.1
# Thu, 18 Jun 2020 20:09:53 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9e88f215fab896e3a7d1d2ce75c0d79960b236066e9033b97e76ca7f01ff2fdc`  
		Last Modified: Tue, 09 Jun 2020 01:48:12 GMT  
		Size: 46.1 MB (46094854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1130784446f3179c75741e18b159e7bca5d46db60bb1f9f57d67953023a50899`  
		Last Modified: Tue, 09 Jun 2020 02:37:03 GMT  
		Size: 10.8 MB (10772863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e32fbc0a9c533b460544bce821a796b4f02dd4da61100073a18fba329807ae`  
		Last Modified: Tue, 09 Jun 2020 02:37:01 GMT  
		Size: 4.6 MB (4561121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e9df71276e8af2305be9b32aca4dd788168bd7fe3c6029ddd8e4e8057f7d33`  
		Last Modified: Tue, 09 Jun 2020 02:37:31 GMT  
		Size: 51.6 MB (51615859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c496d702f58d364bb0ec81531f18a35844eb95f0f9e0dff097b6588eaa8fb7`  
		Last Modified: Tue, 09 Jun 2020 02:38:54 GMT  
		Size: 220.0 MB (219960753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399d9f86bb9f3cf9ef83ed8d3c204b9f1b9283c169ed9e53a8f4fa399cd3c571`  
		Last Modified: Thu, 18 Jun 2020 20:12:29 GMT  
		Size: 151.2 MB (151158825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
