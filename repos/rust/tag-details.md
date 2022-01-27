<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `rust`

-	[`rust:1`](#rust1)
-	[`rust:1-alpine`](#rust1-alpine)
-	[`rust:1-alpine3.14`](#rust1-alpine314)
-	[`rust:1-alpine3.15`](#rust1-alpine315)
-	[`rust:1-bullseye`](#rust1-bullseye)
-	[`rust:1-buster`](#rust1-buster)
-	[`rust:1-slim`](#rust1-slim)
-	[`rust:1-slim-bullseye`](#rust1-slim-bullseye)
-	[`rust:1-slim-buster`](#rust1-slim-buster)
-	[`rust:1.58`](#rust158)
-	[`rust:1.58-alpine`](#rust158-alpine)
-	[`rust:1.58-alpine3.14`](#rust158-alpine314)
-	[`rust:1.58-alpine3.15`](#rust158-alpine315)
-	[`rust:1.58-bullseye`](#rust158-bullseye)
-	[`rust:1.58-buster`](#rust158-buster)
-	[`rust:1.58-slim`](#rust158-slim)
-	[`rust:1.58-slim-bullseye`](#rust158-slim-bullseye)
-	[`rust:1.58-slim-buster`](#rust158-slim-buster)
-	[`rust:1.58.1`](#rust1581)
-	[`rust:1.58.1-alpine`](#rust1581-alpine)
-	[`rust:1.58.1-alpine3.14`](#rust1581-alpine314)
-	[`rust:1.58.1-alpine3.15`](#rust1581-alpine315)
-	[`rust:1.58.1-bullseye`](#rust1581-bullseye)
-	[`rust:1.58.1-buster`](#rust1581-buster)
-	[`rust:1.58.1-slim`](#rust1581-slim)
-	[`rust:1.58.1-slim-bullseye`](#rust1581-slim-bullseye)
-	[`rust:1.58.1-slim-buster`](#rust1581-slim-buster)
-	[`rust:alpine`](#rustalpine)
-	[`rust:alpine3.14`](#rustalpine314)
-	[`rust:alpine3.15`](#rustalpine315)
-	[`rust:bullseye`](#rustbullseye)
-	[`rust:buster`](#rustbuster)
-	[`rust:latest`](#rustlatest)
-	[`rust:slim`](#rustslim)
-	[`rust:slim-bullseye`](#rustslim-bullseye)
-	[`rust:slim-buster`](#rustslim-buster)

## `rust:1`

```console
$ docker pull rust@sha256:8ad28b7355e19dad2677624622bad1cc978b6fd34b45e75d17c25f558f94a934
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1` - linux; amd64

```console
$ docker pull rust@sha256:d46142e07db17a179a9cd18bc814c5c7e1499fdd12147f9249ee48c540aec0d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.2 MB (466162023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:269d9943b0d310e1ab49a55e14752596567a74daa37270c6217abfc33f48f7f5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 02:26:40 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Thu, 27 Jan 2022 02:26:56 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808edda3c2e855dc13af758b35cefbcc417ad1ab4fead7f72234b09aeda893a0`  
		Last Modified: Wed, 26 Jan 2022 02:23:16 GMT  
		Size: 196.5 MB (196529197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4671d83ec37ad7f7bf397a8340e76ed6b965029035e63a4a2043351fcd40d892`  
		Last Modified: Thu, 27 Jan 2022 02:30:45 GMT  
		Size: 144.1 MB (144123702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1` - linux; arm variant v7

```console
$ docker pull rust@sha256:32e5c60294d2cd912122e23d42e330e63a9a8754443b8654a3ea8df1e75ba397
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **483.2 MB (483165594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8faf3dd2fdb2285b82cf07285b1b0bf7d34d46d0478e7996e3f0369398d7528b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:59:11 GMT
ADD file:848bf729bc16d3b188567f096ee1c0386cb49825a06eef396401278afee2f4c7 in / 
# Tue, 21 Dec 2021 01:59:12 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:46:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:46:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:47:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:49:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 06:11:05 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 06:11:46 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:fd92fbcda272f5935dcd0dfea445cba0152208f83c8fc8d2cb74c85379145c42`  
		Last Modified: Tue, 21 Dec 2021 02:14:41 GMT  
		Size: 50.1 MB (50121433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a6987ee02fad9d702adbd7921b8e1776b1a091773dd47886055113b1d7ba62`  
		Last Modified: Tue, 21 Dec 2021 03:11:46 GMT  
		Size: 4.9 MB (4922490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6d85cbb278c8e4845f79838154b77c36931e65f9b5bb9b8f56c92f41f72e27`  
		Last Modified: Tue, 21 Dec 2021 03:11:47 GMT  
		Size: 10.2 MB (10217004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bd566d277d8d03e1b76768a074dd92306bc287eef88c42a08ef5b48b842fa1`  
		Last Modified: Tue, 21 Dec 2021 03:12:37 GMT  
		Size: 50.3 MB (50328047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edcf448232b2036e5813fc0174bcd35c3a967a79cf2ef79bc2bfb0410c7b176e`  
		Last Modified: Tue, 21 Dec 2021 03:14:27 GMT  
		Size: 167.0 MB (166954318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2393fcae1480a3e448c675f4654fccb4999808ae81fd8438665649bd7809cd`  
		Last Modified: Fri, 21 Jan 2022 06:22:33 GMT  
		Size: 200.6 MB (200622302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:71e628671e7232373f1babb49f78f1751c5151af8ac6dc2c5cfaacf60c08c627
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **529.3 MB (529331157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28baec511a7c725b2502fe4dbcda7a5e4740cb19806b922bfcbfbb35cd1d9c13`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:38:28 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 08:38:45 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cb4eca0cebfb68f0cb8dd7e6c0c67b880fcae929406705b4d43a2df4fa48eb`  
		Last Modified: Wed, 26 Jan 2022 02:24:49 GMT  
		Size: 189.4 MB (189420652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2d141dc211541426cd6794767a1439b2ead45ccdae9e55c89c1f6d1b46ce7b`  
		Last Modified: Wed, 26 Jan 2022 08:43:08 GMT  
		Size: 215.8 MB (215834728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1` - linux; 386

```console
$ docker pull rust@sha256:00a04734a44749afb4e6a7c8c294d3e9a5c169bb091601036d41044241f8d9eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.8 MB (515847461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9787ce8e926d4bc03f1104f353c79e89b71d8453c15fa4f707118ef27a84595e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:39:40 GMT
ADD file:b77df0839dfb103f5f16329bfa0dcf40c1a73b02e312bb2be40ad620f64e7949 in / 
# Tue, 21 Dec 2021 01:39:44 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:13:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:13:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:13:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:14:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 01:40:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:40:45 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:c13b09ebb011541c3f3a6e423452bf5046e5ba48dfee18e88cc3e3df477c0baa`  
		Last Modified: Tue, 21 Dec 2021 01:48:09 GMT  
		Size: 55.9 MB (55925399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0db4e702162a700c3f00a3624f94bbfa81fd2077b8c5cf57f455659259295a`  
		Last Modified: Tue, 21 Dec 2021 02:25:41 GMT  
		Size: 5.3 MB (5282974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4fb971a29956de966e154c96a2d7f1eb56aed081b583947be033c05d7c69797`  
		Last Modified: Tue, 21 Dec 2021 02:25:42 GMT  
		Size: 11.3 MB (11250616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb3ec563e1e552271ac9c80a2b348ebf47401940583ca295fc5f1378ca9d3ac`  
		Last Modified: Tue, 21 Dec 2021 02:26:11 GMT  
		Size: 55.9 MB (55917390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2c2a9657022eac58df44f2cef58c0e28b506b12f67dece31bf9bd280de6d6f`  
		Last Modified: Tue, 21 Dec 2021 02:27:07 GMT  
		Size: 199.4 MB (199449263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae4e6ced7d216b439b6a4b3cfffd9957baaa2093e769d5da2f657972bb99a96`  
		Last Modified: Fri, 21 Jan 2022 01:45:38 GMT  
		Size: 188.0 MB (188021819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-alpine`

```console
$ docker pull rust@sha256:b61698ea823c6f9bc726272d7783867d89e79ca87e9944998739ce619da7699a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:1-alpine` - linux; amd64

```console
$ docker pull rust@sha256:d4c641c867f8d60f1f4da8edc19da4ea6543dd54f5cfd4c4cb713a438f9ed079
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.6 MB (269634647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:953451d7b194820db2946de86d08aa997c88d7e3f5f728f577d20cf4c4c210d9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Thu, 13 Jan 2022 20:26:04 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 21 Jan 2022 01:22:17 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:22:38 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93cd12ff80a853b96704224019bf0b85bbe94d9b9456b619b95ab0a8dbdf40d`  
		Last Modified: Thu, 13 Jan 2022 20:31:39 GMT  
		Size: 42.5 MB (42495579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9781e95f2a775fd7a289185a1bcbd1e616c15547d6ab73d8e78dfbb1c99514c`  
		Last Modified: Fri, 21 Jan 2022 01:28:49 GMT  
		Size: 224.3 MB (224320655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-alpine` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:58a1a37e622250ca1f6f16bb1449e714632dcd7deddc0e2f38b8a05c92e54e55
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.0 MB (254960114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8a5a57c57976585d381f3fd0fe33476127b6dda4fa4e767a620e54314c92118`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Thu, 13 Jan 2022 20:42:58 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 21 Jan 2022 01:42:50 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:43:07 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec7b33c7ee4d79979b266a321f626981b48087e7524811342d73ce2e2eb9e57`  
		Last Modified: Thu, 13 Jan 2022 20:49:23 GMT  
		Size: 36.1 MB (36087204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fec8b7bac538e28495e4763ae0710d8b74d160b4b9b4cda13fbf6269d3283f`  
		Last Modified: Fri, 21 Jan 2022 01:49:44 GMT  
		Size: 216.2 MB (216157476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-alpine3.14`

```console
$ docker pull rust@sha256:2292543650f33917efbb8da25a303848cc72fad0cb95a0320277f99d3ce92046
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:1-alpine3.14` - linux; amd64

```console
$ docker pull rust@sha256:fbc0cfaa6261179ca7653cc2b20ca9c3e936f3416a911a27a28694f8fb23b8b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.5 MB (269494735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e35d9d35ab3792f9f41494f2fa73e8057080db430deb0bceddf896a605a6582`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 07:44:00 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 21 Jan 2022 01:21:49 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:22:11 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95f12a5672fd92cc370cc8ec78127e6c52a6d61404662fab9d5643b661f3e8b`  
		Last Modified: Sat, 13 Nov 2021 07:46:42 GMT  
		Size: 42.4 MB (42351276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be615768698a2e1df78b3e911bccea805cbacfcb7972586bb677332badfe97fb`  
		Last Modified: Fri, 21 Jan 2022 01:27:52 GMT  
		Size: 224.3 MB (224320478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:7dd68b020a1550ed5cd7974188763c0831aea119f73fd1327b25972b6656962f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.8 MB (254813562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45aad15a39b3ffaf28e25228529764e9ad0408ff6182c9a9f30b8ab31fdb92fc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 17:55:55 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 21 Jan 2022 01:42:27 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:42:44 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3394b2150e94a1388a8ac369dcfa5974566be0e105ccecfe1f50dbeedd25887d`  
		Last Modified: Fri, 12 Nov 2021 17:58:34 GMT  
		Size: 35.9 MB (35938392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d19cdf6d774da55657d17c1d24e8390cce8b2f8cced8100d85ea1e51c82d13e`  
		Last Modified: Fri, 21 Jan 2022 01:48:56 GMT  
		Size: 216.2 MB (216157470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-alpine3.15`

```console
$ docker pull rust@sha256:b61698ea823c6f9bc726272d7783867d89e79ca87e9944998739ce619da7699a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:1-alpine3.15` - linux; amd64

```console
$ docker pull rust@sha256:d4c641c867f8d60f1f4da8edc19da4ea6543dd54f5cfd4c4cb713a438f9ed079
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.6 MB (269634647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:953451d7b194820db2946de86d08aa997c88d7e3f5f728f577d20cf4c4c210d9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Thu, 13 Jan 2022 20:26:04 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 21 Jan 2022 01:22:17 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:22:38 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93cd12ff80a853b96704224019bf0b85bbe94d9b9456b619b95ab0a8dbdf40d`  
		Last Modified: Thu, 13 Jan 2022 20:31:39 GMT  
		Size: 42.5 MB (42495579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9781e95f2a775fd7a289185a1bcbd1e616c15547d6ab73d8e78dfbb1c99514c`  
		Last Modified: Fri, 21 Jan 2022 01:28:49 GMT  
		Size: 224.3 MB (224320655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:58a1a37e622250ca1f6f16bb1449e714632dcd7deddc0e2f38b8a05c92e54e55
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.0 MB (254960114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8a5a57c57976585d381f3fd0fe33476127b6dda4fa4e767a620e54314c92118`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Thu, 13 Jan 2022 20:42:58 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 21 Jan 2022 01:42:50 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:43:07 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec7b33c7ee4d79979b266a321f626981b48087e7524811342d73ce2e2eb9e57`  
		Last Modified: Thu, 13 Jan 2022 20:49:23 GMT  
		Size: 36.1 MB (36087204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fec8b7bac538e28495e4763ae0710d8b74d160b4b9b4cda13fbf6269d3283f`  
		Last Modified: Fri, 21 Jan 2022 01:49:44 GMT  
		Size: 216.2 MB (216157476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-bullseye`

```console
$ docker pull rust@sha256:8ad28b7355e19dad2677624622bad1cc978b6fd34b45e75d17c25f558f94a934
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-bullseye` - linux; amd64

```console
$ docker pull rust@sha256:d46142e07db17a179a9cd18bc814c5c7e1499fdd12147f9249ee48c540aec0d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.2 MB (466162023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:269d9943b0d310e1ab49a55e14752596567a74daa37270c6217abfc33f48f7f5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 02:26:40 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Thu, 27 Jan 2022 02:26:56 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808edda3c2e855dc13af758b35cefbcc417ad1ab4fead7f72234b09aeda893a0`  
		Last Modified: Wed, 26 Jan 2022 02:23:16 GMT  
		Size: 196.5 MB (196529197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4671d83ec37ad7f7bf397a8340e76ed6b965029035e63a4a2043351fcd40d892`  
		Last Modified: Thu, 27 Jan 2022 02:30:45 GMT  
		Size: 144.1 MB (144123702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-bullseye` - linux; arm variant v7

```console
$ docker pull rust@sha256:32e5c60294d2cd912122e23d42e330e63a9a8754443b8654a3ea8df1e75ba397
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **483.2 MB (483165594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8faf3dd2fdb2285b82cf07285b1b0bf7d34d46d0478e7996e3f0369398d7528b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:59:11 GMT
ADD file:848bf729bc16d3b188567f096ee1c0386cb49825a06eef396401278afee2f4c7 in / 
# Tue, 21 Dec 2021 01:59:12 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:46:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:46:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:47:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:49:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 06:11:05 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 06:11:46 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:fd92fbcda272f5935dcd0dfea445cba0152208f83c8fc8d2cb74c85379145c42`  
		Last Modified: Tue, 21 Dec 2021 02:14:41 GMT  
		Size: 50.1 MB (50121433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a6987ee02fad9d702adbd7921b8e1776b1a091773dd47886055113b1d7ba62`  
		Last Modified: Tue, 21 Dec 2021 03:11:46 GMT  
		Size: 4.9 MB (4922490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6d85cbb278c8e4845f79838154b77c36931e65f9b5bb9b8f56c92f41f72e27`  
		Last Modified: Tue, 21 Dec 2021 03:11:47 GMT  
		Size: 10.2 MB (10217004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bd566d277d8d03e1b76768a074dd92306bc287eef88c42a08ef5b48b842fa1`  
		Last Modified: Tue, 21 Dec 2021 03:12:37 GMT  
		Size: 50.3 MB (50328047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edcf448232b2036e5813fc0174bcd35c3a967a79cf2ef79bc2bfb0410c7b176e`  
		Last Modified: Tue, 21 Dec 2021 03:14:27 GMT  
		Size: 167.0 MB (166954318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2393fcae1480a3e448c675f4654fccb4999808ae81fd8438665649bd7809cd`  
		Last Modified: Fri, 21 Jan 2022 06:22:33 GMT  
		Size: 200.6 MB (200622302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-bullseye` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:71e628671e7232373f1babb49f78f1751c5151af8ac6dc2c5cfaacf60c08c627
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **529.3 MB (529331157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28baec511a7c725b2502fe4dbcda7a5e4740cb19806b922bfcbfbb35cd1d9c13`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:38:28 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 08:38:45 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cb4eca0cebfb68f0cb8dd7e6c0c67b880fcae929406705b4d43a2df4fa48eb`  
		Last Modified: Wed, 26 Jan 2022 02:24:49 GMT  
		Size: 189.4 MB (189420652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2d141dc211541426cd6794767a1439b2ead45ccdae9e55c89c1f6d1b46ce7b`  
		Last Modified: Wed, 26 Jan 2022 08:43:08 GMT  
		Size: 215.8 MB (215834728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-bullseye` - linux; 386

```console
$ docker pull rust@sha256:00a04734a44749afb4e6a7c8c294d3e9a5c169bb091601036d41044241f8d9eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.8 MB (515847461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9787ce8e926d4bc03f1104f353c79e89b71d8453c15fa4f707118ef27a84595e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:39:40 GMT
ADD file:b77df0839dfb103f5f16329bfa0dcf40c1a73b02e312bb2be40ad620f64e7949 in / 
# Tue, 21 Dec 2021 01:39:44 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:13:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:13:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:13:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:14:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 01:40:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:40:45 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:c13b09ebb011541c3f3a6e423452bf5046e5ba48dfee18e88cc3e3df477c0baa`  
		Last Modified: Tue, 21 Dec 2021 01:48:09 GMT  
		Size: 55.9 MB (55925399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0db4e702162a700c3f00a3624f94bbfa81fd2077b8c5cf57f455659259295a`  
		Last Modified: Tue, 21 Dec 2021 02:25:41 GMT  
		Size: 5.3 MB (5282974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4fb971a29956de966e154c96a2d7f1eb56aed081b583947be033c05d7c69797`  
		Last Modified: Tue, 21 Dec 2021 02:25:42 GMT  
		Size: 11.3 MB (11250616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb3ec563e1e552271ac9c80a2b348ebf47401940583ca295fc5f1378ca9d3ac`  
		Last Modified: Tue, 21 Dec 2021 02:26:11 GMT  
		Size: 55.9 MB (55917390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2c2a9657022eac58df44f2cef58c0e28b506b12f67dece31bf9bd280de6d6f`  
		Last Modified: Tue, 21 Dec 2021 02:27:07 GMT  
		Size: 199.4 MB (199449263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae4e6ced7d216b439b6a4b3cfffd9957baaa2093e769d5da2f657972bb99a96`  
		Last Modified: Fri, 21 Jan 2022 01:45:38 GMT  
		Size: 188.0 MB (188021819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-buster`

```console
$ docker pull rust@sha256:e3a1c9b64e1c028851e24fba7d846dbe11edb2463fdb2e4bae2b731c0bc86463
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-buster` - linux; amd64

```console
$ docker pull rust@sha256:5dad83d6154d9b7d5a454e487292a818f1a49c310d22d28d027dace34ade540d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **456.7 MB (456656132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4737b5f9e43d2dc30e66ad37c2bf4a078f46b8b9e7e751b650e9e082e76e1a7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:47 GMT
ADD file:a290acee3581e1e9c42c0a37b53086a8f070cb0730179be81a6ba24a620b6ee4 in / 
# Wed, 26 Jan 2022 01:40:47 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 02:25:47 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Thu, 27 Jan 2022 02:26:02 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:a024302f8a017855dd20a107ace079dd543c4bdfa8e7c11472771babbe298d2b`  
		Last Modified: Wed, 26 Jan 2022 01:47:01 GMT  
		Size: 50.4 MB (50437057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289773030fdc98afe6cc53bdd0c05332ea8ff21ad836afa1d3042388953c43f8`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 7.8 MB (7833856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bb8b3399fe8dd0b83bd5e32a97e5183ab235d6fb4cc0b5dfabb20e6653e715`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 10.0 MB (9997205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c63da771697b362929cecc84777e8cfbb716ff3d575b999854d83ada039b695`  
		Last Modified: Wed, 26 Jan 2022 02:23:53 GMT  
		Size: 51.8 MB (51839910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf1b23b1e4b1867b70ba7f0614dff34bdb468c2a860a7b162c74c2b451494c0`  
		Last Modified: Wed, 26 Jan 2022 02:24:38 GMT  
		Size: 192.4 MB (192424405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbadc5241c680bb76f81237047194a1d408a37104d21cfc421439a941bc0d5a3`  
		Last Modified: Thu, 27 Jan 2022 02:29:05 GMT  
		Size: 144.1 MB (144123699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:1ccaa939ec2bcd17833886a87ae632de27c7b25738510f45f9573a0a6802f50b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **479.0 MB (478973771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e5e34aeb2594b6b0ea9e8b59acf1d371889f6b13ace574de70235c1cb3cdab3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:17 GMT
ADD file:36bf5b8bdd9066b06cc35d26df3f4dad2b1cbcb41985b85f070ed97a3e85f8a9 in / 
# Tue, 21 Dec 2021 02:00:18 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:49:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:50:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:53:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 06:08:33 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 06:09:16 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:328389035fdd79ece4f520541a84b3de974050fe012ed1566da6b869dd34ea29`  
		Last Modified: Tue, 21 Dec 2021 02:16:11 GMT  
		Size: 45.9 MB (45918102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80397c5626b1d4e58b7b7dd9219674dd86caa03ddcaac1d3d6791189a44b0ff`  
		Last Modified: Tue, 21 Dec 2021 03:14:47 GMT  
		Size: 7.1 MB (7125168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816c475148f8e55cc2b8593f29d0ddd67ad1359f3c69061f043d461495bad179`  
		Last Modified: Tue, 21 Dec 2021 03:14:48 GMT  
		Size: 9.3 MB (9343808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d30bc5ea112783bdcbfaba962b58338c0f61b12d68a5cc7474c0b639098c6a`  
		Last Modified: Tue, 21 Dec 2021 03:15:32 GMT  
		Size: 47.4 MB (47356397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93be0f932a74231c59bf289b331a4b22b2346e3532b93f7c9a3d1eb60859f40b`  
		Last Modified: Tue, 21 Dec 2021 03:17:17 GMT  
		Size: 168.6 MB (168607961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e21137e326fc09ba91d9592481ee83a4c7e5b8458ffd21c0f488c9edb3d3bbd`  
		Last Modified: Fri, 21 Jan 2022 06:17:28 GMT  
		Size: 200.6 MB (200622335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:611b00bf3064be66516b9bd9af0a31bbdf0d7535edb4ea5fa6ee5e41bf6c157b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **518.7 MB (518694576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bc36b7a17a62b420f4f1b26c9a9ffee6132533be64f06904a8e51a73622d362`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:41 GMT
ADD file:98a75269e438ff15cee16ad2763fe2698fb436bc4770c0ca27c059f66b65e56a in / 
# Wed, 26 Jan 2022 01:42:42 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:14:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:14:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:15:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:37:25 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 08:37:44 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:ccd458f933f7966e412773ee1551aaf2433a5bf9adaae519e2ac7c9c3f8b5f89`  
		Last Modified: Wed, 26 Jan 2022 01:49:28 GMT  
		Size: 49.2 MB (49223041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3524e6d2c855bef1f32da73e00738b2e5e91e6a346d19f8b33e8e8117c82748`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 7.7 MB (7695112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cc9cf00cd9023559aeda43668c7d9d621318631bab103ae03b8a3787260048`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 9.8 MB (9767300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f0325e59cadc58f4e81c6a282319b0c01f54964ef989205974a6557cf15040`  
		Last Modified: Wed, 26 Jan 2022 02:25:25 GMT  
		Size: 52.2 MB (52168727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b289063aa004828178bcfddecfcf2fda082ce1cb1657eb68a9ef23e027a510b`  
		Last Modified: Wed, 26 Jan 2022 02:26:00 GMT  
		Size: 184.0 MB (184005857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af714e5ef49569fce78ac8d86129c0d70407051af674aadee820dbf5f6d118a`  
		Last Modified: Wed, 26 Jan 2022 08:41:20 GMT  
		Size: 215.8 MB (215834539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-buster` - linux; 386

```console
$ docker pull rust@sha256:4fde2447b7b5bd85bc6e955b14004027e985963d6db7377793371fcb4d904374
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **510.0 MB (509970484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24aac74c874dfb49adbce2fad1afd33ce899db1b13c2342e96e959c68eb4b7a4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:24 GMT
ADD file:4e982be228380a8d7632e31f19e39ed55ee76fb1db32130fa88d696904d6acde in / 
# Tue, 21 Dec 2021 01:40:25 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:15:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:15:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:15:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:17:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 01:38:53 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:39:15 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:342b01a61e0af68dc09681004efdfcf66d0443632988d6f247dd7b34bc18b1db`  
		Last Modified: Tue, 21 Dec 2021 01:49:14 GMT  
		Size: 51.2 MB (51207766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4759b0dba897041c21e226a9db50a85ca5685f19bb5036f16df5b231fd177919`  
		Last Modified: Tue, 21 Dec 2021 02:27:24 GMT  
		Size: 8.0 MB (8000238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a258e8ae475665e88b0ebd438d4a945fa152a99c6d2ff863c06087a6dd4c7d`  
		Last Modified: Tue, 21 Dec 2021 02:27:24 GMT  
		Size: 10.3 MB (10340145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7754201e052c276668b8474d86f55c0df401d90074d1090dc57d978ce0be1a2d`  
		Last Modified: Tue, 21 Dec 2021 02:27:48 GMT  
		Size: 53.4 MB (53438278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc31fef36efd395cde421ab27002334aa7c40a276b0a299acd89ff60b7f13ff`  
		Last Modified: Tue, 21 Dec 2021 02:28:41 GMT  
		Size: 199.0 MB (198962209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b9165c2bb91b10d141c07f8acf538767f6a2e6e3cc9c6fa70487f5f76c7ecc`  
		Last Modified: Fri, 21 Jan 2022 01:43:30 GMT  
		Size: 188.0 MB (188021848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-slim`

```console
$ docker pull rust@sha256:aef724360894cd51ff66420b688dacc811cd1591094ab9561e1a541da366d02b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-slim` - linux; amd64

```console
$ docker pull rust@sha256:c65c489f71effc81ac327df299f4f4b18f02f52a495c928949d9faef37be5c0e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.6 MB (235616218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3d2ecb28032ee0b780251c0e12ba34e4ea2b00bb6c1f54aef24cb70e40d5389`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 02:27:01 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Thu, 27 Jan 2022 02:27:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7c57d6ee4402b697e1f62306aeebe04fca5a4fcfcdd2a1c53900a71bd1ec9d`  
		Last Modified: Thu, 27 Jan 2022 02:31:42 GMT  
		Size: 204.2 MB (204249961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim` - linux; arm variant v7

```console
$ docker pull rust@sha256:5e320dc7dac05018ef56f8e75e29af46cf2b854a2bcd2c5274ec1d0838cfcfbc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.5 MB (269473502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90e30db66a12fb0b6695e5f16320fc49d165f635623f83b53332460ae2d6fd20`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 10:50:56 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 10:52:09 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6a8aa1e46b451ab566c5071e58dce324c2116d376905dec3cffab784b91947`  
		Last Modified: Wed, 26 Jan 2022 10:59:37 GMT  
		Size: 242.9 MB (242908569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:1a9113137065ce5dad9ac0092210e8df36bc896c8d44d156d3cf95a34cf4bd1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.6 MB (301595417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3c255aa040881fa57bc6f56400f12b12ab822a4448a2daa2ad75a6a412195c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:38:53 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 08:39:21 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e175c7caf143e560d9a469fb403bce557467bd7bfd7053747deacafb33fd93f1`  
		Last Modified: Wed, 26 Jan 2022 08:44:18 GMT  
		Size: 271.5 MB (271538643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim` - linux; 386

```console
$ docker pull rust@sha256:52f7d0a7ee12b806c72fc52a9123ef1df65d00645df4c9d91eb3ae8e5d3f56a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281164943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b10b451f292da4629eb4863abeb9d24f63cbce0d73a15e5c1eb595aef34a9b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Fri, 21 Jan 2022 01:40:55 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:41:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867d4c40cb0c2add04a2801c038bb1d2cc2eb532b2a7500c8c657c89ad2dc859`  
		Last Modified: Fri, 21 Jan 2022 01:47:04 GMT  
		Size: 248.8 MB (248794093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-slim-bullseye`

```console
$ docker pull rust@sha256:aef724360894cd51ff66420b688dacc811cd1591094ab9561e1a541da366d02b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-slim-bullseye` - linux; amd64

```console
$ docker pull rust@sha256:c65c489f71effc81ac327df299f4f4b18f02f52a495c928949d9faef37be5c0e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.6 MB (235616218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3d2ecb28032ee0b780251c0e12ba34e4ea2b00bb6c1f54aef24cb70e40d5389`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 02:27:01 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Thu, 27 Jan 2022 02:27:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7c57d6ee4402b697e1f62306aeebe04fca5a4fcfcdd2a1c53900a71bd1ec9d`  
		Last Modified: Thu, 27 Jan 2022 02:31:42 GMT  
		Size: 204.2 MB (204249961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-bullseye` - linux; arm variant v7

```console
$ docker pull rust@sha256:5e320dc7dac05018ef56f8e75e29af46cf2b854a2bcd2c5274ec1d0838cfcfbc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.5 MB (269473502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90e30db66a12fb0b6695e5f16320fc49d165f635623f83b53332460ae2d6fd20`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 10:50:56 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 10:52:09 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6a8aa1e46b451ab566c5071e58dce324c2116d376905dec3cffab784b91947`  
		Last Modified: Wed, 26 Jan 2022 10:59:37 GMT  
		Size: 242.9 MB (242908569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:1a9113137065ce5dad9ac0092210e8df36bc896c8d44d156d3cf95a34cf4bd1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.6 MB (301595417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3c255aa040881fa57bc6f56400f12b12ab822a4448a2daa2ad75a6a412195c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:38:53 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 08:39:21 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e175c7caf143e560d9a469fb403bce557467bd7bfd7053747deacafb33fd93f1`  
		Last Modified: Wed, 26 Jan 2022 08:44:18 GMT  
		Size: 271.5 MB (271538643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-bullseye` - linux; 386

```console
$ docker pull rust@sha256:52f7d0a7ee12b806c72fc52a9123ef1df65d00645df4c9d91eb3ae8e5d3f56a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281164943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b10b451f292da4629eb4863abeb9d24f63cbce0d73a15e5c1eb595aef34a9b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Fri, 21 Jan 2022 01:40:55 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:41:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867d4c40cb0c2add04a2801c038bb1d2cc2eb532b2a7500c8c657c89ad2dc859`  
		Last Modified: Fri, 21 Jan 2022 01:47:04 GMT  
		Size: 248.8 MB (248794093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-slim-buster`

```console
$ docker pull rust@sha256:f97b60397f841696adf7d5094e96d9f32db8b338dd0fa1a6ba3b15f6a8cbbac7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-slim-buster` - linux; amd64

```console
$ docker pull rust@sha256:d70392f42ab0402a067f47cb645ad4c5cb2fccd8de913707b5e9ffe51dccdcc7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.7 MB (216691424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d210d9c6ad548acf5f3bacefc02a1a1b844bd0c695b5d03c01d5f972efa43d23`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 02:26:06 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Thu, 27 Jan 2022 02:26:34 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfd01e1add41d50399c9c7261d9675981c573a096b2db958c6bdb4d0ba3df6e`  
		Last Modified: Thu, 27 Jan 2022 02:29:58 GMT  
		Size: 189.5 MB (189537693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:61d6f5bed2e9fd94e378eab4c9fc5a451caef607f6ac14ffc3fe0f5f7c6109e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.3 MB (256276557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b30e8b184d6c2e016890c87dc71ab25296222a2e934531f2e31c6a7d61046271`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:12 GMT
ADD file:ca8132e20773f7037458cc53fe20a7116f93c21c7479be5a2a1d739495dbe44e in / 
# Wed, 26 Jan 2022 01:43:13 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 10:49:05 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 10:50:20 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:20cc49690d9072283406c1c11e9b1dc1a247782cc8daa526b375d4a7f1cb6a94`  
		Last Modified: Wed, 26 Jan 2022 01:59:27 GMT  
		Size: 22.8 MB (22754397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539f3b7106a14210296dc07ec5c5275b3b7124abffcf23c25d6f79ae330d28b1`  
		Last Modified: Wed, 26 Jan 2022 10:56:40 GMT  
		Size: 233.5 MB (233522160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:fd60d456c8c1818a9f71d0063e20a1d869aa48429afae7f81f24a9b51883a4d1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.0 MB (281957084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35221a2f076a920466686f0e6c540ef9879dfe37e9adaa83ea380eb09bcb5e74`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:37:51 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 08:38:18 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2765579f339812249621170a70c8cf8430422b746c7163efc3ffe0d2a5b00c6e`  
		Last Modified: Wed, 26 Jan 2022 08:42:15 GMT  
		Size: 256.0 MB (256033868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-buster` - linux; 386

```console
$ docker pull rust@sha256:17efe31938303253b8d9e3afa66de629c033db64a3d9831623d9eb1443865fc7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.8 MB (265819912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07de88a206564ac8ad3534d14868b8b1af2b6375eaf06529bca7af5dc6f685d0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:45 GMT
ADD file:78342a77df22ca22804ea5aec6415ce10c1fdc35687f1b25c5f86850f41d3905 in / 
# Tue, 21 Dec 2021 01:40:45 GMT
CMD ["bash"]
# Fri, 21 Jan 2022 01:39:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:40:14 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:16e3a221bce3a5f7f4a71f72926f381ff9c6141ccb5918b7ea924ff7f7f09d06`  
		Last Modified: Tue, 21 Dec 2021 01:49:46 GMT  
		Size: 27.8 MB (27804573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d81babe2c3794639ff06bb2e5ad026aca8afabb13a8d2e7006bf1795a7e7f4`  
		Last Modified: Fri, 21 Jan 2022 01:44:39 GMT  
		Size: 238.0 MB (238015339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.58`

```console
$ docker pull rust@sha256:8ad28b7355e19dad2677624622bad1cc978b6fd34b45e75d17c25f558f94a934
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.58` - linux; amd64

```console
$ docker pull rust@sha256:d46142e07db17a179a9cd18bc814c5c7e1499fdd12147f9249ee48c540aec0d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.2 MB (466162023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:269d9943b0d310e1ab49a55e14752596567a74daa37270c6217abfc33f48f7f5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 02:26:40 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Thu, 27 Jan 2022 02:26:56 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808edda3c2e855dc13af758b35cefbcc417ad1ab4fead7f72234b09aeda893a0`  
		Last Modified: Wed, 26 Jan 2022 02:23:16 GMT  
		Size: 196.5 MB (196529197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4671d83ec37ad7f7bf397a8340e76ed6b965029035e63a4a2043351fcd40d892`  
		Last Modified: Thu, 27 Jan 2022 02:30:45 GMT  
		Size: 144.1 MB (144123702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58` - linux; arm variant v7

```console
$ docker pull rust@sha256:32e5c60294d2cd912122e23d42e330e63a9a8754443b8654a3ea8df1e75ba397
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **483.2 MB (483165594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8faf3dd2fdb2285b82cf07285b1b0bf7d34d46d0478e7996e3f0369398d7528b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:59:11 GMT
ADD file:848bf729bc16d3b188567f096ee1c0386cb49825a06eef396401278afee2f4c7 in / 
# Tue, 21 Dec 2021 01:59:12 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:46:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:46:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:47:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:49:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 06:11:05 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 06:11:46 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:fd92fbcda272f5935dcd0dfea445cba0152208f83c8fc8d2cb74c85379145c42`  
		Last Modified: Tue, 21 Dec 2021 02:14:41 GMT  
		Size: 50.1 MB (50121433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a6987ee02fad9d702adbd7921b8e1776b1a091773dd47886055113b1d7ba62`  
		Last Modified: Tue, 21 Dec 2021 03:11:46 GMT  
		Size: 4.9 MB (4922490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6d85cbb278c8e4845f79838154b77c36931e65f9b5bb9b8f56c92f41f72e27`  
		Last Modified: Tue, 21 Dec 2021 03:11:47 GMT  
		Size: 10.2 MB (10217004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bd566d277d8d03e1b76768a074dd92306bc287eef88c42a08ef5b48b842fa1`  
		Last Modified: Tue, 21 Dec 2021 03:12:37 GMT  
		Size: 50.3 MB (50328047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edcf448232b2036e5813fc0174bcd35c3a967a79cf2ef79bc2bfb0410c7b176e`  
		Last Modified: Tue, 21 Dec 2021 03:14:27 GMT  
		Size: 167.0 MB (166954318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2393fcae1480a3e448c675f4654fccb4999808ae81fd8438665649bd7809cd`  
		Last Modified: Fri, 21 Jan 2022 06:22:33 GMT  
		Size: 200.6 MB (200622302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:71e628671e7232373f1babb49f78f1751c5151af8ac6dc2c5cfaacf60c08c627
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **529.3 MB (529331157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28baec511a7c725b2502fe4dbcda7a5e4740cb19806b922bfcbfbb35cd1d9c13`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:38:28 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 08:38:45 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cb4eca0cebfb68f0cb8dd7e6c0c67b880fcae929406705b4d43a2df4fa48eb`  
		Last Modified: Wed, 26 Jan 2022 02:24:49 GMT  
		Size: 189.4 MB (189420652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2d141dc211541426cd6794767a1439b2ead45ccdae9e55c89c1f6d1b46ce7b`  
		Last Modified: Wed, 26 Jan 2022 08:43:08 GMT  
		Size: 215.8 MB (215834728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58` - linux; 386

```console
$ docker pull rust@sha256:00a04734a44749afb4e6a7c8c294d3e9a5c169bb091601036d41044241f8d9eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.8 MB (515847461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9787ce8e926d4bc03f1104f353c79e89b71d8453c15fa4f707118ef27a84595e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:39:40 GMT
ADD file:b77df0839dfb103f5f16329bfa0dcf40c1a73b02e312bb2be40ad620f64e7949 in / 
# Tue, 21 Dec 2021 01:39:44 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:13:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:13:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:13:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:14:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 01:40:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:40:45 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:c13b09ebb011541c3f3a6e423452bf5046e5ba48dfee18e88cc3e3df477c0baa`  
		Last Modified: Tue, 21 Dec 2021 01:48:09 GMT  
		Size: 55.9 MB (55925399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0db4e702162a700c3f00a3624f94bbfa81fd2077b8c5cf57f455659259295a`  
		Last Modified: Tue, 21 Dec 2021 02:25:41 GMT  
		Size: 5.3 MB (5282974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4fb971a29956de966e154c96a2d7f1eb56aed081b583947be033c05d7c69797`  
		Last Modified: Tue, 21 Dec 2021 02:25:42 GMT  
		Size: 11.3 MB (11250616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb3ec563e1e552271ac9c80a2b348ebf47401940583ca295fc5f1378ca9d3ac`  
		Last Modified: Tue, 21 Dec 2021 02:26:11 GMT  
		Size: 55.9 MB (55917390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2c2a9657022eac58df44f2cef58c0e28b506b12f67dece31bf9bd280de6d6f`  
		Last Modified: Tue, 21 Dec 2021 02:27:07 GMT  
		Size: 199.4 MB (199449263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae4e6ced7d216b439b6a4b3cfffd9957baaa2093e769d5da2f657972bb99a96`  
		Last Modified: Fri, 21 Jan 2022 01:45:38 GMT  
		Size: 188.0 MB (188021819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.58-alpine`

```console
$ docker pull rust@sha256:b61698ea823c6f9bc726272d7783867d89e79ca87e9944998739ce619da7699a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:1.58-alpine` - linux; amd64

```console
$ docker pull rust@sha256:d4c641c867f8d60f1f4da8edc19da4ea6543dd54f5cfd4c4cb713a438f9ed079
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.6 MB (269634647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:953451d7b194820db2946de86d08aa997c88d7e3f5f728f577d20cf4c4c210d9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Thu, 13 Jan 2022 20:26:04 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 21 Jan 2022 01:22:17 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:22:38 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93cd12ff80a853b96704224019bf0b85bbe94d9b9456b619b95ab0a8dbdf40d`  
		Last Modified: Thu, 13 Jan 2022 20:31:39 GMT  
		Size: 42.5 MB (42495579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9781e95f2a775fd7a289185a1bcbd1e616c15547d6ab73d8e78dfbb1c99514c`  
		Last Modified: Fri, 21 Jan 2022 01:28:49 GMT  
		Size: 224.3 MB (224320655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58-alpine` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:58a1a37e622250ca1f6f16bb1449e714632dcd7deddc0e2f38b8a05c92e54e55
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.0 MB (254960114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8a5a57c57976585d381f3fd0fe33476127b6dda4fa4e767a620e54314c92118`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Thu, 13 Jan 2022 20:42:58 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 21 Jan 2022 01:42:50 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:43:07 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec7b33c7ee4d79979b266a321f626981b48087e7524811342d73ce2e2eb9e57`  
		Last Modified: Thu, 13 Jan 2022 20:49:23 GMT  
		Size: 36.1 MB (36087204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fec8b7bac538e28495e4763ae0710d8b74d160b4b9b4cda13fbf6269d3283f`  
		Last Modified: Fri, 21 Jan 2022 01:49:44 GMT  
		Size: 216.2 MB (216157476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.58-alpine3.14`

```console
$ docker pull rust@sha256:2292543650f33917efbb8da25a303848cc72fad0cb95a0320277f99d3ce92046
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:1.58-alpine3.14` - linux; amd64

```console
$ docker pull rust@sha256:fbc0cfaa6261179ca7653cc2b20ca9c3e936f3416a911a27a28694f8fb23b8b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.5 MB (269494735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e35d9d35ab3792f9f41494f2fa73e8057080db430deb0bceddf896a605a6582`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 07:44:00 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 21 Jan 2022 01:21:49 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:22:11 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95f12a5672fd92cc370cc8ec78127e6c52a6d61404662fab9d5643b661f3e8b`  
		Last Modified: Sat, 13 Nov 2021 07:46:42 GMT  
		Size: 42.4 MB (42351276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be615768698a2e1df78b3e911bccea805cbacfcb7972586bb677332badfe97fb`  
		Last Modified: Fri, 21 Jan 2022 01:27:52 GMT  
		Size: 224.3 MB (224320478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:7dd68b020a1550ed5cd7974188763c0831aea119f73fd1327b25972b6656962f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.8 MB (254813562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45aad15a39b3ffaf28e25228529764e9ad0408ff6182c9a9f30b8ab31fdb92fc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 17:55:55 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 21 Jan 2022 01:42:27 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:42:44 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3394b2150e94a1388a8ac369dcfa5974566be0e105ccecfe1f50dbeedd25887d`  
		Last Modified: Fri, 12 Nov 2021 17:58:34 GMT  
		Size: 35.9 MB (35938392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d19cdf6d774da55657d17c1d24e8390cce8b2f8cced8100d85ea1e51c82d13e`  
		Last Modified: Fri, 21 Jan 2022 01:48:56 GMT  
		Size: 216.2 MB (216157470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.58-alpine3.15`

```console
$ docker pull rust@sha256:b61698ea823c6f9bc726272d7783867d89e79ca87e9944998739ce619da7699a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:1.58-alpine3.15` - linux; amd64

```console
$ docker pull rust@sha256:d4c641c867f8d60f1f4da8edc19da4ea6543dd54f5cfd4c4cb713a438f9ed079
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.6 MB (269634647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:953451d7b194820db2946de86d08aa997c88d7e3f5f728f577d20cf4c4c210d9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Thu, 13 Jan 2022 20:26:04 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 21 Jan 2022 01:22:17 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:22:38 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93cd12ff80a853b96704224019bf0b85bbe94d9b9456b619b95ab0a8dbdf40d`  
		Last Modified: Thu, 13 Jan 2022 20:31:39 GMT  
		Size: 42.5 MB (42495579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9781e95f2a775fd7a289185a1bcbd1e616c15547d6ab73d8e78dfbb1c99514c`  
		Last Modified: Fri, 21 Jan 2022 01:28:49 GMT  
		Size: 224.3 MB (224320655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:58a1a37e622250ca1f6f16bb1449e714632dcd7deddc0e2f38b8a05c92e54e55
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.0 MB (254960114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8a5a57c57976585d381f3fd0fe33476127b6dda4fa4e767a620e54314c92118`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Thu, 13 Jan 2022 20:42:58 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 21 Jan 2022 01:42:50 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:43:07 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec7b33c7ee4d79979b266a321f626981b48087e7524811342d73ce2e2eb9e57`  
		Last Modified: Thu, 13 Jan 2022 20:49:23 GMT  
		Size: 36.1 MB (36087204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fec8b7bac538e28495e4763ae0710d8b74d160b4b9b4cda13fbf6269d3283f`  
		Last Modified: Fri, 21 Jan 2022 01:49:44 GMT  
		Size: 216.2 MB (216157476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.58-bullseye`

```console
$ docker pull rust@sha256:8ad28b7355e19dad2677624622bad1cc978b6fd34b45e75d17c25f558f94a934
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.58-bullseye` - linux; amd64

```console
$ docker pull rust@sha256:d46142e07db17a179a9cd18bc814c5c7e1499fdd12147f9249ee48c540aec0d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.2 MB (466162023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:269d9943b0d310e1ab49a55e14752596567a74daa37270c6217abfc33f48f7f5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 02:26:40 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Thu, 27 Jan 2022 02:26:56 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808edda3c2e855dc13af758b35cefbcc417ad1ab4fead7f72234b09aeda893a0`  
		Last Modified: Wed, 26 Jan 2022 02:23:16 GMT  
		Size: 196.5 MB (196529197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4671d83ec37ad7f7bf397a8340e76ed6b965029035e63a4a2043351fcd40d892`  
		Last Modified: Thu, 27 Jan 2022 02:30:45 GMT  
		Size: 144.1 MB (144123702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58-bullseye` - linux; arm variant v7

```console
$ docker pull rust@sha256:32e5c60294d2cd912122e23d42e330e63a9a8754443b8654a3ea8df1e75ba397
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **483.2 MB (483165594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8faf3dd2fdb2285b82cf07285b1b0bf7d34d46d0478e7996e3f0369398d7528b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:59:11 GMT
ADD file:848bf729bc16d3b188567f096ee1c0386cb49825a06eef396401278afee2f4c7 in / 
# Tue, 21 Dec 2021 01:59:12 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:46:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:46:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:47:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:49:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 06:11:05 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 06:11:46 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:fd92fbcda272f5935dcd0dfea445cba0152208f83c8fc8d2cb74c85379145c42`  
		Last Modified: Tue, 21 Dec 2021 02:14:41 GMT  
		Size: 50.1 MB (50121433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a6987ee02fad9d702adbd7921b8e1776b1a091773dd47886055113b1d7ba62`  
		Last Modified: Tue, 21 Dec 2021 03:11:46 GMT  
		Size: 4.9 MB (4922490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6d85cbb278c8e4845f79838154b77c36931e65f9b5bb9b8f56c92f41f72e27`  
		Last Modified: Tue, 21 Dec 2021 03:11:47 GMT  
		Size: 10.2 MB (10217004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bd566d277d8d03e1b76768a074dd92306bc287eef88c42a08ef5b48b842fa1`  
		Last Modified: Tue, 21 Dec 2021 03:12:37 GMT  
		Size: 50.3 MB (50328047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edcf448232b2036e5813fc0174bcd35c3a967a79cf2ef79bc2bfb0410c7b176e`  
		Last Modified: Tue, 21 Dec 2021 03:14:27 GMT  
		Size: 167.0 MB (166954318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2393fcae1480a3e448c675f4654fccb4999808ae81fd8438665649bd7809cd`  
		Last Modified: Fri, 21 Jan 2022 06:22:33 GMT  
		Size: 200.6 MB (200622302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58-bullseye` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:71e628671e7232373f1babb49f78f1751c5151af8ac6dc2c5cfaacf60c08c627
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **529.3 MB (529331157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28baec511a7c725b2502fe4dbcda7a5e4740cb19806b922bfcbfbb35cd1d9c13`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:38:28 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 08:38:45 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cb4eca0cebfb68f0cb8dd7e6c0c67b880fcae929406705b4d43a2df4fa48eb`  
		Last Modified: Wed, 26 Jan 2022 02:24:49 GMT  
		Size: 189.4 MB (189420652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2d141dc211541426cd6794767a1439b2ead45ccdae9e55c89c1f6d1b46ce7b`  
		Last Modified: Wed, 26 Jan 2022 08:43:08 GMT  
		Size: 215.8 MB (215834728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58-bullseye` - linux; 386

```console
$ docker pull rust@sha256:00a04734a44749afb4e6a7c8c294d3e9a5c169bb091601036d41044241f8d9eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.8 MB (515847461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9787ce8e926d4bc03f1104f353c79e89b71d8453c15fa4f707118ef27a84595e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:39:40 GMT
ADD file:b77df0839dfb103f5f16329bfa0dcf40c1a73b02e312bb2be40ad620f64e7949 in / 
# Tue, 21 Dec 2021 01:39:44 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:13:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:13:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:13:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:14:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 01:40:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:40:45 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:c13b09ebb011541c3f3a6e423452bf5046e5ba48dfee18e88cc3e3df477c0baa`  
		Last Modified: Tue, 21 Dec 2021 01:48:09 GMT  
		Size: 55.9 MB (55925399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0db4e702162a700c3f00a3624f94bbfa81fd2077b8c5cf57f455659259295a`  
		Last Modified: Tue, 21 Dec 2021 02:25:41 GMT  
		Size: 5.3 MB (5282974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4fb971a29956de966e154c96a2d7f1eb56aed081b583947be033c05d7c69797`  
		Last Modified: Tue, 21 Dec 2021 02:25:42 GMT  
		Size: 11.3 MB (11250616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb3ec563e1e552271ac9c80a2b348ebf47401940583ca295fc5f1378ca9d3ac`  
		Last Modified: Tue, 21 Dec 2021 02:26:11 GMT  
		Size: 55.9 MB (55917390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2c2a9657022eac58df44f2cef58c0e28b506b12f67dece31bf9bd280de6d6f`  
		Last Modified: Tue, 21 Dec 2021 02:27:07 GMT  
		Size: 199.4 MB (199449263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae4e6ced7d216b439b6a4b3cfffd9957baaa2093e769d5da2f657972bb99a96`  
		Last Modified: Fri, 21 Jan 2022 01:45:38 GMT  
		Size: 188.0 MB (188021819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.58-buster`

```console
$ docker pull rust@sha256:e3a1c9b64e1c028851e24fba7d846dbe11edb2463fdb2e4bae2b731c0bc86463
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.58-buster` - linux; amd64

```console
$ docker pull rust@sha256:5dad83d6154d9b7d5a454e487292a818f1a49c310d22d28d027dace34ade540d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **456.7 MB (456656132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4737b5f9e43d2dc30e66ad37c2bf4a078f46b8b9e7e751b650e9e082e76e1a7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:47 GMT
ADD file:a290acee3581e1e9c42c0a37b53086a8f070cb0730179be81a6ba24a620b6ee4 in / 
# Wed, 26 Jan 2022 01:40:47 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 02:25:47 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Thu, 27 Jan 2022 02:26:02 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:a024302f8a017855dd20a107ace079dd543c4bdfa8e7c11472771babbe298d2b`  
		Last Modified: Wed, 26 Jan 2022 01:47:01 GMT  
		Size: 50.4 MB (50437057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289773030fdc98afe6cc53bdd0c05332ea8ff21ad836afa1d3042388953c43f8`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 7.8 MB (7833856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bb8b3399fe8dd0b83bd5e32a97e5183ab235d6fb4cc0b5dfabb20e6653e715`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 10.0 MB (9997205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c63da771697b362929cecc84777e8cfbb716ff3d575b999854d83ada039b695`  
		Last Modified: Wed, 26 Jan 2022 02:23:53 GMT  
		Size: 51.8 MB (51839910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf1b23b1e4b1867b70ba7f0614dff34bdb468c2a860a7b162c74c2b451494c0`  
		Last Modified: Wed, 26 Jan 2022 02:24:38 GMT  
		Size: 192.4 MB (192424405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbadc5241c680bb76f81237047194a1d408a37104d21cfc421439a941bc0d5a3`  
		Last Modified: Thu, 27 Jan 2022 02:29:05 GMT  
		Size: 144.1 MB (144123699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:1ccaa939ec2bcd17833886a87ae632de27c7b25738510f45f9573a0a6802f50b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **479.0 MB (478973771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e5e34aeb2594b6b0ea9e8b59acf1d371889f6b13ace574de70235c1cb3cdab3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:17 GMT
ADD file:36bf5b8bdd9066b06cc35d26df3f4dad2b1cbcb41985b85f070ed97a3e85f8a9 in / 
# Tue, 21 Dec 2021 02:00:18 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:49:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:50:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:53:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 06:08:33 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 06:09:16 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:328389035fdd79ece4f520541a84b3de974050fe012ed1566da6b869dd34ea29`  
		Last Modified: Tue, 21 Dec 2021 02:16:11 GMT  
		Size: 45.9 MB (45918102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80397c5626b1d4e58b7b7dd9219674dd86caa03ddcaac1d3d6791189a44b0ff`  
		Last Modified: Tue, 21 Dec 2021 03:14:47 GMT  
		Size: 7.1 MB (7125168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816c475148f8e55cc2b8593f29d0ddd67ad1359f3c69061f043d461495bad179`  
		Last Modified: Tue, 21 Dec 2021 03:14:48 GMT  
		Size: 9.3 MB (9343808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d30bc5ea112783bdcbfaba962b58338c0f61b12d68a5cc7474c0b639098c6a`  
		Last Modified: Tue, 21 Dec 2021 03:15:32 GMT  
		Size: 47.4 MB (47356397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93be0f932a74231c59bf289b331a4b22b2346e3532b93f7c9a3d1eb60859f40b`  
		Last Modified: Tue, 21 Dec 2021 03:17:17 GMT  
		Size: 168.6 MB (168607961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e21137e326fc09ba91d9592481ee83a4c7e5b8458ffd21c0f488c9edb3d3bbd`  
		Last Modified: Fri, 21 Jan 2022 06:17:28 GMT  
		Size: 200.6 MB (200622335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:611b00bf3064be66516b9bd9af0a31bbdf0d7535edb4ea5fa6ee5e41bf6c157b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **518.7 MB (518694576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bc36b7a17a62b420f4f1b26c9a9ffee6132533be64f06904a8e51a73622d362`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:41 GMT
ADD file:98a75269e438ff15cee16ad2763fe2698fb436bc4770c0ca27c059f66b65e56a in / 
# Wed, 26 Jan 2022 01:42:42 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:14:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:14:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:15:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:37:25 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 08:37:44 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:ccd458f933f7966e412773ee1551aaf2433a5bf9adaae519e2ac7c9c3f8b5f89`  
		Last Modified: Wed, 26 Jan 2022 01:49:28 GMT  
		Size: 49.2 MB (49223041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3524e6d2c855bef1f32da73e00738b2e5e91e6a346d19f8b33e8e8117c82748`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 7.7 MB (7695112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cc9cf00cd9023559aeda43668c7d9d621318631bab103ae03b8a3787260048`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 9.8 MB (9767300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f0325e59cadc58f4e81c6a282319b0c01f54964ef989205974a6557cf15040`  
		Last Modified: Wed, 26 Jan 2022 02:25:25 GMT  
		Size: 52.2 MB (52168727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b289063aa004828178bcfddecfcf2fda082ce1cb1657eb68a9ef23e027a510b`  
		Last Modified: Wed, 26 Jan 2022 02:26:00 GMT  
		Size: 184.0 MB (184005857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af714e5ef49569fce78ac8d86129c0d70407051af674aadee820dbf5f6d118a`  
		Last Modified: Wed, 26 Jan 2022 08:41:20 GMT  
		Size: 215.8 MB (215834539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58-buster` - linux; 386

```console
$ docker pull rust@sha256:4fde2447b7b5bd85bc6e955b14004027e985963d6db7377793371fcb4d904374
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **510.0 MB (509970484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24aac74c874dfb49adbce2fad1afd33ce899db1b13c2342e96e959c68eb4b7a4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:24 GMT
ADD file:4e982be228380a8d7632e31f19e39ed55ee76fb1db32130fa88d696904d6acde in / 
# Tue, 21 Dec 2021 01:40:25 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:15:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:15:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:15:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:17:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 01:38:53 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:39:15 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:342b01a61e0af68dc09681004efdfcf66d0443632988d6f247dd7b34bc18b1db`  
		Last Modified: Tue, 21 Dec 2021 01:49:14 GMT  
		Size: 51.2 MB (51207766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4759b0dba897041c21e226a9db50a85ca5685f19bb5036f16df5b231fd177919`  
		Last Modified: Tue, 21 Dec 2021 02:27:24 GMT  
		Size: 8.0 MB (8000238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a258e8ae475665e88b0ebd438d4a945fa152a99c6d2ff863c06087a6dd4c7d`  
		Last Modified: Tue, 21 Dec 2021 02:27:24 GMT  
		Size: 10.3 MB (10340145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7754201e052c276668b8474d86f55c0df401d90074d1090dc57d978ce0be1a2d`  
		Last Modified: Tue, 21 Dec 2021 02:27:48 GMT  
		Size: 53.4 MB (53438278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc31fef36efd395cde421ab27002334aa7c40a276b0a299acd89ff60b7f13ff`  
		Last Modified: Tue, 21 Dec 2021 02:28:41 GMT  
		Size: 199.0 MB (198962209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b9165c2bb91b10d141c07f8acf538767f6a2e6e3cc9c6fa70487f5f76c7ecc`  
		Last Modified: Fri, 21 Jan 2022 01:43:30 GMT  
		Size: 188.0 MB (188021848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.58-slim`

```console
$ docker pull rust@sha256:aef724360894cd51ff66420b688dacc811cd1591094ab9561e1a541da366d02b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.58-slim` - linux; amd64

```console
$ docker pull rust@sha256:c65c489f71effc81ac327df299f4f4b18f02f52a495c928949d9faef37be5c0e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.6 MB (235616218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3d2ecb28032ee0b780251c0e12ba34e4ea2b00bb6c1f54aef24cb70e40d5389`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 02:27:01 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Thu, 27 Jan 2022 02:27:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7c57d6ee4402b697e1f62306aeebe04fca5a4fcfcdd2a1c53900a71bd1ec9d`  
		Last Modified: Thu, 27 Jan 2022 02:31:42 GMT  
		Size: 204.2 MB (204249961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58-slim` - linux; arm variant v7

```console
$ docker pull rust@sha256:5e320dc7dac05018ef56f8e75e29af46cf2b854a2bcd2c5274ec1d0838cfcfbc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.5 MB (269473502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90e30db66a12fb0b6695e5f16320fc49d165f635623f83b53332460ae2d6fd20`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 10:50:56 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 10:52:09 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6a8aa1e46b451ab566c5071e58dce324c2116d376905dec3cffab784b91947`  
		Last Modified: Wed, 26 Jan 2022 10:59:37 GMT  
		Size: 242.9 MB (242908569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58-slim` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:1a9113137065ce5dad9ac0092210e8df36bc896c8d44d156d3cf95a34cf4bd1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.6 MB (301595417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3c255aa040881fa57bc6f56400f12b12ab822a4448a2daa2ad75a6a412195c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:38:53 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 08:39:21 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e175c7caf143e560d9a469fb403bce557467bd7bfd7053747deacafb33fd93f1`  
		Last Modified: Wed, 26 Jan 2022 08:44:18 GMT  
		Size: 271.5 MB (271538643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58-slim` - linux; 386

```console
$ docker pull rust@sha256:52f7d0a7ee12b806c72fc52a9123ef1df65d00645df4c9d91eb3ae8e5d3f56a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281164943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b10b451f292da4629eb4863abeb9d24f63cbce0d73a15e5c1eb595aef34a9b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Fri, 21 Jan 2022 01:40:55 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:41:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867d4c40cb0c2add04a2801c038bb1d2cc2eb532b2a7500c8c657c89ad2dc859`  
		Last Modified: Fri, 21 Jan 2022 01:47:04 GMT  
		Size: 248.8 MB (248794093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.58-slim-bullseye`

```console
$ docker pull rust@sha256:aef724360894cd51ff66420b688dacc811cd1591094ab9561e1a541da366d02b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.58-slim-bullseye` - linux; amd64

```console
$ docker pull rust@sha256:c65c489f71effc81ac327df299f4f4b18f02f52a495c928949d9faef37be5c0e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.6 MB (235616218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3d2ecb28032ee0b780251c0e12ba34e4ea2b00bb6c1f54aef24cb70e40d5389`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 02:27:01 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Thu, 27 Jan 2022 02:27:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7c57d6ee4402b697e1f62306aeebe04fca5a4fcfcdd2a1c53900a71bd1ec9d`  
		Last Modified: Thu, 27 Jan 2022 02:31:42 GMT  
		Size: 204.2 MB (204249961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58-slim-bullseye` - linux; arm variant v7

```console
$ docker pull rust@sha256:5e320dc7dac05018ef56f8e75e29af46cf2b854a2bcd2c5274ec1d0838cfcfbc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.5 MB (269473502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90e30db66a12fb0b6695e5f16320fc49d165f635623f83b53332460ae2d6fd20`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 10:50:56 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 10:52:09 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6a8aa1e46b451ab566c5071e58dce324c2116d376905dec3cffab784b91947`  
		Last Modified: Wed, 26 Jan 2022 10:59:37 GMT  
		Size: 242.9 MB (242908569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:1a9113137065ce5dad9ac0092210e8df36bc896c8d44d156d3cf95a34cf4bd1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.6 MB (301595417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3c255aa040881fa57bc6f56400f12b12ab822a4448a2daa2ad75a6a412195c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:38:53 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 08:39:21 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e175c7caf143e560d9a469fb403bce557467bd7bfd7053747deacafb33fd93f1`  
		Last Modified: Wed, 26 Jan 2022 08:44:18 GMT  
		Size: 271.5 MB (271538643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58-slim-bullseye` - linux; 386

```console
$ docker pull rust@sha256:52f7d0a7ee12b806c72fc52a9123ef1df65d00645df4c9d91eb3ae8e5d3f56a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281164943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b10b451f292da4629eb4863abeb9d24f63cbce0d73a15e5c1eb595aef34a9b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Fri, 21 Jan 2022 01:40:55 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:41:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867d4c40cb0c2add04a2801c038bb1d2cc2eb532b2a7500c8c657c89ad2dc859`  
		Last Modified: Fri, 21 Jan 2022 01:47:04 GMT  
		Size: 248.8 MB (248794093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.58-slim-buster`

```console
$ docker pull rust@sha256:f97b60397f841696adf7d5094e96d9f32db8b338dd0fa1a6ba3b15f6a8cbbac7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.58-slim-buster` - linux; amd64

```console
$ docker pull rust@sha256:d70392f42ab0402a067f47cb645ad4c5cb2fccd8de913707b5e9ffe51dccdcc7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.7 MB (216691424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d210d9c6ad548acf5f3bacefc02a1a1b844bd0c695b5d03c01d5f972efa43d23`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 02:26:06 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Thu, 27 Jan 2022 02:26:34 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfd01e1add41d50399c9c7261d9675981c573a096b2db958c6bdb4d0ba3df6e`  
		Last Modified: Thu, 27 Jan 2022 02:29:58 GMT  
		Size: 189.5 MB (189537693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58-slim-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:61d6f5bed2e9fd94e378eab4c9fc5a451caef607f6ac14ffc3fe0f5f7c6109e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.3 MB (256276557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b30e8b184d6c2e016890c87dc71ab25296222a2e934531f2e31c6a7d61046271`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:12 GMT
ADD file:ca8132e20773f7037458cc53fe20a7116f93c21c7479be5a2a1d739495dbe44e in / 
# Wed, 26 Jan 2022 01:43:13 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 10:49:05 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 10:50:20 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:20cc49690d9072283406c1c11e9b1dc1a247782cc8daa526b375d4a7f1cb6a94`  
		Last Modified: Wed, 26 Jan 2022 01:59:27 GMT  
		Size: 22.8 MB (22754397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539f3b7106a14210296dc07ec5c5275b3b7124abffcf23c25d6f79ae330d28b1`  
		Last Modified: Wed, 26 Jan 2022 10:56:40 GMT  
		Size: 233.5 MB (233522160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58-slim-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:fd60d456c8c1818a9f71d0063e20a1d869aa48429afae7f81f24a9b51883a4d1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.0 MB (281957084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35221a2f076a920466686f0e6c540ef9879dfe37e9adaa83ea380eb09bcb5e74`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:37:51 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 08:38:18 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2765579f339812249621170a70c8cf8430422b746c7163efc3ffe0d2a5b00c6e`  
		Last Modified: Wed, 26 Jan 2022 08:42:15 GMT  
		Size: 256.0 MB (256033868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58-slim-buster` - linux; 386

```console
$ docker pull rust@sha256:17efe31938303253b8d9e3afa66de629c033db64a3d9831623d9eb1443865fc7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.8 MB (265819912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07de88a206564ac8ad3534d14868b8b1af2b6375eaf06529bca7af5dc6f685d0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:45 GMT
ADD file:78342a77df22ca22804ea5aec6415ce10c1fdc35687f1b25c5f86850f41d3905 in / 
# Tue, 21 Dec 2021 01:40:45 GMT
CMD ["bash"]
# Fri, 21 Jan 2022 01:39:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:40:14 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:16e3a221bce3a5f7f4a71f72926f381ff9c6141ccb5918b7ea924ff7f7f09d06`  
		Last Modified: Tue, 21 Dec 2021 01:49:46 GMT  
		Size: 27.8 MB (27804573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d81babe2c3794639ff06bb2e5ad026aca8afabb13a8d2e7006bf1795a7e7f4`  
		Last Modified: Fri, 21 Jan 2022 01:44:39 GMT  
		Size: 238.0 MB (238015339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.58.1`

```console
$ docker pull rust@sha256:8ad28b7355e19dad2677624622bad1cc978b6fd34b45e75d17c25f558f94a934
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.58.1` - linux; amd64

```console
$ docker pull rust@sha256:d46142e07db17a179a9cd18bc814c5c7e1499fdd12147f9249ee48c540aec0d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.2 MB (466162023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:269d9943b0d310e1ab49a55e14752596567a74daa37270c6217abfc33f48f7f5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 02:26:40 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Thu, 27 Jan 2022 02:26:56 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808edda3c2e855dc13af758b35cefbcc417ad1ab4fead7f72234b09aeda893a0`  
		Last Modified: Wed, 26 Jan 2022 02:23:16 GMT  
		Size: 196.5 MB (196529197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4671d83ec37ad7f7bf397a8340e76ed6b965029035e63a4a2043351fcd40d892`  
		Last Modified: Thu, 27 Jan 2022 02:30:45 GMT  
		Size: 144.1 MB (144123702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58.1` - linux; arm variant v7

```console
$ docker pull rust@sha256:32e5c60294d2cd912122e23d42e330e63a9a8754443b8654a3ea8df1e75ba397
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **483.2 MB (483165594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8faf3dd2fdb2285b82cf07285b1b0bf7d34d46d0478e7996e3f0369398d7528b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:59:11 GMT
ADD file:848bf729bc16d3b188567f096ee1c0386cb49825a06eef396401278afee2f4c7 in / 
# Tue, 21 Dec 2021 01:59:12 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:46:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:46:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:47:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:49:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 06:11:05 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 06:11:46 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:fd92fbcda272f5935dcd0dfea445cba0152208f83c8fc8d2cb74c85379145c42`  
		Last Modified: Tue, 21 Dec 2021 02:14:41 GMT  
		Size: 50.1 MB (50121433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a6987ee02fad9d702adbd7921b8e1776b1a091773dd47886055113b1d7ba62`  
		Last Modified: Tue, 21 Dec 2021 03:11:46 GMT  
		Size: 4.9 MB (4922490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6d85cbb278c8e4845f79838154b77c36931e65f9b5bb9b8f56c92f41f72e27`  
		Last Modified: Tue, 21 Dec 2021 03:11:47 GMT  
		Size: 10.2 MB (10217004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bd566d277d8d03e1b76768a074dd92306bc287eef88c42a08ef5b48b842fa1`  
		Last Modified: Tue, 21 Dec 2021 03:12:37 GMT  
		Size: 50.3 MB (50328047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edcf448232b2036e5813fc0174bcd35c3a967a79cf2ef79bc2bfb0410c7b176e`  
		Last Modified: Tue, 21 Dec 2021 03:14:27 GMT  
		Size: 167.0 MB (166954318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2393fcae1480a3e448c675f4654fccb4999808ae81fd8438665649bd7809cd`  
		Last Modified: Fri, 21 Jan 2022 06:22:33 GMT  
		Size: 200.6 MB (200622302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58.1` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:71e628671e7232373f1babb49f78f1751c5151af8ac6dc2c5cfaacf60c08c627
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **529.3 MB (529331157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28baec511a7c725b2502fe4dbcda7a5e4740cb19806b922bfcbfbb35cd1d9c13`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:38:28 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 08:38:45 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cb4eca0cebfb68f0cb8dd7e6c0c67b880fcae929406705b4d43a2df4fa48eb`  
		Last Modified: Wed, 26 Jan 2022 02:24:49 GMT  
		Size: 189.4 MB (189420652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2d141dc211541426cd6794767a1439b2ead45ccdae9e55c89c1f6d1b46ce7b`  
		Last Modified: Wed, 26 Jan 2022 08:43:08 GMT  
		Size: 215.8 MB (215834728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58.1` - linux; 386

```console
$ docker pull rust@sha256:00a04734a44749afb4e6a7c8c294d3e9a5c169bb091601036d41044241f8d9eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.8 MB (515847461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9787ce8e926d4bc03f1104f353c79e89b71d8453c15fa4f707118ef27a84595e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:39:40 GMT
ADD file:b77df0839dfb103f5f16329bfa0dcf40c1a73b02e312bb2be40ad620f64e7949 in / 
# Tue, 21 Dec 2021 01:39:44 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:13:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:13:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:13:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:14:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 01:40:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:40:45 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:c13b09ebb011541c3f3a6e423452bf5046e5ba48dfee18e88cc3e3df477c0baa`  
		Last Modified: Tue, 21 Dec 2021 01:48:09 GMT  
		Size: 55.9 MB (55925399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0db4e702162a700c3f00a3624f94bbfa81fd2077b8c5cf57f455659259295a`  
		Last Modified: Tue, 21 Dec 2021 02:25:41 GMT  
		Size: 5.3 MB (5282974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4fb971a29956de966e154c96a2d7f1eb56aed081b583947be033c05d7c69797`  
		Last Modified: Tue, 21 Dec 2021 02:25:42 GMT  
		Size: 11.3 MB (11250616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb3ec563e1e552271ac9c80a2b348ebf47401940583ca295fc5f1378ca9d3ac`  
		Last Modified: Tue, 21 Dec 2021 02:26:11 GMT  
		Size: 55.9 MB (55917390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2c2a9657022eac58df44f2cef58c0e28b506b12f67dece31bf9bd280de6d6f`  
		Last Modified: Tue, 21 Dec 2021 02:27:07 GMT  
		Size: 199.4 MB (199449263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae4e6ced7d216b439b6a4b3cfffd9957baaa2093e769d5da2f657972bb99a96`  
		Last Modified: Fri, 21 Jan 2022 01:45:38 GMT  
		Size: 188.0 MB (188021819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.58.1-alpine`

```console
$ docker pull rust@sha256:b61698ea823c6f9bc726272d7783867d89e79ca87e9944998739ce619da7699a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:1.58.1-alpine` - linux; amd64

```console
$ docker pull rust@sha256:d4c641c867f8d60f1f4da8edc19da4ea6543dd54f5cfd4c4cb713a438f9ed079
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.6 MB (269634647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:953451d7b194820db2946de86d08aa997c88d7e3f5f728f577d20cf4c4c210d9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Thu, 13 Jan 2022 20:26:04 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 21 Jan 2022 01:22:17 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:22:38 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93cd12ff80a853b96704224019bf0b85bbe94d9b9456b619b95ab0a8dbdf40d`  
		Last Modified: Thu, 13 Jan 2022 20:31:39 GMT  
		Size: 42.5 MB (42495579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9781e95f2a775fd7a289185a1bcbd1e616c15547d6ab73d8e78dfbb1c99514c`  
		Last Modified: Fri, 21 Jan 2022 01:28:49 GMT  
		Size: 224.3 MB (224320655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58.1-alpine` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:58a1a37e622250ca1f6f16bb1449e714632dcd7deddc0e2f38b8a05c92e54e55
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.0 MB (254960114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8a5a57c57976585d381f3fd0fe33476127b6dda4fa4e767a620e54314c92118`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Thu, 13 Jan 2022 20:42:58 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 21 Jan 2022 01:42:50 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:43:07 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec7b33c7ee4d79979b266a321f626981b48087e7524811342d73ce2e2eb9e57`  
		Last Modified: Thu, 13 Jan 2022 20:49:23 GMT  
		Size: 36.1 MB (36087204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fec8b7bac538e28495e4763ae0710d8b74d160b4b9b4cda13fbf6269d3283f`  
		Last Modified: Fri, 21 Jan 2022 01:49:44 GMT  
		Size: 216.2 MB (216157476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.58.1-alpine3.14`

```console
$ docker pull rust@sha256:2292543650f33917efbb8da25a303848cc72fad0cb95a0320277f99d3ce92046
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:1.58.1-alpine3.14` - linux; amd64

```console
$ docker pull rust@sha256:fbc0cfaa6261179ca7653cc2b20ca9c3e936f3416a911a27a28694f8fb23b8b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.5 MB (269494735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e35d9d35ab3792f9f41494f2fa73e8057080db430deb0bceddf896a605a6582`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 07:44:00 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 21 Jan 2022 01:21:49 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:22:11 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95f12a5672fd92cc370cc8ec78127e6c52a6d61404662fab9d5643b661f3e8b`  
		Last Modified: Sat, 13 Nov 2021 07:46:42 GMT  
		Size: 42.4 MB (42351276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be615768698a2e1df78b3e911bccea805cbacfcb7972586bb677332badfe97fb`  
		Last Modified: Fri, 21 Jan 2022 01:27:52 GMT  
		Size: 224.3 MB (224320478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58.1-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:7dd68b020a1550ed5cd7974188763c0831aea119f73fd1327b25972b6656962f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.8 MB (254813562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45aad15a39b3ffaf28e25228529764e9ad0408ff6182c9a9f30b8ab31fdb92fc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 17:55:55 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 21 Jan 2022 01:42:27 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:42:44 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3394b2150e94a1388a8ac369dcfa5974566be0e105ccecfe1f50dbeedd25887d`  
		Last Modified: Fri, 12 Nov 2021 17:58:34 GMT  
		Size: 35.9 MB (35938392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d19cdf6d774da55657d17c1d24e8390cce8b2f8cced8100d85ea1e51c82d13e`  
		Last Modified: Fri, 21 Jan 2022 01:48:56 GMT  
		Size: 216.2 MB (216157470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.58.1-alpine3.15`

```console
$ docker pull rust@sha256:b61698ea823c6f9bc726272d7783867d89e79ca87e9944998739ce619da7699a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:1.58.1-alpine3.15` - linux; amd64

```console
$ docker pull rust@sha256:d4c641c867f8d60f1f4da8edc19da4ea6543dd54f5cfd4c4cb713a438f9ed079
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.6 MB (269634647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:953451d7b194820db2946de86d08aa997c88d7e3f5f728f577d20cf4c4c210d9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Thu, 13 Jan 2022 20:26:04 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 21 Jan 2022 01:22:17 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:22:38 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93cd12ff80a853b96704224019bf0b85bbe94d9b9456b619b95ab0a8dbdf40d`  
		Last Modified: Thu, 13 Jan 2022 20:31:39 GMT  
		Size: 42.5 MB (42495579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9781e95f2a775fd7a289185a1bcbd1e616c15547d6ab73d8e78dfbb1c99514c`  
		Last Modified: Fri, 21 Jan 2022 01:28:49 GMT  
		Size: 224.3 MB (224320655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58.1-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:58a1a37e622250ca1f6f16bb1449e714632dcd7deddc0e2f38b8a05c92e54e55
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.0 MB (254960114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8a5a57c57976585d381f3fd0fe33476127b6dda4fa4e767a620e54314c92118`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Thu, 13 Jan 2022 20:42:58 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 21 Jan 2022 01:42:50 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:43:07 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec7b33c7ee4d79979b266a321f626981b48087e7524811342d73ce2e2eb9e57`  
		Last Modified: Thu, 13 Jan 2022 20:49:23 GMT  
		Size: 36.1 MB (36087204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fec8b7bac538e28495e4763ae0710d8b74d160b4b9b4cda13fbf6269d3283f`  
		Last Modified: Fri, 21 Jan 2022 01:49:44 GMT  
		Size: 216.2 MB (216157476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.58.1-bullseye`

```console
$ docker pull rust@sha256:8ad28b7355e19dad2677624622bad1cc978b6fd34b45e75d17c25f558f94a934
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.58.1-bullseye` - linux; amd64

```console
$ docker pull rust@sha256:d46142e07db17a179a9cd18bc814c5c7e1499fdd12147f9249ee48c540aec0d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.2 MB (466162023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:269d9943b0d310e1ab49a55e14752596567a74daa37270c6217abfc33f48f7f5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 02:26:40 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Thu, 27 Jan 2022 02:26:56 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808edda3c2e855dc13af758b35cefbcc417ad1ab4fead7f72234b09aeda893a0`  
		Last Modified: Wed, 26 Jan 2022 02:23:16 GMT  
		Size: 196.5 MB (196529197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4671d83ec37ad7f7bf397a8340e76ed6b965029035e63a4a2043351fcd40d892`  
		Last Modified: Thu, 27 Jan 2022 02:30:45 GMT  
		Size: 144.1 MB (144123702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58.1-bullseye` - linux; arm variant v7

```console
$ docker pull rust@sha256:32e5c60294d2cd912122e23d42e330e63a9a8754443b8654a3ea8df1e75ba397
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **483.2 MB (483165594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8faf3dd2fdb2285b82cf07285b1b0bf7d34d46d0478e7996e3f0369398d7528b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:59:11 GMT
ADD file:848bf729bc16d3b188567f096ee1c0386cb49825a06eef396401278afee2f4c7 in / 
# Tue, 21 Dec 2021 01:59:12 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:46:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:46:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:47:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:49:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 06:11:05 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 06:11:46 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:fd92fbcda272f5935dcd0dfea445cba0152208f83c8fc8d2cb74c85379145c42`  
		Last Modified: Tue, 21 Dec 2021 02:14:41 GMT  
		Size: 50.1 MB (50121433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a6987ee02fad9d702adbd7921b8e1776b1a091773dd47886055113b1d7ba62`  
		Last Modified: Tue, 21 Dec 2021 03:11:46 GMT  
		Size: 4.9 MB (4922490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6d85cbb278c8e4845f79838154b77c36931e65f9b5bb9b8f56c92f41f72e27`  
		Last Modified: Tue, 21 Dec 2021 03:11:47 GMT  
		Size: 10.2 MB (10217004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bd566d277d8d03e1b76768a074dd92306bc287eef88c42a08ef5b48b842fa1`  
		Last Modified: Tue, 21 Dec 2021 03:12:37 GMT  
		Size: 50.3 MB (50328047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edcf448232b2036e5813fc0174bcd35c3a967a79cf2ef79bc2bfb0410c7b176e`  
		Last Modified: Tue, 21 Dec 2021 03:14:27 GMT  
		Size: 167.0 MB (166954318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2393fcae1480a3e448c675f4654fccb4999808ae81fd8438665649bd7809cd`  
		Last Modified: Fri, 21 Jan 2022 06:22:33 GMT  
		Size: 200.6 MB (200622302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58.1-bullseye` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:71e628671e7232373f1babb49f78f1751c5151af8ac6dc2c5cfaacf60c08c627
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **529.3 MB (529331157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28baec511a7c725b2502fe4dbcda7a5e4740cb19806b922bfcbfbb35cd1d9c13`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:38:28 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 08:38:45 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cb4eca0cebfb68f0cb8dd7e6c0c67b880fcae929406705b4d43a2df4fa48eb`  
		Last Modified: Wed, 26 Jan 2022 02:24:49 GMT  
		Size: 189.4 MB (189420652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2d141dc211541426cd6794767a1439b2ead45ccdae9e55c89c1f6d1b46ce7b`  
		Last Modified: Wed, 26 Jan 2022 08:43:08 GMT  
		Size: 215.8 MB (215834728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58.1-bullseye` - linux; 386

```console
$ docker pull rust@sha256:00a04734a44749afb4e6a7c8c294d3e9a5c169bb091601036d41044241f8d9eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.8 MB (515847461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9787ce8e926d4bc03f1104f353c79e89b71d8453c15fa4f707118ef27a84595e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:39:40 GMT
ADD file:b77df0839dfb103f5f16329bfa0dcf40c1a73b02e312bb2be40ad620f64e7949 in / 
# Tue, 21 Dec 2021 01:39:44 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:13:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:13:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:13:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:14:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 01:40:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:40:45 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:c13b09ebb011541c3f3a6e423452bf5046e5ba48dfee18e88cc3e3df477c0baa`  
		Last Modified: Tue, 21 Dec 2021 01:48:09 GMT  
		Size: 55.9 MB (55925399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0db4e702162a700c3f00a3624f94bbfa81fd2077b8c5cf57f455659259295a`  
		Last Modified: Tue, 21 Dec 2021 02:25:41 GMT  
		Size: 5.3 MB (5282974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4fb971a29956de966e154c96a2d7f1eb56aed081b583947be033c05d7c69797`  
		Last Modified: Tue, 21 Dec 2021 02:25:42 GMT  
		Size: 11.3 MB (11250616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb3ec563e1e552271ac9c80a2b348ebf47401940583ca295fc5f1378ca9d3ac`  
		Last Modified: Tue, 21 Dec 2021 02:26:11 GMT  
		Size: 55.9 MB (55917390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2c2a9657022eac58df44f2cef58c0e28b506b12f67dece31bf9bd280de6d6f`  
		Last Modified: Tue, 21 Dec 2021 02:27:07 GMT  
		Size: 199.4 MB (199449263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae4e6ced7d216b439b6a4b3cfffd9957baaa2093e769d5da2f657972bb99a96`  
		Last Modified: Fri, 21 Jan 2022 01:45:38 GMT  
		Size: 188.0 MB (188021819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.58.1-buster`

```console
$ docker pull rust@sha256:e3a1c9b64e1c028851e24fba7d846dbe11edb2463fdb2e4bae2b731c0bc86463
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.58.1-buster` - linux; amd64

```console
$ docker pull rust@sha256:5dad83d6154d9b7d5a454e487292a818f1a49c310d22d28d027dace34ade540d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **456.7 MB (456656132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4737b5f9e43d2dc30e66ad37c2bf4a078f46b8b9e7e751b650e9e082e76e1a7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:47 GMT
ADD file:a290acee3581e1e9c42c0a37b53086a8f070cb0730179be81a6ba24a620b6ee4 in / 
# Wed, 26 Jan 2022 01:40:47 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 02:25:47 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Thu, 27 Jan 2022 02:26:02 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:a024302f8a017855dd20a107ace079dd543c4bdfa8e7c11472771babbe298d2b`  
		Last Modified: Wed, 26 Jan 2022 01:47:01 GMT  
		Size: 50.4 MB (50437057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289773030fdc98afe6cc53bdd0c05332ea8ff21ad836afa1d3042388953c43f8`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 7.8 MB (7833856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bb8b3399fe8dd0b83bd5e32a97e5183ab235d6fb4cc0b5dfabb20e6653e715`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 10.0 MB (9997205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c63da771697b362929cecc84777e8cfbb716ff3d575b999854d83ada039b695`  
		Last Modified: Wed, 26 Jan 2022 02:23:53 GMT  
		Size: 51.8 MB (51839910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf1b23b1e4b1867b70ba7f0614dff34bdb468c2a860a7b162c74c2b451494c0`  
		Last Modified: Wed, 26 Jan 2022 02:24:38 GMT  
		Size: 192.4 MB (192424405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbadc5241c680bb76f81237047194a1d408a37104d21cfc421439a941bc0d5a3`  
		Last Modified: Thu, 27 Jan 2022 02:29:05 GMT  
		Size: 144.1 MB (144123699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58.1-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:1ccaa939ec2bcd17833886a87ae632de27c7b25738510f45f9573a0a6802f50b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **479.0 MB (478973771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e5e34aeb2594b6b0ea9e8b59acf1d371889f6b13ace574de70235c1cb3cdab3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:17 GMT
ADD file:36bf5b8bdd9066b06cc35d26df3f4dad2b1cbcb41985b85f070ed97a3e85f8a9 in / 
# Tue, 21 Dec 2021 02:00:18 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:49:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:50:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:53:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 06:08:33 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 06:09:16 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:328389035fdd79ece4f520541a84b3de974050fe012ed1566da6b869dd34ea29`  
		Last Modified: Tue, 21 Dec 2021 02:16:11 GMT  
		Size: 45.9 MB (45918102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80397c5626b1d4e58b7b7dd9219674dd86caa03ddcaac1d3d6791189a44b0ff`  
		Last Modified: Tue, 21 Dec 2021 03:14:47 GMT  
		Size: 7.1 MB (7125168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816c475148f8e55cc2b8593f29d0ddd67ad1359f3c69061f043d461495bad179`  
		Last Modified: Tue, 21 Dec 2021 03:14:48 GMT  
		Size: 9.3 MB (9343808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d30bc5ea112783bdcbfaba962b58338c0f61b12d68a5cc7474c0b639098c6a`  
		Last Modified: Tue, 21 Dec 2021 03:15:32 GMT  
		Size: 47.4 MB (47356397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93be0f932a74231c59bf289b331a4b22b2346e3532b93f7c9a3d1eb60859f40b`  
		Last Modified: Tue, 21 Dec 2021 03:17:17 GMT  
		Size: 168.6 MB (168607961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e21137e326fc09ba91d9592481ee83a4c7e5b8458ffd21c0f488c9edb3d3bbd`  
		Last Modified: Fri, 21 Jan 2022 06:17:28 GMT  
		Size: 200.6 MB (200622335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58.1-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:611b00bf3064be66516b9bd9af0a31bbdf0d7535edb4ea5fa6ee5e41bf6c157b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **518.7 MB (518694576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bc36b7a17a62b420f4f1b26c9a9ffee6132533be64f06904a8e51a73622d362`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:41 GMT
ADD file:98a75269e438ff15cee16ad2763fe2698fb436bc4770c0ca27c059f66b65e56a in / 
# Wed, 26 Jan 2022 01:42:42 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:14:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:14:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:15:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:37:25 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 08:37:44 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:ccd458f933f7966e412773ee1551aaf2433a5bf9adaae519e2ac7c9c3f8b5f89`  
		Last Modified: Wed, 26 Jan 2022 01:49:28 GMT  
		Size: 49.2 MB (49223041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3524e6d2c855bef1f32da73e00738b2e5e91e6a346d19f8b33e8e8117c82748`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 7.7 MB (7695112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cc9cf00cd9023559aeda43668c7d9d621318631bab103ae03b8a3787260048`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 9.8 MB (9767300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f0325e59cadc58f4e81c6a282319b0c01f54964ef989205974a6557cf15040`  
		Last Modified: Wed, 26 Jan 2022 02:25:25 GMT  
		Size: 52.2 MB (52168727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b289063aa004828178bcfddecfcf2fda082ce1cb1657eb68a9ef23e027a510b`  
		Last Modified: Wed, 26 Jan 2022 02:26:00 GMT  
		Size: 184.0 MB (184005857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af714e5ef49569fce78ac8d86129c0d70407051af674aadee820dbf5f6d118a`  
		Last Modified: Wed, 26 Jan 2022 08:41:20 GMT  
		Size: 215.8 MB (215834539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58.1-buster` - linux; 386

```console
$ docker pull rust@sha256:4fde2447b7b5bd85bc6e955b14004027e985963d6db7377793371fcb4d904374
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **510.0 MB (509970484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24aac74c874dfb49adbce2fad1afd33ce899db1b13c2342e96e959c68eb4b7a4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:24 GMT
ADD file:4e982be228380a8d7632e31f19e39ed55ee76fb1db32130fa88d696904d6acde in / 
# Tue, 21 Dec 2021 01:40:25 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:15:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:15:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:15:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:17:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 01:38:53 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:39:15 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:342b01a61e0af68dc09681004efdfcf66d0443632988d6f247dd7b34bc18b1db`  
		Last Modified: Tue, 21 Dec 2021 01:49:14 GMT  
		Size: 51.2 MB (51207766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4759b0dba897041c21e226a9db50a85ca5685f19bb5036f16df5b231fd177919`  
		Last Modified: Tue, 21 Dec 2021 02:27:24 GMT  
		Size: 8.0 MB (8000238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a258e8ae475665e88b0ebd438d4a945fa152a99c6d2ff863c06087a6dd4c7d`  
		Last Modified: Tue, 21 Dec 2021 02:27:24 GMT  
		Size: 10.3 MB (10340145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7754201e052c276668b8474d86f55c0df401d90074d1090dc57d978ce0be1a2d`  
		Last Modified: Tue, 21 Dec 2021 02:27:48 GMT  
		Size: 53.4 MB (53438278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc31fef36efd395cde421ab27002334aa7c40a276b0a299acd89ff60b7f13ff`  
		Last Modified: Tue, 21 Dec 2021 02:28:41 GMT  
		Size: 199.0 MB (198962209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b9165c2bb91b10d141c07f8acf538767f6a2e6e3cc9c6fa70487f5f76c7ecc`  
		Last Modified: Fri, 21 Jan 2022 01:43:30 GMT  
		Size: 188.0 MB (188021848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.58.1-slim`

```console
$ docker pull rust@sha256:aef724360894cd51ff66420b688dacc811cd1591094ab9561e1a541da366d02b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.58.1-slim` - linux; amd64

```console
$ docker pull rust@sha256:c65c489f71effc81ac327df299f4f4b18f02f52a495c928949d9faef37be5c0e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.6 MB (235616218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3d2ecb28032ee0b780251c0e12ba34e4ea2b00bb6c1f54aef24cb70e40d5389`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 02:27:01 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Thu, 27 Jan 2022 02:27:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7c57d6ee4402b697e1f62306aeebe04fca5a4fcfcdd2a1c53900a71bd1ec9d`  
		Last Modified: Thu, 27 Jan 2022 02:31:42 GMT  
		Size: 204.2 MB (204249961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58.1-slim` - linux; arm variant v7

```console
$ docker pull rust@sha256:5e320dc7dac05018ef56f8e75e29af46cf2b854a2bcd2c5274ec1d0838cfcfbc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.5 MB (269473502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90e30db66a12fb0b6695e5f16320fc49d165f635623f83b53332460ae2d6fd20`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 10:50:56 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 10:52:09 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6a8aa1e46b451ab566c5071e58dce324c2116d376905dec3cffab784b91947`  
		Last Modified: Wed, 26 Jan 2022 10:59:37 GMT  
		Size: 242.9 MB (242908569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58.1-slim` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:1a9113137065ce5dad9ac0092210e8df36bc896c8d44d156d3cf95a34cf4bd1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.6 MB (301595417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3c255aa040881fa57bc6f56400f12b12ab822a4448a2daa2ad75a6a412195c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:38:53 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 08:39:21 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e175c7caf143e560d9a469fb403bce557467bd7bfd7053747deacafb33fd93f1`  
		Last Modified: Wed, 26 Jan 2022 08:44:18 GMT  
		Size: 271.5 MB (271538643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58.1-slim` - linux; 386

```console
$ docker pull rust@sha256:52f7d0a7ee12b806c72fc52a9123ef1df65d00645df4c9d91eb3ae8e5d3f56a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281164943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b10b451f292da4629eb4863abeb9d24f63cbce0d73a15e5c1eb595aef34a9b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Fri, 21 Jan 2022 01:40:55 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:41:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867d4c40cb0c2add04a2801c038bb1d2cc2eb532b2a7500c8c657c89ad2dc859`  
		Last Modified: Fri, 21 Jan 2022 01:47:04 GMT  
		Size: 248.8 MB (248794093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.58.1-slim-bullseye`

```console
$ docker pull rust@sha256:aef724360894cd51ff66420b688dacc811cd1591094ab9561e1a541da366d02b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.58.1-slim-bullseye` - linux; amd64

```console
$ docker pull rust@sha256:c65c489f71effc81ac327df299f4f4b18f02f52a495c928949d9faef37be5c0e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.6 MB (235616218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3d2ecb28032ee0b780251c0e12ba34e4ea2b00bb6c1f54aef24cb70e40d5389`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 02:27:01 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Thu, 27 Jan 2022 02:27:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7c57d6ee4402b697e1f62306aeebe04fca5a4fcfcdd2a1c53900a71bd1ec9d`  
		Last Modified: Thu, 27 Jan 2022 02:31:42 GMT  
		Size: 204.2 MB (204249961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58.1-slim-bullseye` - linux; arm variant v7

```console
$ docker pull rust@sha256:5e320dc7dac05018ef56f8e75e29af46cf2b854a2bcd2c5274ec1d0838cfcfbc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.5 MB (269473502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90e30db66a12fb0b6695e5f16320fc49d165f635623f83b53332460ae2d6fd20`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 10:50:56 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 10:52:09 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6a8aa1e46b451ab566c5071e58dce324c2116d376905dec3cffab784b91947`  
		Last Modified: Wed, 26 Jan 2022 10:59:37 GMT  
		Size: 242.9 MB (242908569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58.1-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:1a9113137065ce5dad9ac0092210e8df36bc896c8d44d156d3cf95a34cf4bd1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.6 MB (301595417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3c255aa040881fa57bc6f56400f12b12ab822a4448a2daa2ad75a6a412195c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:38:53 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 08:39:21 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e175c7caf143e560d9a469fb403bce557467bd7bfd7053747deacafb33fd93f1`  
		Last Modified: Wed, 26 Jan 2022 08:44:18 GMT  
		Size: 271.5 MB (271538643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58.1-slim-bullseye` - linux; 386

```console
$ docker pull rust@sha256:52f7d0a7ee12b806c72fc52a9123ef1df65d00645df4c9d91eb3ae8e5d3f56a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281164943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b10b451f292da4629eb4863abeb9d24f63cbce0d73a15e5c1eb595aef34a9b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Fri, 21 Jan 2022 01:40:55 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:41:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867d4c40cb0c2add04a2801c038bb1d2cc2eb532b2a7500c8c657c89ad2dc859`  
		Last Modified: Fri, 21 Jan 2022 01:47:04 GMT  
		Size: 248.8 MB (248794093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.58.1-slim-buster`

```console
$ docker pull rust@sha256:f97b60397f841696adf7d5094e96d9f32db8b338dd0fa1a6ba3b15f6a8cbbac7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.58.1-slim-buster` - linux; amd64

```console
$ docker pull rust@sha256:d70392f42ab0402a067f47cb645ad4c5cb2fccd8de913707b5e9ffe51dccdcc7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.7 MB (216691424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d210d9c6ad548acf5f3bacefc02a1a1b844bd0c695b5d03c01d5f972efa43d23`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 02:26:06 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Thu, 27 Jan 2022 02:26:34 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfd01e1add41d50399c9c7261d9675981c573a096b2db958c6bdb4d0ba3df6e`  
		Last Modified: Thu, 27 Jan 2022 02:29:58 GMT  
		Size: 189.5 MB (189537693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58.1-slim-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:61d6f5bed2e9fd94e378eab4c9fc5a451caef607f6ac14ffc3fe0f5f7c6109e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.3 MB (256276557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b30e8b184d6c2e016890c87dc71ab25296222a2e934531f2e31c6a7d61046271`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:12 GMT
ADD file:ca8132e20773f7037458cc53fe20a7116f93c21c7479be5a2a1d739495dbe44e in / 
# Wed, 26 Jan 2022 01:43:13 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 10:49:05 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 10:50:20 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:20cc49690d9072283406c1c11e9b1dc1a247782cc8daa526b375d4a7f1cb6a94`  
		Last Modified: Wed, 26 Jan 2022 01:59:27 GMT  
		Size: 22.8 MB (22754397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539f3b7106a14210296dc07ec5c5275b3b7124abffcf23c25d6f79ae330d28b1`  
		Last Modified: Wed, 26 Jan 2022 10:56:40 GMT  
		Size: 233.5 MB (233522160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58.1-slim-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:fd60d456c8c1818a9f71d0063e20a1d869aa48429afae7f81f24a9b51883a4d1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.0 MB (281957084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35221a2f076a920466686f0e6c540ef9879dfe37e9adaa83ea380eb09bcb5e74`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:37:51 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 08:38:18 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2765579f339812249621170a70c8cf8430422b746c7163efc3ffe0d2a5b00c6e`  
		Last Modified: Wed, 26 Jan 2022 08:42:15 GMT  
		Size: 256.0 MB (256033868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.58.1-slim-buster` - linux; 386

```console
$ docker pull rust@sha256:17efe31938303253b8d9e3afa66de629c033db64a3d9831623d9eb1443865fc7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.8 MB (265819912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07de88a206564ac8ad3534d14868b8b1af2b6375eaf06529bca7af5dc6f685d0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:45 GMT
ADD file:78342a77df22ca22804ea5aec6415ce10c1fdc35687f1b25c5f86850f41d3905 in / 
# Tue, 21 Dec 2021 01:40:45 GMT
CMD ["bash"]
# Fri, 21 Jan 2022 01:39:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:40:14 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:16e3a221bce3a5f7f4a71f72926f381ff9c6141ccb5918b7ea924ff7f7f09d06`  
		Last Modified: Tue, 21 Dec 2021 01:49:46 GMT  
		Size: 27.8 MB (27804573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d81babe2c3794639ff06bb2e5ad026aca8afabb13a8d2e7006bf1795a7e7f4`  
		Last Modified: Fri, 21 Jan 2022 01:44:39 GMT  
		Size: 238.0 MB (238015339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:alpine`

```console
$ docker pull rust@sha256:b61698ea823c6f9bc726272d7783867d89e79ca87e9944998739ce619da7699a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:alpine` - linux; amd64

```console
$ docker pull rust@sha256:d4c641c867f8d60f1f4da8edc19da4ea6543dd54f5cfd4c4cb713a438f9ed079
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.6 MB (269634647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:953451d7b194820db2946de86d08aa997c88d7e3f5f728f577d20cf4c4c210d9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Thu, 13 Jan 2022 20:26:04 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 21 Jan 2022 01:22:17 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:22:38 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93cd12ff80a853b96704224019bf0b85bbe94d9b9456b619b95ab0a8dbdf40d`  
		Last Modified: Thu, 13 Jan 2022 20:31:39 GMT  
		Size: 42.5 MB (42495579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9781e95f2a775fd7a289185a1bcbd1e616c15547d6ab73d8e78dfbb1c99514c`  
		Last Modified: Fri, 21 Jan 2022 01:28:49 GMT  
		Size: 224.3 MB (224320655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:alpine` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:58a1a37e622250ca1f6f16bb1449e714632dcd7deddc0e2f38b8a05c92e54e55
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.0 MB (254960114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8a5a57c57976585d381f3fd0fe33476127b6dda4fa4e767a620e54314c92118`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Thu, 13 Jan 2022 20:42:58 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 21 Jan 2022 01:42:50 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:43:07 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec7b33c7ee4d79979b266a321f626981b48087e7524811342d73ce2e2eb9e57`  
		Last Modified: Thu, 13 Jan 2022 20:49:23 GMT  
		Size: 36.1 MB (36087204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fec8b7bac538e28495e4763ae0710d8b74d160b4b9b4cda13fbf6269d3283f`  
		Last Modified: Fri, 21 Jan 2022 01:49:44 GMT  
		Size: 216.2 MB (216157476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:alpine3.14`

```console
$ docker pull rust@sha256:2292543650f33917efbb8da25a303848cc72fad0cb95a0320277f99d3ce92046
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:alpine3.14` - linux; amd64

```console
$ docker pull rust@sha256:fbc0cfaa6261179ca7653cc2b20ca9c3e936f3416a911a27a28694f8fb23b8b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.5 MB (269494735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e35d9d35ab3792f9f41494f2fa73e8057080db430deb0bceddf896a605a6582`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 07:44:00 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 21 Jan 2022 01:21:49 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:22:11 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95f12a5672fd92cc370cc8ec78127e6c52a6d61404662fab9d5643b661f3e8b`  
		Last Modified: Sat, 13 Nov 2021 07:46:42 GMT  
		Size: 42.4 MB (42351276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be615768698a2e1df78b3e911bccea805cbacfcb7972586bb677332badfe97fb`  
		Last Modified: Fri, 21 Jan 2022 01:27:52 GMT  
		Size: 224.3 MB (224320478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:alpine3.14` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:7dd68b020a1550ed5cd7974188763c0831aea119f73fd1327b25972b6656962f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.8 MB (254813562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45aad15a39b3ffaf28e25228529764e9ad0408ff6182c9a9f30b8ab31fdb92fc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 17:55:55 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 21 Jan 2022 01:42:27 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:42:44 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3394b2150e94a1388a8ac369dcfa5974566be0e105ccecfe1f50dbeedd25887d`  
		Last Modified: Fri, 12 Nov 2021 17:58:34 GMT  
		Size: 35.9 MB (35938392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d19cdf6d774da55657d17c1d24e8390cce8b2f8cced8100d85ea1e51c82d13e`  
		Last Modified: Fri, 21 Jan 2022 01:48:56 GMT  
		Size: 216.2 MB (216157470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:alpine3.15`

```console
$ docker pull rust@sha256:b61698ea823c6f9bc726272d7783867d89e79ca87e9944998739ce619da7699a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:alpine3.15` - linux; amd64

```console
$ docker pull rust@sha256:d4c641c867f8d60f1f4da8edc19da4ea6543dd54f5cfd4c4cb713a438f9ed079
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.6 MB (269634647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:953451d7b194820db2946de86d08aa997c88d7e3f5f728f577d20cf4c4c210d9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Thu, 13 Jan 2022 20:26:04 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 21 Jan 2022 01:22:17 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:22:38 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93cd12ff80a853b96704224019bf0b85bbe94d9b9456b619b95ab0a8dbdf40d`  
		Last Modified: Thu, 13 Jan 2022 20:31:39 GMT  
		Size: 42.5 MB (42495579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9781e95f2a775fd7a289185a1bcbd1e616c15547d6ab73d8e78dfbb1c99514c`  
		Last Modified: Fri, 21 Jan 2022 01:28:49 GMT  
		Size: 224.3 MB (224320655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:alpine3.15` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:58a1a37e622250ca1f6f16bb1449e714632dcd7deddc0e2f38b8a05c92e54e55
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.0 MB (254960114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8a5a57c57976585d381f3fd0fe33476127b6dda4fa4e767a620e54314c92118`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Thu, 13 Jan 2022 20:42:58 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Fri, 21 Jan 2022 01:42:50 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:43:07 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec7b33c7ee4d79979b266a321f626981b48087e7524811342d73ce2e2eb9e57`  
		Last Modified: Thu, 13 Jan 2022 20:49:23 GMT  
		Size: 36.1 MB (36087204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fec8b7bac538e28495e4763ae0710d8b74d160b4b9b4cda13fbf6269d3283f`  
		Last Modified: Fri, 21 Jan 2022 01:49:44 GMT  
		Size: 216.2 MB (216157476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:bullseye`

```console
$ docker pull rust@sha256:8ad28b7355e19dad2677624622bad1cc978b6fd34b45e75d17c25f558f94a934
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:bullseye` - linux; amd64

```console
$ docker pull rust@sha256:d46142e07db17a179a9cd18bc814c5c7e1499fdd12147f9249ee48c540aec0d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.2 MB (466162023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:269d9943b0d310e1ab49a55e14752596567a74daa37270c6217abfc33f48f7f5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 02:26:40 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Thu, 27 Jan 2022 02:26:56 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808edda3c2e855dc13af758b35cefbcc417ad1ab4fead7f72234b09aeda893a0`  
		Last Modified: Wed, 26 Jan 2022 02:23:16 GMT  
		Size: 196.5 MB (196529197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4671d83ec37ad7f7bf397a8340e76ed6b965029035e63a4a2043351fcd40d892`  
		Last Modified: Thu, 27 Jan 2022 02:30:45 GMT  
		Size: 144.1 MB (144123702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:bullseye` - linux; arm variant v7

```console
$ docker pull rust@sha256:32e5c60294d2cd912122e23d42e330e63a9a8754443b8654a3ea8df1e75ba397
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **483.2 MB (483165594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8faf3dd2fdb2285b82cf07285b1b0bf7d34d46d0478e7996e3f0369398d7528b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:59:11 GMT
ADD file:848bf729bc16d3b188567f096ee1c0386cb49825a06eef396401278afee2f4c7 in / 
# Tue, 21 Dec 2021 01:59:12 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:46:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:46:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:47:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:49:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 06:11:05 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 06:11:46 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:fd92fbcda272f5935dcd0dfea445cba0152208f83c8fc8d2cb74c85379145c42`  
		Last Modified: Tue, 21 Dec 2021 02:14:41 GMT  
		Size: 50.1 MB (50121433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a6987ee02fad9d702adbd7921b8e1776b1a091773dd47886055113b1d7ba62`  
		Last Modified: Tue, 21 Dec 2021 03:11:46 GMT  
		Size: 4.9 MB (4922490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6d85cbb278c8e4845f79838154b77c36931e65f9b5bb9b8f56c92f41f72e27`  
		Last Modified: Tue, 21 Dec 2021 03:11:47 GMT  
		Size: 10.2 MB (10217004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bd566d277d8d03e1b76768a074dd92306bc287eef88c42a08ef5b48b842fa1`  
		Last Modified: Tue, 21 Dec 2021 03:12:37 GMT  
		Size: 50.3 MB (50328047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edcf448232b2036e5813fc0174bcd35c3a967a79cf2ef79bc2bfb0410c7b176e`  
		Last Modified: Tue, 21 Dec 2021 03:14:27 GMT  
		Size: 167.0 MB (166954318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2393fcae1480a3e448c675f4654fccb4999808ae81fd8438665649bd7809cd`  
		Last Modified: Fri, 21 Jan 2022 06:22:33 GMT  
		Size: 200.6 MB (200622302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:bullseye` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:71e628671e7232373f1babb49f78f1751c5151af8ac6dc2c5cfaacf60c08c627
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **529.3 MB (529331157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28baec511a7c725b2502fe4dbcda7a5e4740cb19806b922bfcbfbb35cd1d9c13`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:38:28 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 08:38:45 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cb4eca0cebfb68f0cb8dd7e6c0c67b880fcae929406705b4d43a2df4fa48eb`  
		Last Modified: Wed, 26 Jan 2022 02:24:49 GMT  
		Size: 189.4 MB (189420652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2d141dc211541426cd6794767a1439b2ead45ccdae9e55c89c1f6d1b46ce7b`  
		Last Modified: Wed, 26 Jan 2022 08:43:08 GMT  
		Size: 215.8 MB (215834728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:bullseye` - linux; 386

```console
$ docker pull rust@sha256:00a04734a44749afb4e6a7c8c294d3e9a5c169bb091601036d41044241f8d9eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.8 MB (515847461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9787ce8e926d4bc03f1104f353c79e89b71d8453c15fa4f707118ef27a84595e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:39:40 GMT
ADD file:b77df0839dfb103f5f16329bfa0dcf40c1a73b02e312bb2be40ad620f64e7949 in / 
# Tue, 21 Dec 2021 01:39:44 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:13:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:13:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:13:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:14:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 01:40:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:40:45 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:c13b09ebb011541c3f3a6e423452bf5046e5ba48dfee18e88cc3e3df477c0baa`  
		Last Modified: Tue, 21 Dec 2021 01:48:09 GMT  
		Size: 55.9 MB (55925399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0db4e702162a700c3f00a3624f94bbfa81fd2077b8c5cf57f455659259295a`  
		Last Modified: Tue, 21 Dec 2021 02:25:41 GMT  
		Size: 5.3 MB (5282974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4fb971a29956de966e154c96a2d7f1eb56aed081b583947be033c05d7c69797`  
		Last Modified: Tue, 21 Dec 2021 02:25:42 GMT  
		Size: 11.3 MB (11250616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb3ec563e1e552271ac9c80a2b348ebf47401940583ca295fc5f1378ca9d3ac`  
		Last Modified: Tue, 21 Dec 2021 02:26:11 GMT  
		Size: 55.9 MB (55917390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2c2a9657022eac58df44f2cef58c0e28b506b12f67dece31bf9bd280de6d6f`  
		Last Modified: Tue, 21 Dec 2021 02:27:07 GMT  
		Size: 199.4 MB (199449263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae4e6ced7d216b439b6a4b3cfffd9957baaa2093e769d5da2f657972bb99a96`  
		Last Modified: Fri, 21 Jan 2022 01:45:38 GMT  
		Size: 188.0 MB (188021819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:buster`

```console
$ docker pull rust@sha256:e3a1c9b64e1c028851e24fba7d846dbe11edb2463fdb2e4bae2b731c0bc86463
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:buster` - linux; amd64

```console
$ docker pull rust@sha256:5dad83d6154d9b7d5a454e487292a818f1a49c310d22d28d027dace34ade540d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **456.7 MB (456656132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4737b5f9e43d2dc30e66ad37c2bf4a078f46b8b9e7e751b650e9e082e76e1a7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:47 GMT
ADD file:a290acee3581e1e9c42c0a37b53086a8f070cb0730179be81a6ba24a620b6ee4 in / 
# Wed, 26 Jan 2022 01:40:47 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 02:25:47 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Thu, 27 Jan 2022 02:26:02 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:a024302f8a017855dd20a107ace079dd543c4bdfa8e7c11472771babbe298d2b`  
		Last Modified: Wed, 26 Jan 2022 01:47:01 GMT  
		Size: 50.4 MB (50437057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289773030fdc98afe6cc53bdd0c05332ea8ff21ad836afa1d3042388953c43f8`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 7.8 MB (7833856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bb8b3399fe8dd0b83bd5e32a97e5183ab235d6fb4cc0b5dfabb20e6653e715`  
		Last Modified: Wed, 26 Jan 2022 02:23:32 GMT  
		Size: 10.0 MB (9997205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c63da771697b362929cecc84777e8cfbb716ff3d575b999854d83ada039b695`  
		Last Modified: Wed, 26 Jan 2022 02:23:53 GMT  
		Size: 51.8 MB (51839910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf1b23b1e4b1867b70ba7f0614dff34bdb468c2a860a7b162c74c2b451494c0`  
		Last Modified: Wed, 26 Jan 2022 02:24:38 GMT  
		Size: 192.4 MB (192424405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbadc5241c680bb76f81237047194a1d408a37104d21cfc421439a941bc0d5a3`  
		Last Modified: Thu, 27 Jan 2022 02:29:05 GMT  
		Size: 144.1 MB (144123699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:1ccaa939ec2bcd17833886a87ae632de27c7b25738510f45f9573a0a6802f50b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **479.0 MB (478973771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e5e34aeb2594b6b0ea9e8b59acf1d371889f6b13ace574de70235c1cb3cdab3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:17 GMT
ADD file:36bf5b8bdd9066b06cc35d26df3f4dad2b1cbcb41985b85f070ed97a3e85f8a9 in / 
# Tue, 21 Dec 2021 02:00:18 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:49:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:50:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:53:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 06:08:33 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 06:09:16 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:328389035fdd79ece4f520541a84b3de974050fe012ed1566da6b869dd34ea29`  
		Last Modified: Tue, 21 Dec 2021 02:16:11 GMT  
		Size: 45.9 MB (45918102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80397c5626b1d4e58b7b7dd9219674dd86caa03ddcaac1d3d6791189a44b0ff`  
		Last Modified: Tue, 21 Dec 2021 03:14:47 GMT  
		Size: 7.1 MB (7125168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816c475148f8e55cc2b8593f29d0ddd67ad1359f3c69061f043d461495bad179`  
		Last Modified: Tue, 21 Dec 2021 03:14:48 GMT  
		Size: 9.3 MB (9343808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d30bc5ea112783bdcbfaba962b58338c0f61b12d68a5cc7474c0b639098c6a`  
		Last Modified: Tue, 21 Dec 2021 03:15:32 GMT  
		Size: 47.4 MB (47356397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93be0f932a74231c59bf289b331a4b22b2346e3532b93f7c9a3d1eb60859f40b`  
		Last Modified: Tue, 21 Dec 2021 03:17:17 GMT  
		Size: 168.6 MB (168607961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e21137e326fc09ba91d9592481ee83a4c7e5b8458ffd21c0f488c9edb3d3bbd`  
		Last Modified: Fri, 21 Jan 2022 06:17:28 GMT  
		Size: 200.6 MB (200622335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:611b00bf3064be66516b9bd9af0a31bbdf0d7535edb4ea5fa6ee5e41bf6c157b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **518.7 MB (518694576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bc36b7a17a62b420f4f1b26c9a9ffee6132533be64f06904a8e51a73622d362`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:41 GMT
ADD file:98a75269e438ff15cee16ad2763fe2698fb436bc4770c0ca27c059f66b65e56a in / 
# Wed, 26 Jan 2022 01:42:42 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:14:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:14:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:15:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:37:25 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 08:37:44 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:ccd458f933f7966e412773ee1551aaf2433a5bf9adaae519e2ac7c9c3f8b5f89`  
		Last Modified: Wed, 26 Jan 2022 01:49:28 GMT  
		Size: 49.2 MB (49223041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3524e6d2c855bef1f32da73e00738b2e5e91e6a346d19f8b33e8e8117c82748`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 7.7 MB (7695112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cc9cf00cd9023559aeda43668c7d9d621318631bab103ae03b8a3787260048`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 9.8 MB (9767300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f0325e59cadc58f4e81c6a282319b0c01f54964ef989205974a6557cf15040`  
		Last Modified: Wed, 26 Jan 2022 02:25:25 GMT  
		Size: 52.2 MB (52168727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b289063aa004828178bcfddecfcf2fda082ce1cb1657eb68a9ef23e027a510b`  
		Last Modified: Wed, 26 Jan 2022 02:26:00 GMT  
		Size: 184.0 MB (184005857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af714e5ef49569fce78ac8d86129c0d70407051af674aadee820dbf5f6d118a`  
		Last Modified: Wed, 26 Jan 2022 08:41:20 GMT  
		Size: 215.8 MB (215834539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:buster` - linux; 386

```console
$ docker pull rust@sha256:4fde2447b7b5bd85bc6e955b14004027e985963d6db7377793371fcb4d904374
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **510.0 MB (509970484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24aac74c874dfb49adbce2fad1afd33ce899db1b13c2342e96e959c68eb4b7a4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:24 GMT
ADD file:4e982be228380a8d7632e31f19e39ed55ee76fb1db32130fa88d696904d6acde in / 
# Tue, 21 Dec 2021 01:40:25 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:15:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:15:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:15:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:17:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 01:38:53 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:39:15 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:342b01a61e0af68dc09681004efdfcf66d0443632988d6f247dd7b34bc18b1db`  
		Last Modified: Tue, 21 Dec 2021 01:49:14 GMT  
		Size: 51.2 MB (51207766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4759b0dba897041c21e226a9db50a85ca5685f19bb5036f16df5b231fd177919`  
		Last Modified: Tue, 21 Dec 2021 02:27:24 GMT  
		Size: 8.0 MB (8000238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a258e8ae475665e88b0ebd438d4a945fa152a99c6d2ff863c06087a6dd4c7d`  
		Last Modified: Tue, 21 Dec 2021 02:27:24 GMT  
		Size: 10.3 MB (10340145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7754201e052c276668b8474d86f55c0df401d90074d1090dc57d978ce0be1a2d`  
		Last Modified: Tue, 21 Dec 2021 02:27:48 GMT  
		Size: 53.4 MB (53438278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc31fef36efd395cde421ab27002334aa7c40a276b0a299acd89ff60b7f13ff`  
		Last Modified: Tue, 21 Dec 2021 02:28:41 GMT  
		Size: 199.0 MB (198962209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b9165c2bb91b10d141c07f8acf538767f6a2e6e3cc9c6fa70487f5f76c7ecc`  
		Last Modified: Fri, 21 Jan 2022 01:43:30 GMT  
		Size: 188.0 MB (188021848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:latest`

```console
$ docker pull rust@sha256:8ad28b7355e19dad2677624622bad1cc978b6fd34b45e75d17c25f558f94a934
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:latest` - linux; amd64

```console
$ docker pull rust@sha256:d46142e07db17a179a9cd18bc814c5c7e1499fdd12147f9249ee48c540aec0d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.2 MB (466162023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:269d9943b0d310e1ab49a55e14752596567a74daa37270c6217abfc33f48f7f5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 02:26:40 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Thu, 27 Jan 2022 02:26:56 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808edda3c2e855dc13af758b35cefbcc417ad1ab4fead7f72234b09aeda893a0`  
		Last Modified: Wed, 26 Jan 2022 02:23:16 GMT  
		Size: 196.5 MB (196529197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4671d83ec37ad7f7bf397a8340e76ed6b965029035e63a4a2043351fcd40d892`  
		Last Modified: Thu, 27 Jan 2022 02:30:45 GMT  
		Size: 144.1 MB (144123702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:latest` - linux; arm variant v7

```console
$ docker pull rust@sha256:32e5c60294d2cd912122e23d42e330e63a9a8754443b8654a3ea8df1e75ba397
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **483.2 MB (483165594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8faf3dd2fdb2285b82cf07285b1b0bf7d34d46d0478e7996e3f0369398d7528b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:59:11 GMT
ADD file:848bf729bc16d3b188567f096ee1c0386cb49825a06eef396401278afee2f4c7 in / 
# Tue, 21 Dec 2021 01:59:12 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:46:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:46:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:47:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:49:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 06:11:05 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 06:11:46 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:fd92fbcda272f5935dcd0dfea445cba0152208f83c8fc8d2cb74c85379145c42`  
		Last Modified: Tue, 21 Dec 2021 02:14:41 GMT  
		Size: 50.1 MB (50121433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a6987ee02fad9d702adbd7921b8e1776b1a091773dd47886055113b1d7ba62`  
		Last Modified: Tue, 21 Dec 2021 03:11:46 GMT  
		Size: 4.9 MB (4922490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6d85cbb278c8e4845f79838154b77c36931e65f9b5bb9b8f56c92f41f72e27`  
		Last Modified: Tue, 21 Dec 2021 03:11:47 GMT  
		Size: 10.2 MB (10217004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bd566d277d8d03e1b76768a074dd92306bc287eef88c42a08ef5b48b842fa1`  
		Last Modified: Tue, 21 Dec 2021 03:12:37 GMT  
		Size: 50.3 MB (50328047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edcf448232b2036e5813fc0174bcd35c3a967a79cf2ef79bc2bfb0410c7b176e`  
		Last Modified: Tue, 21 Dec 2021 03:14:27 GMT  
		Size: 167.0 MB (166954318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2393fcae1480a3e448c675f4654fccb4999808ae81fd8438665649bd7809cd`  
		Last Modified: Fri, 21 Jan 2022 06:22:33 GMT  
		Size: 200.6 MB (200622302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:latest` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:71e628671e7232373f1babb49f78f1751c5151af8ac6dc2c5cfaacf60c08c627
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **529.3 MB (529331157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28baec511a7c725b2502fe4dbcda7a5e4740cb19806b922bfcbfbb35cd1d9c13`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 08:38:28 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 08:38:45 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cb4eca0cebfb68f0cb8dd7e6c0c67b880fcae929406705b4d43a2df4fa48eb`  
		Last Modified: Wed, 26 Jan 2022 02:24:49 GMT  
		Size: 189.4 MB (189420652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2d141dc211541426cd6794767a1439b2ead45ccdae9e55c89c1f6d1b46ce7b`  
		Last Modified: Wed, 26 Jan 2022 08:43:08 GMT  
		Size: 215.8 MB (215834728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:latest` - linux; 386

```console
$ docker pull rust@sha256:00a04734a44749afb4e6a7c8c294d3e9a5c169bb091601036d41044241f8d9eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.8 MB (515847461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9787ce8e926d4bc03f1104f353c79e89b71d8453c15fa4f707118ef27a84595e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:39:40 GMT
ADD file:b77df0839dfb103f5f16329bfa0dcf40c1a73b02e312bb2be40ad620f64e7949 in / 
# Tue, 21 Dec 2021 01:39:44 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:13:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:13:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:13:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:14:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 01:40:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:40:45 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:c13b09ebb011541c3f3a6e423452bf5046e5ba48dfee18e88cc3e3df477c0baa`  
		Last Modified: Tue, 21 Dec 2021 01:48:09 GMT  
		Size: 55.9 MB (55925399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0db4e702162a700c3f00a3624f94bbfa81fd2077b8c5cf57f455659259295a`  
		Last Modified: Tue, 21 Dec 2021 02:25:41 GMT  
		Size: 5.3 MB (5282974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4fb971a29956de966e154c96a2d7f1eb56aed081b583947be033c05d7c69797`  
		Last Modified: Tue, 21 Dec 2021 02:25:42 GMT  
		Size: 11.3 MB (11250616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb3ec563e1e552271ac9c80a2b348ebf47401940583ca295fc5f1378ca9d3ac`  
		Last Modified: Tue, 21 Dec 2021 02:26:11 GMT  
		Size: 55.9 MB (55917390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2c2a9657022eac58df44f2cef58c0e28b506b12f67dece31bf9bd280de6d6f`  
		Last Modified: Tue, 21 Dec 2021 02:27:07 GMT  
		Size: 199.4 MB (199449263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae4e6ced7d216b439b6a4b3cfffd9957baaa2093e769d5da2f657972bb99a96`  
		Last Modified: Fri, 21 Jan 2022 01:45:38 GMT  
		Size: 188.0 MB (188021819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:slim`

```console
$ docker pull rust@sha256:aef724360894cd51ff66420b688dacc811cd1591094ab9561e1a541da366d02b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:slim` - linux; amd64

```console
$ docker pull rust@sha256:c65c489f71effc81ac327df299f4f4b18f02f52a495c928949d9faef37be5c0e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.6 MB (235616218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3d2ecb28032ee0b780251c0e12ba34e4ea2b00bb6c1f54aef24cb70e40d5389`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 02:27:01 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Thu, 27 Jan 2022 02:27:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7c57d6ee4402b697e1f62306aeebe04fca5a4fcfcdd2a1c53900a71bd1ec9d`  
		Last Modified: Thu, 27 Jan 2022 02:31:42 GMT  
		Size: 204.2 MB (204249961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim` - linux; arm variant v7

```console
$ docker pull rust@sha256:5e320dc7dac05018ef56f8e75e29af46cf2b854a2bcd2c5274ec1d0838cfcfbc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.5 MB (269473502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90e30db66a12fb0b6695e5f16320fc49d165f635623f83b53332460ae2d6fd20`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 10:50:56 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 10:52:09 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6a8aa1e46b451ab566c5071e58dce324c2116d376905dec3cffab784b91947`  
		Last Modified: Wed, 26 Jan 2022 10:59:37 GMT  
		Size: 242.9 MB (242908569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:1a9113137065ce5dad9ac0092210e8df36bc896c8d44d156d3cf95a34cf4bd1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.6 MB (301595417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3c255aa040881fa57bc6f56400f12b12ab822a4448a2daa2ad75a6a412195c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:38:53 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 08:39:21 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e175c7caf143e560d9a469fb403bce557467bd7bfd7053747deacafb33fd93f1`  
		Last Modified: Wed, 26 Jan 2022 08:44:18 GMT  
		Size: 271.5 MB (271538643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim` - linux; 386

```console
$ docker pull rust@sha256:52f7d0a7ee12b806c72fc52a9123ef1df65d00645df4c9d91eb3ae8e5d3f56a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281164943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b10b451f292da4629eb4863abeb9d24f63cbce0d73a15e5c1eb595aef34a9b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Fri, 21 Jan 2022 01:40:55 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:41:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867d4c40cb0c2add04a2801c038bb1d2cc2eb532b2a7500c8c657c89ad2dc859`  
		Last Modified: Fri, 21 Jan 2022 01:47:04 GMT  
		Size: 248.8 MB (248794093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:slim-bullseye`

```console
$ docker pull rust@sha256:aef724360894cd51ff66420b688dacc811cd1591094ab9561e1a541da366d02b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:slim-bullseye` - linux; amd64

```console
$ docker pull rust@sha256:c65c489f71effc81ac327df299f4f4b18f02f52a495c928949d9faef37be5c0e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.6 MB (235616218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3d2ecb28032ee0b780251c0e12ba34e4ea2b00bb6c1f54aef24cb70e40d5389`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 02:27:01 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Thu, 27 Jan 2022 02:27:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7c57d6ee4402b697e1f62306aeebe04fca5a4fcfcdd2a1c53900a71bd1ec9d`  
		Last Modified: Thu, 27 Jan 2022 02:31:42 GMT  
		Size: 204.2 MB (204249961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-bullseye` - linux; arm variant v7

```console
$ docker pull rust@sha256:5e320dc7dac05018ef56f8e75e29af46cf2b854a2bcd2c5274ec1d0838cfcfbc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.5 MB (269473502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90e30db66a12fb0b6695e5f16320fc49d165f635623f83b53332460ae2d6fd20`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 10:50:56 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 10:52:09 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6a8aa1e46b451ab566c5071e58dce324c2116d376905dec3cffab784b91947`  
		Last Modified: Wed, 26 Jan 2022 10:59:37 GMT  
		Size: 242.9 MB (242908569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:1a9113137065ce5dad9ac0092210e8df36bc896c8d44d156d3cf95a34cf4bd1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.6 MB (301595417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3c255aa040881fa57bc6f56400f12b12ab822a4448a2daa2ad75a6a412195c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:38:53 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 08:39:21 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e175c7caf143e560d9a469fb403bce557467bd7bfd7053747deacafb33fd93f1`  
		Last Modified: Wed, 26 Jan 2022 08:44:18 GMT  
		Size: 271.5 MB (271538643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-bullseye` - linux; 386

```console
$ docker pull rust@sha256:52f7d0a7ee12b806c72fc52a9123ef1df65d00645df4c9d91eb3ae8e5d3f56a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281164943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b10b451f292da4629eb4863abeb9d24f63cbce0d73a15e5c1eb595aef34a9b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Fri, 21 Jan 2022 01:40:55 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:41:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867d4c40cb0c2add04a2801c038bb1d2cc2eb532b2a7500c8c657c89ad2dc859`  
		Last Modified: Fri, 21 Jan 2022 01:47:04 GMT  
		Size: 248.8 MB (248794093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:slim-buster`

```console
$ docker pull rust@sha256:f97b60397f841696adf7d5094e96d9f32db8b338dd0fa1a6ba3b15f6a8cbbac7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:slim-buster` - linux; amd64

```console
$ docker pull rust@sha256:d70392f42ab0402a067f47cb645ad4c5cb2fccd8de913707b5e9ffe51dccdcc7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.7 MB (216691424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d210d9c6ad548acf5f3bacefc02a1a1b844bd0c695b5d03c01d5f972efa43d23`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 02:26:06 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Thu, 27 Jan 2022 02:26:34 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfd01e1add41d50399c9c7261d9675981c573a096b2db958c6bdb4d0ba3df6e`  
		Last Modified: Thu, 27 Jan 2022 02:29:58 GMT  
		Size: 189.5 MB (189537693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:61d6f5bed2e9fd94e378eab4c9fc5a451caef607f6ac14ffc3fe0f5f7c6109e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.3 MB (256276557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b30e8b184d6c2e016890c87dc71ab25296222a2e934531f2e31c6a7d61046271`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:12 GMT
ADD file:ca8132e20773f7037458cc53fe20a7116f93c21c7479be5a2a1d739495dbe44e in / 
# Wed, 26 Jan 2022 01:43:13 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 10:49:05 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 10:50:20 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:20cc49690d9072283406c1c11e9b1dc1a247782cc8daa526b375d4a7f1cb6a94`  
		Last Modified: Wed, 26 Jan 2022 01:59:27 GMT  
		Size: 22.8 MB (22754397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539f3b7106a14210296dc07ec5c5275b3b7124abffcf23c25d6f79ae330d28b1`  
		Last Modified: Wed, 26 Jan 2022 10:56:40 GMT  
		Size: 233.5 MB (233522160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:fd60d456c8c1818a9f71d0063e20a1d869aa48429afae7f81f24a9b51883a4d1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.0 MB (281957084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35221a2f076a920466686f0e6c540ef9879dfe37e9adaa83ea380eb09bcb5e74`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:37:51 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Wed, 26 Jan 2022 08:38:18 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2765579f339812249621170a70c8cf8430422b746c7163efc3ffe0d2a5b00c6e`  
		Last Modified: Wed, 26 Jan 2022 08:42:15 GMT  
		Size: 256.0 MB (256033868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-buster` - linux; 386

```console
$ docker pull rust@sha256:17efe31938303253b8d9e3afa66de629c033db64a3d9831623d9eb1443865fc7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.8 MB (265819912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07de88a206564ac8ad3534d14868b8b1af2b6375eaf06529bca7af5dc6f685d0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:45 GMT
ADD file:78342a77df22ca22804ea5aec6415ce10c1fdc35687f1b25c5f86850f41d3905 in / 
# Tue, 21 Dec 2021 01:40:45 GMT
CMD ["bash"]
# Fri, 21 Jan 2022 01:39:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.58.1
# Fri, 21 Jan 2022 01:40:14 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:16e3a221bce3a5f7f4a71f72926f381ff9c6141ccb5918b7ea924ff7f7f09d06`  
		Last Modified: Tue, 21 Dec 2021 01:49:46 GMT  
		Size: 27.8 MB (27804573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d81babe2c3794639ff06bb2e5ad026aca8afabb13a8d2e7006bf1795a7e7f4`  
		Last Modified: Fri, 21 Jan 2022 01:44:39 GMT  
		Size: 238.0 MB (238015339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
