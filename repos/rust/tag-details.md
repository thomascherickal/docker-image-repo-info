<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `rust`

-	[`rust:1`](#rust1)
-	[`rust:1.46`](#rust146)
-	[`rust:1.46.0`](#rust1460)
-	[`rust:1.46.0-alpine`](#rust1460-alpine)
-	[`rust:1.46.0-alpine3.11`](#rust1460-alpine311)
-	[`rust:1.46.0-alpine3.12`](#rust1460-alpine312)
-	[`rust:1.46.0-buster`](#rust1460-buster)
-	[`rust:1.46.0-slim`](#rust1460-slim)
-	[`rust:1.46.0-slim-buster`](#rust1460-slim-buster)
-	[`rust:1.46-alpine`](#rust146-alpine)
-	[`rust:1.46-alpine3.11`](#rust146-alpine311)
-	[`rust:1.46-alpine3.12`](#rust146-alpine312)
-	[`rust:1.46-buster`](#rust146-buster)
-	[`rust:1.46-slim`](#rust146-slim)
-	[`rust:1.46-slim-buster`](#rust146-slim-buster)
-	[`rust:1-alpine`](#rust1-alpine)
-	[`rust:1-alpine3.11`](#rust1-alpine311)
-	[`rust:1-alpine3.12`](#rust1-alpine312)
-	[`rust:1-buster`](#rust1-buster)
-	[`rust:1-slim`](#rust1-slim)
-	[`rust:1-slim-buster`](#rust1-slim-buster)
-	[`rust:alpine`](#rustalpine)
-	[`rust:alpine3.11`](#rustalpine311)
-	[`rust:alpine3.12`](#rustalpine312)
-	[`rust:buster`](#rustbuster)
-	[`rust:latest`](#rustlatest)
-	[`rust:slim`](#rustslim)
-	[`rust:slim-buster`](#rustslim-buster)

## `rust:1`

```console
$ docker pull rust@sha256:32110fb328d3c3280f06f10c8efcdb1c31fe12057e01a24668c64bf9c419ab56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1` - linux; amd64

```console
$ docker pull rust@sha256:2c7564a1e4f3223d11bd061cb46b485e57bbfa921821cf857184e64ffc4274e7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **430.1 MB (430091356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc1c343b9048272e2bca499029570351dc36b2e28792661a50d3113d94ca577`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:33 GMT
ADD file:4b03b5f551e3fbdf47ec609712007327828f7530cc3455c43bbcdcaf449a75a9 in / 
# Tue, 04 Aug 2020 15:42:34 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:26:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:26:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 23:26:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:27:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Aug 2020 18:25:43 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:25:55 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:d6ff36c9ec4822c9ff8953560f7ba41653b348a9c1136755e653575f58fbded7`  
		Last Modified: Tue, 04 Aug 2020 15:48:55 GMT  
		Size: 50.4 MB (50396000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c958d65b3090aefea91284d018b2a86530a3c8174b72616c4e76993c696a5797`  
		Last Modified: Tue, 04 Aug 2020 23:39:28 GMT  
		Size: 7.8 MB (7811570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edaf0a6b092f5673ec05b40edb606ce58881b2f40494251117d31805225ef064`  
		Last Modified: Tue, 04 Aug 2020 23:39:27 GMT  
		Size: 10.0 MB (9996337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80931cf6881673fd161a3fd73e8971fe4a569fd7fbb44e956d261ca58d97dfab`  
		Last Modified: Tue, 04 Aug 2020 23:39:45 GMT  
		Size: 51.8 MB (51829826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1b8aca3825e6c3b57e28c8075180f97879161dd58333de13f6b6da0f842af3`  
		Last Modified: Tue, 04 Aug 2020 23:40:24 GMT  
		Size: 192.2 MB (192243499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119498f32df8c0465d687487ca4344eee7ce0c46f80306ea7a34e1c01ff3b461`  
		Last Modified: Thu, 27 Aug 2020 18:27:47 GMT  
		Size: 117.8 MB (117814124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1` - linux; arm variant v7

```console
$ docker pull rust@sha256:955a1c50eaa60d2317a3c758f2b3a37279dae2dee22504db1435766e394d5aa2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.1 MB (413120940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d13b78091ac4db478dc13e5a884c6ca2f05145626411e48050a629300d82f95`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:26 GMT
ADD file:aaf5c6340b3d662631775fa4536c2e48e9f68b6cc8d53e18fb8fd76ae41b305e in / 
# Tue, 04 Aug 2020 04:56:28 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:52:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 07:53:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 07:54:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 00:07:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 13:46:49 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Tue, 01 Sep 2020 13:47:14 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:e7cf402ee4b1ba67e92813d50297a082bbdbdd4d47f6aeb62f2316b81d5dc843`  
		Last Modified: Tue, 04 Aug 2020 05:04:56 GMT  
		Size: 45.9 MB (45869261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff6bd4a89fc21d80ca6924320f86708f35ddea71c7aa34a408a5b64257c764e`  
		Last Modified: Tue, 04 Aug 2020 08:25:56 GMT  
		Size: 7.1 MB (7097820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48f5852a753b7731e5d374567ae9b64e309805758f336c76d5f13bb67c94e20`  
		Last Modified: Tue, 04 Aug 2020 08:25:56 GMT  
		Size: 9.3 MB (9343353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58a93b33dd4d533cc1e04eab8045940d69cb287134aa90c982e3d248739044e`  
		Last Modified: Tue, 04 Aug 2020 08:26:25 GMT  
		Size: 47.4 MB (47355829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06127c17626f8d326b4f2e347e5a9704709941e8a54307a18eda808550446f4`  
		Last Modified: Tue, 01 Sep 2020 00:34:27 GMT  
		Size: 168.5 MB (168488015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567b372ca3cbd9ece4bae988da44aa8716a5eefcb84de9eaf3b962c9beea3c19`  
		Last Modified: Tue, 01 Sep 2020 13:48:25 GMT  
		Size: 135.0 MB (134966662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:56f26196d5917a7f3eb5a0959b42784b77f15325548635789d860d2a7df41958
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.4 MB (448385389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a94406c21898c4d41dc168a007bb4ada2fb5067d3d0ac2ad9487149498cc6855`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:06 GMT
ADD file:ce999027b153d392f8a0f85e2e7a17b9279f3cf7ad0e45192378d527275f99c6 in / 
# Tue, 04 Aug 2020 06:57:08 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 11:10:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 11:10:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 11:10:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Aug 2020 23:44:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 11:03:47 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Tue, 01 Sep 2020 11:04:06 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:d5517ee72007172d5b814636405254dea459120ce08f85777bb287d106a6a240`  
		Last Modified: Tue, 04 Aug 2020 07:03:41 GMT  
		Size: 49.2 MB (49175491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0283897ad4463628bd259e1cbb5eb788e7df554b42ae17fc6f5d02c4a56035c2`  
		Last Modified: Tue, 04 Aug 2020 11:23:01 GMT  
		Size: 7.7 MB (7681458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3feb40d9f5fecfa098b8f7ece6c287c6fd61b114043c8b4647359120a7d943a3`  
		Last Modified: Tue, 04 Aug 2020 11:23:02 GMT  
		Size: 10.0 MB (9983917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86b5fabb62f79acd92186da3c02d23bd8c15d79603a700959b582bd9e62854c`  
		Last Modified: Tue, 04 Aug 2020 11:23:28 GMT  
		Size: 52.2 MB (52163657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ee967f71756804b49b0fb35332bc52b41de2364092ad4c62717b9e3a5e383b`  
		Last Modified: Mon, 31 Aug 2020 23:52:53 GMT  
		Size: 183.8 MB (183788908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f3befe013d7e08e1a2f38383730ab7476092cc35afa3cd17e0ab0ad6c05f69`  
		Last Modified: Tue, 01 Sep 2020 11:05:09 GMT  
		Size: 145.6 MB (145591958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1` - linux; 386

```console
$ docker pull rust@sha256:e158d68ef891c1f41edd6f1bf2adafdcdb360ca98302865d6d35a8ed44236bdd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **459.6 MB (459573291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b478370ac3f9a4831eda8c07897d44711b2b6e81dda7bc8c5694f00f544dd694`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:21 GMT
ADD file:e8aac36755acd0915e9f9bae82fc8fcd0bbc3911ca4a5a40e104b2a4ebce44da in / 
# Tue, 04 Aug 2020 03:37:21 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:06:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:06:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 08:07:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Aug 2020 23:41:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 11:16:42 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Tue, 01 Sep 2020 11:17:06 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:b19305c328889ec69ec0d76e403c2cbc4603e5f27213a0e4d5f6597feefcf6e1`  
		Last Modified: Tue, 04 Aug 2020 03:42:18 GMT  
		Size: 51.2 MB (51158828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d9322a54f80129fd5cd69b7be3ac6ba44b9a0268afcbd10876508eb0f9264c`  
		Last Modified: Tue, 04 Aug 2020 08:25:50 GMT  
		Size: 8.0 MB (7981119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571a7f32100867eafa619a9265416538a2a374b88219902c6270b6f023d19061`  
		Last Modified: Tue, 04 Aug 2020 08:25:51 GMT  
		Size: 10.3 MB (10338494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3ea04987808c324433cf4b1b813ccf6528f9bf603422fbee2725c1e4018eb8`  
		Last Modified: Tue, 04 Aug 2020 08:26:25 GMT  
		Size: 53.4 MB (53433408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f5bab8ea37e9aaec5e57e6ad1fec0818250ec45b7449995899fd030ba8e2b7`  
		Last Modified: Mon, 31 Aug 2020 23:50:11 GMT  
		Size: 198.8 MB (198807590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca1ae032aa8c7efd60c9d3157f80b527ed10af124ec20b7d68b2d9af558506c`  
		Last Modified: Tue, 01 Sep 2020 11:18:29 GMT  
		Size: 137.9 MB (137853852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.46`

```console
$ docker pull rust@sha256:32110fb328d3c3280f06f10c8efcdb1c31fe12057e01a24668c64bf9c419ab56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.46` - linux; amd64

```console
$ docker pull rust@sha256:2c7564a1e4f3223d11bd061cb46b485e57bbfa921821cf857184e64ffc4274e7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **430.1 MB (430091356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc1c343b9048272e2bca499029570351dc36b2e28792661a50d3113d94ca577`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:33 GMT
ADD file:4b03b5f551e3fbdf47ec609712007327828f7530cc3455c43bbcdcaf449a75a9 in / 
# Tue, 04 Aug 2020 15:42:34 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:26:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:26:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 23:26:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:27:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Aug 2020 18:25:43 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:25:55 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:d6ff36c9ec4822c9ff8953560f7ba41653b348a9c1136755e653575f58fbded7`  
		Last Modified: Tue, 04 Aug 2020 15:48:55 GMT  
		Size: 50.4 MB (50396000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c958d65b3090aefea91284d018b2a86530a3c8174b72616c4e76993c696a5797`  
		Last Modified: Tue, 04 Aug 2020 23:39:28 GMT  
		Size: 7.8 MB (7811570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edaf0a6b092f5673ec05b40edb606ce58881b2f40494251117d31805225ef064`  
		Last Modified: Tue, 04 Aug 2020 23:39:27 GMT  
		Size: 10.0 MB (9996337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80931cf6881673fd161a3fd73e8971fe4a569fd7fbb44e956d261ca58d97dfab`  
		Last Modified: Tue, 04 Aug 2020 23:39:45 GMT  
		Size: 51.8 MB (51829826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1b8aca3825e6c3b57e28c8075180f97879161dd58333de13f6b6da0f842af3`  
		Last Modified: Tue, 04 Aug 2020 23:40:24 GMT  
		Size: 192.2 MB (192243499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119498f32df8c0465d687487ca4344eee7ce0c46f80306ea7a34e1c01ff3b461`  
		Last Modified: Thu, 27 Aug 2020 18:27:47 GMT  
		Size: 117.8 MB (117814124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.46` - linux; arm variant v7

```console
$ docker pull rust@sha256:955a1c50eaa60d2317a3c758f2b3a37279dae2dee22504db1435766e394d5aa2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.1 MB (413120940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d13b78091ac4db478dc13e5a884c6ca2f05145626411e48050a629300d82f95`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:26 GMT
ADD file:aaf5c6340b3d662631775fa4536c2e48e9f68b6cc8d53e18fb8fd76ae41b305e in / 
# Tue, 04 Aug 2020 04:56:28 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:52:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 07:53:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 07:54:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 00:07:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 13:46:49 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Tue, 01 Sep 2020 13:47:14 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:e7cf402ee4b1ba67e92813d50297a082bbdbdd4d47f6aeb62f2316b81d5dc843`  
		Last Modified: Tue, 04 Aug 2020 05:04:56 GMT  
		Size: 45.9 MB (45869261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff6bd4a89fc21d80ca6924320f86708f35ddea71c7aa34a408a5b64257c764e`  
		Last Modified: Tue, 04 Aug 2020 08:25:56 GMT  
		Size: 7.1 MB (7097820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48f5852a753b7731e5d374567ae9b64e309805758f336c76d5f13bb67c94e20`  
		Last Modified: Tue, 04 Aug 2020 08:25:56 GMT  
		Size: 9.3 MB (9343353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58a93b33dd4d533cc1e04eab8045940d69cb287134aa90c982e3d248739044e`  
		Last Modified: Tue, 04 Aug 2020 08:26:25 GMT  
		Size: 47.4 MB (47355829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06127c17626f8d326b4f2e347e5a9704709941e8a54307a18eda808550446f4`  
		Last Modified: Tue, 01 Sep 2020 00:34:27 GMT  
		Size: 168.5 MB (168488015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567b372ca3cbd9ece4bae988da44aa8716a5eefcb84de9eaf3b962c9beea3c19`  
		Last Modified: Tue, 01 Sep 2020 13:48:25 GMT  
		Size: 135.0 MB (134966662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.46` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:56f26196d5917a7f3eb5a0959b42784b77f15325548635789d860d2a7df41958
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.4 MB (448385389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a94406c21898c4d41dc168a007bb4ada2fb5067d3d0ac2ad9487149498cc6855`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:06 GMT
ADD file:ce999027b153d392f8a0f85e2e7a17b9279f3cf7ad0e45192378d527275f99c6 in / 
# Tue, 04 Aug 2020 06:57:08 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 11:10:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 11:10:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 11:10:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Aug 2020 23:44:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 11:03:47 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Tue, 01 Sep 2020 11:04:06 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:d5517ee72007172d5b814636405254dea459120ce08f85777bb287d106a6a240`  
		Last Modified: Tue, 04 Aug 2020 07:03:41 GMT  
		Size: 49.2 MB (49175491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0283897ad4463628bd259e1cbb5eb788e7df554b42ae17fc6f5d02c4a56035c2`  
		Last Modified: Tue, 04 Aug 2020 11:23:01 GMT  
		Size: 7.7 MB (7681458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3feb40d9f5fecfa098b8f7ece6c287c6fd61b114043c8b4647359120a7d943a3`  
		Last Modified: Tue, 04 Aug 2020 11:23:02 GMT  
		Size: 10.0 MB (9983917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86b5fabb62f79acd92186da3c02d23bd8c15d79603a700959b582bd9e62854c`  
		Last Modified: Tue, 04 Aug 2020 11:23:28 GMT  
		Size: 52.2 MB (52163657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ee967f71756804b49b0fb35332bc52b41de2364092ad4c62717b9e3a5e383b`  
		Last Modified: Mon, 31 Aug 2020 23:52:53 GMT  
		Size: 183.8 MB (183788908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f3befe013d7e08e1a2f38383730ab7476092cc35afa3cd17e0ab0ad6c05f69`  
		Last Modified: Tue, 01 Sep 2020 11:05:09 GMT  
		Size: 145.6 MB (145591958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.46` - linux; 386

```console
$ docker pull rust@sha256:e158d68ef891c1f41edd6f1bf2adafdcdb360ca98302865d6d35a8ed44236bdd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **459.6 MB (459573291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b478370ac3f9a4831eda8c07897d44711b2b6e81dda7bc8c5694f00f544dd694`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:21 GMT
ADD file:e8aac36755acd0915e9f9bae82fc8fcd0bbc3911ca4a5a40e104b2a4ebce44da in / 
# Tue, 04 Aug 2020 03:37:21 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:06:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:06:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 08:07:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Aug 2020 23:41:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 11:16:42 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Tue, 01 Sep 2020 11:17:06 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:b19305c328889ec69ec0d76e403c2cbc4603e5f27213a0e4d5f6597feefcf6e1`  
		Last Modified: Tue, 04 Aug 2020 03:42:18 GMT  
		Size: 51.2 MB (51158828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d9322a54f80129fd5cd69b7be3ac6ba44b9a0268afcbd10876508eb0f9264c`  
		Last Modified: Tue, 04 Aug 2020 08:25:50 GMT  
		Size: 8.0 MB (7981119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571a7f32100867eafa619a9265416538a2a374b88219902c6270b6f023d19061`  
		Last Modified: Tue, 04 Aug 2020 08:25:51 GMT  
		Size: 10.3 MB (10338494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3ea04987808c324433cf4b1b813ccf6528f9bf603422fbee2725c1e4018eb8`  
		Last Modified: Tue, 04 Aug 2020 08:26:25 GMT  
		Size: 53.4 MB (53433408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f5bab8ea37e9aaec5e57e6ad1fec0818250ec45b7449995899fd030ba8e2b7`  
		Last Modified: Mon, 31 Aug 2020 23:50:11 GMT  
		Size: 198.8 MB (198807590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca1ae032aa8c7efd60c9d3157f80b527ed10af124ec20b7d68b2d9af558506c`  
		Last Modified: Tue, 01 Sep 2020 11:18:29 GMT  
		Size: 137.9 MB (137853852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.46.0`

```console
$ docker pull rust@sha256:32110fb328d3c3280f06f10c8efcdb1c31fe12057e01a24668c64bf9c419ab56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.46.0` - linux; amd64

```console
$ docker pull rust@sha256:2c7564a1e4f3223d11bd061cb46b485e57bbfa921821cf857184e64ffc4274e7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **430.1 MB (430091356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc1c343b9048272e2bca499029570351dc36b2e28792661a50d3113d94ca577`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:33 GMT
ADD file:4b03b5f551e3fbdf47ec609712007327828f7530cc3455c43bbcdcaf449a75a9 in / 
# Tue, 04 Aug 2020 15:42:34 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:26:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:26:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 23:26:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:27:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Aug 2020 18:25:43 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:25:55 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:d6ff36c9ec4822c9ff8953560f7ba41653b348a9c1136755e653575f58fbded7`  
		Last Modified: Tue, 04 Aug 2020 15:48:55 GMT  
		Size: 50.4 MB (50396000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c958d65b3090aefea91284d018b2a86530a3c8174b72616c4e76993c696a5797`  
		Last Modified: Tue, 04 Aug 2020 23:39:28 GMT  
		Size: 7.8 MB (7811570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edaf0a6b092f5673ec05b40edb606ce58881b2f40494251117d31805225ef064`  
		Last Modified: Tue, 04 Aug 2020 23:39:27 GMT  
		Size: 10.0 MB (9996337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80931cf6881673fd161a3fd73e8971fe4a569fd7fbb44e956d261ca58d97dfab`  
		Last Modified: Tue, 04 Aug 2020 23:39:45 GMT  
		Size: 51.8 MB (51829826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1b8aca3825e6c3b57e28c8075180f97879161dd58333de13f6b6da0f842af3`  
		Last Modified: Tue, 04 Aug 2020 23:40:24 GMT  
		Size: 192.2 MB (192243499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119498f32df8c0465d687487ca4344eee7ce0c46f80306ea7a34e1c01ff3b461`  
		Last Modified: Thu, 27 Aug 2020 18:27:47 GMT  
		Size: 117.8 MB (117814124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.46.0` - linux; arm variant v7

```console
$ docker pull rust@sha256:955a1c50eaa60d2317a3c758f2b3a37279dae2dee22504db1435766e394d5aa2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.1 MB (413120940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d13b78091ac4db478dc13e5a884c6ca2f05145626411e48050a629300d82f95`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:26 GMT
ADD file:aaf5c6340b3d662631775fa4536c2e48e9f68b6cc8d53e18fb8fd76ae41b305e in / 
# Tue, 04 Aug 2020 04:56:28 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:52:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 07:53:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 07:54:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 00:07:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 13:46:49 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Tue, 01 Sep 2020 13:47:14 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:e7cf402ee4b1ba67e92813d50297a082bbdbdd4d47f6aeb62f2316b81d5dc843`  
		Last Modified: Tue, 04 Aug 2020 05:04:56 GMT  
		Size: 45.9 MB (45869261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff6bd4a89fc21d80ca6924320f86708f35ddea71c7aa34a408a5b64257c764e`  
		Last Modified: Tue, 04 Aug 2020 08:25:56 GMT  
		Size: 7.1 MB (7097820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48f5852a753b7731e5d374567ae9b64e309805758f336c76d5f13bb67c94e20`  
		Last Modified: Tue, 04 Aug 2020 08:25:56 GMT  
		Size: 9.3 MB (9343353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58a93b33dd4d533cc1e04eab8045940d69cb287134aa90c982e3d248739044e`  
		Last Modified: Tue, 04 Aug 2020 08:26:25 GMT  
		Size: 47.4 MB (47355829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06127c17626f8d326b4f2e347e5a9704709941e8a54307a18eda808550446f4`  
		Last Modified: Tue, 01 Sep 2020 00:34:27 GMT  
		Size: 168.5 MB (168488015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567b372ca3cbd9ece4bae988da44aa8716a5eefcb84de9eaf3b962c9beea3c19`  
		Last Modified: Tue, 01 Sep 2020 13:48:25 GMT  
		Size: 135.0 MB (134966662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.46.0` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:56f26196d5917a7f3eb5a0959b42784b77f15325548635789d860d2a7df41958
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.4 MB (448385389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a94406c21898c4d41dc168a007bb4ada2fb5067d3d0ac2ad9487149498cc6855`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:06 GMT
ADD file:ce999027b153d392f8a0f85e2e7a17b9279f3cf7ad0e45192378d527275f99c6 in / 
# Tue, 04 Aug 2020 06:57:08 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 11:10:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 11:10:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 11:10:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Aug 2020 23:44:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 11:03:47 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Tue, 01 Sep 2020 11:04:06 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:d5517ee72007172d5b814636405254dea459120ce08f85777bb287d106a6a240`  
		Last Modified: Tue, 04 Aug 2020 07:03:41 GMT  
		Size: 49.2 MB (49175491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0283897ad4463628bd259e1cbb5eb788e7df554b42ae17fc6f5d02c4a56035c2`  
		Last Modified: Tue, 04 Aug 2020 11:23:01 GMT  
		Size: 7.7 MB (7681458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3feb40d9f5fecfa098b8f7ece6c287c6fd61b114043c8b4647359120a7d943a3`  
		Last Modified: Tue, 04 Aug 2020 11:23:02 GMT  
		Size: 10.0 MB (9983917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86b5fabb62f79acd92186da3c02d23bd8c15d79603a700959b582bd9e62854c`  
		Last Modified: Tue, 04 Aug 2020 11:23:28 GMT  
		Size: 52.2 MB (52163657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ee967f71756804b49b0fb35332bc52b41de2364092ad4c62717b9e3a5e383b`  
		Last Modified: Mon, 31 Aug 2020 23:52:53 GMT  
		Size: 183.8 MB (183788908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f3befe013d7e08e1a2f38383730ab7476092cc35afa3cd17e0ab0ad6c05f69`  
		Last Modified: Tue, 01 Sep 2020 11:05:09 GMT  
		Size: 145.6 MB (145591958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.46.0` - linux; 386

```console
$ docker pull rust@sha256:e158d68ef891c1f41edd6f1bf2adafdcdb360ca98302865d6d35a8ed44236bdd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **459.6 MB (459573291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b478370ac3f9a4831eda8c07897d44711b2b6e81dda7bc8c5694f00f544dd694`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:21 GMT
ADD file:e8aac36755acd0915e9f9bae82fc8fcd0bbc3911ca4a5a40e104b2a4ebce44da in / 
# Tue, 04 Aug 2020 03:37:21 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:06:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:06:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 08:07:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Aug 2020 23:41:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 11:16:42 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Tue, 01 Sep 2020 11:17:06 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:b19305c328889ec69ec0d76e403c2cbc4603e5f27213a0e4d5f6597feefcf6e1`  
		Last Modified: Tue, 04 Aug 2020 03:42:18 GMT  
		Size: 51.2 MB (51158828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d9322a54f80129fd5cd69b7be3ac6ba44b9a0268afcbd10876508eb0f9264c`  
		Last Modified: Tue, 04 Aug 2020 08:25:50 GMT  
		Size: 8.0 MB (7981119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571a7f32100867eafa619a9265416538a2a374b88219902c6270b6f023d19061`  
		Last Modified: Tue, 04 Aug 2020 08:25:51 GMT  
		Size: 10.3 MB (10338494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3ea04987808c324433cf4b1b813ccf6528f9bf603422fbee2725c1e4018eb8`  
		Last Modified: Tue, 04 Aug 2020 08:26:25 GMT  
		Size: 53.4 MB (53433408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f5bab8ea37e9aaec5e57e6ad1fec0818250ec45b7449995899fd030ba8e2b7`  
		Last Modified: Mon, 31 Aug 2020 23:50:11 GMT  
		Size: 198.8 MB (198807590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca1ae032aa8c7efd60c9d3157f80b527ed10af124ec20b7d68b2d9af558506c`  
		Last Modified: Tue, 01 Sep 2020 11:18:29 GMT  
		Size: 137.9 MB (137853852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.46.0-alpine`

```console
$ docker pull rust@sha256:c9890db1527309a88994b12dfe5e1ed695518037367ffb74df76a66bfc303ef5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1.46.0-alpine` - linux; amd64

```console
$ docker pull rust@sha256:bf15122548d85a37667751cc13e1da6b1e1c288ef6d57449afaf79c796d77978
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.9 MB (193940545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16c57101cc99b4a5a3f817eebfcf782de4bd0717944f26b383c0e31090e9914c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 18 Jun 2020 19:22:19 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 27 Aug 2020 18:26:51 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:27:11 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.22.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "cee31c6f72b953c6293fd5d40142c7d61aa85db2a5ea81b3519fe1b492148dc9 *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host x86_64-unknown-linux-musl;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
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
	-	`sha256:4947720ce5d0f6bf41c2d45682cf4aa8e55d9eb1ada4dfda806dedaac31228f3`  
		Last Modified: Thu, 27 Aug 2020 18:29:23 GMT  
		Size: 143.5 MB (143530073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.46.0-alpine3.11`

```console
$ docker pull rust@sha256:644c097a0703d567bcc2e72a9f26affa172cd2be74c0d0bebcd2eb1b45f66298
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1.46.0-alpine3.11` - linux; amd64

```console
$ docker pull rust@sha256:99596dc88c80ea5984c233f8a6057d25724aaa20b883b58e32648067f4d4d310
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.8 MB (182760067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fab160737bb14788a092fd07ff755de0b51caa67cbbd8581428630a8f8f695d3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:43:51 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 27 Aug 2020 18:26:29 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:26:45 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.22.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "cee31c6f72b953c6293fd5d40142c7d61aa85db2a5ea81b3519fe1b492148dc9 *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host x86_64-unknown-linux-musl;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
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
	-	`sha256:a012b535c7038638f5e2bcb45e46b32b06010197931db0037bb5169b92849b79`  
		Last Modified: Thu, 27 Aug 2020 18:28:55 GMT  
		Size: 143.5 MB (143530108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.46.0-alpine3.12`

```console
$ docker pull rust@sha256:c9890db1527309a88994b12dfe5e1ed695518037367ffb74df76a66bfc303ef5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1.46.0-alpine3.12` - linux; amd64

```console
$ docker pull rust@sha256:bf15122548d85a37667751cc13e1da6b1e1c288ef6d57449afaf79c796d77978
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.9 MB (193940545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16c57101cc99b4a5a3f817eebfcf782de4bd0717944f26b383c0e31090e9914c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 18 Jun 2020 19:22:19 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 27 Aug 2020 18:26:51 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:27:11 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.22.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "cee31c6f72b953c6293fd5d40142c7d61aa85db2a5ea81b3519fe1b492148dc9 *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host x86_64-unknown-linux-musl;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
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
	-	`sha256:4947720ce5d0f6bf41c2d45682cf4aa8e55d9eb1ada4dfda806dedaac31228f3`  
		Last Modified: Thu, 27 Aug 2020 18:29:23 GMT  
		Size: 143.5 MB (143530073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.46.0-buster`

```console
$ docker pull rust@sha256:32110fb328d3c3280f06f10c8efcdb1c31fe12057e01a24668c64bf9c419ab56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.46.0-buster` - linux; amd64

```console
$ docker pull rust@sha256:2c7564a1e4f3223d11bd061cb46b485e57bbfa921821cf857184e64ffc4274e7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **430.1 MB (430091356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc1c343b9048272e2bca499029570351dc36b2e28792661a50d3113d94ca577`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:33 GMT
ADD file:4b03b5f551e3fbdf47ec609712007327828f7530cc3455c43bbcdcaf449a75a9 in / 
# Tue, 04 Aug 2020 15:42:34 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:26:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:26:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 23:26:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:27:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Aug 2020 18:25:43 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:25:55 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:d6ff36c9ec4822c9ff8953560f7ba41653b348a9c1136755e653575f58fbded7`  
		Last Modified: Tue, 04 Aug 2020 15:48:55 GMT  
		Size: 50.4 MB (50396000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c958d65b3090aefea91284d018b2a86530a3c8174b72616c4e76993c696a5797`  
		Last Modified: Tue, 04 Aug 2020 23:39:28 GMT  
		Size: 7.8 MB (7811570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edaf0a6b092f5673ec05b40edb606ce58881b2f40494251117d31805225ef064`  
		Last Modified: Tue, 04 Aug 2020 23:39:27 GMT  
		Size: 10.0 MB (9996337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80931cf6881673fd161a3fd73e8971fe4a569fd7fbb44e956d261ca58d97dfab`  
		Last Modified: Tue, 04 Aug 2020 23:39:45 GMT  
		Size: 51.8 MB (51829826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1b8aca3825e6c3b57e28c8075180f97879161dd58333de13f6b6da0f842af3`  
		Last Modified: Tue, 04 Aug 2020 23:40:24 GMT  
		Size: 192.2 MB (192243499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119498f32df8c0465d687487ca4344eee7ce0c46f80306ea7a34e1c01ff3b461`  
		Last Modified: Thu, 27 Aug 2020 18:27:47 GMT  
		Size: 117.8 MB (117814124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.46.0-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:955a1c50eaa60d2317a3c758f2b3a37279dae2dee22504db1435766e394d5aa2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.1 MB (413120940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d13b78091ac4db478dc13e5a884c6ca2f05145626411e48050a629300d82f95`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:26 GMT
ADD file:aaf5c6340b3d662631775fa4536c2e48e9f68b6cc8d53e18fb8fd76ae41b305e in / 
# Tue, 04 Aug 2020 04:56:28 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:52:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 07:53:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 07:54:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 00:07:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 13:46:49 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Tue, 01 Sep 2020 13:47:14 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:e7cf402ee4b1ba67e92813d50297a082bbdbdd4d47f6aeb62f2316b81d5dc843`  
		Last Modified: Tue, 04 Aug 2020 05:04:56 GMT  
		Size: 45.9 MB (45869261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff6bd4a89fc21d80ca6924320f86708f35ddea71c7aa34a408a5b64257c764e`  
		Last Modified: Tue, 04 Aug 2020 08:25:56 GMT  
		Size: 7.1 MB (7097820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48f5852a753b7731e5d374567ae9b64e309805758f336c76d5f13bb67c94e20`  
		Last Modified: Tue, 04 Aug 2020 08:25:56 GMT  
		Size: 9.3 MB (9343353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58a93b33dd4d533cc1e04eab8045940d69cb287134aa90c982e3d248739044e`  
		Last Modified: Tue, 04 Aug 2020 08:26:25 GMT  
		Size: 47.4 MB (47355829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06127c17626f8d326b4f2e347e5a9704709941e8a54307a18eda808550446f4`  
		Last Modified: Tue, 01 Sep 2020 00:34:27 GMT  
		Size: 168.5 MB (168488015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567b372ca3cbd9ece4bae988da44aa8716a5eefcb84de9eaf3b962c9beea3c19`  
		Last Modified: Tue, 01 Sep 2020 13:48:25 GMT  
		Size: 135.0 MB (134966662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.46.0-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:56f26196d5917a7f3eb5a0959b42784b77f15325548635789d860d2a7df41958
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.4 MB (448385389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a94406c21898c4d41dc168a007bb4ada2fb5067d3d0ac2ad9487149498cc6855`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:06 GMT
ADD file:ce999027b153d392f8a0f85e2e7a17b9279f3cf7ad0e45192378d527275f99c6 in / 
# Tue, 04 Aug 2020 06:57:08 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 11:10:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 11:10:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 11:10:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Aug 2020 23:44:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 11:03:47 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Tue, 01 Sep 2020 11:04:06 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:d5517ee72007172d5b814636405254dea459120ce08f85777bb287d106a6a240`  
		Last Modified: Tue, 04 Aug 2020 07:03:41 GMT  
		Size: 49.2 MB (49175491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0283897ad4463628bd259e1cbb5eb788e7df554b42ae17fc6f5d02c4a56035c2`  
		Last Modified: Tue, 04 Aug 2020 11:23:01 GMT  
		Size: 7.7 MB (7681458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3feb40d9f5fecfa098b8f7ece6c287c6fd61b114043c8b4647359120a7d943a3`  
		Last Modified: Tue, 04 Aug 2020 11:23:02 GMT  
		Size: 10.0 MB (9983917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86b5fabb62f79acd92186da3c02d23bd8c15d79603a700959b582bd9e62854c`  
		Last Modified: Tue, 04 Aug 2020 11:23:28 GMT  
		Size: 52.2 MB (52163657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ee967f71756804b49b0fb35332bc52b41de2364092ad4c62717b9e3a5e383b`  
		Last Modified: Mon, 31 Aug 2020 23:52:53 GMT  
		Size: 183.8 MB (183788908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f3befe013d7e08e1a2f38383730ab7476092cc35afa3cd17e0ab0ad6c05f69`  
		Last Modified: Tue, 01 Sep 2020 11:05:09 GMT  
		Size: 145.6 MB (145591958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.46.0-buster` - linux; 386

```console
$ docker pull rust@sha256:e158d68ef891c1f41edd6f1bf2adafdcdb360ca98302865d6d35a8ed44236bdd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **459.6 MB (459573291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b478370ac3f9a4831eda8c07897d44711b2b6e81dda7bc8c5694f00f544dd694`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:21 GMT
ADD file:e8aac36755acd0915e9f9bae82fc8fcd0bbc3911ca4a5a40e104b2a4ebce44da in / 
# Tue, 04 Aug 2020 03:37:21 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:06:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:06:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 08:07:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Aug 2020 23:41:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 11:16:42 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Tue, 01 Sep 2020 11:17:06 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:b19305c328889ec69ec0d76e403c2cbc4603e5f27213a0e4d5f6597feefcf6e1`  
		Last Modified: Tue, 04 Aug 2020 03:42:18 GMT  
		Size: 51.2 MB (51158828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d9322a54f80129fd5cd69b7be3ac6ba44b9a0268afcbd10876508eb0f9264c`  
		Last Modified: Tue, 04 Aug 2020 08:25:50 GMT  
		Size: 8.0 MB (7981119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571a7f32100867eafa619a9265416538a2a374b88219902c6270b6f023d19061`  
		Last Modified: Tue, 04 Aug 2020 08:25:51 GMT  
		Size: 10.3 MB (10338494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3ea04987808c324433cf4b1b813ccf6528f9bf603422fbee2725c1e4018eb8`  
		Last Modified: Tue, 04 Aug 2020 08:26:25 GMT  
		Size: 53.4 MB (53433408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f5bab8ea37e9aaec5e57e6ad1fec0818250ec45b7449995899fd030ba8e2b7`  
		Last Modified: Mon, 31 Aug 2020 23:50:11 GMT  
		Size: 198.8 MB (198807590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca1ae032aa8c7efd60c9d3157f80b527ed10af124ec20b7d68b2d9af558506c`  
		Last Modified: Tue, 01 Sep 2020 11:18:29 GMT  
		Size: 137.9 MB (137853852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.46.0-slim`

```console
$ docker pull rust@sha256:f85a3e023d743567b5e50e2bc4ebb7346c9c075ba7dd9e6d80944029fbd1486c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.46.0-slim` - linux; amd64

```console
$ docker pull rust@sha256:49d07d2db02fa0841e7ed32fae4cacb9fa1ee8a04c0a94704ff63b5e1e3eb7dd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190291843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3861b3896a2d81d06bae7f5953cbaebfebf963be0ec236f9e23765813399e1eb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:25:59 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:26:23 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f015bf9c4dd2d9ed612318f06172c4f6897767bd5f1499c86f8a4aecfc7365e`  
		Last Modified: Thu, 27 Aug 2020 18:28:22 GMT  
		Size: 163.2 MB (163199722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.46.0-slim` - linux; arm variant v7

```console
$ docker pull rust@sha256:19524eb52c32eeeb7ed07b47b612168ab8df8b703777675fa63ef790648cfdbc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.6 MB (190554246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87cca1ed4a91bd2358018dbe889d39425ab96100e85bc14a216a1dab68294473`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:49 GMT
ADD file:16169b615697a126ae57dc01f7c4902fb9d9bc1e8595af43293700fa030808cc in / 
# Tue, 04 Aug 2020 04:56:51 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:03:24 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:04:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:d7fe0a1b85ffd3158c62ab2e06ab004dc957cd133ba7129fb9c69c4586f407c9`  
		Last Modified: Tue, 04 Aug 2020 05:05:19 GMT  
		Size: 22.7 MB (22699792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33747b5bf9abc484825c2d846a0336eebce4d644e84a492222bd96ba0bb68afd`  
		Last Modified: Thu, 27 Aug 2020 18:07:04 GMT  
		Size: 167.9 MB (167854454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.46.0-slim` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:27a8acfbf882283d60faef75b1f21bc7473806e28be6c42e3cdb8ffd435a60e4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.6 MB (211636430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feaf923665d1dd9d4df676a0879afc8c240b3a1a11aa2197a4e7d82f7a26e260`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:29 GMT
ADD file:90ba7821623ab55fc1073647cc611cc45f5e306ade734910e587021971483eec in / 
# Tue, 04 Aug 2020 06:57:31 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:46:17 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:46:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:3742235f1882fee5cca1effc4ca0f0c7c180bbe169800a85daedcf3968b0d8f0`  
		Last Modified: Tue, 04 Aug 2020 07:04:03 GMT  
		Size: 25.8 MB (25849301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5562b9af59dfc44a93f04d4499240af3fd48e4b7fb7302fc1e704b62903af586`  
		Last Modified: Thu, 27 Aug 2020 18:49:12 GMT  
		Size: 185.8 MB (185787129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.46.0-slim` - linux; 386

```console
$ docker pull rust@sha256:075ed84cdfefb54e0059ff9d0dd93064c4843decedaf92314e53c392926d6358
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.6 MB (215582587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f7770bf7c551767284e71e7bf5dc9768cface5153f77dcc8e36dfadffdc1759`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:35 GMT
ADD file:cc791c21e6022a12dd1445a35f4cca9392ad8edfe34ea5852f3e87862c943628 in / 
# Tue, 04 Aug 2020 03:37:35 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:41:02 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:41:35 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:23ad22c16ab9d635a179d5d341096c34912941507b0c77ac97083b9795d8516f`  
		Last Modified: Tue, 04 Aug 2020 03:42:33 GMT  
		Size: 27.8 MB (27750435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9c10f6e7a2a850ab44763fa49cb09d7f46f4a741cab45df2e767d541b0ebc0`  
		Last Modified: Thu, 27 Aug 2020 18:43:30 GMT  
		Size: 187.8 MB (187832152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.46.0-slim-buster`

```console
$ docker pull rust@sha256:f85a3e023d743567b5e50e2bc4ebb7346c9c075ba7dd9e6d80944029fbd1486c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.46.0-slim-buster` - linux; amd64

```console
$ docker pull rust@sha256:49d07d2db02fa0841e7ed32fae4cacb9fa1ee8a04c0a94704ff63b5e1e3eb7dd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190291843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3861b3896a2d81d06bae7f5953cbaebfebf963be0ec236f9e23765813399e1eb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:25:59 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:26:23 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f015bf9c4dd2d9ed612318f06172c4f6897767bd5f1499c86f8a4aecfc7365e`  
		Last Modified: Thu, 27 Aug 2020 18:28:22 GMT  
		Size: 163.2 MB (163199722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.46.0-slim-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:19524eb52c32eeeb7ed07b47b612168ab8df8b703777675fa63ef790648cfdbc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.6 MB (190554246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87cca1ed4a91bd2358018dbe889d39425ab96100e85bc14a216a1dab68294473`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:49 GMT
ADD file:16169b615697a126ae57dc01f7c4902fb9d9bc1e8595af43293700fa030808cc in / 
# Tue, 04 Aug 2020 04:56:51 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:03:24 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:04:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:d7fe0a1b85ffd3158c62ab2e06ab004dc957cd133ba7129fb9c69c4586f407c9`  
		Last Modified: Tue, 04 Aug 2020 05:05:19 GMT  
		Size: 22.7 MB (22699792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33747b5bf9abc484825c2d846a0336eebce4d644e84a492222bd96ba0bb68afd`  
		Last Modified: Thu, 27 Aug 2020 18:07:04 GMT  
		Size: 167.9 MB (167854454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.46.0-slim-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:27a8acfbf882283d60faef75b1f21bc7473806e28be6c42e3cdb8ffd435a60e4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.6 MB (211636430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feaf923665d1dd9d4df676a0879afc8c240b3a1a11aa2197a4e7d82f7a26e260`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:29 GMT
ADD file:90ba7821623ab55fc1073647cc611cc45f5e306ade734910e587021971483eec in / 
# Tue, 04 Aug 2020 06:57:31 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:46:17 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:46:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:3742235f1882fee5cca1effc4ca0f0c7c180bbe169800a85daedcf3968b0d8f0`  
		Last Modified: Tue, 04 Aug 2020 07:04:03 GMT  
		Size: 25.8 MB (25849301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5562b9af59dfc44a93f04d4499240af3fd48e4b7fb7302fc1e704b62903af586`  
		Last Modified: Thu, 27 Aug 2020 18:49:12 GMT  
		Size: 185.8 MB (185787129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.46.0-slim-buster` - linux; 386

```console
$ docker pull rust@sha256:075ed84cdfefb54e0059ff9d0dd93064c4843decedaf92314e53c392926d6358
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.6 MB (215582587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f7770bf7c551767284e71e7bf5dc9768cface5153f77dcc8e36dfadffdc1759`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:35 GMT
ADD file:cc791c21e6022a12dd1445a35f4cca9392ad8edfe34ea5852f3e87862c943628 in / 
# Tue, 04 Aug 2020 03:37:35 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:41:02 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:41:35 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:23ad22c16ab9d635a179d5d341096c34912941507b0c77ac97083b9795d8516f`  
		Last Modified: Tue, 04 Aug 2020 03:42:33 GMT  
		Size: 27.8 MB (27750435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9c10f6e7a2a850ab44763fa49cb09d7f46f4a741cab45df2e767d541b0ebc0`  
		Last Modified: Thu, 27 Aug 2020 18:43:30 GMT  
		Size: 187.8 MB (187832152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.46-alpine`

```console
$ docker pull rust@sha256:c9890db1527309a88994b12dfe5e1ed695518037367ffb74df76a66bfc303ef5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1.46-alpine` - linux; amd64

```console
$ docker pull rust@sha256:bf15122548d85a37667751cc13e1da6b1e1c288ef6d57449afaf79c796d77978
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.9 MB (193940545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16c57101cc99b4a5a3f817eebfcf782de4bd0717944f26b383c0e31090e9914c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 18 Jun 2020 19:22:19 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 27 Aug 2020 18:26:51 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:27:11 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.22.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "cee31c6f72b953c6293fd5d40142c7d61aa85db2a5ea81b3519fe1b492148dc9 *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host x86_64-unknown-linux-musl;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
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
	-	`sha256:4947720ce5d0f6bf41c2d45682cf4aa8e55d9eb1ada4dfda806dedaac31228f3`  
		Last Modified: Thu, 27 Aug 2020 18:29:23 GMT  
		Size: 143.5 MB (143530073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.46-alpine3.11`

```console
$ docker pull rust@sha256:644c097a0703d567bcc2e72a9f26affa172cd2be74c0d0bebcd2eb1b45f66298
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1.46-alpine3.11` - linux; amd64

```console
$ docker pull rust@sha256:99596dc88c80ea5984c233f8a6057d25724aaa20b883b58e32648067f4d4d310
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.8 MB (182760067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fab160737bb14788a092fd07ff755de0b51caa67cbbd8581428630a8f8f695d3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:43:51 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 27 Aug 2020 18:26:29 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:26:45 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.22.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "cee31c6f72b953c6293fd5d40142c7d61aa85db2a5ea81b3519fe1b492148dc9 *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host x86_64-unknown-linux-musl;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
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
	-	`sha256:a012b535c7038638f5e2bcb45e46b32b06010197931db0037bb5169b92849b79`  
		Last Modified: Thu, 27 Aug 2020 18:28:55 GMT  
		Size: 143.5 MB (143530108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.46-alpine3.12`

```console
$ docker pull rust@sha256:c9890db1527309a88994b12dfe5e1ed695518037367ffb74df76a66bfc303ef5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1.46-alpine3.12` - linux; amd64

```console
$ docker pull rust@sha256:bf15122548d85a37667751cc13e1da6b1e1c288ef6d57449afaf79c796d77978
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.9 MB (193940545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16c57101cc99b4a5a3f817eebfcf782de4bd0717944f26b383c0e31090e9914c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 18 Jun 2020 19:22:19 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 27 Aug 2020 18:26:51 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:27:11 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.22.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "cee31c6f72b953c6293fd5d40142c7d61aa85db2a5ea81b3519fe1b492148dc9 *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host x86_64-unknown-linux-musl;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
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
	-	`sha256:4947720ce5d0f6bf41c2d45682cf4aa8e55d9eb1ada4dfda806dedaac31228f3`  
		Last Modified: Thu, 27 Aug 2020 18:29:23 GMT  
		Size: 143.5 MB (143530073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.46-buster`

```console
$ docker pull rust@sha256:32110fb328d3c3280f06f10c8efcdb1c31fe12057e01a24668c64bf9c419ab56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.46-buster` - linux; amd64

```console
$ docker pull rust@sha256:2c7564a1e4f3223d11bd061cb46b485e57bbfa921821cf857184e64ffc4274e7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **430.1 MB (430091356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc1c343b9048272e2bca499029570351dc36b2e28792661a50d3113d94ca577`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:33 GMT
ADD file:4b03b5f551e3fbdf47ec609712007327828f7530cc3455c43bbcdcaf449a75a9 in / 
# Tue, 04 Aug 2020 15:42:34 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:26:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:26:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 23:26:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:27:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Aug 2020 18:25:43 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:25:55 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:d6ff36c9ec4822c9ff8953560f7ba41653b348a9c1136755e653575f58fbded7`  
		Last Modified: Tue, 04 Aug 2020 15:48:55 GMT  
		Size: 50.4 MB (50396000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c958d65b3090aefea91284d018b2a86530a3c8174b72616c4e76993c696a5797`  
		Last Modified: Tue, 04 Aug 2020 23:39:28 GMT  
		Size: 7.8 MB (7811570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edaf0a6b092f5673ec05b40edb606ce58881b2f40494251117d31805225ef064`  
		Last Modified: Tue, 04 Aug 2020 23:39:27 GMT  
		Size: 10.0 MB (9996337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80931cf6881673fd161a3fd73e8971fe4a569fd7fbb44e956d261ca58d97dfab`  
		Last Modified: Tue, 04 Aug 2020 23:39:45 GMT  
		Size: 51.8 MB (51829826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1b8aca3825e6c3b57e28c8075180f97879161dd58333de13f6b6da0f842af3`  
		Last Modified: Tue, 04 Aug 2020 23:40:24 GMT  
		Size: 192.2 MB (192243499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119498f32df8c0465d687487ca4344eee7ce0c46f80306ea7a34e1c01ff3b461`  
		Last Modified: Thu, 27 Aug 2020 18:27:47 GMT  
		Size: 117.8 MB (117814124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.46-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:955a1c50eaa60d2317a3c758f2b3a37279dae2dee22504db1435766e394d5aa2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.1 MB (413120940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d13b78091ac4db478dc13e5a884c6ca2f05145626411e48050a629300d82f95`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:26 GMT
ADD file:aaf5c6340b3d662631775fa4536c2e48e9f68b6cc8d53e18fb8fd76ae41b305e in / 
# Tue, 04 Aug 2020 04:56:28 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:52:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 07:53:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 07:54:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 00:07:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 13:46:49 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Tue, 01 Sep 2020 13:47:14 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:e7cf402ee4b1ba67e92813d50297a082bbdbdd4d47f6aeb62f2316b81d5dc843`  
		Last Modified: Tue, 04 Aug 2020 05:04:56 GMT  
		Size: 45.9 MB (45869261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff6bd4a89fc21d80ca6924320f86708f35ddea71c7aa34a408a5b64257c764e`  
		Last Modified: Tue, 04 Aug 2020 08:25:56 GMT  
		Size: 7.1 MB (7097820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48f5852a753b7731e5d374567ae9b64e309805758f336c76d5f13bb67c94e20`  
		Last Modified: Tue, 04 Aug 2020 08:25:56 GMT  
		Size: 9.3 MB (9343353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58a93b33dd4d533cc1e04eab8045940d69cb287134aa90c982e3d248739044e`  
		Last Modified: Tue, 04 Aug 2020 08:26:25 GMT  
		Size: 47.4 MB (47355829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06127c17626f8d326b4f2e347e5a9704709941e8a54307a18eda808550446f4`  
		Last Modified: Tue, 01 Sep 2020 00:34:27 GMT  
		Size: 168.5 MB (168488015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567b372ca3cbd9ece4bae988da44aa8716a5eefcb84de9eaf3b962c9beea3c19`  
		Last Modified: Tue, 01 Sep 2020 13:48:25 GMT  
		Size: 135.0 MB (134966662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.46-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:56f26196d5917a7f3eb5a0959b42784b77f15325548635789d860d2a7df41958
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.4 MB (448385389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a94406c21898c4d41dc168a007bb4ada2fb5067d3d0ac2ad9487149498cc6855`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:06 GMT
ADD file:ce999027b153d392f8a0f85e2e7a17b9279f3cf7ad0e45192378d527275f99c6 in / 
# Tue, 04 Aug 2020 06:57:08 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 11:10:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 11:10:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 11:10:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Aug 2020 23:44:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 11:03:47 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Tue, 01 Sep 2020 11:04:06 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:d5517ee72007172d5b814636405254dea459120ce08f85777bb287d106a6a240`  
		Last Modified: Tue, 04 Aug 2020 07:03:41 GMT  
		Size: 49.2 MB (49175491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0283897ad4463628bd259e1cbb5eb788e7df554b42ae17fc6f5d02c4a56035c2`  
		Last Modified: Tue, 04 Aug 2020 11:23:01 GMT  
		Size: 7.7 MB (7681458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3feb40d9f5fecfa098b8f7ece6c287c6fd61b114043c8b4647359120a7d943a3`  
		Last Modified: Tue, 04 Aug 2020 11:23:02 GMT  
		Size: 10.0 MB (9983917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86b5fabb62f79acd92186da3c02d23bd8c15d79603a700959b582bd9e62854c`  
		Last Modified: Tue, 04 Aug 2020 11:23:28 GMT  
		Size: 52.2 MB (52163657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ee967f71756804b49b0fb35332bc52b41de2364092ad4c62717b9e3a5e383b`  
		Last Modified: Mon, 31 Aug 2020 23:52:53 GMT  
		Size: 183.8 MB (183788908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f3befe013d7e08e1a2f38383730ab7476092cc35afa3cd17e0ab0ad6c05f69`  
		Last Modified: Tue, 01 Sep 2020 11:05:09 GMT  
		Size: 145.6 MB (145591958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.46-buster` - linux; 386

```console
$ docker pull rust@sha256:e158d68ef891c1f41edd6f1bf2adafdcdb360ca98302865d6d35a8ed44236bdd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **459.6 MB (459573291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b478370ac3f9a4831eda8c07897d44711b2b6e81dda7bc8c5694f00f544dd694`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:21 GMT
ADD file:e8aac36755acd0915e9f9bae82fc8fcd0bbc3911ca4a5a40e104b2a4ebce44da in / 
# Tue, 04 Aug 2020 03:37:21 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:06:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:06:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 08:07:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Aug 2020 23:41:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 11:16:42 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Tue, 01 Sep 2020 11:17:06 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:b19305c328889ec69ec0d76e403c2cbc4603e5f27213a0e4d5f6597feefcf6e1`  
		Last Modified: Tue, 04 Aug 2020 03:42:18 GMT  
		Size: 51.2 MB (51158828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d9322a54f80129fd5cd69b7be3ac6ba44b9a0268afcbd10876508eb0f9264c`  
		Last Modified: Tue, 04 Aug 2020 08:25:50 GMT  
		Size: 8.0 MB (7981119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571a7f32100867eafa619a9265416538a2a374b88219902c6270b6f023d19061`  
		Last Modified: Tue, 04 Aug 2020 08:25:51 GMT  
		Size: 10.3 MB (10338494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3ea04987808c324433cf4b1b813ccf6528f9bf603422fbee2725c1e4018eb8`  
		Last Modified: Tue, 04 Aug 2020 08:26:25 GMT  
		Size: 53.4 MB (53433408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f5bab8ea37e9aaec5e57e6ad1fec0818250ec45b7449995899fd030ba8e2b7`  
		Last Modified: Mon, 31 Aug 2020 23:50:11 GMT  
		Size: 198.8 MB (198807590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca1ae032aa8c7efd60c9d3157f80b527ed10af124ec20b7d68b2d9af558506c`  
		Last Modified: Tue, 01 Sep 2020 11:18:29 GMT  
		Size: 137.9 MB (137853852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.46-slim`

```console
$ docker pull rust@sha256:f85a3e023d743567b5e50e2bc4ebb7346c9c075ba7dd9e6d80944029fbd1486c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.46-slim` - linux; amd64

```console
$ docker pull rust@sha256:49d07d2db02fa0841e7ed32fae4cacb9fa1ee8a04c0a94704ff63b5e1e3eb7dd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190291843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3861b3896a2d81d06bae7f5953cbaebfebf963be0ec236f9e23765813399e1eb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:25:59 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:26:23 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f015bf9c4dd2d9ed612318f06172c4f6897767bd5f1499c86f8a4aecfc7365e`  
		Last Modified: Thu, 27 Aug 2020 18:28:22 GMT  
		Size: 163.2 MB (163199722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.46-slim` - linux; arm variant v7

```console
$ docker pull rust@sha256:19524eb52c32eeeb7ed07b47b612168ab8df8b703777675fa63ef790648cfdbc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.6 MB (190554246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87cca1ed4a91bd2358018dbe889d39425ab96100e85bc14a216a1dab68294473`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:49 GMT
ADD file:16169b615697a126ae57dc01f7c4902fb9d9bc1e8595af43293700fa030808cc in / 
# Tue, 04 Aug 2020 04:56:51 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:03:24 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:04:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:d7fe0a1b85ffd3158c62ab2e06ab004dc957cd133ba7129fb9c69c4586f407c9`  
		Last Modified: Tue, 04 Aug 2020 05:05:19 GMT  
		Size: 22.7 MB (22699792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33747b5bf9abc484825c2d846a0336eebce4d644e84a492222bd96ba0bb68afd`  
		Last Modified: Thu, 27 Aug 2020 18:07:04 GMT  
		Size: 167.9 MB (167854454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.46-slim` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:27a8acfbf882283d60faef75b1f21bc7473806e28be6c42e3cdb8ffd435a60e4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.6 MB (211636430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feaf923665d1dd9d4df676a0879afc8c240b3a1a11aa2197a4e7d82f7a26e260`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:29 GMT
ADD file:90ba7821623ab55fc1073647cc611cc45f5e306ade734910e587021971483eec in / 
# Tue, 04 Aug 2020 06:57:31 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:46:17 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:46:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:3742235f1882fee5cca1effc4ca0f0c7c180bbe169800a85daedcf3968b0d8f0`  
		Last Modified: Tue, 04 Aug 2020 07:04:03 GMT  
		Size: 25.8 MB (25849301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5562b9af59dfc44a93f04d4499240af3fd48e4b7fb7302fc1e704b62903af586`  
		Last Modified: Thu, 27 Aug 2020 18:49:12 GMT  
		Size: 185.8 MB (185787129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.46-slim` - linux; 386

```console
$ docker pull rust@sha256:075ed84cdfefb54e0059ff9d0dd93064c4843decedaf92314e53c392926d6358
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.6 MB (215582587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f7770bf7c551767284e71e7bf5dc9768cface5153f77dcc8e36dfadffdc1759`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:35 GMT
ADD file:cc791c21e6022a12dd1445a35f4cca9392ad8edfe34ea5852f3e87862c943628 in / 
# Tue, 04 Aug 2020 03:37:35 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:41:02 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:41:35 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:23ad22c16ab9d635a179d5d341096c34912941507b0c77ac97083b9795d8516f`  
		Last Modified: Tue, 04 Aug 2020 03:42:33 GMT  
		Size: 27.8 MB (27750435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9c10f6e7a2a850ab44763fa49cb09d7f46f4a741cab45df2e767d541b0ebc0`  
		Last Modified: Thu, 27 Aug 2020 18:43:30 GMT  
		Size: 187.8 MB (187832152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.46-slim-buster`

```console
$ docker pull rust@sha256:f85a3e023d743567b5e50e2bc4ebb7346c9c075ba7dd9e6d80944029fbd1486c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.46-slim-buster` - linux; amd64

```console
$ docker pull rust@sha256:49d07d2db02fa0841e7ed32fae4cacb9fa1ee8a04c0a94704ff63b5e1e3eb7dd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190291843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3861b3896a2d81d06bae7f5953cbaebfebf963be0ec236f9e23765813399e1eb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:25:59 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:26:23 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f015bf9c4dd2d9ed612318f06172c4f6897767bd5f1499c86f8a4aecfc7365e`  
		Last Modified: Thu, 27 Aug 2020 18:28:22 GMT  
		Size: 163.2 MB (163199722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.46-slim-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:19524eb52c32eeeb7ed07b47b612168ab8df8b703777675fa63ef790648cfdbc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.6 MB (190554246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87cca1ed4a91bd2358018dbe889d39425ab96100e85bc14a216a1dab68294473`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:49 GMT
ADD file:16169b615697a126ae57dc01f7c4902fb9d9bc1e8595af43293700fa030808cc in / 
# Tue, 04 Aug 2020 04:56:51 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:03:24 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:04:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:d7fe0a1b85ffd3158c62ab2e06ab004dc957cd133ba7129fb9c69c4586f407c9`  
		Last Modified: Tue, 04 Aug 2020 05:05:19 GMT  
		Size: 22.7 MB (22699792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33747b5bf9abc484825c2d846a0336eebce4d644e84a492222bd96ba0bb68afd`  
		Last Modified: Thu, 27 Aug 2020 18:07:04 GMT  
		Size: 167.9 MB (167854454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.46-slim-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:27a8acfbf882283d60faef75b1f21bc7473806e28be6c42e3cdb8ffd435a60e4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.6 MB (211636430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feaf923665d1dd9d4df676a0879afc8c240b3a1a11aa2197a4e7d82f7a26e260`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:29 GMT
ADD file:90ba7821623ab55fc1073647cc611cc45f5e306ade734910e587021971483eec in / 
# Tue, 04 Aug 2020 06:57:31 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:46:17 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:46:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:3742235f1882fee5cca1effc4ca0f0c7c180bbe169800a85daedcf3968b0d8f0`  
		Last Modified: Tue, 04 Aug 2020 07:04:03 GMT  
		Size: 25.8 MB (25849301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5562b9af59dfc44a93f04d4499240af3fd48e4b7fb7302fc1e704b62903af586`  
		Last Modified: Thu, 27 Aug 2020 18:49:12 GMT  
		Size: 185.8 MB (185787129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.46-slim-buster` - linux; 386

```console
$ docker pull rust@sha256:075ed84cdfefb54e0059ff9d0dd93064c4843decedaf92314e53c392926d6358
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.6 MB (215582587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f7770bf7c551767284e71e7bf5dc9768cface5153f77dcc8e36dfadffdc1759`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:35 GMT
ADD file:cc791c21e6022a12dd1445a35f4cca9392ad8edfe34ea5852f3e87862c943628 in / 
# Tue, 04 Aug 2020 03:37:35 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:41:02 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:41:35 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:23ad22c16ab9d635a179d5d341096c34912941507b0c77ac97083b9795d8516f`  
		Last Modified: Tue, 04 Aug 2020 03:42:33 GMT  
		Size: 27.8 MB (27750435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9c10f6e7a2a850ab44763fa49cb09d7f46f4a741cab45df2e767d541b0ebc0`  
		Last Modified: Thu, 27 Aug 2020 18:43:30 GMT  
		Size: 187.8 MB (187832152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-alpine`

```console
$ docker pull rust@sha256:c9890db1527309a88994b12dfe5e1ed695518037367ffb74df76a66bfc303ef5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1-alpine` - linux; amd64

```console
$ docker pull rust@sha256:bf15122548d85a37667751cc13e1da6b1e1c288ef6d57449afaf79c796d77978
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.9 MB (193940545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16c57101cc99b4a5a3f817eebfcf782de4bd0717944f26b383c0e31090e9914c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 18 Jun 2020 19:22:19 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 27 Aug 2020 18:26:51 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:27:11 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.22.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "cee31c6f72b953c6293fd5d40142c7d61aa85db2a5ea81b3519fe1b492148dc9 *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host x86_64-unknown-linux-musl;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
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
	-	`sha256:4947720ce5d0f6bf41c2d45682cf4aa8e55d9eb1ada4dfda806dedaac31228f3`  
		Last Modified: Thu, 27 Aug 2020 18:29:23 GMT  
		Size: 143.5 MB (143530073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-alpine3.11`

```console
$ docker pull rust@sha256:644c097a0703d567bcc2e72a9f26affa172cd2be74c0d0bebcd2eb1b45f66298
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1-alpine3.11` - linux; amd64

```console
$ docker pull rust@sha256:99596dc88c80ea5984c233f8a6057d25724aaa20b883b58e32648067f4d4d310
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.8 MB (182760067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fab160737bb14788a092fd07ff755de0b51caa67cbbd8581428630a8f8f695d3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:43:51 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 27 Aug 2020 18:26:29 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:26:45 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.22.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "cee31c6f72b953c6293fd5d40142c7d61aa85db2a5ea81b3519fe1b492148dc9 *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host x86_64-unknown-linux-musl;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
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
	-	`sha256:a012b535c7038638f5e2bcb45e46b32b06010197931db0037bb5169b92849b79`  
		Last Modified: Thu, 27 Aug 2020 18:28:55 GMT  
		Size: 143.5 MB (143530108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-alpine3.12`

```console
$ docker pull rust@sha256:c9890db1527309a88994b12dfe5e1ed695518037367ffb74df76a66bfc303ef5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1-alpine3.12` - linux; amd64

```console
$ docker pull rust@sha256:bf15122548d85a37667751cc13e1da6b1e1c288ef6d57449afaf79c796d77978
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.9 MB (193940545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16c57101cc99b4a5a3f817eebfcf782de4bd0717944f26b383c0e31090e9914c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 18 Jun 2020 19:22:19 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 27 Aug 2020 18:26:51 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:27:11 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.22.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "cee31c6f72b953c6293fd5d40142c7d61aa85db2a5ea81b3519fe1b492148dc9 *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host x86_64-unknown-linux-musl;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
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
	-	`sha256:4947720ce5d0f6bf41c2d45682cf4aa8e55d9eb1ada4dfda806dedaac31228f3`  
		Last Modified: Thu, 27 Aug 2020 18:29:23 GMT  
		Size: 143.5 MB (143530073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-buster`

```console
$ docker pull rust@sha256:32110fb328d3c3280f06f10c8efcdb1c31fe12057e01a24668c64bf9c419ab56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-buster` - linux; amd64

```console
$ docker pull rust@sha256:2c7564a1e4f3223d11bd061cb46b485e57bbfa921821cf857184e64ffc4274e7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **430.1 MB (430091356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc1c343b9048272e2bca499029570351dc36b2e28792661a50d3113d94ca577`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:33 GMT
ADD file:4b03b5f551e3fbdf47ec609712007327828f7530cc3455c43bbcdcaf449a75a9 in / 
# Tue, 04 Aug 2020 15:42:34 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:26:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:26:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 23:26:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:27:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Aug 2020 18:25:43 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:25:55 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:d6ff36c9ec4822c9ff8953560f7ba41653b348a9c1136755e653575f58fbded7`  
		Last Modified: Tue, 04 Aug 2020 15:48:55 GMT  
		Size: 50.4 MB (50396000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c958d65b3090aefea91284d018b2a86530a3c8174b72616c4e76993c696a5797`  
		Last Modified: Tue, 04 Aug 2020 23:39:28 GMT  
		Size: 7.8 MB (7811570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edaf0a6b092f5673ec05b40edb606ce58881b2f40494251117d31805225ef064`  
		Last Modified: Tue, 04 Aug 2020 23:39:27 GMT  
		Size: 10.0 MB (9996337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80931cf6881673fd161a3fd73e8971fe4a569fd7fbb44e956d261ca58d97dfab`  
		Last Modified: Tue, 04 Aug 2020 23:39:45 GMT  
		Size: 51.8 MB (51829826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1b8aca3825e6c3b57e28c8075180f97879161dd58333de13f6b6da0f842af3`  
		Last Modified: Tue, 04 Aug 2020 23:40:24 GMT  
		Size: 192.2 MB (192243499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119498f32df8c0465d687487ca4344eee7ce0c46f80306ea7a34e1c01ff3b461`  
		Last Modified: Thu, 27 Aug 2020 18:27:47 GMT  
		Size: 117.8 MB (117814124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:955a1c50eaa60d2317a3c758f2b3a37279dae2dee22504db1435766e394d5aa2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.1 MB (413120940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d13b78091ac4db478dc13e5a884c6ca2f05145626411e48050a629300d82f95`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:26 GMT
ADD file:aaf5c6340b3d662631775fa4536c2e48e9f68b6cc8d53e18fb8fd76ae41b305e in / 
# Tue, 04 Aug 2020 04:56:28 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:52:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 07:53:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 07:54:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 00:07:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 13:46:49 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Tue, 01 Sep 2020 13:47:14 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:e7cf402ee4b1ba67e92813d50297a082bbdbdd4d47f6aeb62f2316b81d5dc843`  
		Last Modified: Tue, 04 Aug 2020 05:04:56 GMT  
		Size: 45.9 MB (45869261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff6bd4a89fc21d80ca6924320f86708f35ddea71c7aa34a408a5b64257c764e`  
		Last Modified: Tue, 04 Aug 2020 08:25:56 GMT  
		Size: 7.1 MB (7097820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48f5852a753b7731e5d374567ae9b64e309805758f336c76d5f13bb67c94e20`  
		Last Modified: Tue, 04 Aug 2020 08:25:56 GMT  
		Size: 9.3 MB (9343353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58a93b33dd4d533cc1e04eab8045940d69cb287134aa90c982e3d248739044e`  
		Last Modified: Tue, 04 Aug 2020 08:26:25 GMT  
		Size: 47.4 MB (47355829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06127c17626f8d326b4f2e347e5a9704709941e8a54307a18eda808550446f4`  
		Last Modified: Tue, 01 Sep 2020 00:34:27 GMT  
		Size: 168.5 MB (168488015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567b372ca3cbd9ece4bae988da44aa8716a5eefcb84de9eaf3b962c9beea3c19`  
		Last Modified: Tue, 01 Sep 2020 13:48:25 GMT  
		Size: 135.0 MB (134966662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:56f26196d5917a7f3eb5a0959b42784b77f15325548635789d860d2a7df41958
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.4 MB (448385389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a94406c21898c4d41dc168a007bb4ada2fb5067d3d0ac2ad9487149498cc6855`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:06 GMT
ADD file:ce999027b153d392f8a0f85e2e7a17b9279f3cf7ad0e45192378d527275f99c6 in / 
# Tue, 04 Aug 2020 06:57:08 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 11:10:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 11:10:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 11:10:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Aug 2020 23:44:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 11:03:47 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Tue, 01 Sep 2020 11:04:06 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:d5517ee72007172d5b814636405254dea459120ce08f85777bb287d106a6a240`  
		Last Modified: Tue, 04 Aug 2020 07:03:41 GMT  
		Size: 49.2 MB (49175491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0283897ad4463628bd259e1cbb5eb788e7df554b42ae17fc6f5d02c4a56035c2`  
		Last Modified: Tue, 04 Aug 2020 11:23:01 GMT  
		Size: 7.7 MB (7681458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3feb40d9f5fecfa098b8f7ece6c287c6fd61b114043c8b4647359120a7d943a3`  
		Last Modified: Tue, 04 Aug 2020 11:23:02 GMT  
		Size: 10.0 MB (9983917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86b5fabb62f79acd92186da3c02d23bd8c15d79603a700959b582bd9e62854c`  
		Last Modified: Tue, 04 Aug 2020 11:23:28 GMT  
		Size: 52.2 MB (52163657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ee967f71756804b49b0fb35332bc52b41de2364092ad4c62717b9e3a5e383b`  
		Last Modified: Mon, 31 Aug 2020 23:52:53 GMT  
		Size: 183.8 MB (183788908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f3befe013d7e08e1a2f38383730ab7476092cc35afa3cd17e0ab0ad6c05f69`  
		Last Modified: Tue, 01 Sep 2020 11:05:09 GMT  
		Size: 145.6 MB (145591958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-buster` - linux; 386

```console
$ docker pull rust@sha256:e158d68ef891c1f41edd6f1bf2adafdcdb360ca98302865d6d35a8ed44236bdd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **459.6 MB (459573291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b478370ac3f9a4831eda8c07897d44711b2b6e81dda7bc8c5694f00f544dd694`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:21 GMT
ADD file:e8aac36755acd0915e9f9bae82fc8fcd0bbc3911ca4a5a40e104b2a4ebce44da in / 
# Tue, 04 Aug 2020 03:37:21 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:06:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:06:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 08:07:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Aug 2020 23:41:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 11:16:42 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Tue, 01 Sep 2020 11:17:06 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:b19305c328889ec69ec0d76e403c2cbc4603e5f27213a0e4d5f6597feefcf6e1`  
		Last Modified: Tue, 04 Aug 2020 03:42:18 GMT  
		Size: 51.2 MB (51158828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d9322a54f80129fd5cd69b7be3ac6ba44b9a0268afcbd10876508eb0f9264c`  
		Last Modified: Tue, 04 Aug 2020 08:25:50 GMT  
		Size: 8.0 MB (7981119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571a7f32100867eafa619a9265416538a2a374b88219902c6270b6f023d19061`  
		Last Modified: Tue, 04 Aug 2020 08:25:51 GMT  
		Size: 10.3 MB (10338494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3ea04987808c324433cf4b1b813ccf6528f9bf603422fbee2725c1e4018eb8`  
		Last Modified: Tue, 04 Aug 2020 08:26:25 GMT  
		Size: 53.4 MB (53433408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f5bab8ea37e9aaec5e57e6ad1fec0818250ec45b7449995899fd030ba8e2b7`  
		Last Modified: Mon, 31 Aug 2020 23:50:11 GMT  
		Size: 198.8 MB (198807590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca1ae032aa8c7efd60c9d3157f80b527ed10af124ec20b7d68b2d9af558506c`  
		Last Modified: Tue, 01 Sep 2020 11:18:29 GMT  
		Size: 137.9 MB (137853852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-slim`

```console
$ docker pull rust@sha256:f85a3e023d743567b5e50e2bc4ebb7346c9c075ba7dd9e6d80944029fbd1486c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-slim` - linux; amd64

```console
$ docker pull rust@sha256:49d07d2db02fa0841e7ed32fae4cacb9fa1ee8a04c0a94704ff63b5e1e3eb7dd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190291843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3861b3896a2d81d06bae7f5953cbaebfebf963be0ec236f9e23765813399e1eb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:25:59 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:26:23 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f015bf9c4dd2d9ed612318f06172c4f6897767bd5f1499c86f8a4aecfc7365e`  
		Last Modified: Thu, 27 Aug 2020 18:28:22 GMT  
		Size: 163.2 MB (163199722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim` - linux; arm variant v7

```console
$ docker pull rust@sha256:19524eb52c32eeeb7ed07b47b612168ab8df8b703777675fa63ef790648cfdbc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.6 MB (190554246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87cca1ed4a91bd2358018dbe889d39425ab96100e85bc14a216a1dab68294473`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:49 GMT
ADD file:16169b615697a126ae57dc01f7c4902fb9d9bc1e8595af43293700fa030808cc in / 
# Tue, 04 Aug 2020 04:56:51 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:03:24 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:04:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:d7fe0a1b85ffd3158c62ab2e06ab004dc957cd133ba7129fb9c69c4586f407c9`  
		Last Modified: Tue, 04 Aug 2020 05:05:19 GMT  
		Size: 22.7 MB (22699792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33747b5bf9abc484825c2d846a0336eebce4d644e84a492222bd96ba0bb68afd`  
		Last Modified: Thu, 27 Aug 2020 18:07:04 GMT  
		Size: 167.9 MB (167854454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:27a8acfbf882283d60faef75b1f21bc7473806e28be6c42e3cdb8ffd435a60e4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.6 MB (211636430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feaf923665d1dd9d4df676a0879afc8c240b3a1a11aa2197a4e7d82f7a26e260`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:29 GMT
ADD file:90ba7821623ab55fc1073647cc611cc45f5e306ade734910e587021971483eec in / 
# Tue, 04 Aug 2020 06:57:31 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:46:17 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:46:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:3742235f1882fee5cca1effc4ca0f0c7c180bbe169800a85daedcf3968b0d8f0`  
		Last Modified: Tue, 04 Aug 2020 07:04:03 GMT  
		Size: 25.8 MB (25849301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5562b9af59dfc44a93f04d4499240af3fd48e4b7fb7302fc1e704b62903af586`  
		Last Modified: Thu, 27 Aug 2020 18:49:12 GMT  
		Size: 185.8 MB (185787129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim` - linux; 386

```console
$ docker pull rust@sha256:075ed84cdfefb54e0059ff9d0dd93064c4843decedaf92314e53c392926d6358
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.6 MB (215582587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f7770bf7c551767284e71e7bf5dc9768cface5153f77dcc8e36dfadffdc1759`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:35 GMT
ADD file:cc791c21e6022a12dd1445a35f4cca9392ad8edfe34ea5852f3e87862c943628 in / 
# Tue, 04 Aug 2020 03:37:35 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:41:02 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:41:35 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:23ad22c16ab9d635a179d5d341096c34912941507b0c77ac97083b9795d8516f`  
		Last Modified: Tue, 04 Aug 2020 03:42:33 GMT  
		Size: 27.8 MB (27750435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9c10f6e7a2a850ab44763fa49cb09d7f46f4a741cab45df2e767d541b0ebc0`  
		Last Modified: Thu, 27 Aug 2020 18:43:30 GMT  
		Size: 187.8 MB (187832152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-slim-buster`

```console
$ docker pull rust@sha256:f85a3e023d743567b5e50e2bc4ebb7346c9c075ba7dd9e6d80944029fbd1486c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-slim-buster` - linux; amd64

```console
$ docker pull rust@sha256:49d07d2db02fa0841e7ed32fae4cacb9fa1ee8a04c0a94704ff63b5e1e3eb7dd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190291843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3861b3896a2d81d06bae7f5953cbaebfebf963be0ec236f9e23765813399e1eb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:25:59 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:26:23 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f015bf9c4dd2d9ed612318f06172c4f6897767bd5f1499c86f8a4aecfc7365e`  
		Last Modified: Thu, 27 Aug 2020 18:28:22 GMT  
		Size: 163.2 MB (163199722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:19524eb52c32eeeb7ed07b47b612168ab8df8b703777675fa63ef790648cfdbc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.6 MB (190554246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87cca1ed4a91bd2358018dbe889d39425ab96100e85bc14a216a1dab68294473`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:49 GMT
ADD file:16169b615697a126ae57dc01f7c4902fb9d9bc1e8595af43293700fa030808cc in / 
# Tue, 04 Aug 2020 04:56:51 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:03:24 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:04:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:d7fe0a1b85ffd3158c62ab2e06ab004dc957cd133ba7129fb9c69c4586f407c9`  
		Last Modified: Tue, 04 Aug 2020 05:05:19 GMT  
		Size: 22.7 MB (22699792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33747b5bf9abc484825c2d846a0336eebce4d644e84a492222bd96ba0bb68afd`  
		Last Modified: Thu, 27 Aug 2020 18:07:04 GMT  
		Size: 167.9 MB (167854454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:27a8acfbf882283d60faef75b1f21bc7473806e28be6c42e3cdb8ffd435a60e4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.6 MB (211636430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feaf923665d1dd9d4df676a0879afc8c240b3a1a11aa2197a4e7d82f7a26e260`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:29 GMT
ADD file:90ba7821623ab55fc1073647cc611cc45f5e306ade734910e587021971483eec in / 
# Tue, 04 Aug 2020 06:57:31 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:46:17 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:46:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:3742235f1882fee5cca1effc4ca0f0c7c180bbe169800a85daedcf3968b0d8f0`  
		Last Modified: Tue, 04 Aug 2020 07:04:03 GMT  
		Size: 25.8 MB (25849301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5562b9af59dfc44a93f04d4499240af3fd48e4b7fb7302fc1e704b62903af586`  
		Last Modified: Thu, 27 Aug 2020 18:49:12 GMT  
		Size: 185.8 MB (185787129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-buster` - linux; 386

```console
$ docker pull rust@sha256:075ed84cdfefb54e0059ff9d0dd93064c4843decedaf92314e53c392926d6358
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.6 MB (215582587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f7770bf7c551767284e71e7bf5dc9768cface5153f77dcc8e36dfadffdc1759`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:35 GMT
ADD file:cc791c21e6022a12dd1445a35f4cca9392ad8edfe34ea5852f3e87862c943628 in / 
# Tue, 04 Aug 2020 03:37:35 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:41:02 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:41:35 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:23ad22c16ab9d635a179d5d341096c34912941507b0c77ac97083b9795d8516f`  
		Last Modified: Tue, 04 Aug 2020 03:42:33 GMT  
		Size: 27.8 MB (27750435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9c10f6e7a2a850ab44763fa49cb09d7f46f4a741cab45df2e767d541b0ebc0`  
		Last Modified: Thu, 27 Aug 2020 18:43:30 GMT  
		Size: 187.8 MB (187832152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:alpine`

```console
$ docker pull rust@sha256:c9890db1527309a88994b12dfe5e1ed695518037367ffb74df76a66bfc303ef5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:alpine` - linux; amd64

```console
$ docker pull rust@sha256:bf15122548d85a37667751cc13e1da6b1e1c288ef6d57449afaf79c796d77978
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.9 MB (193940545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16c57101cc99b4a5a3f817eebfcf782de4bd0717944f26b383c0e31090e9914c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 18 Jun 2020 19:22:19 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 27 Aug 2020 18:26:51 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:27:11 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.22.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "cee31c6f72b953c6293fd5d40142c7d61aa85db2a5ea81b3519fe1b492148dc9 *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host x86_64-unknown-linux-musl;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
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
	-	`sha256:4947720ce5d0f6bf41c2d45682cf4aa8e55d9eb1ada4dfda806dedaac31228f3`  
		Last Modified: Thu, 27 Aug 2020 18:29:23 GMT  
		Size: 143.5 MB (143530073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:alpine3.11`

```console
$ docker pull rust@sha256:644c097a0703d567bcc2e72a9f26affa172cd2be74c0d0bebcd2eb1b45f66298
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:alpine3.11` - linux; amd64

```console
$ docker pull rust@sha256:99596dc88c80ea5984c233f8a6057d25724aaa20b883b58e32648067f4d4d310
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.8 MB (182760067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fab160737bb14788a092fd07ff755de0b51caa67cbbd8581428630a8f8f695d3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:43:51 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 27 Aug 2020 18:26:29 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:26:45 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.22.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "cee31c6f72b953c6293fd5d40142c7d61aa85db2a5ea81b3519fe1b492148dc9 *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host x86_64-unknown-linux-musl;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
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
	-	`sha256:a012b535c7038638f5e2bcb45e46b32b06010197931db0037bb5169b92849b79`  
		Last Modified: Thu, 27 Aug 2020 18:28:55 GMT  
		Size: 143.5 MB (143530108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:alpine3.12`

```console
$ docker pull rust@sha256:c9890db1527309a88994b12dfe5e1ed695518037367ffb74df76a66bfc303ef5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:alpine3.12` - linux; amd64

```console
$ docker pull rust@sha256:bf15122548d85a37667751cc13e1da6b1e1c288ef6d57449afaf79c796d77978
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.9 MB (193940545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16c57101cc99b4a5a3f817eebfcf782de4bd0717944f26b383c0e31090e9914c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 18 Jun 2020 19:22:19 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 27 Aug 2020 18:26:51 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:27:11 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.22.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "cee31c6f72b953c6293fd5d40142c7d61aa85db2a5ea81b3519fe1b492148dc9 *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host x86_64-unknown-linux-musl;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
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
	-	`sha256:4947720ce5d0f6bf41c2d45682cf4aa8e55d9eb1ada4dfda806dedaac31228f3`  
		Last Modified: Thu, 27 Aug 2020 18:29:23 GMT  
		Size: 143.5 MB (143530073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:buster`

```console
$ docker pull rust@sha256:32110fb328d3c3280f06f10c8efcdb1c31fe12057e01a24668c64bf9c419ab56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:buster` - linux; amd64

```console
$ docker pull rust@sha256:2c7564a1e4f3223d11bd061cb46b485e57bbfa921821cf857184e64ffc4274e7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **430.1 MB (430091356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc1c343b9048272e2bca499029570351dc36b2e28792661a50d3113d94ca577`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:33 GMT
ADD file:4b03b5f551e3fbdf47ec609712007327828f7530cc3455c43bbcdcaf449a75a9 in / 
# Tue, 04 Aug 2020 15:42:34 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:26:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:26:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 23:26:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:27:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Aug 2020 18:25:43 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:25:55 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:d6ff36c9ec4822c9ff8953560f7ba41653b348a9c1136755e653575f58fbded7`  
		Last Modified: Tue, 04 Aug 2020 15:48:55 GMT  
		Size: 50.4 MB (50396000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c958d65b3090aefea91284d018b2a86530a3c8174b72616c4e76993c696a5797`  
		Last Modified: Tue, 04 Aug 2020 23:39:28 GMT  
		Size: 7.8 MB (7811570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edaf0a6b092f5673ec05b40edb606ce58881b2f40494251117d31805225ef064`  
		Last Modified: Tue, 04 Aug 2020 23:39:27 GMT  
		Size: 10.0 MB (9996337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80931cf6881673fd161a3fd73e8971fe4a569fd7fbb44e956d261ca58d97dfab`  
		Last Modified: Tue, 04 Aug 2020 23:39:45 GMT  
		Size: 51.8 MB (51829826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1b8aca3825e6c3b57e28c8075180f97879161dd58333de13f6b6da0f842af3`  
		Last Modified: Tue, 04 Aug 2020 23:40:24 GMT  
		Size: 192.2 MB (192243499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119498f32df8c0465d687487ca4344eee7ce0c46f80306ea7a34e1c01ff3b461`  
		Last Modified: Thu, 27 Aug 2020 18:27:47 GMT  
		Size: 117.8 MB (117814124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:955a1c50eaa60d2317a3c758f2b3a37279dae2dee22504db1435766e394d5aa2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.1 MB (413120940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d13b78091ac4db478dc13e5a884c6ca2f05145626411e48050a629300d82f95`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:26 GMT
ADD file:aaf5c6340b3d662631775fa4536c2e48e9f68b6cc8d53e18fb8fd76ae41b305e in / 
# Tue, 04 Aug 2020 04:56:28 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:52:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 07:53:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 07:54:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 00:07:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 13:46:49 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Tue, 01 Sep 2020 13:47:14 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:e7cf402ee4b1ba67e92813d50297a082bbdbdd4d47f6aeb62f2316b81d5dc843`  
		Last Modified: Tue, 04 Aug 2020 05:04:56 GMT  
		Size: 45.9 MB (45869261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff6bd4a89fc21d80ca6924320f86708f35ddea71c7aa34a408a5b64257c764e`  
		Last Modified: Tue, 04 Aug 2020 08:25:56 GMT  
		Size: 7.1 MB (7097820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48f5852a753b7731e5d374567ae9b64e309805758f336c76d5f13bb67c94e20`  
		Last Modified: Tue, 04 Aug 2020 08:25:56 GMT  
		Size: 9.3 MB (9343353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58a93b33dd4d533cc1e04eab8045940d69cb287134aa90c982e3d248739044e`  
		Last Modified: Tue, 04 Aug 2020 08:26:25 GMT  
		Size: 47.4 MB (47355829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06127c17626f8d326b4f2e347e5a9704709941e8a54307a18eda808550446f4`  
		Last Modified: Tue, 01 Sep 2020 00:34:27 GMT  
		Size: 168.5 MB (168488015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567b372ca3cbd9ece4bae988da44aa8716a5eefcb84de9eaf3b962c9beea3c19`  
		Last Modified: Tue, 01 Sep 2020 13:48:25 GMT  
		Size: 135.0 MB (134966662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:56f26196d5917a7f3eb5a0959b42784b77f15325548635789d860d2a7df41958
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.4 MB (448385389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a94406c21898c4d41dc168a007bb4ada2fb5067d3d0ac2ad9487149498cc6855`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:06 GMT
ADD file:ce999027b153d392f8a0f85e2e7a17b9279f3cf7ad0e45192378d527275f99c6 in / 
# Tue, 04 Aug 2020 06:57:08 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 11:10:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 11:10:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 11:10:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Aug 2020 23:44:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 11:03:47 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Tue, 01 Sep 2020 11:04:06 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:d5517ee72007172d5b814636405254dea459120ce08f85777bb287d106a6a240`  
		Last Modified: Tue, 04 Aug 2020 07:03:41 GMT  
		Size: 49.2 MB (49175491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0283897ad4463628bd259e1cbb5eb788e7df554b42ae17fc6f5d02c4a56035c2`  
		Last Modified: Tue, 04 Aug 2020 11:23:01 GMT  
		Size: 7.7 MB (7681458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3feb40d9f5fecfa098b8f7ece6c287c6fd61b114043c8b4647359120a7d943a3`  
		Last Modified: Tue, 04 Aug 2020 11:23:02 GMT  
		Size: 10.0 MB (9983917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86b5fabb62f79acd92186da3c02d23bd8c15d79603a700959b582bd9e62854c`  
		Last Modified: Tue, 04 Aug 2020 11:23:28 GMT  
		Size: 52.2 MB (52163657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ee967f71756804b49b0fb35332bc52b41de2364092ad4c62717b9e3a5e383b`  
		Last Modified: Mon, 31 Aug 2020 23:52:53 GMT  
		Size: 183.8 MB (183788908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f3befe013d7e08e1a2f38383730ab7476092cc35afa3cd17e0ab0ad6c05f69`  
		Last Modified: Tue, 01 Sep 2020 11:05:09 GMT  
		Size: 145.6 MB (145591958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:buster` - linux; 386

```console
$ docker pull rust@sha256:e158d68ef891c1f41edd6f1bf2adafdcdb360ca98302865d6d35a8ed44236bdd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **459.6 MB (459573291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b478370ac3f9a4831eda8c07897d44711b2b6e81dda7bc8c5694f00f544dd694`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:21 GMT
ADD file:e8aac36755acd0915e9f9bae82fc8fcd0bbc3911ca4a5a40e104b2a4ebce44da in / 
# Tue, 04 Aug 2020 03:37:21 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:06:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:06:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 08:07:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Aug 2020 23:41:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 11:16:42 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Tue, 01 Sep 2020 11:17:06 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:b19305c328889ec69ec0d76e403c2cbc4603e5f27213a0e4d5f6597feefcf6e1`  
		Last Modified: Tue, 04 Aug 2020 03:42:18 GMT  
		Size: 51.2 MB (51158828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d9322a54f80129fd5cd69b7be3ac6ba44b9a0268afcbd10876508eb0f9264c`  
		Last Modified: Tue, 04 Aug 2020 08:25:50 GMT  
		Size: 8.0 MB (7981119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571a7f32100867eafa619a9265416538a2a374b88219902c6270b6f023d19061`  
		Last Modified: Tue, 04 Aug 2020 08:25:51 GMT  
		Size: 10.3 MB (10338494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3ea04987808c324433cf4b1b813ccf6528f9bf603422fbee2725c1e4018eb8`  
		Last Modified: Tue, 04 Aug 2020 08:26:25 GMT  
		Size: 53.4 MB (53433408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f5bab8ea37e9aaec5e57e6ad1fec0818250ec45b7449995899fd030ba8e2b7`  
		Last Modified: Mon, 31 Aug 2020 23:50:11 GMT  
		Size: 198.8 MB (198807590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca1ae032aa8c7efd60c9d3157f80b527ed10af124ec20b7d68b2d9af558506c`  
		Last Modified: Tue, 01 Sep 2020 11:18:29 GMT  
		Size: 137.9 MB (137853852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:latest`

```console
$ docker pull rust@sha256:32110fb328d3c3280f06f10c8efcdb1c31fe12057e01a24668c64bf9c419ab56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:latest` - linux; amd64

```console
$ docker pull rust@sha256:2c7564a1e4f3223d11bd061cb46b485e57bbfa921821cf857184e64ffc4274e7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **430.1 MB (430091356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc1c343b9048272e2bca499029570351dc36b2e28792661a50d3113d94ca577`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:33 GMT
ADD file:4b03b5f551e3fbdf47ec609712007327828f7530cc3455c43bbcdcaf449a75a9 in / 
# Tue, 04 Aug 2020 15:42:34 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:26:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:26:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 23:26:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:27:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Aug 2020 18:25:43 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:25:55 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:d6ff36c9ec4822c9ff8953560f7ba41653b348a9c1136755e653575f58fbded7`  
		Last Modified: Tue, 04 Aug 2020 15:48:55 GMT  
		Size: 50.4 MB (50396000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c958d65b3090aefea91284d018b2a86530a3c8174b72616c4e76993c696a5797`  
		Last Modified: Tue, 04 Aug 2020 23:39:28 GMT  
		Size: 7.8 MB (7811570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edaf0a6b092f5673ec05b40edb606ce58881b2f40494251117d31805225ef064`  
		Last Modified: Tue, 04 Aug 2020 23:39:27 GMT  
		Size: 10.0 MB (9996337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80931cf6881673fd161a3fd73e8971fe4a569fd7fbb44e956d261ca58d97dfab`  
		Last Modified: Tue, 04 Aug 2020 23:39:45 GMT  
		Size: 51.8 MB (51829826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1b8aca3825e6c3b57e28c8075180f97879161dd58333de13f6b6da0f842af3`  
		Last Modified: Tue, 04 Aug 2020 23:40:24 GMT  
		Size: 192.2 MB (192243499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119498f32df8c0465d687487ca4344eee7ce0c46f80306ea7a34e1c01ff3b461`  
		Last Modified: Thu, 27 Aug 2020 18:27:47 GMT  
		Size: 117.8 MB (117814124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:latest` - linux; arm variant v7

```console
$ docker pull rust@sha256:955a1c50eaa60d2317a3c758f2b3a37279dae2dee22504db1435766e394d5aa2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.1 MB (413120940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d13b78091ac4db478dc13e5a884c6ca2f05145626411e48050a629300d82f95`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:26 GMT
ADD file:aaf5c6340b3d662631775fa4536c2e48e9f68b6cc8d53e18fb8fd76ae41b305e in / 
# Tue, 04 Aug 2020 04:56:28 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:52:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 07:53:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 07:54:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 00:07:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 13:46:49 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Tue, 01 Sep 2020 13:47:14 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:e7cf402ee4b1ba67e92813d50297a082bbdbdd4d47f6aeb62f2316b81d5dc843`  
		Last Modified: Tue, 04 Aug 2020 05:04:56 GMT  
		Size: 45.9 MB (45869261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff6bd4a89fc21d80ca6924320f86708f35ddea71c7aa34a408a5b64257c764e`  
		Last Modified: Tue, 04 Aug 2020 08:25:56 GMT  
		Size: 7.1 MB (7097820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48f5852a753b7731e5d374567ae9b64e309805758f336c76d5f13bb67c94e20`  
		Last Modified: Tue, 04 Aug 2020 08:25:56 GMT  
		Size: 9.3 MB (9343353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58a93b33dd4d533cc1e04eab8045940d69cb287134aa90c982e3d248739044e`  
		Last Modified: Tue, 04 Aug 2020 08:26:25 GMT  
		Size: 47.4 MB (47355829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06127c17626f8d326b4f2e347e5a9704709941e8a54307a18eda808550446f4`  
		Last Modified: Tue, 01 Sep 2020 00:34:27 GMT  
		Size: 168.5 MB (168488015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567b372ca3cbd9ece4bae988da44aa8716a5eefcb84de9eaf3b962c9beea3c19`  
		Last Modified: Tue, 01 Sep 2020 13:48:25 GMT  
		Size: 135.0 MB (134966662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:latest` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:56f26196d5917a7f3eb5a0959b42784b77f15325548635789d860d2a7df41958
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.4 MB (448385389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a94406c21898c4d41dc168a007bb4ada2fb5067d3d0ac2ad9487149498cc6855`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:06 GMT
ADD file:ce999027b153d392f8a0f85e2e7a17b9279f3cf7ad0e45192378d527275f99c6 in / 
# Tue, 04 Aug 2020 06:57:08 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 11:10:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 11:10:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 11:10:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Aug 2020 23:44:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 11:03:47 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Tue, 01 Sep 2020 11:04:06 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:d5517ee72007172d5b814636405254dea459120ce08f85777bb287d106a6a240`  
		Last Modified: Tue, 04 Aug 2020 07:03:41 GMT  
		Size: 49.2 MB (49175491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0283897ad4463628bd259e1cbb5eb788e7df554b42ae17fc6f5d02c4a56035c2`  
		Last Modified: Tue, 04 Aug 2020 11:23:01 GMT  
		Size: 7.7 MB (7681458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3feb40d9f5fecfa098b8f7ece6c287c6fd61b114043c8b4647359120a7d943a3`  
		Last Modified: Tue, 04 Aug 2020 11:23:02 GMT  
		Size: 10.0 MB (9983917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86b5fabb62f79acd92186da3c02d23bd8c15d79603a700959b582bd9e62854c`  
		Last Modified: Tue, 04 Aug 2020 11:23:28 GMT  
		Size: 52.2 MB (52163657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ee967f71756804b49b0fb35332bc52b41de2364092ad4c62717b9e3a5e383b`  
		Last Modified: Mon, 31 Aug 2020 23:52:53 GMT  
		Size: 183.8 MB (183788908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f3befe013d7e08e1a2f38383730ab7476092cc35afa3cd17e0ab0ad6c05f69`  
		Last Modified: Tue, 01 Sep 2020 11:05:09 GMT  
		Size: 145.6 MB (145591958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:latest` - linux; 386

```console
$ docker pull rust@sha256:e158d68ef891c1f41edd6f1bf2adafdcdb360ca98302865d6d35a8ed44236bdd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **459.6 MB (459573291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b478370ac3f9a4831eda8c07897d44711b2b6e81dda7bc8c5694f00f544dd694`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:21 GMT
ADD file:e8aac36755acd0915e9f9bae82fc8fcd0bbc3911ca4a5a40e104b2a4ebce44da in / 
# Tue, 04 Aug 2020 03:37:21 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:06:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:06:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 08:07:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Aug 2020 23:41:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 11:16:42 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Tue, 01 Sep 2020 11:17:06 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:b19305c328889ec69ec0d76e403c2cbc4603e5f27213a0e4d5f6597feefcf6e1`  
		Last Modified: Tue, 04 Aug 2020 03:42:18 GMT  
		Size: 51.2 MB (51158828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d9322a54f80129fd5cd69b7be3ac6ba44b9a0268afcbd10876508eb0f9264c`  
		Last Modified: Tue, 04 Aug 2020 08:25:50 GMT  
		Size: 8.0 MB (7981119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571a7f32100867eafa619a9265416538a2a374b88219902c6270b6f023d19061`  
		Last Modified: Tue, 04 Aug 2020 08:25:51 GMT  
		Size: 10.3 MB (10338494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3ea04987808c324433cf4b1b813ccf6528f9bf603422fbee2725c1e4018eb8`  
		Last Modified: Tue, 04 Aug 2020 08:26:25 GMT  
		Size: 53.4 MB (53433408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f5bab8ea37e9aaec5e57e6ad1fec0818250ec45b7449995899fd030ba8e2b7`  
		Last Modified: Mon, 31 Aug 2020 23:50:11 GMT  
		Size: 198.8 MB (198807590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca1ae032aa8c7efd60c9d3157f80b527ed10af124ec20b7d68b2d9af558506c`  
		Last Modified: Tue, 01 Sep 2020 11:18:29 GMT  
		Size: 137.9 MB (137853852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:slim`

```console
$ docker pull rust@sha256:f85a3e023d743567b5e50e2bc4ebb7346c9c075ba7dd9e6d80944029fbd1486c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:slim` - linux; amd64

```console
$ docker pull rust@sha256:49d07d2db02fa0841e7ed32fae4cacb9fa1ee8a04c0a94704ff63b5e1e3eb7dd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190291843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3861b3896a2d81d06bae7f5953cbaebfebf963be0ec236f9e23765813399e1eb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:25:59 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:26:23 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f015bf9c4dd2d9ed612318f06172c4f6897767bd5f1499c86f8a4aecfc7365e`  
		Last Modified: Thu, 27 Aug 2020 18:28:22 GMT  
		Size: 163.2 MB (163199722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim` - linux; arm variant v7

```console
$ docker pull rust@sha256:19524eb52c32eeeb7ed07b47b612168ab8df8b703777675fa63ef790648cfdbc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.6 MB (190554246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87cca1ed4a91bd2358018dbe889d39425ab96100e85bc14a216a1dab68294473`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:49 GMT
ADD file:16169b615697a126ae57dc01f7c4902fb9d9bc1e8595af43293700fa030808cc in / 
# Tue, 04 Aug 2020 04:56:51 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:03:24 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:04:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:d7fe0a1b85ffd3158c62ab2e06ab004dc957cd133ba7129fb9c69c4586f407c9`  
		Last Modified: Tue, 04 Aug 2020 05:05:19 GMT  
		Size: 22.7 MB (22699792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33747b5bf9abc484825c2d846a0336eebce4d644e84a492222bd96ba0bb68afd`  
		Last Modified: Thu, 27 Aug 2020 18:07:04 GMT  
		Size: 167.9 MB (167854454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:27a8acfbf882283d60faef75b1f21bc7473806e28be6c42e3cdb8ffd435a60e4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.6 MB (211636430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feaf923665d1dd9d4df676a0879afc8c240b3a1a11aa2197a4e7d82f7a26e260`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:29 GMT
ADD file:90ba7821623ab55fc1073647cc611cc45f5e306ade734910e587021971483eec in / 
# Tue, 04 Aug 2020 06:57:31 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:46:17 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:46:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:3742235f1882fee5cca1effc4ca0f0c7c180bbe169800a85daedcf3968b0d8f0`  
		Last Modified: Tue, 04 Aug 2020 07:04:03 GMT  
		Size: 25.8 MB (25849301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5562b9af59dfc44a93f04d4499240af3fd48e4b7fb7302fc1e704b62903af586`  
		Last Modified: Thu, 27 Aug 2020 18:49:12 GMT  
		Size: 185.8 MB (185787129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim` - linux; 386

```console
$ docker pull rust@sha256:075ed84cdfefb54e0059ff9d0dd93064c4843decedaf92314e53c392926d6358
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.6 MB (215582587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f7770bf7c551767284e71e7bf5dc9768cface5153f77dcc8e36dfadffdc1759`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:35 GMT
ADD file:cc791c21e6022a12dd1445a35f4cca9392ad8edfe34ea5852f3e87862c943628 in / 
# Tue, 04 Aug 2020 03:37:35 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:41:02 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:41:35 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:23ad22c16ab9d635a179d5d341096c34912941507b0c77ac97083b9795d8516f`  
		Last Modified: Tue, 04 Aug 2020 03:42:33 GMT  
		Size: 27.8 MB (27750435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9c10f6e7a2a850ab44763fa49cb09d7f46f4a741cab45df2e767d541b0ebc0`  
		Last Modified: Thu, 27 Aug 2020 18:43:30 GMT  
		Size: 187.8 MB (187832152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:slim-buster`

```console
$ docker pull rust@sha256:f85a3e023d743567b5e50e2bc4ebb7346c9c075ba7dd9e6d80944029fbd1486c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:slim-buster` - linux; amd64

```console
$ docker pull rust@sha256:49d07d2db02fa0841e7ed32fae4cacb9fa1ee8a04c0a94704ff63b5e1e3eb7dd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190291843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3861b3896a2d81d06bae7f5953cbaebfebf963be0ec236f9e23765813399e1eb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:25:59 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:26:23 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f015bf9c4dd2d9ed612318f06172c4f6897767bd5f1499c86f8a4aecfc7365e`  
		Last Modified: Thu, 27 Aug 2020 18:28:22 GMT  
		Size: 163.2 MB (163199722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:19524eb52c32eeeb7ed07b47b612168ab8df8b703777675fa63ef790648cfdbc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.6 MB (190554246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87cca1ed4a91bd2358018dbe889d39425ab96100e85bc14a216a1dab68294473`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:56:49 GMT
ADD file:16169b615697a126ae57dc01f7c4902fb9d9bc1e8595af43293700fa030808cc in / 
# Tue, 04 Aug 2020 04:56:51 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:03:24 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:04:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:d7fe0a1b85ffd3158c62ab2e06ab004dc957cd133ba7129fb9c69c4586f407c9`  
		Last Modified: Tue, 04 Aug 2020 05:05:19 GMT  
		Size: 22.7 MB (22699792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33747b5bf9abc484825c2d846a0336eebce4d644e84a492222bd96ba0bb68afd`  
		Last Modified: Thu, 27 Aug 2020 18:07:04 GMT  
		Size: 167.9 MB (167854454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:27a8acfbf882283d60faef75b1f21bc7473806e28be6c42e3cdb8ffd435a60e4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.6 MB (211636430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feaf923665d1dd9d4df676a0879afc8c240b3a1a11aa2197a4e7d82f7a26e260`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:29 GMT
ADD file:90ba7821623ab55fc1073647cc611cc45f5e306ade734910e587021971483eec in / 
# Tue, 04 Aug 2020 06:57:31 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:46:17 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:46:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:3742235f1882fee5cca1effc4ca0f0c7c180bbe169800a85daedcf3968b0d8f0`  
		Last Modified: Tue, 04 Aug 2020 07:04:03 GMT  
		Size: 25.8 MB (25849301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5562b9af59dfc44a93f04d4499240af3fd48e4b7fb7302fc1e704b62903af586`  
		Last Modified: Thu, 27 Aug 2020 18:49:12 GMT  
		Size: 185.8 MB (185787129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-buster` - linux; 386

```console
$ docker pull rust@sha256:075ed84cdfefb54e0059ff9d0dd93064c4843decedaf92314e53c392926d6358
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.6 MB (215582587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f7770bf7c551767284e71e7bf5dc9768cface5153f77dcc8e36dfadffdc1759`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:35 GMT
ADD file:cc791c21e6022a12dd1445a35f4cca9392ad8edfe34ea5852f3e87862c943628 in / 
# Tue, 04 Aug 2020 03:37:35 GMT
CMD ["bash"]
# Thu, 27 Aug 2020 18:41:02 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.46.0
# Thu, 27 Aug 2020 18:41:35 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='49c96f3f74be82f4752b8bffcf81961dea5e6e94ce1ccba94435f12e871c3bdb' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='5a2be2919319e8778698fa9998002d1ec720efe7cb4f6ee4affb006b5e73f1be' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='d93ef6f91dab8299f46eef26a56c2d97c66271cea60bf004f2f088a86a697078' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e3d0ae3cfce5c6941f74fed61ca83e53d4cd2deb431b906cbd0687f246efede4' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.22.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:23ad22c16ab9d635a179d5d341096c34912941507b0c77ac97083b9795d8516f`  
		Last Modified: Tue, 04 Aug 2020 03:42:33 GMT  
		Size: 27.8 MB (27750435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9c10f6e7a2a850ab44763fa49cb09d7f46f4a741cab45df2e767d541b0ebc0`  
		Last Modified: Thu, 27 Aug 2020 18:43:30 GMT  
		Size: 187.8 MB (187832152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
