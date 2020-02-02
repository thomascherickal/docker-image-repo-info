<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `rust`

-	[`rust:1`](#rust1)
-	[`rust:1.41`](#rust141)
-	[`rust:1.41.0`](#rust1410)
-	[`rust:1.41.0-alpine`](#rust1410-alpine)
-	[`rust:1.41.0-alpine3.10`](#rust1410-alpine310)
-	[`rust:1.41.0-alpine3.11`](#rust1410-alpine311)
-	[`rust:1.41.0-buster`](#rust1410-buster)
-	[`rust:1.41.0-slim`](#rust1410-slim)
-	[`rust:1.41.0-slim-buster`](#rust1410-slim-buster)
-	[`rust:1.41.0-slim-stretch`](#rust1410-slim-stretch)
-	[`rust:1.41.0-stretch`](#rust1410-stretch)
-	[`rust:1.41-alpine`](#rust141-alpine)
-	[`rust:1.41-alpine3.10`](#rust141-alpine310)
-	[`rust:1.41-alpine3.11`](#rust141-alpine311)
-	[`rust:1.41-buster`](#rust141-buster)
-	[`rust:1.41-slim`](#rust141-slim)
-	[`rust:1.41-slim-buster`](#rust141-slim-buster)
-	[`rust:1.41-slim-stretch`](#rust141-slim-stretch)
-	[`rust:1.41-stretch`](#rust141-stretch)
-	[`rust:1-alpine`](#rust1-alpine)
-	[`rust:1-alpine3.10`](#rust1-alpine310)
-	[`rust:1-alpine3.11`](#rust1-alpine311)
-	[`rust:1-buster`](#rust1-buster)
-	[`rust:1-slim`](#rust1-slim)
-	[`rust:1-slim-buster`](#rust1-slim-buster)
-	[`rust:1-slim-stretch`](#rust1-slim-stretch)
-	[`rust:1-stretch`](#rust1-stretch)
-	[`rust:alpine`](#rustalpine)
-	[`rust:alpine3.10`](#rustalpine310)
-	[`rust:alpine3.11`](#rustalpine311)
-	[`rust:buster`](#rustbuster)
-	[`rust:latest`](#rustlatest)
-	[`rust:slim`](#rustslim)
-	[`rust:slim-buster`](#rustslim-buster)
-	[`rust:slim-stretch`](#rustslim-stretch)
-	[`rust:stretch`](#ruststretch)

## `rust:1`

```console
$ docker pull rust@sha256:920b5c1b275778169a8c35f767c9c238ac9391f8a666d3ee159a1a2a26088a25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1` - linux; amd64

```console
$ docker pull rust@sha256:d59df245b22bfef90c2d29c1691e6a3ff679feb95d400b69626bae74898efab3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.7 MB (441693460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db33159e3388e178392ca314fbd8ecebb9fb430b73a29538302486e29cec6bc1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:08 GMT
ADD file:d6d0bdf8cb07a7a0dc32e9df50ac80ca1a524c3fa48136892ded195061f2194c in / 
# Sat, 28 Dec 2019 04:21:09 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:47:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:47:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 04:47:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:48:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Jan 2020 23:58:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:58:35 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:8f0fdd3eaac017684c880d836abdaf02f9db7ac8ecca970356482e3d8e315650`  
		Last Modified: Sat, 28 Dec 2019 04:25:39 GMT  
		Size: 50.4 MB (50379720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d918eaefd9de8a1595f56900fdb8ab65a03d64b1da1078da7c0b0bf6f7552a14`  
		Last Modified: Sat, 28 Dec 2019 05:01:44 GMT  
		Size: 7.8 MB (7811715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bf3e3107f525b7dea5b3cdfd15f62666066202105a0aaddbab2a02aefad1f7`  
		Last Modified: Sat, 28 Dec 2019 05:01:44 GMT  
		Size: 10.0 MB (9996202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27622921edb2aae9e0cb64f71a81b4a7cfef8f6a6c766514a018815834ba4e14`  
		Last Modified: Sat, 28 Dec 2019 05:02:00 GMT  
		Size: 51.8 MB (51790562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfa0aa1ae2c54d0de4b6ad0ee4d9f795c93368ae7d87801784c1f8ae624ac33`  
		Last Modified: Sat, 28 Dec 2019 05:02:36 GMT  
		Size: 192.0 MB (192044395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b109c91c0639fd55a93a5688b1bc7501e434396daabd93d714b72b106996a82a`  
		Last Modified: Fri, 31 Jan 2020 00:01:48 GMT  
		Size: 129.7 MB (129670866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1` - linux; arm variant v7

```console
$ docker pull rust@sha256:f4b13a8a2df73cfd225ce928f3574e1169b288e8448e004659d35d303ba1b82f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **420.0 MB (420018522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af6c4b7927d04a1c76f6b24226aa2702d2a7de368154e22aa531e7e986d7c227`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:06 GMT
ADD file:a57a312731f174c4b03031908ff95f49d7055d8c196439f0ed07ed9c4834d993 in / 
# Sat, 01 Feb 2020 17:00:08 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:00:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 18:01:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:03:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 03:16:56 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 03:17:21 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9bbb41bca8c6254da5088d03354297b1309dc75c2ccc738416025f89709ae5ee`  
		Last Modified: Sat, 01 Feb 2020 17:07:28 GMT  
		Size: 45.9 MB (45859700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239e4acdbc2ab88c89aa359fbab11429ea6d7bd93ea589a22c6bbb833ff82b93`  
		Last Modified: Sat, 01 Feb 2020 18:25:50 GMT  
		Size: 7.1 MB (7096223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6b4707a3c3aff9cb939fc058b869c5412e78c37e43eb0b653565460495537`  
		Last Modified: Sat, 01 Feb 2020 18:25:50 GMT  
		Size: 9.3 MB (9343278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e096c4fc8c629edca6da3ce5a9e95288512cb11e3d3d01a6e49078d19c2acca`  
		Last Modified: Sat, 01 Feb 2020 18:26:13 GMT  
		Size: 47.3 MB (47315591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6953ecf4273071529462518748f048f49a05530ae24d8fc6841919de312f2fc`  
		Last Modified: Sat, 01 Feb 2020 18:27:03 GMT  
		Size: 168.4 MB (168379144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f84f54aa922c34c20237ad8b624417ee33ea2f0c7940b127d3043d241b53bd`  
		Last Modified: Sun, 02 Feb 2020 03:21:00 GMT  
		Size: 142.0 MB (142024586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:cc4933ffae4311c25299ae5b6a8e115241533bed5ca5e71dd7df717e0ca3b760
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.5 MB (441531085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:779e2f51436aa1328b240e1b38f7b6758d6acb69f2a4eae5f652148e28a16a8e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:40:41 GMT
ADD file:88b3d02fc98aa9138e694bee7d5d1b61b295e4a1c7fae399bf24e52eeff7a5ae in / 
# Sat, 28 Dec 2019 04:40:45 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:04:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:05:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:05:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:08:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Jan 2020 23:45:22 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:45:39 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:627706d65d1d9b4038d8fd40db52238d4f11d9130a01f23ffae9bf5d41ac5933`  
		Last Modified: Sat, 28 Dec 2019 04:46:38 GMT  
		Size: 49.2 MB (49171876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ac1923ab7a97ecdde2a4f034a8b716d51594ba6fc823c6aaac579c31f51906`  
		Last Modified: Sat, 28 Dec 2019 06:21:16 GMT  
		Size: 7.7 MB (7681148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b000e01546d5b9b3a40a3797f15bc0a1f579786c5ec8da31cbe9502f1927d367`  
		Last Modified: Sat, 28 Dec 2019 06:21:16 GMT  
		Size: 10.0 MB (9983835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8fe6ebd465d85dc79039fbd39712f1fadf5d7ac5fbefe405ef7a4f957a94ce`  
		Last Modified: Sat, 28 Dec 2019 06:21:39 GMT  
		Size: 52.1 MB (52102816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d739211b59b4a5cab55db8d8ce73eb5edfb9d5d91addf9f7aab0b9d9fa90b06`  
		Last Modified: Sat, 28 Dec 2019 06:22:32 GMT  
		Size: 183.6 MB (183566016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cff33cb79d34d36837bc747d7bd54401995ea5a541d92619b14c3ab0c8e2eb`  
		Last Modified: Thu, 30 Jan 2020 23:48:59 GMT  
		Size: 139.0 MB (139025394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1` - linux; 386

```console
$ docker pull rust@sha256:e1de980dfbedecb976f80c981e8ce689d9abd5cb15cff9306ada02436a5e4465
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.8 MB (466848765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:158b1b1e4c720838da8354351980c8022084cbec76ba03427a8a8699853c514f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:21 GMT
ADD file:b637f96d557a570f8ab83b28f7b9cdd128958359dd30dc2e03df70b799e132aa in / 
# Sat, 01 Feb 2020 16:39:21 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:23:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:24:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:24:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:25:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 01:26:51 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 01:27:16 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:2b34644a479c82db66a603c0b0a1d990911345f8646498fa9b050f306d0e6bf2`  
		Last Modified: Sat, 01 Feb 2020 16:44:10 GMT  
		Size: 51.1 MB (51141949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2f611c9392c4fe86735b477d61fda0e95ea77486175a737114c51586ecce86`  
		Last Modified: Sat, 01 Feb 2020 17:42:17 GMT  
		Size: 8.0 MB (7981506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69713757cc2d87c3255331d40f5061a73ef412208961f1ddd67a59a375397fda`  
		Last Modified: Sat, 01 Feb 2020 17:42:17 GMT  
		Size: 10.3 MB (10338479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956cf07a321afcfed99809a380a1905660e378188fd33d97f136551450be347a`  
		Last Modified: Sat, 01 Feb 2020 17:42:36 GMT  
		Size: 53.4 MB (53380753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8bfbd246f3a4ba9d861315c676a9a9e6524857c085e71b18b492882b063bff`  
		Last Modified: Sat, 01 Feb 2020 17:43:24 GMT  
		Size: 198.7 MB (198719863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b623bef7c51ab75de28495552321d02b2d6b4d6537933d893f18d155b414204a`  
		Last Modified: Sun, 02 Feb 2020 01:31:32 GMT  
		Size: 145.3 MB (145286215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.41`

```console
$ docker pull rust@sha256:920b5c1b275778169a8c35f767c9c238ac9391f8a666d3ee159a1a2a26088a25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.41` - linux; amd64

```console
$ docker pull rust@sha256:d59df245b22bfef90c2d29c1691e6a3ff679feb95d400b69626bae74898efab3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.7 MB (441693460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db33159e3388e178392ca314fbd8ecebb9fb430b73a29538302486e29cec6bc1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:08 GMT
ADD file:d6d0bdf8cb07a7a0dc32e9df50ac80ca1a524c3fa48136892ded195061f2194c in / 
# Sat, 28 Dec 2019 04:21:09 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:47:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:47:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 04:47:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:48:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Jan 2020 23:58:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:58:35 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:8f0fdd3eaac017684c880d836abdaf02f9db7ac8ecca970356482e3d8e315650`  
		Last Modified: Sat, 28 Dec 2019 04:25:39 GMT  
		Size: 50.4 MB (50379720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d918eaefd9de8a1595f56900fdb8ab65a03d64b1da1078da7c0b0bf6f7552a14`  
		Last Modified: Sat, 28 Dec 2019 05:01:44 GMT  
		Size: 7.8 MB (7811715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bf3e3107f525b7dea5b3cdfd15f62666066202105a0aaddbab2a02aefad1f7`  
		Last Modified: Sat, 28 Dec 2019 05:01:44 GMT  
		Size: 10.0 MB (9996202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27622921edb2aae9e0cb64f71a81b4a7cfef8f6a6c766514a018815834ba4e14`  
		Last Modified: Sat, 28 Dec 2019 05:02:00 GMT  
		Size: 51.8 MB (51790562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfa0aa1ae2c54d0de4b6ad0ee4d9f795c93368ae7d87801784c1f8ae624ac33`  
		Last Modified: Sat, 28 Dec 2019 05:02:36 GMT  
		Size: 192.0 MB (192044395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b109c91c0639fd55a93a5688b1bc7501e434396daabd93d714b72b106996a82a`  
		Last Modified: Fri, 31 Jan 2020 00:01:48 GMT  
		Size: 129.7 MB (129670866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41` - linux; arm variant v7

```console
$ docker pull rust@sha256:f4b13a8a2df73cfd225ce928f3574e1169b288e8448e004659d35d303ba1b82f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **420.0 MB (420018522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af6c4b7927d04a1c76f6b24226aa2702d2a7de368154e22aa531e7e986d7c227`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:06 GMT
ADD file:a57a312731f174c4b03031908ff95f49d7055d8c196439f0ed07ed9c4834d993 in / 
# Sat, 01 Feb 2020 17:00:08 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:00:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 18:01:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:03:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 03:16:56 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 03:17:21 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9bbb41bca8c6254da5088d03354297b1309dc75c2ccc738416025f89709ae5ee`  
		Last Modified: Sat, 01 Feb 2020 17:07:28 GMT  
		Size: 45.9 MB (45859700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239e4acdbc2ab88c89aa359fbab11429ea6d7bd93ea589a22c6bbb833ff82b93`  
		Last Modified: Sat, 01 Feb 2020 18:25:50 GMT  
		Size: 7.1 MB (7096223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6b4707a3c3aff9cb939fc058b869c5412e78c37e43eb0b653565460495537`  
		Last Modified: Sat, 01 Feb 2020 18:25:50 GMT  
		Size: 9.3 MB (9343278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e096c4fc8c629edca6da3ce5a9e95288512cb11e3d3d01a6e49078d19c2acca`  
		Last Modified: Sat, 01 Feb 2020 18:26:13 GMT  
		Size: 47.3 MB (47315591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6953ecf4273071529462518748f048f49a05530ae24d8fc6841919de312f2fc`  
		Last Modified: Sat, 01 Feb 2020 18:27:03 GMT  
		Size: 168.4 MB (168379144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f84f54aa922c34c20237ad8b624417ee33ea2f0c7940b127d3043d241b53bd`  
		Last Modified: Sun, 02 Feb 2020 03:21:00 GMT  
		Size: 142.0 MB (142024586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:cc4933ffae4311c25299ae5b6a8e115241533bed5ca5e71dd7df717e0ca3b760
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.5 MB (441531085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:779e2f51436aa1328b240e1b38f7b6758d6acb69f2a4eae5f652148e28a16a8e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:40:41 GMT
ADD file:88b3d02fc98aa9138e694bee7d5d1b61b295e4a1c7fae399bf24e52eeff7a5ae in / 
# Sat, 28 Dec 2019 04:40:45 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:04:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:05:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:05:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:08:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Jan 2020 23:45:22 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:45:39 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:627706d65d1d9b4038d8fd40db52238d4f11d9130a01f23ffae9bf5d41ac5933`  
		Last Modified: Sat, 28 Dec 2019 04:46:38 GMT  
		Size: 49.2 MB (49171876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ac1923ab7a97ecdde2a4f034a8b716d51594ba6fc823c6aaac579c31f51906`  
		Last Modified: Sat, 28 Dec 2019 06:21:16 GMT  
		Size: 7.7 MB (7681148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b000e01546d5b9b3a40a3797f15bc0a1f579786c5ec8da31cbe9502f1927d367`  
		Last Modified: Sat, 28 Dec 2019 06:21:16 GMT  
		Size: 10.0 MB (9983835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8fe6ebd465d85dc79039fbd39712f1fadf5d7ac5fbefe405ef7a4f957a94ce`  
		Last Modified: Sat, 28 Dec 2019 06:21:39 GMT  
		Size: 52.1 MB (52102816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d739211b59b4a5cab55db8d8ce73eb5edfb9d5d91addf9f7aab0b9d9fa90b06`  
		Last Modified: Sat, 28 Dec 2019 06:22:32 GMT  
		Size: 183.6 MB (183566016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cff33cb79d34d36837bc747d7bd54401995ea5a541d92619b14c3ab0c8e2eb`  
		Last Modified: Thu, 30 Jan 2020 23:48:59 GMT  
		Size: 139.0 MB (139025394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41` - linux; 386

```console
$ docker pull rust@sha256:e1de980dfbedecb976f80c981e8ce689d9abd5cb15cff9306ada02436a5e4465
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.8 MB (466848765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:158b1b1e4c720838da8354351980c8022084cbec76ba03427a8a8699853c514f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:21 GMT
ADD file:b637f96d557a570f8ab83b28f7b9cdd128958359dd30dc2e03df70b799e132aa in / 
# Sat, 01 Feb 2020 16:39:21 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:23:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:24:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:24:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:25:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 01:26:51 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 01:27:16 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:2b34644a479c82db66a603c0b0a1d990911345f8646498fa9b050f306d0e6bf2`  
		Last Modified: Sat, 01 Feb 2020 16:44:10 GMT  
		Size: 51.1 MB (51141949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2f611c9392c4fe86735b477d61fda0e95ea77486175a737114c51586ecce86`  
		Last Modified: Sat, 01 Feb 2020 17:42:17 GMT  
		Size: 8.0 MB (7981506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69713757cc2d87c3255331d40f5061a73ef412208961f1ddd67a59a375397fda`  
		Last Modified: Sat, 01 Feb 2020 17:42:17 GMT  
		Size: 10.3 MB (10338479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956cf07a321afcfed99809a380a1905660e378188fd33d97f136551450be347a`  
		Last Modified: Sat, 01 Feb 2020 17:42:36 GMT  
		Size: 53.4 MB (53380753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8bfbd246f3a4ba9d861315c676a9a9e6524857c085e71b18b492882b063bff`  
		Last Modified: Sat, 01 Feb 2020 17:43:24 GMT  
		Size: 198.7 MB (198719863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b623bef7c51ab75de28495552321d02b2d6b4d6537933d893f18d155b414204a`  
		Last Modified: Sun, 02 Feb 2020 01:31:32 GMT  
		Size: 145.3 MB (145286215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.41.0`

```console
$ docker pull rust@sha256:920b5c1b275778169a8c35f767c9c238ac9391f8a666d3ee159a1a2a26088a25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.41.0` - linux; amd64

```console
$ docker pull rust@sha256:d59df245b22bfef90c2d29c1691e6a3ff679feb95d400b69626bae74898efab3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.7 MB (441693460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db33159e3388e178392ca314fbd8ecebb9fb430b73a29538302486e29cec6bc1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:08 GMT
ADD file:d6d0bdf8cb07a7a0dc32e9df50ac80ca1a524c3fa48136892ded195061f2194c in / 
# Sat, 28 Dec 2019 04:21:09 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:47:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:47:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 04:47:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:48:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Jan 2020 23:58:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:58:35 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:8f0fdd3eaac017684c880d836abdaf02f9db7ac8ecca970356482e3d8e315650`  
		Last Modified: Sat, 28 Dec 2019 04:25:39 GMT  
		Size: 50.4 MB (50379720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d918eaefd9de8a1595f56900fdb8ab65a03d64b1da1078da7c0b0bf6f7552a14`  
		Last Modified: Sat, 28 Dec 2019 05:01:44 GMT  
		Size: 7.8 MB (7811715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bf3e3107f525b7dea5b3cdfd15f62666066202105a0aaddbab2a02aefad1f7`  
		Last Modified: Sat, 28 Dec 2019 05:01:44 GMT  
		Size: 10.0 MB (9996202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27622921edb2aae9e0cb64f71a81b4a7cfef8f6a6c766514a018815834ba4e14`  
		Last Modified: Sat, 28 Dec 2019 05:02:00 GMT  
		Size: 51.8 MB (51790562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfa0aa1ae2c54d0de4b6ad0ee4d9f795c93368ae7d87801784c1f8ae624ac33`  
		Last Modified: Sat, 28 Dec 2019 05:02:36 GMT  
		Size: 192.0 MB (192044395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b109c91c0639fd55a93a5688b1bc7501e434396daabd93d714b72b106996a82a`  
		Last Modified: Fri, 31 Jan 2020 00:01:48 GMT  
		Size: 129.7 MB (129670866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41.0` - linux; arm variant v7

```console
$ docker pull rust@sha256:f4b13a8a2df73cfd225ce928f3574e1169b288e8448e004659d35d303ba1b82f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **420.0 MB (420018522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af6c4b7927d04a1c76f6b24226aa2702d2a7de368154e22aa531e7e986d7c227`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:06 GMT
ADD file:a57a312731f174c4b03031908ff95f49d7055d8c196439f0ed07ed9c4834d993 in / 
# Sat, 01 Feb 2020 17:00:08 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:00:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 18:01:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:03:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 03:16:56 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 03:17:21 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9bbb41bca8c6254da5088d03354297b1309dc75c2ccc738416025f89709ae5ee`  
		Last Modified: Sat, 01 Feb 2020 17:07:28 GMT  
		Size: 45.9 MB (45859700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239e4acdbc2ab88c89aa359fbab11429ea6d7bd93ea589a22c6bbb833ff82b93`  
		Last Modified: Sat, 01 Feb 2020 18:25:50 GMT  
		Size: 7.1 MB (7096223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6b4707a3c3aff9cb939fc058b869c5412e78c37e43eb0b653565460495537`  
		Last Modified: Sat, 01 Feb 2020 18:25:50 GMT  
		Size: 9.3 MB (9343278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e096c4fc8c629edca6da3ce5a9e95288512cb11e3d3d01a6e49078d19c2acca`  
		Last Modified: Sat, 01 Feb 2020 18:26:13 GMT  
		Size: 47.3 MB (47315591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6953ecf4273071529462518748f048f49a05530ae24d8fc6841919de312f2fc`  
		Last Modified: Sat, 01 Feb 2020 18:27:03 GMT  
		Size: 168.4 MB (168379144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f84f54aa922c34c20237ad8b624417ee33ea2f0c7940b127d3043d241b53bd`  
		Last Modified: Sun, 02 Feb 2020 03:21:00 GMT  
		Size: 142.0 MB (142024586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41.0` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:cc4933ffae4311c25299ae5b6a8e115241533bed5ca5e71dd7df717e0ca3b760
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.5 MB (441531085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:779e2f51436aa1328b240e1b38f7b6758d6acb69f2a4eae5f652148e28a16a8e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:40:41 GMT
ADD file:88b3d02fc98aa9138e694bee7d5d1b61b295e4a1c7fae399bf24e52eeff7a5ae in / 
# Sat, 28 Dec 2019 04:40:45 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:04:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:05:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:05:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:08:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Jan 2020 23:45:22 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:45:39 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:627706d65d1d9b4038d8fd40db52238d4f11d9130a01f23ffae9bf5d41ac5933`  
		Last Modified: Sat, 28 Dec 2019 04:46:38 GMT  
		Size: 49.2 MB (49171876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ac1923ab7a97ecdde2a4f034a8b716d51594ba6fc823c6aaac579c31f51906`  
		Last Modified: Sat, 28 Dec 2019 06:21:16 GMT  
		Size: 7.7 MB (7681148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b000e01546d5b9b3a40a3797f15bc0a1f579786c5ec8da31cbe9502f1927d367`  
		Last Modified: Sat, 28 Dec 2019 06:21:16 GMT  
		Size: 10.0 MB (9983835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8fe6ebd465d85dc79039fbd39712f1fadf5d7ac5fbefe405ef7a4f957a94ce`  
		Last Modified: Sat, 28 Dec 2019 06:21:39 GMT  
		Size: 52.1 MB (52102816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d739211b59b4a5cab55db8d8ce73eb5edfb9d5d91addf9f7aab0b9d9fa90b06`  
		Last Modified: Sat, 28 Dec 2019 06:22:32 GMT  
		Size: 183.6 MB (183566016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cff33cb79d34d36837bc747d7bd54401995ea5a541d92619b14c3ab0c8e2eb`  
		Last Modified: Thu, 30 Jan 2020 23:48:59 GMT  
		Size: 139.0 MB (139025394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41.0` - linux; 386

```console
$ docker pull rust@sha256:e1de980dfbedecb976f80c981e8ce689d9abd5cb15cff9306ada02436a5e4465
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.8 MB (466848765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:158b1b1e4c720838da8354351980c8022084cbec76ba03427a8a8699853c514f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:21 GMT
ADD file:b637f96d557a570f8ab83b28f7b9cdd128958359dd30dc2e03df70b799e132aa in / 
# Sat, 01 Feb 2020 16:39:21 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:23:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:24:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:24:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:25:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 01:26:51 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 01:27:16 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:2b34644a479c82db66a603c0b0a1d990911345f8646498fa9b050f306d0e6bf2`  
		Last Modified: Sat, 01 Feb 2020 16:44:10 GMT  
		Size: 51.1 MB (51141949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2f611c9392c4fe86735b477d61fda0e95ea77486175a737114c51586ecce86`  
		Last Modified: Sat, 01 Feb 2020 17:42:17 GMT  
		Size: 8.0 MB (7981506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69713757cc2d87c3255331d40f5061a73ef412208961f1ddd67a59a375397fda`  
		Last Modified: Sat, 01 Feb 2020 17:42:17 GMT  
		Size: 10.3 MB (10338479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956cf07a321afcfed99809a380a1905660e378188fd33d97f136551450be347a`  
		Last Modified: Sat, 01 Feb 2020 17:42:36 GMT  
		Size: 53.4 MB (53380753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8bfbd246f3a4ba9d861315c676a9a9e6524857c085e71b18b492882b063bff`  
		Last Modified: Sat, 01 Feb 2020 17:43:24 GMT  
		Size: 198.7 MB (198719863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b623bef7c51ab75de28495552321d02b2d6b4d6537933d893f18d155b414204a`  
		Last Modified: Sun, 02 Feb 2020 01:31:32 GMT  
		Size: 145.3 MB (145286215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.41.0-alpine`

```console
$ docker pull rust@sha256:174277b6eb8de98ba66882a88b81e9dc8bce7864d3b4c7e1471778d1d2d368a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1.41.0-alpine` - linux; amd64

```console
$ docker pull rust@sha256:fe545e8f5ad12baa7ce768a7fed3ca081647cf324fe2e3282df1a7a37a8b5e63
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.3 MB (133272665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f952798c43f276fb7cacefa3fa22ba95226a2a8554669dbd559dce10b4b7b74`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Tue, 21 Jan 2020 21:26:53 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 30 Jan 2020 23:59:32 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:59:41 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.21.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "0c86d467982bdf5c4b8d844bf8c3f7fc602cc4ac30b29262b8941d6d8b363d7e *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409bef176e35cb7d5f61284ce84fc883b72774cc0736c7286117d258c6bf7a3e`  
		Last Modified: Tue, 21 Jan 2020 21:27:29 GMT  
		Size: 36.4 MB (36417023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed492dc040c10c2f241f489b18b5cf7cc4dd2808c83d6544d5e5e563180e096`  
		Last Modified: Fri, 31 Jan 2020 00:03:25 GMT  
		Size: 94.1 MB (94052685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.41.0-alpine3.10`

```console
$ docker pull rust@sha256:e199301d1242c027a8d532ea1b976cb5f1063af6f1bee394c539b94fee66cf28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1.41.0-alpine3.10` - linux; amd64

```console
$ docker pull rust@sha256:06a34ea0c8dca19912d7c326664f636f94e520d2cce1b2af55f3d3e6881936fe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.8 MB (130823278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:718c95e2d38f3cbcec4c7e0237dc2ef6fb5c5d5428bb5b3e67d50a421f0aec19`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 05:59:59 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 30 Jan 2020 23:59:19 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:59:28 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.21.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "0c86d467982bdf5c4b8d844bf8c3f7fc602cc4ac30b29262b8941d6d8b363d7e *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4894ab3ba23d1a77df9f98d547d9f3afeb033693fd523558a1e88651178b4d54`  
		Last Modified: Fri, 24 Jan 2020 06:01:10 GMT  
		Size: 34.0 MB (33983603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b138b4be762363e564b1547030500da8ddb0c0262f2e4430ec61192a46790b`  
		Last Modified: Fri, 31 Jan 2020 00:03:04 GMT  
		Size: 94.1 MB (94052713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.41.0-alpine3.11`

```console
$ docker pull rust@sha256:174277b6eb8de98ba66882a88b81e9dc8bce7864d3b4c7e1471778d1d2d368a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1.41.0-alpine3.11` - linux; amd64

```console
$ docker pull rust@sha256:fe545e8f5ad12baa7ce768a7fed3ca081647cf324fe2e3282df1a7a37a8b5e63
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.3 MB (133272665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f952798c43f276fb7cacefa3fa22ba95226a2a8554669dbd559dce10b4b7b74`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Tue, 21 Jan 2020 21:26:53 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 30 Jan 2020 23:59:32 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:59:41 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.21.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "0c86d467982bdf5c4b8d844bf8c3f7fc602cc4ac30b29262b8941d6d8b363d7e *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409bef176e35cb7d5f61284ce84fc883b72774cc0736c7286117d258c6bf7a3e`  
		Last Modified: Tue, 21 Jan 2020 21:27:29 GMT  
		Size: 36.4 MB (36417023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed492dc040c10c2f241f489b18b5cf7cc4dd2808c83d6544d5e5e563180e096`  
		Last Modified: Fri, 31 Jan 2020 00:03:25 GMT  
		Size: 94.1 MB (94052685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.41.0-buster`

```console
$ docker pull rust@sha256:920b5c1b275778169a8c35f767c9c238ac9391f8a666d3ee159a1a2a26088a25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.41.0-buster` - linux; amd64

```console
$ docker pull rust@sha256:d59df245b22bfef90c2d29c1691e6a3ff679feb95d400b69626bae74898efab3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.7 MB (441693460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db33159e3388e178392ca314fbd8ecebb9fb430b73a29538302486e29cec6bc1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:08 GMT
ADD file:d6d0bdf8cb07a7a0dc32e9df50ac80ca1a524c3fa48136892ded195061f2194c in / 
# Sat, 28 Dec 2019 04:21:09 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:47:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:47:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 04:47:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:48:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Jan 2020 23:58:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:58:35 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:8f0fdd3eaac017684c880d836abdaf02f9db7ac8ecca970356482e3d8e315650`  
		Last Modified: Sat, 28 Dec 2019 04:25:39 GMT  
		Size: 50.4 MB (50379720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d918eaefd9de8a1595f56900fdb8ab65a03d64b1da1078da7c0b0bf6f7552a14`  
		Last Modified: Sat, 28 Dec 2019 05:01:44 GMT  
		Size: 7.8 MB (7811715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bf3e3107f525b7dea5b3cdfd15f62666066202105a0aaddbab2a02aefad1f7`  
		Last Modified: Sat, 28 Dec 2019 05:01:44 GMT  
		Size: 10.0 MB (9996202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27622921edb2aae9e0cb64f71a81b4a7cfef8f6a6c766514a018815834ba4e14`  
		Last Modified: Sat, 28 Dec 2019 05:02:00 GMT  
		Size: 51.8 MB (51790562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfa0aa1ae2c54d0de4b6ad0ee4d9f795c93368ae7d87801784c1f8ae624ac33`  
		Last Modified: Sat, 28 Dec 2019 05:02:36 GMT  
		Size: 192.0 MB (192044395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b109c91c0639fd55a93a5688b1bc7501e434396daabd93d714b72b106996a82a`  
		Last Modified: Fri, 31 Jan 2020 00:01:48 GMT  
		Size: 129.7 MB (129670866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41.0-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:f4b13a8a2df73cfd225ce928f3574e1169b288e8448e004659d35d303ba1b82f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **420.0 MB (420018522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af6c4b7927d04a1c76f6b24226aa2702d2a7de368154e22aa531e7e986d7c227`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:06 GMT
ADD file:a57a312731f174c4b03031908ff95f49d7055d8c196439f0ed07ed9c4834d993 in / 
# Sat, 01 Feb 2020 17:00:08 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:00:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 18:01:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:03:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 03:16:56 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 03:17:21 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9bbb41bca8c6254da5088d03354297b1309dc75c2ccc738416025f89709ae5ee`  
		Last Modified: Sat, 01 Feb 2020 17:07:28 GMT  
		Size: 45.9 MB (45859700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239e4acdbc2ab88c89aa359fbab11429ea6d7bd93ea589a22c6bbb833ff82b93`  
		Last Modified: Sat, 01 Feb 2020 18:25:50 GMT  
		Size: 7.1 MB (7096223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6b4707a3c3aff9cb939fc058b869c5412e78c37e43eb0b653565460495537`  
		Last Modified: Sat, 01 Feb 2020 18:25:50 GMT  
		Size: 9.3 MB (9343278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e096c4fc8c629edca6da3ce5a9e95288512cb11e3d3d01a6e49078d19c2acca`  
		Last Modified: Sat, 01 Feb 2020 18:26:13 GMT  
		Size: 47.3 MB (47315591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6953ecf4273071529462518748f048f49a05530ae24d8fc6841919de312f2fc`  
		Last Modified: Sat, 01 Feb 2020 18:27:03 GMT  
		Size: 168.4 MB (168379144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f84f54aa922c34c20237ad8b624417ee33ea2f0c7940b127d3043d241b53bd`  
		Last Modified: Sun, 02 Feb 2020 03:21:00 GMT  
		Size: 142.0 MB (142024586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41.0-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:cc4933ffae4311c25299ae5b6a8e115241533bed5ca5e71dd7df717e0ca3b760
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.5 MB (441531085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:779e2f51436aa1328b240e1b38f7b6758d6acb69f2a4eae5f652148e28a16a8e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:40:41 GMT
ADD file:88b3d02fc98aa9138e694bee7d5d1b61b295e4a1c7fae399bf24e52eeff7a5ae in / 
# Sat, 28 Dec 2019 04:40:45 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:04:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:05:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:05:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:08:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Jan 2020 23:45:22 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:45:39 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:627706d65d1d9b4038d8fd40db52238d4f11d9130a01f23ffae9bf5d41ac5933`  
		Last Modified: Sat, 28 Dec 2019 04:46:38 GMT  
		Size: 49.2 MB (49171876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ac1923ab7a97ecdde2a4f034a8b716d51594ba6fc823c6aaac579c31f51906`  
		Last Modified: Sat, 28 Dec 2019 06:21:16 GMT  
		Size: 7.7 MB (7681148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b000e01546d5b9b3a40a3797f15bc0a1f579786c5ec8da31cbe9502f1927d367`  
		Last Modified: Sat, 28 Dec 2019 06:21:16 GMT  
		Size: 10.0 MB (9983835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8fe6ebd465d85dc79039fbd39712f1fadf5d7ac5fbefe405ef7a4f957a94ce`  
		Last Modified: Sat, 28 Dec 2019 06:21:39 GMT  
		Size: 52.1 MB (52102816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d739211b59b4a5cab55db8d8ce73eb5edfb9d5d91addf9f7aab0b9d9fa90b06`  
		Last Modified: Sat, 28 Dec 2019 06:22:32 GMT  
		Size: 183.6 MB (183566016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cff33cb79d34d36837bc747d7bd54401995ea5a541d92619b14c3ab0c8e2eb`  
		Last Modified: Thu, 30 Jan 2020 23:48:59 GMT  
		Size: 139.0 MB (139025394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41.0-buster` - linux; 386

```console
$ docker pull rust@sha256:e1de980dfbedecb976f80c981e8ce689d9abd5cb15cff9306ada02436a5e4465
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.8 MB (466848765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:158b1b1e4c720838da8354351980c8022084cbec76ba03427a8a8699853c514f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:21 GMT
ADD file:b637f96d557a570f8ab83b28f7b9cdd128958359dd30dc2e03df70b799e132aa in / 
# Sat, 01 Feb 2020 16:39:21 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:23:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:24:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:24:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:25:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 01:26:51 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 01:27:16 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:2b34644a479c82db66a603c0b0a1d990911345f8646498fa9b050f306d0e6bf2`  
		Last Modified: Sat, 01 Feb 2020 16:44:10 GMT  
		Size: 51.1 MB (51141949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2f611c9392c4fe86735b477d61fda0e95ea77486175a737114c51586ecce86`  
		Last Modified: Sat, 01 Feb 2020 17:42:17 GMT  
		Size: 8.0 MB (7981506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69713757cc2d87c3255331d40f5061a73ef412208961f1ddd67a59a375397fda`  
		Last Modified: Sat, 01 Feb 2020 17:42:17 GMT  
		Size: 10.3 MB (10338479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956cf07a321afcfed99809a380a1905660e378188fd33d97f136551450be347a`  
		Last Modified: Sat, 01 Feb 2020 17:42:36 GMT  
		Size: 53.4 MB (53380753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8bfbd246f3a4ba9d861315c676a9a9e6524857c085e71b18b492882b063bff`  
		Last Modified: Sat, 01 Feb 2020 17:43:24 GMT  
		Size: 198.7 MB (198719863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b623bef7c51ab75de28495552321d02b2d6b4d6537933d893f18d155b414204a`  
		Last Modified: Sun, 02 Feb 2020 01:31:32 GMT  
		Size: 145.3 MB (145286215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.41.0-slim`

```console
$ docker pull rust@sha256:9c5a689ef6db939e940e061754a2b9a1841de8f86c2aa597c6fef6e5ceae631f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.41.0-slim` - linux; amd64

```console
$ docker pull rust@sha256:3fa8907a8030936ddf8785dd8339fc4ac64a8125c17e4a0ad1370524fcf83080
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202144548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:288fd60b2b05cb16b0a07371e5d69a0e30ce6a7d5a809fef31c9e1aad26ed7fd`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Thu, 30 Jan 2020 23:58:40 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:59:12 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4b6ea1105b5642d3cfab2b6fc2e4bc35a7c619b6cf9d1f1a74e56d944416b8`  
		Last Modified: Fri, 31 Jan 2020 00:02:40 GMT  
		Size: 175.1 MB (175052274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41.0-slim` - linux; arm variant v7

```console
$ docker pull rust@sha256:ff2a1737cb5103afe6786f50a0340e8e52bfabe14523eb58fa1b2f9b8811acc6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.6 MB (197616259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d70333cde16926a90ea171253fd5353a3c875c45e0545febb78c6fd0c9637a0`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 03:17:30 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 03:18:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcd7ca587ec66d5a119fa12058b0cb1efb357adfaf91ad6ce5dc9a8250c6b3b`  
		Last Modified: Sun, 02 Feb 2020 03:22:02 GMT  
		Size: 174.9 MB (174917121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41.0-slim` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:c332927372fd374053c15e96604081147f07cb23ac35c35e390de9e74a34fa5e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.1 MB (205078984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85242a1a07815d02d847a6d1de41cfca4a9c2e239740d90dd84dd0fada10aef5`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Thu, 30 Jan 2020 23:45:48 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:46:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15b43da91b755c785745bcf6dd8b619aa403485ba00e712b498bc6efb09482d`  
		Last Modified: Thu, 30 Jan 2020 23:49:59 GMT  
		Size: 179.2 MB (179228282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41.0-slim` - linux; 386

```console
$ docker pull rust@sha256:0b932c1020eee53546fffda34009bc0c6cdbfa0d496e863eb18846d65dd89290
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.0 MB (223015002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b3d3432b91e42b3062b27d190a1f8578b427582a142ec5858e9b2c88a57ca1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 01:27:25 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 01:28:20 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350f4532a56d213c594ac0bc23a3cd8cdc364f385832905798ff101a2cc9136f`  
		Last Modified: Sun, 02 Feb 2020 01:32:45 GMT  
		Size: 195.3 MB (195267950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.41.0-slim-buster`

```console
$ docker pull rust@sha256:9c5a689ef6db939e940e061754a2b9a1841de8f86c2aa597c6fef6e5ceae631f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.41.0-slim-buster` - linux; amd64

```console
$ docker pull rust@sha256:3fa8907a8030936ddf8785dd8339fc4ac64a8125c17e4a0ad1370524fcf83080
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202144548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:288fd60b2b05cb16b0a07371e5d69a0e30ce6a7d5a809fef31c9e1aad26ed7fd`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Thu, 30 Jan 2020 23:58:40 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:59:12 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4b6ea1105b5642d3cfab2b6fc2e4bc35a7c619b6cf9d1f1a74e56d944416b8`  
		Last Modified: Fri, 31 Jan 2020 00:02:40 GMT  
		Size: 175.1 MB (175052274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41.0-slim-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:ff2a1737cb5103afe6786f50a0340e8e52bfabe14523eb58fa1b2f9b8811acc6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.6 MB (197616259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d70333cde16926a90ea171253fd5353a3c875c45e0545febb78c6fd0c9637a0`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 03:17:30 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 03:18:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcd7ca587ec66d5a119fa12058b0cb1efb357adfaf91ad6ce5dc9a8250c6b3b`  
		Last Modified: Sun, 02 Feb 2020 03:22:02 GMT  
		Size: 174.9 MB (174917121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41.0-slim-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:c332927372fd374053c15e96604081147f07cb23ac35c35e390de9e74a34fa5e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.1 MB (205078984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85242a1a07815d02d847a6d1de41cfca4a9c2e239740d90dd84dd0fada10aef5`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Thu, 30 Jan 2020 23:45:48 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:46:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15b43da91b755c785745bcf6dd8b619aa403485ba00e712b498bc6efb09482d`  
		Last Modified: Thu, 30 Jan 2020 23:49:59 GMT  
		Size: 179.2 MB (179228282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41.0-slim-buster` - linux; 386

```console
$ docker pull rust@sha256:0b932c1020eee53546fffda34009bc0c6cdbfa0d496e863eb18846d65dd89290
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.0 MB (223015002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b3d3432b91e42b3062b27d190a1f8578b427582a142ec5858e9b2c88a57ca1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 01:27:25 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 01:28:20 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350f4532a56d213c594ac0bc23a3cd8cdc364f385832905798ff101a2cc9136f`  
		Last Modified: Sun, 02 Feb 2020 01:32:45 GMT  
		Size: 195.3 MB (195267950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.41.0-slim-stretch`

```console
$ docker pull rust@sha256:54c28eb493584efa368f8ad3b842a82f95321479f511c092719071cd6c9da5d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.41.0-slim-stretch` - linux; amd64

```console
$ docker pull rust@sha256:8988a0ace70a25adc0076a21458d807fa08cecde92a8126c66bd0febdc0f099e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190094499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80efe80a4223e96acebcd908e5ef8fecd93781a5a9fa24de654e0265c7988e26`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:47 GMT
ADD file:90a2c81769a336bed3f731f44a385f2a65b0916f517a0b77c06c224579bf9a9a in / 
# Sat, 28 Dec 2019 04:23:47 GMT
CMD ["bash"]
# Thu, 30 Jan 2020 23:57:50 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:58:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:804555ee037604c40de144f9f8da0d826d38db82f15d74cded32790fe279a8f6`  
		Last Modified: Sat, 28 Dec 2019 04:28:38 GMT  
		Size: 22.5 MB (22524609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56e4802f7cdd484d276f0cfc4639961be839a95b6ffae7e536ae840b4fa5d8a`  
		Last Modified: Fri, 31 Jan 2020 00:01:21 GMT  
		Size: 167.6 MB (167569890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41.0-slim-stretch` - linux; arm variant v7

```console
$ docker pull rust@sha256:b0379f8ec7a9155f4ff13fa0957914ce3ba88b80ce5c22923c4ead2a9f89e451
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.4 MB (189398124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:690fad015da49bc6b577df128d04eccc8ee0176e7b0a897ed1111100cba598ef`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:04:29 GMT
ADD file:6ac430a42a1f2a6cc8b0a3565e518bd0e3a47b01d524b86cd3dd4e7f4606fd53 in / 
# Sat, 01 Feb 2020 17:04:31 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 03:15:52 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 03:16:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:6bc458b0813423b9e351a5604c0d71a4853d970ea22b23fedc8683af12dbc13c`  
		Last Modified: Sat, 01 Feb 2020 17:11:31 GMT  
		Size: 19.3 MB (19311624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c966b45d91cbdbbddb23863703ccd1856379b3e0d4ad838d8acee8c431b5717f`  
		Last Modified: Sun, 02 Feb 2020 03:20:10 GMT  
		Size: 170.1 MB (170086500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41.0-slim-stretch` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:b527a9fcdb5d6a90ce0de4fbbc161e962b09a62c009cd1e7114704f286379112
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.0 MB (190038348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea06f0967e1a0beb570f23c6f7dba5d4cf594b4a83455394d7194de9f956c551`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:43:36 GMT
ADD file:ba40f5080cbd89c576c350bfe5acfe16f2ec59636fdb082efc3a8cef66ae7cb7 in / 
# Sat, 28 Dec 2019 04:43:39 GMT
CMD ["bash"]
# Thu, 30 Jan 2020 23:44:29 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:45:11 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:588374d57fdb5120d024340eef3d8927af23a5b806d41b4f049ee430a153c0b4`  
		Last Modified: Sat, 28 Dec 2019 04:49:14 GMT  
		Size: 20.4 MB (20385801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e8a34c9e29def30493e1870ffa929495298009b05360083f22181d4453f839`  
		Last Modified: Thu, 30 Jan 2020 23:48:17 GMT  
		Size: 169.7 MB (169652547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41.0-slim-stretch` - linux; 386

```console
$ docker pull rust@sha256:b78ee7fab6baf80ca227645cda796eace6e3a676f35bb0d95939452dcc51c55c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.3 MB (210336495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2972082f643a87cf18629e0d194514767086084c493f5ef4811290a49c0bc022`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:07 GMT
ADD file:c9b4696be461d46d96c760441f34e219e229f90bc6946125b2f809218c3456ce in / 
# Sat, 01 Feb 2020 16:42:07 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 01:25:48 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 01:26:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:4f51b031b74b1f7fab6310c197fd7534181ba2db1f0cec6686fb9e9a82abbb9c`  
		Last Modified: Sat, 01 Feb 2020 16:47:27 GMT  
		Size: 23.2 MB (23152156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea943a600d5130a3a8ddcf69ed3eda4147d98c45f6c499d1f940b1bf24f9c28f`  
		Last Modified: Sun, 02 Feb 2020 01:30:26 GMT  
		Size: 187.2 MB (187184339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.41.0-stretch`

```console
$ docker pull rust@sha256:b37b4a8bf6cd1080fb9a379ee680c2fcc90121d67fb3a04bb76e4484a9544d43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.41.0-stretch` - linux; amd64

```console
$ docker pull rust@sha256:ff4627ba92fdf9d566bbd64ace1dc4184125d8e91a71ccd45fdf555fd17ebe52
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **455.1 MB (455102608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b1293d4b2e209d0e4854e3dbaf3ed403291aa20f01b64c71c3e0c1c7330561c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:33 GMT
ADD file:8f7dc710e276f54a3a73d34b6b8fa261950a781d68ceb7401fa18dabc601c5a5 in / 
# Sat, 28 Dec 2019 04:23:34 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:58:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:58:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 04:59:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:00:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Jan 2020 23:57:32 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:57:45 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:146bd6a886182fde06fbf747470b1c89814bc8ab1c96fdf1aef6107171959fe6`  
		Last Modified: Sat, 28 Dec 2019 04:28:25 GMT  
		Size: 45.4 MB (45380744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9935d0c62ace92b388be202275e222007d6cac10b9c1f2c1ea63af38c09ea7ab`  
		Last Modified: Sat, 28 Dec 2019 05:04:30 GMT  
		Size: 10.8 MB (10797221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0efb86e80601b5bbdbb7c406426982c4202d339687c14c3941b364527e2249`  
		Last Modified: Sat, 28 Dec 2019 05:04:28 GMT  
		Size: 4.3 MB (4340114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e705a4c4fd310b96bfb3d7928428e65f0d3f5bad0cd0bda1434aee1d89418468`  
		Last Modified: Sat, 28 Dec 2019 05:04:45 GMT  
		Size: 50.1 MB (50072671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c877b722db6f4d4297c21f07162d21fa6ac6f51d03360f75e24cfa3bcaefe57d`  
		Last Modified: Sat, 28 Dec 2019 05:05:38 GMT  
		Size: 214.8 MB (214840548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec7021710852d02bcf8dc866ab78921203814c4f8cb56c6e0717dd899d3dfb1`  
		Last Modified: Fri, 31 Jan 2020 00:00:33 GMT  
		Size: 129.7 MB (129671310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41.0-stretch` - linux; arm variant v7

```console
$ docker pull rust@sha256:95479bdf726ea84f8ce541732a071b898f3a87d69d3e8c10641bbaf327830871
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **439.5 MB (439473862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7e4ba4d1c5cd134afc62cb4f59a2673ee4eb0afa5debe20d887b29870da4991`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:04:08 GMT
ADD file:b7fc54d004d962f2cfb469a1aaa9e689e46dfa2554e0cf44c33981d688adc31b in / 
# Sat, 01 Feb 2020 17:04:09 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:18:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:18:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 18:19:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:23:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 03:15:22 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 03:15:44 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:cc3b08e804cce7e88d9df954b76be506569775afe9cf36316f2fa6c5c9bf3d5c`  
		Last Modified: Sat, 01 Feb 2020 17:11:13 GMT  
		Size: 42.1 MB (42108370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa649f4f33c2131c2969e49352ff247ebe5a62a62b83498c3580f883aa35621e`  
		Last Modified: Sat, 01 Feb 2020 18:31:10 GMT  
		Size: 9.5 MB (9498229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901c0c16dce9409a6a020f4b874b40fb3f7d302fe0b4e7a80a87a7cfbab7da04`  
		Last Modified: Sat, 01 Feb 2020 18:31:10 GMT  
		Size: 3.9 MB (3918766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a264d83dc76a4a25b4110827c1ac6cc620c406edb6b2089cd1117aec271ed`  
		Last Modified: Sat, 01 Feb 2020 18:31:32 GMT  
		Size: 46.4 MB (46400091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:854dcba3350bdff3f923ff69f2dec445f47ef5726d3d15bde4242c2ff122aabc`  
		Last Modified: Sat, 01 Feb 2020 18:32:28 GMT  
		Size: 195.5 MB (195523495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ce99acc39da624b324257b529b5859fe714ab94c38fd36224416818be5f43c`  
		Last Modified: Sun, 02 Feb 2020 03:19:13 GMT  
		Size: 142.0 MB (142024911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41.0-stretch` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:9ecb1e05a3077b32c8bd99e2d9eda52c2b5d79f388b751e61b4f3cfe047fb9ac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **446.3 MB (446292278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f5feafcebe0b3ff73e55d4ca6ee2ffd01eb91352c47ee1da796b47a1d89c8e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:43:15 GMT
ADD file:e439b3c387852978811a6a5a058745ebb9392da7e8936beb4f37ff076e656213 in / 
# Sat, 28 Dec 2019 04:43:17 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:15:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:15:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:16:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:18:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Jan 2020 23:43:59 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:44:18 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:d07bcf5901dfa793fa6b2c4c617e86bcef315b0b092cbfd1a929eefedaf8e3f2`  
		Last Modified: Sat, 28 Dec 2019 04:48:57 GMT  
		Size: 43.2 MB (43166476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f31062581dadb1f69c43e9441040dd46788bf13ae51f20c66929fac82b506b`  
		Last Modified: Sat, 28 Dec 2019 06:24:15 GMT  
		Size: 9.7 MB (9748258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62337a296a607f48a5dc3a7c07639360d98e0e78982ca8e459c832719012f12`  
		Last Modified: Sat, 28 Dec 2019 06:24:15 GMT  
		Size: 4.1 MB (4094448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403697a3e152c7a38ddb9175a90ed2dac97d780421c35949ff80cd67a7d4e596`  
		Last Modified: Sat, 28 Dec 2019 06:24:36 GMT  
		Size: 48.0 MB (48024191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0179cb8c17339f719c763581cefb9e377c016b4f7f4b747a665349e79470363c`  
		Last Modified: Sat, 28 Dec 2019 06:25:35 GMT  
		Size: 202.2 MB (202233183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cddbec6e7f644fe8725ebf72f7dc61a67b27b411e5d4466b522933633e74f5c`  
		Last Modified: Thu, 30 Jan 2020 23:47:26 GMT  
		Size: 139.0 MB (139025722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41.0-stretch` - linux; 386

```console
$ docker pull rust@sha256:1f587d401d8a96d2f338101f37a03cd379241fe760d8f8b4d4fa8d073336f6e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.3 MB (478286932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:979e274dc88223c0d7e5b1ad0fb9236195b93a7e3f6d79c11081b5db16cbec8d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:53 GMT
ADD file:bae1646c4e3069e717d1ee4f6c312c249e96a21d795a639cdfaf338d645c8be9 in / 
# Sat, 01 Feb 2020 16:41:53 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:38:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:38:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:39:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:40:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 01:25:09 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 01:25:38 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:97067fdacc0601fe58a5f782cd09d3c58a214c43b8629a2d92bd7025f46fd265`  
		Last Modified: Sat, 01 Feb 2020 16:47:15 GMT  
		Size: 46.1 MB (46100017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1ac2ac579e53fc74848ab743b53ae2f6e54350989c71359d435c2fef2e5157`  
		Last Modified: Sat, 01 Feb 2020 17:45:45 GMT  
		Size: 10.8 MB (10817587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f7b32e68627ad71130644b1646afb1aa0bcf1f440df145526a73fdbd413f3b`  
		Last Modified: Sat, 01 Feb 2020 17:45:43 GMT  
		Size: 4.6 MB (4561467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b926c1ce2d1cf6b99c32683bf0fd0233d4f71f367d38a16de2ba08e9ecbf1cc2`  
		Last Modified: Sat, 01 Feb 2020 17:46:05 GMT  
		Size: 51.6 MB (51595566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac9b89be3409f23bc9ac380bcfd9f28e0cc2e52b69b8706e0b102211c83abf4`  
		Last Modified: Sat, 01 Feb 2020 17:47:03 GMT  
		Size: 219.9 MB (219925297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69feda6b3fd089c07ee45b4a40f729a67e99bfa21dc5b5eede2fc9efc22d3d01`  
		Last Modified: Sun, 02 Feb 2020 01:29:25 GMT  
		Size: 145.3 MB (145286998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.41-alpine`

```console
$ docker pull rust@sha256:174277b6eb8de98ba66882a88b81e9dc8bce7864d3b4c7e1471778d1d2d368a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1.41-alpine` - linux; amd64

```console
$ docker pull rust@sha256:fe545e8f5ad12baa7ce768a7fed3ca081647cf324fe2e3282df1a7a37a8b5e63
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.3 MB (133272665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f952798c43f276fb7cacefa3fa22ba95226a2a8554669dbd559dce10b4b7b74`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Tue, 21 Jan 2020 21:26:53 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 30 Jan 2020 23:59:32 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:59:41 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.21.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "0c86d467982bdf5c4b8d844bf8c3f7fc602cc4ac30b29262b8941d6d8b363d7e *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409bef176e35cb7d5f61284ce84fc883b72774cc0736c7286117d258c6bf7a3e`  
		Last Modified: Tue, 21 Jan 2020 21:27:29 GMT  
		Size: 36.4 MB (36417023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed492dc040c10c2f241f489b18b5cf7cc4dd2808c83d6544d5e5e563180e096`  
		Last Modified: Fri, 31 Jan 2020 00:03:25 GMT  
		Size: 94.1 MB (94052685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.41-alpine3.10`

```console
$ docker pull rust@sha256:e199301d1242c027a8d532ea1b976cb5f1063af6f1bee394c539b94fee66cf28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1.41-alpine3.10` - linux; amd64

```console
$ docker pull rust@sha256:06a34ea0c8dca19912d7c326664f636f94e520d2cce1b2af55f3d3e6881936fe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.8 MB (130823278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:718c95e2d38f3cbcec4c7e0237dc2ef6fb5c5d5428bb5b3e67d50a421f0aec19`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 05:59:59 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 30 Jan 2020 23:59:19 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:59:28 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.21.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "0c86d467982bdf5c4b8d844bf8c3f7fc602cc4ac30b29262b8941d6d8b363d7e *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4894ab3ba23d1a77df9f98d547d9f3afeb033693fd523558a1e88651178b4d54`  
		Last Modified: Fri, 24 Jan 2020 06:01:10 GMT  
		Size: 34.0 MB (33983603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b138b4be762363e564b1547030500da8ddb0c0262f2e4430ec61192a46790b`  
		Last Modified: Fri, 31 Jan 2020 00:03:04 GMT  
		Size: 94.1 MB (94052713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.41-alpine3.11`

```console
$ docker pull rust@sha256:174277b6eb8de98ba66882a88b81e9dc8bce7864d3b4c7e1471778d1d2d368a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1.41-alpine3.11` - linux; amd64

```console
$ docker pull rust@sha256:fe545e8f5ad12baa7ce768a7fed3ca081647cf324fe2e3282df1a7a37a8b5e63
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.3 MB (133272665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f952798c43f276fb7cacefa3fa22ba95226a2a8554669dbd559dce10b4b7b74`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Tue, 21 Jan 2020 21:26:53 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 30 Jan 2020 23:59:32 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:59:41 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.21.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "0c86d467982bdf5c4b8d844bf8c3f7fc602cc4ac30b29262b8941d6d8b363d7e *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409bef176e35cb7d5f61284ce84fc883b72774cc0736c7286117d258c6bf7a3e`  
		Last Modified: Tue, 21 Jan 2020 21:27:29 GMT  
		Size: 36.4 MB (36417023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed492dc040c10c2f241f489b18b5cf7cc4dd2808c83d6544d5e5e563180e096`  
		Last Modified: Fri, 31 Jan 2020 00:03:25 GMT  
		Size: 94.1 MB (94052685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.41-buster`

```console
$ docker pull rust@sha256:920b5c1b275778169a8c35f767c9c238ac9391f8a666d3ee159a1a2a26088a25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.41-buster` - linux; amd64

```console
$ docker pull rust@sha256:d59df245b22bfef90c2d29c1691e6a3ff679feb95d400b69626bae74898efab3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.7 MB (441693460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db33159e3388e178392ca314fbd8ecebb9fb430b73a29538302486e29cec6bc1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:08 GMT
ADD file:d6d0bdf8cb07a7a0dc32e9df50ac80ca1a524c3fa48136892ded195061f2194c in / 
# Sat, 28 Dec 2019 04:21:09 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:47:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:47:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 04:47:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:48:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Jan 2020 23:58:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:58:35 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:8f0fdd3eaac017684c880d836abdaf02f9db7ac8ecca970356482e3d8e315650`  
		Last Modified: Sat, 28 Dec 2019 04:25:39 GMT  
		Size: 50.4 MB (50379720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d918eaefd9de8a1595f56900fdb8ab65a03d64b1da1078da7c0b0bf6f7552a14`  
		Last Modified: Sat, 28 Dec 2019 05:01:44 GMT  
		Size: 7.8 MB (7811715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bf3e3107f525b7dea5b3cdfd15f62666066202105a0aaddbab2a02aefad1f7`  
		Last Modified: Sat, 28 Dec 2019 05:01:44 GMT  
		Size: 10.0 MB (9996202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27622921edb2aae9e0cb64f71a81b4a7cfef8f6a6c766514a018815834ba4e14`  
		Last Modified: Sat, 28 Dec 2019 05:02:00 GMT  
		Size: 51.8 MB (51790562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfa0aa1ae2c54d0de4b6ad0ee4d9f795c93368ae7d87801784c1f8ae624ac33`  
		Last Modified: Sat, 28 Dec 2019 05:02:36 GMT  
		Size: 192.0 MB (192044395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b109c91c0639fd55a93a5688b1bc7501e434396daabd93d714b72b106996a82a`  
		Last Modified: Fri, 31 Jan 2020 00:01:48 GMT  
		Size: 129.7 MB (129670866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:f4b13a8a2df73cfd225ce928f3574e1169b288e8448e004659d35d303ba1b82f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **420.0 MB (420018522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af6c4b7927d04a1c76f6b24226aa2702d2a7de368154e22aa531e7e986d7c227`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:06 GMT
ADD file:a57a312731f174c4b03031908ff95f49d7055d8c196439f0ed07ed9c4834d993 in / 
# Sat, 01 Feb 2020 17:00:08 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:00:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 18:01:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:03:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 03:16:56 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 03:17:21 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9bbb41bca8c6254da5088d03354297b1309dc75c2ccc738416025f89709ae5ee`  
		Last Modified: Sat, 01 Feb 2020 17:07:28 GMT  
		Size: 45.9 MB (45859700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239e4acdbc2ab88c89aa359fbab11429ea6d7bd93ea589a22c6bbb833ff82b93`  
		Last Modified: Sat, 01 Feb 2020 18:25:50 GMT  
		Size: 7.1 MB (7096223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6b4707a3c3aff9cb939fc058b869c5412e78c37e43eb0b653565460495537`  
		Last Modified: Sat, 01 Feb 2020 18:25:50 GMT  
		Size: 9.3 MB (9343278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e096c4fc8c629edca6da3ce5a9e95288512cb11e3d3d01a6e49078d19c2acca`  
		Last Modified: Sat, 01 Feb 2020 18:26:13 GMT  
		Size: 47.3 MB (47315591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6953ecf4273071529462518748f048f49a05530ae24d8fc6841919de312f2fc`  
		Last Modified: Sat, 01 Feb 2020 18:27:03 GMT  
		Size: 168.4 MB (168379144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f84f54aa922c34c20237ad8b624417ee33ea2f0c7940b127d3043d241b53bd`  
		Last Modified: Sun, 02 Feb 2020 03:21:00 GMT  
		Size: 142.0 MB (142024586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:cc4933ffae4311c25299ae5b6a8e115241533bed5ca5e71dd7df717e0ca3b760
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.5 MB (441531085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:779e2f51436aa1328b240e1b38f7b6758d6acb69f2a4eae5f652148e28a16a8e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:40:41 GMT
ADD file:88b3d02fc98aa9138e694bee7d5d1b61b295e4a1c7fae399bf24e52eeff7a5ae in / 
# Sat, 28 Dec 2019 04:40:45 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:04:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:05:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:05:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:08:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Jan 2020 23:45:22 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:45:39 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:627706d65d1d9b4038d8fd40db52238d4f11d9130a01f23ffae9bf5d41ac5933`  
		Last Modified: Sat, 28 Dec 2019 04:46:38 GMT  
		Size: 49.2 MB (49171876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ac1923ab7a97ecdde2a4f034a8b716d51594ba6fc823c6aaac579c31f51906`  
		Last Modified: Sat, 28 Dec 2019 06:21:16 GMT  
		Size: 7.7 MB (7681148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b000e01546d5b9b3a40a3797f15bc0a1f579786c5ec8da31cbe9502f1927d367`  
		Last Modified: Sat, 28 Dec 2019 06:21:16 GMT  
		Size: 10.0 MB (9983835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8fe6ebd465d85dc79039fbd39712f1fadf5d7ac5fbefe405ef7a4f957a94ce`  
		Last Modified: Sat, 28 Dec 2019 06:21:39 GMT  
		Size: 52.1 MB (52102816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d739211b59b4a5cab55db8d8ce73eb5edfb9d5d91addf9f7aab0b9d9fa90b06`  
		Last Modified: Sat, 28 Dec 2019 06:22:32 GMT  
		Size: 183.6 MB (183566016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cff33cb79d34d36837bc747d7bd54401995ea5a541d92619b14c3ab0c8e2eb`  
		Last Modified: Thu, 30 Jan 2020 23:48:59 GMT  
		Size: 139.0 MB (139025394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41-buster` - linux; 386

```console
$ docker pull rust@sha256:e1de980dfbedecb976f80c981e8ce689d9abd5cb15cff9306ada02436a5e4465
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.8 MB (466848765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:158b1b1e4c720838da8354351980c8022084cbec76ba03427a8a8699853c514f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:21 GMT
ADD file:b637f96d557a570f8ab83b28f7b9cdd128958359dd30dc2e03df70b799e132aa in / 
# Sat, 01 Feb 2020 16:39:21 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:23:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:24:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:24:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:25:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 01:26:51 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 01:27:16 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:2b34644a479c82db66a603c0b0a1d990911345f8646498fa9b050f306d0e6bf2`  
		Last Modified: Sat, 01 Feb 2020 16:44:10 GMT  
		Size: 51.1 MB (51141949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2f611c9392c4fe86735b477d61fda0e95ea77486175a737114c51586ecce86`  
		Last Modified: Sat, 01 Feb 2020 17:42:17 GMT  
		Size: 8.0 MB (7981506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69713757cc2d87c3255331d40f5061a73ef412208961f1ddd67a59a375397fda`  
		Last Modified: Sat, 01 Feb 2020 17:42:17 GMT  
		Size: 10.3 MB (10338479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956cf07a321afcfed99809a380a1905660e378188fd33d97f136551450be347a`  
		Last Modified: Sat, 01 Feb 2020 17:42:36 GMT  
		Size: 53.4 MB (53380753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8bfbd246f3a4ba9d861315c676a9a9e6524857c085e71b18b492882b063bff`  
		Last Modified: Sat, 01 Feb 2020 17:43:24 GMT  
		Size: 198.7 MB (198719863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b623bef7c51ab75de28495552321d02b2d6b4d6537933d893f18d155b414204a`  
		Last Modified: Sun, 02 Feb 2020 01:31:32 GMT  
		Size: 145.3 MB (145286215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.41-slim`

```console
$ docker pull rust@sha256:9c5a689ef6db939e940e061754a2b9a1841de8f86c2aa597c6fef6e5ceae631f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.41-slim` - linux; amd64

```console
$ docker pull rust@sha256:3fa8907a8030936ddf8785dd8339fc4ac64a8125c17e4a0ad1370524fcf83080
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202144548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:288fd60b2b05cb16b0a07371e5d69a0e30ce6a7d5a809fef31c9e1aad26ed7fd`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Thu, 30 Jan 2020 23:58:40 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:59:12 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4b6ea1105b5642d3cfab2b6fc2e4bc35a7c619b6cf9d1f1a74e56d944416b8`  
		Last Modified: Fri, 31 Jan 2020 00:02:40 GMT  
		Size: 175.1 MB (175052274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41-slim` - linux; arm variant v7

```console
$ docker pull rust@sha256:ff2a1737cb5103afe6786f50a0340e8e52bfabe14523eb58fa1b2f9b8811acc6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.6 MB (197616259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d70333cde16926a90ea171253fd5353a3c875c45e0545febb78c6fd0c9637a0`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 03:17:30 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 03:18:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcd7ca587ec66d5a119fa12058b0cb1efb357adfaf91ad6ce5dc9a8250c6b3b`  
		Last Modified: Sun, 02 Feb 2020 03:22:02 GMT  
		Size: 174.9 MB (174917121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41-slim` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:c332927372fd374053c15e96604081147f07cb23ac35c35e390de9e74a34fa5e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.1 MB (205078984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85242a1a07815d02d847a6d1de41cfca4a9c2e239740d90dd84dd0fada10aef5`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Thu, 30 Jan 2020 23:45:48 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:46:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15b43da91b755c785745bcf6dd8b619aa403485ba00e712b498bc6efb09482d`  
		Last Modified: Thu, 30 Jan 2020 23:49:59 GMT  
		Size: 179.2 MB (179228282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41-slim` - linux; 386

```console
$ docker pull rust@sha256:0b932c1020eee53546fffda34009bc0c6cdbfa0d496e863eb18846d65dd89290
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.0 MB (223015002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b3d3432b91e42b3062b27d190a1f8578b427582a142ec5858e9b2c88a57ca1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 01:27:25 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 01:28:20 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350f4532a56d213c594ac0bc23a3cd8cdc364f385832905798ff101a2cc9136f`  
		Last Modified: Sun, 02 Feb 2020 01:32:45 GMT  
		Size: 195.3 MB (195267950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.41-slim-buster`

```console
$ docker pull rust@sha256:9c5a689ef6db939e940e061754a2b9a1841de8f86c2aa597c6fef6e5ceae631f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.41-slim-buster` - linux; amd64

```console
$ docker pull rust@sha256:3fa8907a8030936ddf8785dd8339fc4ac64a8125c17e4a0ad1370524fcf83080
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202144548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:288fd60b2b05cb16b0a07371e5d69a0e30ce6a7d5a809fef31c9e1aad26ed7fd`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Thu, 30 Jan 2020 23:58:40 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:59:12 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4b6ea1105b5642d3cfab2b6fc2e4bc35a7c619b6cf9d1f1a74e56d944416b8`  
		Last Modified: Fri, 31 Jan 2020 00:02:40 GMT  
		Size: 175.1 MB (175052274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41-slim-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:ff2a1737cb5103afe6786f50a0340e8e52bfabe14523eb58fa1b2f9b8811acc6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.6 MB (197616259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d70333cde16926a90ea171253fd5353a3c875c45e0545febb78c6fd0c9637a0`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 03:17:30 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 03:18:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcd7ca587ec66d5a119fa12058b0cb1efb357adfaf91ad6ce5dc9a8250c6b3b`  
		Last Modified: Sun, 02 Feb 2020 03:22:02 GMT  
		Size: 174.9 MB (174917121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41-slim-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:c332927372fd374053c15e96604081147f07cb23ac35c35e390de9e74a34fa5e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.1 MB (205078984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85242a1a07815d02d847a6d1de41cfca4a9c2e239740d90dd84dd0fada10aef5`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Thu, 30 Jan 2020 23:45:48 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:46:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15b43da91b755c785745bcf6dd8b619aa403485ba00e712b498bc6efb09482d`  
		Last Modified: Thu, 30 Jan 2020 23:49:59 GMT  
		Size: 179.2 MB (179228282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41-slim-buster` - linux; 386

```console
$ docker pull rust@sha256:0b932c1020eee53546fffda34009bc0c6cdbfa0d496e863eb18846d65dd89290
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.0 MB (223015002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b3d3432b91e42b3062b27d190a1f8578b427582a142ec5858e9b2c88a57ca1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 01:27:25 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 01:28:20 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350f4532a56d213c594ac0bc23a3cd8cdc364f385832905798ff101a2cc9136f`  
		Last Modified: Sun, 02 Feb 2020 01:32:45 GMT  
		Size: 195.3 MB (195267950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.41-slim-stretch`

```console
$ docker pull rust@sha256:54c28eb493584efa368f8ad3b842a82f95321479f511c092719071cd6c9da5d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.41-slim-stretch` - linux; amd64

```console
$ docker pull rust@sha256:8988a0ace70a25adc0076a21458d807fa08cecde92a8126c66bd0febdc0f099e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190094499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80efe80a4223e96acebcd908e5ef8fecd93781a5a9fa24de654e0265c7988e26`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:47 GMT
ADD file:90a2c81769a336bed3f731f44a385f2a65b0916f517a0b77c06c224579bf9a9a in / 
# Sat, 28 Dec 2019 04:23:47 GMT
CMD ["bash"]
# Thu, 30 Jan 2020 23:57:50 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:58:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:804555ee037604c40de144f9f8da0d826d38db82f15d74cded32790fe279a8f6`  
		Last Modified: Sat, 28 Dec 2019 04:28:38 GMT  
		Size: 22.5 MB (22524609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56e4802f7cdd484d276f0cfc4639961be839a95b6ffae7e536ae840b4fa5d8a`  
		Last Modified: Fri, 31 Jan 2020 00:01:21 GMT  
		Size: 167.6 MB (167569890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41-slim-stretch` - linux; arm variant v7

```console
$ docker pull rust@sha256:b0379f8ec7a9155f4ff13fa0957914ce3ba88b80ce5c22923c4ead2a9f89e451
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.4 MB (189398124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:690fad015da49bc6b577df128d04eccc8ee0176e7b0a897ed1111100cba598ef`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:04:29 GMT
ADD file:6ac430a42a1f2a6cc8b0a3565e518bd0e3a47b01d524b86cd3dd4e7f4606fd53 in / 
# Sat, 01 Feb 2020 17:04:31 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 03:15:52 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 03:16:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:6bc458b0813423b9e351a5604c0d71a4853d970ea22b23fedc8683af12dbc13c`  
		Last Modified: Sat, 01 Feb 2020 17:11:31 GMT  
		Size: 19.3 MB (19311624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c966b45d91cbdbbddb23863703ccd1856379b3e0d4ad838d8acee8c431b5717f`  
		Last Modified: Sun, 02 Feb 2020 03:20:10 GMT  
		Size: 170.1 MB (170086500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41-slim-stretch` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:b527a9fcdb5d6a90ce0de4fbbc161e962b09a62c009cd1e7114704f286379112
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.0 MB (190038348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea06f0967e1a0beb570f23c6f7dba5d4cf594b4a83455394d7194de9f956c551`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:43:36 GMT
ADD file:ba40f5080cbd89c576c350bfe5acfe16f2ec59636fdb082efc3a8cef66ae7cb7 in / 
# Sat, 28 Dec 2019 04:43:39 GMT
CMD ["bash"]
# Thu, 30 Jan 2020 23:44:29 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:45:11 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:588374d57fdb5120d024340eef3d8927af23a5b806d41b4f049ee430a153c0b4`  
		Last Modified: Sat, 28 Dec 2019 04:49:14 GMT  
		Size: 20.4 MB (20385801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e8a34c9e29def30493e1870ffa929495298009b05360083f22181d4453f839`  
		Last Modified: Thu, 30 Jan 2020 23:48:17 GMT  
		Size: 169.7 MB (169652547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41-slim-stretch` - linux; 386

```console
$ docker pull rust@sha256:b78ee7fab6baf80ca227645cda796eace6e3a676f35bb0d95939452dcc51c55c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.3 MB (210336495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2972082f643a87cf18629e0d194514767086084c493f5ef4811290a49c0bc022`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:07 GMT
ADD file:c9b4696be461d46d96c760441f34e219e229f90bc6946125b2f809218c3456ce in / 
# Sat, 01 Feb 2020 16:42:07 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 01:25:48 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 01:26:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:4f51b031b74b1f7fab6310c197fd7534181ba2db1f0cec6686fb9e9a82abbb9c`  
		Last Modified: Sat, 01 Feb 2020 16:47:27 GMT  
		Size: 23.2 MB (23152156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea943a600d5130a3a8ddcf69ed3eda4147d98c45f6c499d1f940b1bf24f9c28f`  
		Last Modified: Sun, 02 Feb 2020 01:30:26 GMT  
		Size: 187.2 MB (187184339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.41-stretch`

```console
$ docker pull rust@sha256:b37b4a8bf6cd1080fb9a379ee680c2fcc90121d67fb3a04bb76e4484a9544d43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1.41-stretch` - linux; amd64

```console
$ docker pull rust@sha256:ff4627ba92fdf9d566bbd64ace1dc4184125d8e91a71ccd45fdf555fd17ebe52
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **455.1 MB (455102608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b1293d4b2e209d0e4854e3dbaf3ed403291aa20f01b64c71c3e0c1c7330561c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:33 GMT
ADD file:8f7dc710e276f54a3a73d34b6b8fa261950a781d68ceb7401fa18dabc601c5a5 in / 
# Sat, 28 Dec 2019 04:23:34 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:58:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:58:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 04:59:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:00:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Jan 2020 23:57:32 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:57:45 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:146bd6a886182fde06fbf747470b1c89814bc8ab1c96fdf1aef6107171959fe6`  
		Last Modified: Sat, 28 Dec 2019 04:28:25 GMT  
		Size: 45.4 MB (45380744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9935d0c62ace92b388be202275e222007d6cac10b9c1f2c1ea63af38c09ea7ab`  
		Last Modified: Sat, 28 Dec 2019 05:04:30 GMT  
		Size: 10.8 MB (10797221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0efb86e80601b5bbdbb7c406426982c4202d339687c14c3941b364527e2249`  
		Last Modified: Sat, 28 Dec 2019 05:04:28 GMT  
		Size: 4.3 MB (4340114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e705a4c4fd310b96bfb3d7928428e65f0d3f5bad0cd0bda1434aee1d89418468`  
		Last Modified: Sat, 28 Dec 2019 05:04:45 GMT  
		Size: 50.1 MB (50072671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c877b722db6f4d4297c21f07162d21fa6ac6f51d03360f75e24cfa3bcaefe57d`  
		Last Modified: Sat, 28 Dec 2019 05:05:38 GMT  
		Size: 214.8 MB (214840548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec7021710852d02bcf8dc866ab78921203814c4f8cb56c6e0717dd899d3dfb1`  
		Last Modified: Fri, 31 Jan 2020 00:00:33 GMT  
		Size: 129.7 MB (129671310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41-stretch` - linux; arm variant v7

```console
$ docker pull rust@sha256:95479bdf726ea84f8ce541732a071b898f3a87d69d3e8c10641bbaf327830871
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **439.5 MB (439473862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7e4ba4d1c5cd134afc62cb4f59a2673ee4eb0afa5debe20d887b29870da4991`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:04:08 GMT
ADD file:b7fc54d004d962f2cfb469a1aaa9e689e46dfa2554e0cf44c33981d688adc31b in / 
# Sat, 01 Feb 2020 17:04:09 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:18:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:18:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 18:19:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:23:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 03:15:22 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 03:15:44 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:cc3b08e804cce7e88d9df954b76be506569775afe9cf36316f2fa6c5c9bf3d5c`  
		Last Modified: Sat, 01 Feb 2020 17:11:13 GMT  
		Size: 42.1 MB (42108370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa649f4f33c2131c2969e49352ff247ebe5a62a62b83498c3580f883aa35621e`  
		Last Modified: Sat, 01 Feb 2020 18:31:10 GMT  
		Size: 9.5 MB (9498229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901c0c16dce9409a6a020f4b874b40fb3f7d302fe0b4e7a80a87a7cfbab7da04`  
		Last Modified: Sat, 01 Feb 2020 18:31:10 GMT  
		Size: 3.9 MB (3918766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a264d83dc76a4a25b4110827c1ac6cc620c406edb6b2089cd1117aec271ed`  
		Last Modified: Sat, 01 Feb 2020 18:31:32 GMT  
		Size: 46.4 MB (46400091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:854dcba3350bdff3f923ff69f2dec445f47ef5726d3d15bde4242c2ff122aabc`  
		Last Modified: Sat, 01 Feb 2020 18:32:28 GMT  
		Size: 195.5 MB (195523495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ce99acc39da624b324257b529b5859fe714ab94c38fd36224416818be5f43c`  
		Last Modified: Sun, 02 Feb 2020 03:19:13 GMT  
		Size: 142.0 MB (142024911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41-stretch` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:9ecb1e05a3077b32c8bd99e2d9eda52c2b5d79f388b751e61b4f3cfe047fb9ac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **446.3 MB (446292278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f5feafcebe0b3ff73e55d4ca6ee2ffd01eb91352c47ee1da796b47a1d89c8e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:43:15 GMT
ADD file:e439b3c387852978811a6a5a058745ebb9392da7e8936beb4f37ff076e656213 in / 
# Sat, 28 Dec 2019 04:43:17 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:15:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:15:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:16:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:18:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Jan 2020 23:43:59 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:44:18 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:d07bcf5901dfa793fa6b2c4c617e86bcef315b0b092cbfd1a929eefedaf8e3f2`  
		Last Modified: Sat, 28 Dec 2019 04:48:57 GMT  
		Size: 43.2 MB (43166476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f31062581dadb1f69c43e9441040dd46788bf13ae51f20c66929fac82b506b`  
		Last Modified: Sat, 28 Dec 2019 06:24:15 GMT  
		Size: 9.7 MB (9748258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62337a296a607f48a5dc3a7c07639360d98e0e78982ca8e459c832719012f12`  
		Last Modified: Sat, 28 Dec 2019 06:24:15 GMT  
		Size: 4.1 MB (4094448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403697a3e152c7a38ddb9175a90ed2dac97d780421c35949ff80cd67a7d4e596`  
		Last Modified: Sat, 28 Dec 2019 06:24:36 GMT  
		Size: 48.0 MB (48024191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0179cb8c17339f719c763581cefb9e377c016b4f7f4b747a665349e79470363c`  
		Last Modified: Sat, 28 Dec 2019 06:25:35 GMT  
		Size: 202.2 MB (202233183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cddbec6e7f644fe8725ebf72f7dc61a67b27b411e5d4466b522933633e74f5c`  
		Last Modified: Thu, 30 Jan 2020 23:47:26 GMT  
		Size: 139.0 MB (139025722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.41-stretch` - linux; 386

```console
$ docker pull rust@sha256:1f587d401d8a96d2f338101f37a03cd379241fe760d8f8b4d4fa8d073336f6e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.3 MB (478286932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:979e274dc88223c0d7e5b1ad0fb9236195b93a7e3f6d79c11081b5db16cbec8d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:53 GMT
ADD file:bae1646c4e3069e717d1ee4f6c312c249e96a21d795a639cdfaf338d645c8be9 in / 
# Sat, 01 Feb 2020 16:41:53 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:38:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:38:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:39:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:40:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 01:25:09 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 01:25:38 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:97067fdacc0601fe58a5f782cd09d3c58a214c43b8629a2d92bd7025f46fd265`  
		Last Modified: Sat, 01 Feb 2020 16:47:15 GMT  
		Size: 46.1 MB (46100017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1ac2ac579e53fc74848ab743b53ae2f6e54350989c71359d435c2fef2e5157`  
		Last Modified: Sat, 01 Feb 2020 17:45:45 GMT  
		Size: 10.8 MB (10817587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f7b32e68627ad71130644b1646afb1aa0bcf1f440df145526a73fdbd413f3b`  
		Last Modified: Sat, 01 Feb 2020 17:45:43 GMT  
		Size: 4.6 MB (4561467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b926c1ce2d1cf6b99c32683bf0fd0233d4f71f367d38a16de2ba08e9ecbf1cc2`  
		Last Modified: Sat, 01 Feb 2020 17:46:05 GMT  
		Size: 51.6 MB (51595566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac9b89be3409f23bc9ac380bcfd9f28e0cc2e52b69b8706e0b102211c83abf4`  
		Last Modified: Sat, 01 Feb 2020 17:47:03 GMT  
		Size: 219.9 MB (219925297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69feda6b3fd089c07ee45b4a40f729a67e99bfa21dc5b5eede2fc9efc22d3d01`  
		Last Modified: Sun, 02 Feb 2020 01:29:25 GMT  
		Size: 145.3 MB (145286998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-alpine`

```console
$ docker pull rust@sha256:174277b6eb8de98ba66882a88b81e9dc8bce7864d3b4c7e1471778d1d2d368a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1-alpine` - linux; amd64

```console
$ docker pull rust@sha256:fe545e8f5ad12baa7ce768a7fed3ca081647cf324fe2e3282df1a7a37a8b5e63
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.3 MB (133272665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f952798c43f276fb7cacefa3fa22ba95226a2a8554669dbd559dce10b4b7b74`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Tue, 21 Jan 2020 21:26:53 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 30 Jan 2020 23:59:32 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:59:41 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.21.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "0c86d467982bdf5c4b8d844bf8c3f7fc602cc4ac30b29262b8941d6d8b363d7e *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409bef176e35cb7d5f61284ce84fc883b72774cc0736c7286117d258c6bf7a3e`  
		Last Modified: Tue, 21 Jan 2020 21:27:29 GMT  
		Size: 36.4 MB (36417023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed492dc040c10c2f241f489b18b5cf7cc4dd2808c83d6544d5e5e563180e096`  
		Last Modified: Fri, 31 Jan 2020 00:03:25 GMT  
		Size: 94.1 MB (94052685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-alpine3.10`

```console
$ docker pull rust@sha256:e199301d1242c027a8d532ea1b976cb5f1063af6f1bee394c539b94fee66cf28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1-alpine3.10` - linux; amd64

```console
$ docker pull rust@sha256:06a34ea0c8dca19912d7c326664f636f94e520d2cce1b2af55f3d3e6881936fe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.8 MB (130823278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:718c95e2d38f3cbcec4c7e0237dc2ef6fb5c5d5428bb5b3e67d50a421f0aec19`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 05:59:59 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 30 Jan 2020 23:59:19 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:59:28 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.21.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "0c86d467982bdf5c4b8d844bf8c3f7fc602cc4ac30b29262b8941d6d8b363d7e *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4894ab3ba23d1a77df9f98d547d9f3afeb033693fd523558a1e88651178b4d54`  
		Last Modified: Fri, 24 Jan 2020 06:01:10 GMT  
		Size: 34.0 MB (33983603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b138b4be762363e564b1547030500da8ddb0c0262f2e4430ec61192a46790b`  
		Last Modified: Fri, 31 Jan 2020 00:03:04 GMT  
		Size: 94.1 MB (94052713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-alpine3.11`

```console
$ docker pull rust@sha256:174277b6eb8de98ba66882a88b81e9dc8bce7864d3b4c7e1471778d1d2d368a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:1-alpine3.11` - linux; amd64

```console
$ docker pull rust@sha256:fe545e8f5ad12baa7ce768a7fed3ca081647cf324fe2e3282df1a7a37a8b5e63
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.3 MB (133272665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f952798c43f276fb7cacefa3fa22ba95226a2a8554669dbd559dce10b4b7b74`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Tue, 21 Jan 2020 21:26:53 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 30 Jan 2020 23:59:32 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:59:41 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.21.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "0c86d467982bdf5c4b8d844bf8c3f7fc602cc4ac30b29262b8941d6d8b363d7e *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409bef176e35cb7d5f61284ce84fc883b72774cc0736c7286117d258c6bf7a3e`  
		Last Modified: Tue, 21 Jan 2020 21:27:29 GMT  
		Size: 36.4 MB (36417023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed492dc040c10c2f241f489b18b5cf7cc4dd2808c83d6544d5e5e563180e096`  
		Last Modified: Fri, 31 Jan 2020 00:03:25 GMT  
		Size: 94.1 MB (94052685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-buster`

```console
$ docker pull rust@sha256:920b5c1b275778169a8c35f767c9c238ac9391f8a666d3ee159a1a2a26088a25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-buster` - linux; amd64

```console
$ docker pull rust@sha256:d59df245b22bfef90c2d29c1691e6a3ff679feb95d400b69626bae74898efab3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.7 MB (441693460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db33159e3388e178392ca314fbd8ecebb9fb430b73a29538302486e29cec6bc1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:08 GMT
ADD file:d6d0bdf8cb07a7a0dc32e9df50ac80ca1a524c3fa48136892ded195061f2194c in / 
# Sat, 28 Dec 2019 04:21:09 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:47:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:47:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 04:47:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:48:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Jan 2020 23:58:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:58:35 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:8f0fdd3eaac017684c880d836abdaf02f9db7ac8ecca970356482e3d8e315650`  
		Last Modified: Sat, 28 Dec 2019 04:25:39 GMT  
		Size: 50.4 MB (50379720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d918eaefd9de8a1595f56900fdb8ab65a03d64b1da1078da7c0b0bf6f7552a14`  
		Last Modified: Sat, 28 Dec 2019 05:01:44 GMT  
		Size: 7.8 MB (7811715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bf3e3107f525b7dea5b3cdfd15f62666066202105a0aaddbab2a02aefad1f7`  
		Last Modified: Sat, 28 Dec 2019 05:01:44 GMT  
		Size: 10.0 MB (9996202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27622921edb2aae9e0cb64f71a81b4a7cfef8f6a6c766514a018815834ba4e14`  
		Last Modified: Sat, 28 Dec 2019 05:02:00 GMT  
		Size: 51.8 MB (51790562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfa0aa1ae2c54d0de4b6ad0ee4d9f795c93368ae7d87801784c1f8ae624ac33`  
		Last Modified: Sat, 28 Dec 2019 05:02:36 GMT  
		Size: 192.0 MB (192044395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b109c91c0639fd55a93a5688b1bc7501e434396daabd93d714b72b106996a82a`  
		Last Modified: Fri, 31 Jan 2020 00:01:48 GMT  
		Size: 129.7 MB (129670866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:f4b13a8a2df73cfd225ce928f3574e1169b288e8448e004659d35d303ba1b82f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **420.0 MB (420018522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af6c4b7927d04a1c76f6b24226aa2702d2a7de368154e22aa531e7e986d7c227`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:06 GMT
ADD file:a57a312731f174c4b03031908ff95f49d7055d8c196439f0ed07ed9c4834d993 in / 
# Sat, 01 Feb 2020 17:00:08 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:00:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 18:01:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:03:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 03:16:56 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 03:17:21 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9bbb41bca8c6254da5088d03354297b1309dc75c2ccc738416025f89709ae5ee`  
		Last Modified: Sat, 01 Feb 2020 17:07:28 GMT  
		Size: 45.9 MB (45859700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239e4acdbc2ab88c89aa359fbab11429ea6d7bd93ea589a22c6bbb833ff82b93`  
		Last Modified: Sat, 01 Feb 2020 18:25:50 GMT  
		Size: 7.1 MB (7096223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6b4707a3c3aff9cb939fc058b869c5412e78c37e43eb0b653565460495537`  
		Last Modified: Sat, 01 Feb 2020 18:25:50 GMT  
		Size: 9.3 MB (9343278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e096c4fc8c629edca6da3ce5a9e95288512cb11e3d3d01a6e49078d19c2acca`  
		Last Modified: Sat, 01 Feb 2020 18:26:13 GMT  
		Size: 47.3 MB (47315591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6953ecf4273071529462518748f048f49a05530ae24d8fc6841919de312f2fc`  
		Last Modified: Sat, 01 Feb 2020 18:27:03 GMT  
		Size: 168.4 MB (168379144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f84f54aa922c34c20237ad8b624417ee33ea2f0c7940b127d3043d241b53bd`  
		Last Modified: Sun, 02 Feb 2020 03:21:00 GMT  
		Size: 142.0 MB (142024586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:cc4933ffae4311c25299ae5b6a8e115241533bed5ca5e71dd7df717e0ca3b760
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.5 MB (441531085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:779e2f51436aa1328b240e1b38f7b6758d6acb69f2a4eae5f652148e28a16a8e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:40:41 GMT
ADD file:88b3d02fc98aa9138e694bee7d5d1b61b295e4a1c7fae399bf24e52eeff7a5ae in / 
# Sat, 28 Dec 2019 04:40:45 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:04:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:05:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:05:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:08:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Jan 2020 23:45:22 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:45:39 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:627706d65d1d9b4038d8fd40db52238d4f11d9130a01f23ffae9bf5d41ac5933`  
		Last Modified: Sat, 28 Dec 2019 04:46:38 GMT  
		Size: 49.2 MB (49171876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ac1923ab7a97ecdde2a4f034a8b716d51594ba6fc823c6aaac579c31f51906`  
		Last Modified: Sat, 28 Dec 2019 06:21:16 GMT  
		Size: 7.7 MB (7681148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b000e01546d5b9b3a40a3797f15bc0a1f579786c5ec8da31cbe9502f1927d367`  
		Last Modified: Sat, 28 Dec 2019 06:21:16 GMT  
		Size: 10.0 MB (9983835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8fe6ebd465d85dc79039fbd39712f1fadf5d7ac5fbefe405ef7a4f957a94ce`  
		Last Modified: Sat, 28 Dec 2019 06:21:39 GMT  
		Size: 52.1 MB (52102816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d739211b59b4a5cab55db8d8ce73eb5edfb9d5d91addf9f7aab0b9d9fa90b06`  
		Last Modified: Sat, 28 Dec 2019 06:22:32 GMT  
		Size: 183.6 MB (183566016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cff33cb79d34d36837bc747d7bd54401995ea5a541d92619b14c3ab0c8e2eb`  
		Last Modified: Thu, 30 Jan 2020 23:48:59 GMT  
		Size: 139.0 MB (139025394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-buster` - linux; 386

```console
$ docker pull rust@sha256:e1de980dfbedecb976f80c981e8ce689d9abd5cb15cff9306ada02436a5e4465
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.8 MB (466848765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:158b1b1e4c720838da8354351980c8022084cbec76ba03427a8a8699853c514f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:21 GMT
ADD file:b637f96d557a570f8ab83b28f7b9cdd128958359dd30dc2e03df70b799e132aa in / 
# Sat, 01 Feb 2020 16:39:21 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:23:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:24:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:24:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:25:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 01:26:51 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 01:27:16 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:2b34644a479c82db66a603c0b0a1d990911345f8646498fa9b050f306d0e6bf2`  
		Last Modified: Sat, 01 Feb 2020 16:44:10 GMT  
		Size: 51.1 MB (51141949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2f611c9392c4fe86735b477d61fda0e95ea77486175a737114c51586ecce86`  
		Last Modified: Sat, 01 Feb 2020 17:42:17 GMT  
		Size: 8.0 MB (7981506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69713757cc2d87c3255331d40f5061a73ef412208961f1ddd67a59a375397fda`  
		Last Modified: Sat, 01 Feb 2020 17:42:17 GMT  
		Size: 10.3 MB (10338479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956cf07a321afcfed99809a380a1905660e378188fd33d97f136551450be347a`  
		Last Modified: Sat, 01 Feb 2020 17:42:36 GMT  
		Size: 53.4 MB (53380753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8bfbd246f3a4ba9d861315c676a9a9e6524857c085e71b18b492882b063bff`  
		Last Modified: Sat, 01 Feb 2020 17:43:24 GMT  
		Size: 198.7 MB (198719863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b623bef7c51ab75de28495552321d02b2d6b4d6537933d893f18d155b414204a`  
		Last Modified: Sun, 02 Feb 2020 01:31:32 GMT  
		Size: 145.3 MB (145286215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-slim`

```console
$ docker pull rust@sha256:9c5a689ef6db939e940e061754a2b9a1841de8f86c2aa597c6fef6e5ceae631f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-slim` - linux; amd64

```console
$ docker pull rust@sha256:3fa8907a8030936ddf8785dd8339fc4ac64a8125c17e4a0ad1370524fcf83080
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202144548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:288fd60b2b05cb16b0a07371e5d69a0e30ce6a7d5a809fef31c9e1aad26ed7fd`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Thu, 30 Jan 2020 23:58:40 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:59:12 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4b6ea1105b5642d3cfab2b6fc2e4bc35a7c619b6cf9d1f1a74e56d944416b8`  
		Last Modified: Fri, 31 Jan 2020 00:02:40 GMT  
		Size: 175.1 MB (175052274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim` - linux; arm variant v7

```console
$ docker pull rust@sha256:ff2a1737cb5103afe6786f50a0340e8e52bfabe14523eb58fa1b2f9b8811acc6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.6 MB (197616259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d70333cde16926a90ea171253fd5353a3c875c45e0545febb78c6fd0c9637a0`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 03:17:30 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 03:18:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcd7ca587ec66d5a119fa12058b0cb1efb357adfaf91ad6ce5dc9a8250c6b3b`  
		Last Modified: Sun, 02 Feb 2020 03:22:02 GMT  
		Size: 174.9 MB (174917121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:c332927372fd374053c15e96604081147f07cb23ac35c35e390de9e74a34fa5e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.1 MB (205078984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85242a1a07815d02d847a6d1de41cfca4a9c2e239740d90dd84dd0fada10aef5`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Thu, 30 Jan 2020 23:45:48 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:46:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15b43da91b755c785745bcf6dd8b619aa403485ba00e712b498bc6efb09482d`  
		Last Modified: Thu, 30 Jan 2020 23:49:59 GMT  
		Size: 179.2 MB (179228282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim` - linux; 386

```console
$ docker pull rust@sha256:0b932c1020eee53546fffda34009bc0c6cdbfa0d496e863eb18846d65dd89290
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.0 MB (223015002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b3d3432b91e42b3062b27d190a1f8578b427582a142ec5858e9b2c88a57ca1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 01:27:25 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 01:28:20 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350f4532a56d213c594ac0bc23a3cd8cdc364f385832905798ff101a2cc9136f`  
		Last Modified: Sun, 02 Feb 2020 01:32:45 GMT  
		Size: 195.3 MB (195267950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-slim-buster`

```console
$ docker pull rust@sha256:9c5a689ef6db939e940e061754a2b9a1841de8f86c2aa597c6fef6e5ceae631f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-slim-buster` - linux; amd64

```console
$ docker pull rust@sha256:3fa8907a8030936ddf8785dd8339fc4ac64a8125c17e4a0ad1370524fcf83080
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202144548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:288fd60b2b05cb16b0a07371e5d69a0e30ce6a7d5a809fef31c9e1aad26ed7fd`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Thu, 30 Jan 2020 23:58:40 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:59:12 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4b6ea1105b5642d3cfab2b6fc2e4bc35a7c619b6cf9d1f1a74e56d944416b8`  
		Last Modified: Fri, 31 Jan 2020 00:02:40 GMT  
		Size: 175.1 MB (175052274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:ff2a1737cb5103afe6786f50a0340e8e52bfabe14523eb58fa1b2f9b8811acc6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.6 MB (197616259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d70333cde16926a90ea171253fd5353a3c875c45e0545febb78c6fd0c9637a0`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 03:17:30 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 03:18:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcd7ca587ec66d5a119fa12058b0cb1efb357adfaf91ad6ce5dc9a8250c6b3b`  
		Last Modified: Sun, 02 Feb 2020 03:22:02 GMT  
		Size: 174.9 MB (174917121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:c332927372fd374053c15e96604081147f07cb23ac35c35e390de9e74a34fa5e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.1 MB (205078984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85242a1a07815d02d847a6d1de41cfca4a9c2e239740d90dd84dd0fada10aef5`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Thu, 30 Jan 2020 23:45:48 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:46:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15b43da91b755c785745bcf6dd8b619aa403485ba00e712b498bc6efb09482d`  
		Last Modified: Thu, 30 Jan 2020 23:49:59 GMT  
		Size: 179.2 MB (179228282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-buster` - linux; 386

```console
$ docker pull rust@sha256:0b932c1020eee53546fffda34009bc0c6cdbfa0d496e863eb18846d65dd89290
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.0 MB (223015002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b3d3432b91e42b3062b27d190a1f8578b427582a142ec5858e9b2c88a57ca1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 01:27:25 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 01:28:20 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350f4532a56d213c594ac0bc23a3cd8cdc364f385832905798ff101a2cc9136f`  
		Last Modified: Sun, 02 Feb 2020 01:32:45 GMT  
		Size: 195.3 MB (195267950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-slim-stretch`

```console
$ docker pull rust@sha256:54c28eb493584efa368f8ad3b842a82f95321479f511c092719071cd6c9da5d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-slim-stretch` - linux; amd64

```console
$ docker pull rust@sha256:8988a0ace70a25adc0076a21458d807fa08cecde92a8126c66bd0febdc0f099e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190094499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80efe80a4223e96acebcd908e5ef8fecd93781a5a9fa24de654e0265c7988e26`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:47 GMT
ADD file:90a2c81769a336bed3f731f44a385f2a65b0916f517a0b77c06c224579bf9a9a in / 
# Sat, 28 Dec 2019 04:23:47 GMT
CMD ["bash"]
# Thu, 30 Jan 2020 23:57:50 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:58:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:804555ee037604c40de144f9f8da0d826d38db82f15d74cded32790fe279a8f6`  
		Last Modified: Sat, 28 Dec 2019 04:28:38 GMT  
		Size: 22.5 MB (22524609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56e4802f7cdd484d276f0cfc4639961be839a95b6ffae7e536ae840b4fa5d8a`  
		Last Modified: Fri, 31 Jan 2020 00:01:21 GMT  
		Size: 167.6 MB (167569890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-stretch` - linux; arm variant v7

```console
$ docker pull rust@sha256:b0379f8ec7a9155f4ff13fa0957914ce3ba88b80ce5c22923c4ead2a9f89e451
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.4 MB (189398124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:690fad015da49bc6b577df128d04eccc8ee0176e7b0a897ed1111100cba598ef`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:04:29 GMT
ADD file:6ac430a42a1f2a6cc8b0a3565e518bd0e3a47b01d524b86cd3dd4e7f4606fd53 in / 
# Sat, 01 Feb 2020 17:04:31 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 03:15:52 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 03:16:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:6bc458b0813423b9e351a5604c0d71a4853d970ea22b23fedc8683af12dbc13c`  
		Last Modified: Sat, 01 Feb 2020 17:11:31 GMT  
		Size: 19.3 MB (19311624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c966b45d91cbdbbddb23863703ccd1856379b3e0d4ad838d8acee8c431b5717f`  
		Last Modified: Sun, 02 Feb 2020 03:20:10 GMT  
		Size: 170.1 MB (170086500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-stretch` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:b527a9fcdb5d6a90ce0de4fbbc161e962b09a62c009cd1e7114704f286379112
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.0 MB (190038348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea06f0967e1a0beb570f23c6f7dba5d4cf594b4a83455394d7194de9f956c551`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:43:36 GMT
ADD file:ba40f5080cbd89c576c350bfe5acfe16f2ec59636fdb082efc3a8cef66ae7cb7 in / 
# Sat, 28 Dec 2019 04:43:39 GMT
CMD ["bash"]
# Thu, 30 Jan 2020 23:44:29 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:45:11 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:588374d57fdb5120d024340eef3d8927af23a5b806d41b4f049ee430a153c0b4`  
		Last Modified: Sat, 28 Dec 2019 04:49:14 GMT  
		Size: 20.4 MB (20385801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e8a34c9e29def30493e1870ffa929495298009b05360083f22181d4453f839`  
		Last Modified: Thu, 30 Jan 2020 23:48:17 GMT  
		Size: 169.7 MB (169652547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-stretch` - linux; 386

```console
$ docker pull rust@sha256:b78ee7fab6baf80ca227645cda796eace6e3a676f35bb0d95939452dcc51c55c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.3 MB (210336495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2972082f643a87cf18629e0d194514767086084c493f5ef4811290a49c0bc022`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:07 GMT
ADD file:c9b4696be461d46d96c760441f34e219e229f90bc6946125b2f809218c3456ce in / 
# Sat, 01 Feb 2020 16:42:07 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 01:25:48 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 01:26:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:4f51b031b74b1f7fab6310c197fd7534181ba2db1f0cec6686fb9e9a82abbb9c`  
		Last Modified: Sat, 01 Feb 2020 16:47:27 GMT  
		Size: 23.2 MB (23152156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea943a600d5130a3a8ddcf69ed3eda4147d98c45f6c499d1f940b1bf24f9c28f`  
		Last Modified: Sun, 02 Feb 2020 01:30:26 GMT  
		Size: 187.2 MB (187184339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-stretch`

```console
$ docker pull rust@sha256:b37b4a8bf6cd1080fb9a379ee680c2fcc90121d67fb3a04bb76e4484a9544d43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-stretch` - linux; amd64

```console
$ docker pull rust@sha256:ff4627ba92fdf9d566bbd64ace1dc4184125d8e91a71ccd45fdf555fd17ebe52
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **455.1 MB (455102608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b1293d4b2e209d0e4854e3dbaf3ed403291aa20f01b64c71c3e0c1c7330561c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:33 GMT
ADD file:8f7dc710e276f54a3a73d34b6b8fa261950a781d68ceb7401fa18dabc601c5a5 in / 
# Sat, 28 Dec 2019 04:23:34 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:58:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:58:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 04:59:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:00:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Jan 2020 23:57:32 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:57:45 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:146bd6a886182fde06fbf747470b1c89814bc8ab1c96fdf1aef6107171959fe6`  
		Last Modified: Sat, 28 Dec 2019 04:28:25 GMT  
		Size: 45.4 MB (45380744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9935d0c62ace92b388be202275e222007d6cac10b9c1f2c1ea63af38c09ea7ab`  
		Last Modified: Sat, 28 Dec 2019 05:04:30 GMT  
		Size: 10.8 MB (10797221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0efb86e80601b5bbdbb7c406426982c4202d339687c14c3941b364527e2249`  
		Last Modified: Sat, 28 Dec 2019 05:04:28 GMT  
		Size: 4.3 MB (4340114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e705a4c4fd310b96bfb3d7928428e65f0d3f5bad0cd0bda1434aee1d89418468`  
		Last Modified: Sat, 28 Dec 2019 05:04:45 GMT  
		Size: 50.1 MB (50072671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c877b722db6f4d4297c21f07162d21fa6ac6f51d03360f75e24cfa3bcaefe57d`  
		Last Modified: Sat, 28 Dec 2019 05:05:38 GMT  
		Size: 214.8 MB (214840548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec7021710852d02bcf8dc866ab78921203814c4f8cb56c6e0717dd899d3dfb1`  
		Last Modified: Fri, 31 Jan 2020 00:00:33 GMT  
		Size: 129.7 MB (129671310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-stretch` - linux; arm variant v7

```console
$ docker pull rust@sha256:95479bdf726ea84f8ce541732a071b898f3a87d69d3e8c10641bbaf327830871
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **439.5 MB (439473862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7e4ba4d1c5cd134afc62cb4f59a2673ee4eb0afa5debe20d887b29870da4991`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:04:08 GMT
ADD file:b7fc54d004d962f2cfb469a1aaa9e689e46dfa2554e0cf44c33981d688adc31b in / 
# Sat, 01 Feb 2020 17:04:09 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:18:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:18:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 18:19:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:23:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 03:15:22 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 03:15:44 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:cc3b08e804cce7e88d9df954b76be506569775afe9cf36316f2fa6c5c9bf3d5c`  
		Last Modified: Sat, 01 Feb 2020 17:11:13 GMT  
		Size: 42.1 MB (42108370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa649f4f33c2131c2969e49352ff247ebe5a62a62b83498c3580f883aa35621e`  
		Last Modified: Sat, 01 Feb 2020 18:31:10 GMT  
		Size: 9.5 MB (9498229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901c0c16dce9409a6a020f4b874b40fb3f7d302fe0b4e7a80a87a7cfbab7da04`  
		Last Modified: Sat, 01 Feb 2020 18:31:10 GMT  
		Size: 3.9 MB (3918766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a264d83dc76a4a25b4110827c1ac6cc620c406edb6b2089cd1117aec271ed`  
		Last Modified: Sat, 01 Feb 2020 18:31:32 GMT  
		Size: 46.4 MB (46400091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:854dcba3350bdff3f923ff69f2dec445f47ef5726d3d15bde4242c2ff122aabc`  
		Last Modified: Sat, 01 Feb 2020 18:32:28 GMT  
		Size: 195.5 MB (195523495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ce99acc39da624b324257b529b5859fe714ab94c38fd36224416818be5f43c`  
		Last Modified: Sun, 02 Feb 2020 03:19:13 GMT  
		Size: 142.0 MB (142024911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-stretch` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:9ecb1e05a3077b32c8bd99e2d9eda52c2b5d79f388b751e61b4f3cfe047fb9ac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **446.3 MB (446292278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f5feafcebe0b3ff73e55d4ca6ee2ffd01eb91352c47ee1da796b47a1d89c8e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:43:15 GMT
ADD file:e439b3c387852978811a6a5a058745ebb9392da7e8936beb4f37ff076e656213 in / 
# Sat, 28 Dec 2019 04:43:17 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:15:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:15:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:16:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:18:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Jan 2020 23:43:59 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:44:18 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:d07bcf5901dfa793fa6b2c4c617e86bcef315b0b092cbfd1a929eefedaf8e3f2`  
		Last Modified: Sat, 28 Dec 2019 04:48:57 GMT  
		Size: 43.2 MB (43166476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f31062581dadb1f69c43e9441040dd46788bf13ae51f20c66929fac82b506b`  
		Last Modified: Sat, 28 Dec 2019 06:24:15 GMT  
		Size: 9.7 MB (9748258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62337a296a607f48a5dc3a7c07639360d98e0e78982ca8e459c832719012f12`  
		Last Modified: Sat, 28 Dec 2019 06:24:15 GMT  
		Size: 4.1 MB (4094448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403697a3e152c7a38ddb9175a90ed2dac97d780421c35949ff80cd67a7d4e596`  
		Last Modified: Sat, 28 Dec 2019 06:24:36 GMT  
		Size: 48.0 MB (48024191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0179cb8c17339f719c763581cefb9e377c016b4f7f4b747a665349e79470363c`  
		Last Modified: Sat, 28 Dec 2019 06:25:35 GMT  
		Size: 202.2 MB (202233183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cddbec6e7f644fe8725ebf72f7dc61a67b27b411e5d4466b522933633e74f5c`  
		Last Modified: Thu, 30 Jan 2020 23:47:26 GMT  
		Size: 139.0 MB (139025722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-stretch` - linux; 386

```console
$ docker pull rust@sha256:1f587d401d8a96d2f338101f37a03cd379241fe760d8f8b4d4fa8d073336f6e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.3 MB (478286932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:979e274dc88223c0d7e5b1ad0fb9236195b93a7e3f6d79c11081b5db16cbec8d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:53 GMT
ADD file:bae1646c4e3069e717d1ee4f6c312c249e96a21d795a639cdfaf338d645c8be9 in / 
# Sat, 01 Feb 2020 16:41:53 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:38:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:38:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:39:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:40:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 01:25:09 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 01:25:38 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:97067fdacc0601fe58a5f782cd09d3c58a214c43b8629a2d92bd7025f46fd265`  
		Last Modified: Sat, 01 Feb 2020 16:47:15 GMT  
		Size: 46.1 MB (46100017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1ac2ac579e53fc74848ab743b53ae2f6e54350989c71359d435c2fef2e5157`  
		Last Modified: Sat, 01 Feb 2020 17:45:45 GMT  
		Size: 10.8 MB (10817587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f7b32e68627ad71130644b1646afb1aa0bcf1f440df145526a73fdbd413f3b`  
		Last Modified: Sat, 01 Feb 2020 17:45:43 GMT  
		Size: 4.6 MB (4561467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b926c1ce2d1cf6b99c32683bf0fd0233d4f71f367d38a16de2ba08e9ecbf1cc2`  
		Last Modified: Sat, 01 Feb 2020 17:46:05 GMT  
		Size: 51.6 MB (51595566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac9b89be3409f23bc9ac380bcfd9f28e0cc2e52b69b8706e0b102211c83abf4`  
		Last Modified: Sat, 01 Feb 2020 17:47:03 GMT  
		Size: 219.9 MB (219925297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69feda6b3fd089c07ee45b4a40f729a67e99bfa21dc5b5eede2fc9efc22d3d01`  
		Last Modified: Sun, 02 Feb 2020 01:29:25 GMT  
		Size: 145.3 MB (145286998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:alpine`

```console
$ docker pull rust@sha256:174277b6eb8de98ba66882a88b81e9dc8bce7864d3b4c7e1471778d1d2d368a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:alpine` - linux; amd64

```console
$ docker pull rust@sha256:fe545e8f5ad12baa7ce768a7fed3ca081647cf324fe2e3282df1a7a37a8b5e63
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.3 MB (133272665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f952798c43f276fb7cacefa3fa22ba95226a2a8554669dbd559dce10b4b7b74`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Tue, 21 Jan 2020 21:26:53 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 30 Jan 2020 23:59:32 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:59:41 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.21.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "0c86d467982bdf5c4b8d844bf8c3f7fc602cc4ac30b29262b8941d6d8b363d7e *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409bef176e35cb7d5f61284ce84fc883b72774cc0736c7286117d258c6bf7a3e`  
		Last Modified: Tue, 21 Jan 2020 21:27:29 GMT  
		Size: 36.4 MB (36417023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed492dc040c10c2f241f489b18b5cf7cc4dd2808c83d6544d5e5e563180e096`  
		Last Modified: Fri, 31 Jan 2020 00:03:25 GMT  
		Size: 94.1 MB (94052685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:alpine3.10`

```console
$ docker pull rust@sha256:e199301d1242c027a8d532ea1b976cb5f1063af6f1bee394c539b94fee66cf28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:alpine3.10` - linux; amd64

```console
$ docker pull rust@sha256:06a34ea0c8dca19912d7c326664f636f94e520d2cce1b2af55f3d3e6881936fe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.8 MB (130823278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:718c95e2d38f3cbcec4c7e0237dc2ef6fb5c5d5428bb5b3e67d50a421f0aec19`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 05:59:59 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 30 Jan 2020 23:59:19 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:59:28 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.21.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "0c86d467982bdf5c4b8d844bf8c3f7fc602cc4ac30b29262b8941d6d8b363d7e *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4894ab3ba23d1a77df9f98d547d9f3afeb033693fd523558a1e88651178b4d54`  
		Last Modified: Fri, 24 Jan 2020 06:01:10 GMT  
		Size: 34.0 MB (33983603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b138b4be762363e564b1547030500da8ddb0c0262f2e4430ec61192a46790b`  
		Last Modified: Fri, 31 Jan 2020 00:03:04 GMT  
		Size: 94.1 MB (94052713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:alpine3.11`

```console
$ docker pull rust@sha256:174277b6eb8de98ba66882a88b81e9dc8bce7864d3b4c7e1471778d1d2d368a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rust:alpine3.11` - linux; amd64

```console
$ docker pull rust@sha256:fe545e8f5ad12baa7ce768a7fed3ca081647cf324fe2e3282df1a7a37a8b5e63
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.3 MB (133272665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f952798c43f276fb7cacefa3fa22ba95226a2a8554669dbd559dce10b4b7b74`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Tue, 21 Jan 2020 21:26:53 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 30 Jan 2020 23:59:32 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:59:41 GMT
RUN set -eux;     url="https://static.rust-lang.org/rustup/archive/1.21.1/x86_64-unknown-linux-musl/rustup-init";     wget "$url";     echo "0c86d467982bdf5c4b8d844bf8c3f7fc602cc4ac30b29262b8941d6d8b363d7e *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409bef176e35cb7d5f61284ce84fc883b72774cc0736c7286117d258c6bf7a3e`  
		Last Modified: Tue, 21 Jan 2020 21:27:29 GMT  
		Size: 36.4 MB (36417023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed492dc040c10c2f241f489b18b5cf7cc4dd2808c83d6544d5e5e563180e096`  
		Last Modified: Fri, 31 Jan 2020 00:03:25 GMT  
		Size: 94.1 MB (94052685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:buster`

```console
$ docker pull rust@sha256:920b5c1b275778169a8c35f767c9c238ac9391f8a666d3ee159a1a2a26088a25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:buster` - linux; amd64

```console
$ docker pull rust@sha256:d59df245b22bfef90c2d29c1691e6a3ff679feb95d400b69626bae74898efab3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.7 MB (441693460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db33159e3388e178392ca314fbd8ecebb9fb430b73a29538302486e29cec6bc1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:08 GMT
ADD file:d6d0bdf8cb07a7a0dc32e9df50ac80ca1a524c3fa48136892ded195061f2194c in / 
# Sat, 28 Dec 2019 04:21:09 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:47:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:47:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 04:47:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:48:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Jan 2020 23:58:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:58:35 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:8f0fdd3eaac017684c880d836abdaf02f9db7ac8ecca970356482e3d8e315650`  
		Last Modified: Sat, 28 Dec 2019 04:25:39 GMT  
		Size: 50.4 MB (50379720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d918eaefd9de8a1595f56900fdb8ab65a03d64b1da1078da7c0b0bf6f7552a14`  
		Last Modified: Sat, 28 Dec 2019 05:01:44 GMT  
		Size: 7.8 MB (7811715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bf3e3107f525b7dea5b3cdfd15f62666066202105a0aaddbab2a02aefad1f7`  
		Last Modified: Sat, 28 Dec 2019 05:01:44 GMT  
		Size: 10.0 MB (9996202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27622921edb2aae9e0cb64f71a81b4a7cfef8f6a6c766514a018815834ba4e14`  
		Last Modified: Sat, 28 Dec 2019 05:02:00 GMT  
		Size: 51.8 MB (51790562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfa0aa1ae2c54d0de4b6ad0ee4d9f795c93368ae7d87801784c1f8ae624ac33`  
		Last Modified: Sat, 28 Dec 2019 05:02:36 GMT  
		Size: 192.0 MB (192044395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b109c91c0639fd55a93a5688b1bc7501e434396daabd93d714b72b106996a82a`  
		Last Modified: Fri, 31 Jan 2020 00:01:48 GMT  
		Size: 129.7 MB (129670866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:f4b13a8a2df73cfd225ce928f3574e1169b288e8448e004659d35d303ba1b82f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **420.0 MB (420018522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af6c4b7927d04a1c76f6b24226aa2702d2a7de368154e22aa531e7e986d7c227`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:06 GMT
ADD file:a57a312731f174c4b03031908ff95f49d7055d8c196439f0ed07ed9c4834d993 in / 
# Sat, 01 Feb 2020 17:00:08 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:00:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 18:01:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:03:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 03:16:56 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 03:17:21 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9bbb41bca8c6254da5088d03354297b1309dc75c2ccc738416025f89709ae5ee`  
		Last Modified: Sat, 01 Feb 2020 17:07:28 GMT  
		Size: 45.9 MB (45859700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239e4acdbc2ab88c89aa359fbab11429ea6d7bd93ea589a22c6bbb833ff82b93`  
		Last Modified: Sat, 01 Feb 2020 18:25:50 GMT  
		Size: 7.1 MB (7096223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6b4707a3c3aff9cb939fc058b869c5412e78c37e43eb0b653565460495537`  
		Last Modified: Sat, 01 Feb 2020 18:25:50 GMT  
		Size: 9.3 MB (9343278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e096c4fc8c629edca6da3ce5a9e95288512cb11e3d3d01a6e49078d19c2acca`  
		Last Modified: Sat, 01 Feb 2020 18:26:13 GMT  
		Size: 47.3 MB (47315591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6953ecf4273071529462518748f048f49a05530ae24d8fc6841919de312f2fc`  
		Last Modified: Sat, 01 Feb 2020 18:27:03 GMT  
		Size: 168.4 MB (168379144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f84f54aa922c34c20237ad8b624417ee33ea2f0c7940b127d3043d241b53bd`  
		Last Modified: Sun, 02 Feb 2020 03:21:00 GMT  
		Size: 142.0 MB (142024586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:cc4933ffae4311c25299ae5b6a8e115241533bed5ca5e71dd7df717e0ca3b760
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.5 MB (441531085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:779e2f51436aa1328b240e1b38f7b6758d6acb69f2a4eae5f652148e28a16a8e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:40:41 GMT
ADD file:88b3d02fc98aa9138e694bee7d5d1b61b295e4a1c7fae399bf24e52eeff7a5ae in / 
# Sat, 28 Dec 2019 04:40:45 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:04:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:05:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:05:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:08:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Jan 2020 23:45:22 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:45:39 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:627706d65d1d9b4038d8fd40db52238d4f11d9130a01f23ffae9bf5d41ac5933`  
		Last Modified: Sat, 28 Dec 2019 04:46:38 GMT  
		Size: 49.2 MB (49171876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ac1923ab7a97ecdde2a4f034a8b716d51594ba6fc823c6aaac579c31f51906`  
		Last Modified: Sat, 28 Dec 2019 06:21:16 GMT  
		Size: 7.7 MB (7681148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b000e01546d5b9b3a40a3797f15bc0a1f579786c5ec8da31cbe9502f1927d367`  
		Last Modified: Sat, 28 Dec 2019 06:21:16 GMT  
		Size: 10.0 MB (9983835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8fe6ebd465d85dc79039fbd39712f1fadf5d7ac5fbefe405ef7a4f957a94ce`  
		Last Modified: Sat, 28 Dec 2019 06:21:39 GMT  
		Size: 52.1 MB (52102816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d739211b59b4a5cab55db8d8ce73eb5edfb9d5d91addf9f7aab0b9d9fa90b06`  
		Last Modified: Sat, 28 Dec 2019 06:22:32 GMT  
		Size: 183.6 MB (183566016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cff33cb79d34d36837bc747d7bd54401995ea5a541d92619b14c3ab0c8e2eb`  
		Last Modified: Thu, 30 Jan 2020 23:48:59 GMT  
		Size: 139.0 MB (139025394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:buster` - linux; 386

```console
$ docker pull rust@sha256:e1de980dfbedecb976f80c981e8ce689d9abd5cb15cff9306ada02436a5e4465
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.8 MB (466848765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:158b1b1e4c720838da8354351980c8022084cbec76ba03427a8a8699853c514f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:21 GMT
ADD file:b637f96d557a570f8ab83b28f7b9cdd128958359dd30dc2e03df70b799e132aa in / 
# Sat, 01 Feb 2020 16:39:21 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:23:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:24:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:24:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:25:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 01:26:51 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 01:27:16 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:2b34644a479c82db66a603c0b0a1d990911345f8646498fa9b050f306d0e6bf2`  
		Last Modified: Sat, 01 Feb 2020 16:44:10 GMT  
		Size: 51.1 MB (51141949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2f611c9392c4fe86735b477d61fda0e95ea77486175a737114c51586ecce86`  
		Last Modified: Sat, 01 Feb 2020 17:42:17 GMT  
		Size: 8.0 MB (7981506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69713757cc2d87c3255331d40f5061a73ef412208961f1ddd67a59a375397fda`  
		Last Modified: Sat, 01 Feb 2020 17:42:17 GMT  
		Size: 10.3 MB (10338479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956cf07a321afcfed99809a380a1905660e378188fd33d97f136551450be347a`  
		Last Modified: Sat, 01 Feb 2020 17:42:36 GMT  
		Size: 53.4 MB (53380753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8bfbd246f3a4ba9d861315c676a9a9e6524857c085e71b18b492882b063bff`  
		Last Modified: Sat, 01 Feb 2020 17:43:24 GMT  
		Size: 198.7 MB (198719863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b623bef7c51ab75de28495552321d02b2d6b4d6537933d893f18d155b414204a`  
		Last Modified: Sun, 02 Feb 2020 01:31:32 GMT  
		Size: 145.3 MB (145286215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:latest`

```console
$ docker pull rust@sha256:920b5c1b275778169a8c35f767c9c238ac9391f8a666d3ee159a1a2a26088a25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:latest` - linux; amd64

```console
$ docker pull rust@sha256:d59df245b22bfef90c2d29c1691e6a3ff679feb95d400b69626bae74898efab3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.7 MB (441693460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db33159e3388e178392ca314fbd8ecebb9fb430b73a29538302486e29cec6bc1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:08 GMT
ADD file:d6d0bdf8cb07a7a0dc32e9df50ac80ca1a524c3fa48136892ded195061f2194c in / 
# Sat, 28 Dec 2019 04:21:09 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:47:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:47:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 04:47:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:48:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Jan 2020 23:58:23 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:58:35 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:8f0fdd3eaac017684c880d836abdaf02f9db7ac8ecca970356482e3d8e315650`  
		Last Modified: Sat, 28 Dec 2019 04:25:39 GMT  
		Size: 50.4 MB (50379720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d918eaefd9de8a1595f56900fdb8ab65a03d64b1da1078da7c0b0bf6f7552a14`  
		Last Modified: Sat, 28 Dec 2019 05:01:44 GMT  
		Size: 7.8 MB (7811715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bf3e3107f525b7dea5b3cdfd15f62666066202105a0aaddbab2a02aefad1f7`  
		Last Modified: Sat, 28 Dec 2019 05:01:44 GMT  
		Size: 10.0 MB (9996202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27622921edb2aae9e0cb64f71a81b4a7cfef8f6a6c766514a018815834ba4e14`  
		Last Modified: Sat, 28 Dec 2019 05:02:00 GMT  
		Size: 51.8 MB (51790562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfa0aa1ae2c54d0de4b6ad0ee4d9f795c93368ae7d87801784c1f8ae624ac33`  
		Last Modified: Sat, 28 Dec 2019 05:02:36 GMT  
		Size: 192.0 MB (192044395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b109c91c0639fd55a93a5688b1bc7501e434396daabd93d714b72b106996a82a`  
		Last Modified: Fri, 31 Jan 2020 00:01:48 GMT  
		Size: 129.7 MB (129670866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:latest` - linux; arm variant v7

```console
$ docker pull rust@sha256:f4b13a8a2df73cfd225ce928f3574e1169b288e8448e004659d35d303ba1b82f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **420.0 MB (420018522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af6c4b7927d04a1c76f6b24226aa2702d2a7de368154e22aa531e7e986d7c227`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:06 GMT
ADD file:a57a312731f174c4b03031908ff95f49d7055d8c196439f0ed07ed9c4834d993 in / 
# Sat, 01 Feb 2020 17:00:08 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:00:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 18:01:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:03:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 03:16:56 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 03:17:21 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9bbb41bca8c6254da5088d03354297b1309dc75c2ccc738416025f89709ae5ee`  
		Last Modified: Sat, 01 Feb 2020 17:07:28 GMT  
		Size: 45.9 MB (45859700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239e4acdbc2ab88c89aa359fbab11429ea6d7bd93ea589a22c6bbb833ff82b93`  
		Last Modified: Sat, 01 Feb 2020 18:25:50 GMT  
		Size: 7.1 MB (7096223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6b4707a3c3aff9cb939fc058b869c5412e78c37e43eb0b653565460495537`  
		Last Modified: Sat, 01 Feb 2020 18:25:50 GMT  
		Size: 9.3 MB (9343278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e096c4fc8c629edca6da3ce5a9e95288512cb11e3d3d01a6e49078d19c2acca`  
		Last Modified: Sat, 01 Feb 2020 18:26:13 GMT  
		Size: 47.3 MB (47315591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6953ecf4273071529462518748f048f49a05530ae24d8fc6841919de312f2fc`  
		Last Modified: Sat, 01 Feb 2020 18:27:03 GMT  
		Size: 168.4 MB (168379144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f84f54aa922c34c20237ad8b624417ee33ea2f0c7940b127d3043d241b53bd`  
		Last Modified: Sun, 02 Feb 2020 03:21:00 GMT  
		Size: 142.0 MB (142024586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:latest` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:cc4933ffae4311c25299ae5b6a8e115241533bed5ca5e71dd7df717e0ca3b760
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.5 MB (441531085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:779e2f51436aa1328b240e1b38f7b6758d6acb69f2a4eae5f652148e28a16a8e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:40:41 GMT
ADD file:88b3d02fc98aa9138e694bee7d5d1b61b295e4a1c7fae399bf24e52eeff7a5ae in / 
# Sat, 28 Dec 2019 04:40:45 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:04:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:05:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:05:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:08:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Jan 2020 23:45:22 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:45:39 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:627706d65d1d9b4038d8fd40db52238d4f11d9130a01f23ffae9bf5d41ac5933`  
		Last Modified: Sat, 28 Dec 2019 04:46:38 GMT  
		Size: 49.2 MB (49171876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ac1923ab7a97ecdde2a4f034a8b716d51594ba6fc823c6aaac579c31f51906`  
		Last Modified: Sat, 28 Dec 2019 06:21:16 GMT  
		Size: 7.7 MB (7681148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b000e01546d5b9b3a40a3797f15bc0a1f579786c5ec8da31cbe9502f1927d367`  
		Last Modified: Sat, 28 Dec 2019 06:21:16 GMT  
		Size: 10.0 MB (9983835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8fe6ebd465d85dc79039fbd39712f1fadf5d7ac5fbefe405ef7a4f957a94ce`  
		Last Modified: Sat, 28 Dec 2019 06:21:39 GMT  
		Size: 52.1 MB (52102816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d739211b59b4a5cab55db8d8ce73eb5edfb9d5d91addf9f7aab0b9d9fa90b06`  
		Last Modified: Sat, 28 Dec 2019 06:22:32 GMT  
		Size: 183.6 MB (183566016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cff33cb79d34d36837bc747d7bd54401995ea5a541d92619b14c3ab0c8e2eb`  
		Last Modified: Thu, 30 Jan 2020 23:48:59 GMT  
		Size: 139.0 MB (139025394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:latest` - linux; 386

```console
$ docker pull rust@sha256:e1de980dfbedecb976f80c981e8ce689d9abd5cb15cff9306ada02436a5e4465
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.8 MB (466848765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:158b1b1e4c720838da8354351980c8022084cbec76ba03427a8a8699853c514f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:21 GMT
ADD file:b637f96d557a570f8ab83b28f7b9cdd128958359dd30dc2e03df70b799e132aa in / 
# Sat, 01 Feb 2020 16:39:21 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:23:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:24:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:24:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:25:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 01:26:51 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 01:27:16 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:2b34644a479c82db66a603c0b0a1d990911345f8646498fa9b050f306d0e6bf2`  
		Last Modified: Sat, 01 Feb 2020 16:44:10 GMT  
		Size: 51.1 MB (51141949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2f611c9392c4fe86735b477d61fda0e95ea77486175a737114c51586ecce86`  
		Last Modified: Sat, 01 Feb 2020 17:42:17 GMT  
		Size: 8.0 MB (7981506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69713757cc2d87c3255331d40f5061a73ef412208961f1ddd67a59a375397fda`  
		Last Modified: Sat, 01 Feb 2020 17:42:17 GMT  
		Size: 10.3 MB (10338479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956cf07a321afcfed99809a380a1905660e378188fd33d97f136551450be347a`  
		Last Modified: Sat, 01 Feb 2020 17:42:36 GMT  
		Size: 53.4 MB (53380753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8bfbd246f3a4ba9d861315c676a9a9e6524857c085e71b18b492882b063bff`  
		Last Modified: Sat, 01 Feb 2020 17:43:24 GMT  
		Size: 198.7 MB (198719863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b623bef7c51ab75de28495552321d02b2d6b4d6537933d893f18d155b414204a`  
		Last Modified: Sun, 02 Feb 2020 01:31:32 GMT  
		Size: 145.3 MB (145286215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:slim`

```console
$ docker pull rust@sha256:9c5a689ef6db939e940e061754a2b9a1841de8f86c2aa597c6fef6e5ceae631f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:slim` - linux; amd64

```console
$ docker pull rust@sha256:3fa8907a8030936ddf8785dd8339fc4ac64a8125c17e4a0ad1370524fcf83080
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202144548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:288fd60b2b05cb16b0a07371e5d69a0e30ce6a7d5a809fef31c9e1aad26ed7fd`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Thu, 30 Jan 2020 23:58:40 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:59:12 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4b6ea1105b5642d3cfab2b6fc2e4bc35a7c619b6cf9d1f1a74e56d944416b8`  
		Last Modified: Fri, 31 Jan 2020 00:02:40 GMT  
		Size: 175.1 MB (175052274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim` - linux; arm variant v7

```console
$ docker pull rust@sha256:ff2a1737cb5103afe6786f50a0340e8e52bfabe14523eb58fa1b2f9b8811acc6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.6 MB (197616259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d70333cde16926a90ea171253fd5353a3c875c45e0545febb78c6fd0c9637a0`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 03:17:30 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 03:18:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcd7ca587ec66d5a119fa12058b0cb1efb357adfaf91ad6ce5dc9a8250c6b3b`  
		Last Modified: Sun, 02 Feb 2020 03:22:02 GMT  
		Size: 174.9 MB (174917121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:c332927372fd374053c15e96604081147f07cb23ac35c35e390de9e74a34fa5e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.1 MB (205078984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85242a1a07815d02d847a6d1de41cfca4a9c2e239740d90dd84dd0fada10aef5`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Thu, 30 Jan 2020 23:45:48 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:46:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15b43da91b755c785745bcf6dd8b619aa403485ba00e712b498bc6efb09482d`  
		Last Modified: Thu, 30 Jan 2020 23:49:59 GMT  
		Size: 179.2 MB (179228282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim` - linux; 386

```console
$ docker pull rust@sha256:0b932c1020eee53546fffda34009bc0c6cdbfa0d496e863eb18846d65dd89290
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.0 MB (223015002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b3d3432b91e42b3062b27d190a1f8578b427582a142ec5858e9b2c88a57ca1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 01:27:25 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 01:28:20 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350f4532a56d213c594ac0bc23a3cd8cdc364f385832905798ff101a2cc9136f`  
		Last Modified: Sun, 02 Feb 2020 01:32:45 GMT  
		Size: 195.3 MB (195267950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:slim-buster`

```console
$ docker pull rust@sha256:9c5a689ef6db939e940e061754a2b9a1841de8f86c2aa597c6fef6e5ceae631f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:slim-buster` - linux; amd64

```console
$ docker pull rust@sha256:3fa8907a8030936ddf8785dd8339fc4ac64a8125c17e4a0ad1370524fcf83080
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202144548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:288fd60b2b05cb16b0a07371e5d69a0e30ce6a7d5a809fef31c9e1aad26ed7fd`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Thu, 30 Jan 2020 23:58:40 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:59:12 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4b6ea1105b5642d3cfab2b6fc2e4bc35a7c619b6cf9d1f1a74e56d944416b8`  
		Last Modified: Fri, 31 Jan 2020 00:02:40 GMT  
		Size: 175.1 MB (175052274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:ff2a1737cb5103afe6786f50a0340e8e52bfabe14523eb58fa1b2f9b8811acc6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.6 MB (197616259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d70333cde16926a90ea171253fd5353a3c875c45e0545febb78c6fd0c9637a0`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 03:17:30 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 03:18:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcd7ca587ec66d5a119fa12058b0cb1efb357adfaf91ad6ce5dc9a8250c6b3b`  
		Last Modified: Sun, 02 Feb 2020 03:22:02 GMT  
		Size: 174.9 MB (174917121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:c332927372fd374053c15e96604081147f07cb23ac35c35e390de9e74a34fa5e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.1 MB (205078984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85242a1a07815d02d847a6d1de41cfca4a9c2e239740d90dd84dd0fada10aef5`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Thu, 30 Jan 2020 23:45:48 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:46:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15b43da91b755c785745bcf6dd8b619aa403485ba00e712b498bc6efb09482d`  
		Last Modified: Thu, 30 Jan 2020 23:49:59 GMT  
		Size: 179.2 MB (179228282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-buster` - linux; 386

```console
$ docker pull rust@sha256:0b932c1020eee53546fffda34009bc0c6cdbfa0d496e863eb18846d65dd89290
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.0 MB (223015002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b3d3432b91e42b3062b27d190a1f8578b427582a142ec5858e9b2c88a57ca1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 01:27:25 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 01:28:20 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350f4532a56d213c594ac0bc23a3cd8cdc364f385832905798ff101a2cc9136f`  
		Last Modified: Sun, 02 Feb 2020 01:32:45 GMT  
		Size: 195.3 MB (195267950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:slim-stretch`

```console
$ docker pull rust@sha256:54c28eb493584efa368f8ad3b842a82f95321479f511c092719071cd6c9da5d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:slim-stretch` - linux; amd64

```console
$ docker pull rust@sha256:8988a0ace70a25adc0076a21458d807fa08cecde92a8126c66bd0febdc0f099e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190094499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80efe80a4223e96acebcd908e5ef8fecd93781a5a9fa24de654e0265c7988e26`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:47 GMT
ADD file:90a2c81769a336bed3f731f44a385f2a65b0916f517a0b77c06c224579bf9a9a in / 
# Sat, 28 Dec 2019 04:23:47 GMT
CMD ["bash"]
# Thu, 30 Jan 2020 23:57:50 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:58:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:804555ee037604c40de144f9f8da0d826d38db82f15d74cded32790fe279a8f6`  
		Last Modified: Sat, 28 Dec 2019 04:28:38 GMT  
		Size: 22.5 MB (22524609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56e4802f7cdd484d276f0cfc4639961be839a95b6ffae7e536ae840b4fa5d8a`  
		Last Modified: Fri, 31 Jan 2020 00:01:21 GMT  
		Size: 167.6 MB (167569890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-stretch` - linux; arm variant v7

```console
$ docker pull rust@sha256:b0379f8ec7a9155f4ff13fa0957914ce3ba88b80ce5c22923c4ead2a9f89e451
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.4 MB (189398124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:690fad015da49bc6b577df128d04eccc8ee0176e7b0a897ed1111100cba598ef`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:04:29 GMT
ADD file:6ac430a42a1f2a6cc8b0a3565e518bd0e3a47b01d524b86cd3dd4e7f4606fd53 in / 
# Sat, 01 Feb 2020 17:04:31 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 03:15:52 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 03:16:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:6bc458b0813423b9e351a5604c0d71a4853d970ea22b23fedc8683af12dbc13c`  
		Last Modified: Sat, 01 Feb 2020 17:11:31 GMT  
		Size: 19.3 MB (19311624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c966b45d91cbdbbddb23863703ccd1856379b3e0d4ad838d8acee8c431b5717f`  
		Last Modified: Sun, 02 Feb 2020 03:20:10 GMT  
		Size: 170.1 MB (170086500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-stretch` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:b527a9fcdb5d6a90ce0de4fbbc161e962b09a62c009cd1e7114704f286379112
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.0 MB (190038348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea06f0967e1a0beb570f23c6f7dba5d4cf594b4a83455394d7194de9f956c551`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:43:36 GMT
ADD file:ba40f5080cbd89c576c350bfe5acfe16f2ec59636fdb082efc3a8cef66ae7cb7 in / 
# Sat, 28 Dec 2019 04:43:39 GMT
CMD ["bash"]
# Thu, 30 Jan 2020 23:44:29 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:45:11 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:588374d57fdb5120d024340eef3d8927af23a5b806d41b4f049ee430a153c0b4`  
		Last Modified: Sat, 28 Dec 2019 04:49:14 GMT  
		Size: 20.4 MB (20385801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e8a34c9e29def30493e1870ffa929495298009b05360083f22181d4453f839`  
		Last Modified: Thu, 30 Jan 2020 23:48:17 GMT  
		Size: 169.7 MB (169652547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-stretch` - linux; 386

```console
$ docker pull rust@sha256:b78ee7fab6baf80ca227645cda796eace6e3a676f35bb0d95939452dcc51c55c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.3 MB (210336495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2972082f643a87cf18629e0d194514767086084c493f5ef4811290a49c0bc022`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:07 GMT
ADD file:c9b4696be461d46d96c760441f34e219e229f90bc6946125b2f809218c3456ce in / 
# Sat, 01 Feb 2020 16:42:07 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 01:25:48 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 01:26:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:4f51b031b74b1f7fab6310c197fd7534181ba2db1f0cec6686fb9e9a82abbb9c`  
		Last Modified: Sat, 01 Feb 2020 16:47:27 GMT  
		Size: 23.2 MB (23152156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea943a600d5130a3a8ddcf69ed3eda4147d98c45f6c499d1f940b1bf24f9c28f`  
		Last Modified: Sun, 02 Feb 2020 01:30:26 GMT  
		Size: 187.2 MB (187184339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:stretch`

```console
$ docker pull rust@sha256:b37b4a8bf6cd1080fb9a379ee680c2fcc90121d67fb3a04bb76e4484a9544d43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:stretch` - linux; amd64

```console
$ docker pull rust@sha256:ff4627ba92fdf9d566bbd64ace1dc4184125d8e91a71ccd45fdf555fd17ebe52
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **455.1 MB (455102608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b1293d4b2e209d0e4854e3dbaf3ed403291aa20f01b64c71c3e0c1c7330561c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:33 GMT
ADD file:8f7dc710e276f54a3a73d34b6b8fa261950a781d68ceb7401fa18dabc601c5a5 in / 
# Sat, 28 Dec 2019 04:23:34 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:58:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:58:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 04:59:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:00:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Jan 2020 23:57:32 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:57:45 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:146bd6a886182fde06fbf747470b1c89814bc8ab1c96fdf1aef6107171959fe6`  
		Last Modified: Sat, 28 Dec 2019 04:28:25 GMT  
		Size: 45.4 MB (45380744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9935d0c62ace92b388be202275e222007d6cac10b9c1f2c1ea63af38c09ea7ab`  
		Last Modified: Sat, 28 Dec 2019 05:04:30 GMT  
		Size: 10.8 MB (10797221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0efb86e80601b5bbdbb7c406426982c4202d339687c14c3941b364527e2249`  
		Last Modified: Sat, 28 Dec 2019 05:04:28 GMT  
		Size: 4.3 MB (4340114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e705a4c4fd310b96bfb3d7928428e65f0d3f5bad0cd0bda1434aee1d89418468`  
		Last Modified: Sat, 28 Dec 2019 05:04:45 GMT  
		Size: 50.1 MB (50072671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c877b722db6f4d4297c21f07162d21fa6ac6f51d03360f75e24cfa3bcaefe57d`  
		Last Modified: Sat, 28 Dec 2019 05:05:38 GMT  
		Size: 214.8 MB (214840548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec7021710852d02bcf8dc866ab78921203814c4f8cb56c6e0717dd899d3dfb1`  
		Last Modified: Fri, 31 Jan 2020 00:00:33 GMT  
		Size: 129.7 MB (129671310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:stretch` - linux; arm variant v7

```console
$ docker pull rust@sha256:95479bdf726ea84f8ce541732a071b898f3a87d69d3e8c10641bbaf327830871
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **439.5 MB (439473862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7e4ba4d1c5cd134afc62cb4f59a2673ee4eb0afa5debe20d887b29870da4991`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:04:08 GMT
ADD file:b7fc54d004d962f2cfb469a1aaa9e689e46dfa2554e0cf44c33981d688adc31b in / 
# Sat, 01 Feb 2020 17:04:09 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:18:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:18:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 18:19:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:23:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 03:15:22 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 03:15:44 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:cc3b08e804cce7e88d9df954b76be506569775afe9cf36316f2fa6c5c9bf3d5c`  
		Last Modified: Sat, 01 Feb 2020 17:11:13 GMT  
		Size: 42.1 MB (42108370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa649f4f33c2131c2969e49352ff247ebe5a62a62b83498c3580f883aa35621e`  
		Last Modified: Sat, 01 Feb 2020 18:31:10 GMT  
		Size: 9.5 MB (9498229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901c0c16dce9409a6a020f4b874b40fb3f7d302fe0b4e7a80a87a7cfbab7da04`  
		Last Modified: Sat, 01 Feb 2020 18:31:10 GMT  
		Size: 3.9 MB (3918766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a264d83dc76a4a25b4110827c1ac6cc620c406edb6b2089cd1117aec271ed`  
		Last Modified: Sat, 01 Feb 2020 18:31:32 GMT  
		Size: 46.4 MB (46400091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:854dcba3350bdff3f923ff69f2dec445f47ef5726d3d15bde4242c2ff122aabc`  
		Last Modified: Sat, 01 Feb 2020 18:32:28 GMT  
		Size: 195.5 MB (195523495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ce99acc39da624b324257b529b5859fe714ab94c38fd36224416818be5f43c`  
		Last Modified: Sun, 02 Feb 2020 03:19:13 GMT  
		Size: 142.0 MB (142024911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:stretch` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:9ecb1e05a3077b32c8bd99e2d9eda52c2b5d79f388b751e61b4f3cfe047fb9ac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **446.3 MB (446292278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f5feafcebe0b3ff73e55d4ca6ee2ffd01eb91352c47ee1da796b47a1d89c8e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:43:15 GMT
ADD file:e439b3c387852978811a6a5a058745ebb9392da7e8936beb4f37ff076e656213 in / 
# Sat, 28 Dec 2019 04:43:17 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:15:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:15:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:16:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:18:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Jan 2020 23:43:59 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Thu, 30 Jan 2020 23:44:18 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:d07bcf5901dfa793fa6b2c4c617e86bcef315b0b092cbfd1a929eefedaf8e3f2`  
		Last Modified: Sat, 28 Dec 2019 04:48:57 GMT  
		Size: 43.2 MB (43166476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f31062581dadb1f69c43e9441040dd46788bf13ae51f20c66929fac82b506b`  
		Last Modified: Sat, 28 Dec 2019 06:24:15 GMT  
		Size: 9.7 MB (9748258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62337a296a607f48a5dc3a7c07639360d98e0e78982ca8e459c832719012f12`  
		Last Modified: Sat, 28 Dec 2019 06:24:15 GMT  
		Size: 4.1 MB (4094448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403697a3e152c7a38ddb9175a90ed2dac97d780421c35949ff80cd67a7d4e596`  
		Last Modified: Sat, 28 Dec 2019 06:24:36 GMT  
		Size: 48.0 MB (48024191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0179cb8c17339f719c763581cefb9e377c016b4f7f4b747a665349e79470363c`  
		Last Modified: Sat, 28 Dec 2019 06:25:35 GMT  
		Size: 202.2 MB (202233183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cddbec6e7f644fe8725ebf72f7dc61a67b27b411e5d4466b522933633e74f5c`  
		Last Modified: Thu, 30 Jan 2020 23:47:26 GMT  
		Size: 139.0 MB (139025722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:stretch` - linux; 386

```console
$ docker pull rust@sha256:1f587d401d8a96d2f338101f37a03cd379241fe760d8f8b4d4fa8d073336f6e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.3 MB (478286932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:979e274dc88223c0d7e5b1ad0fb9236195b93a7e3f6d79c11081b5db16cbec8d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:53 GMT
ADD file:bae1646c4e3069e717d1ee4f6c312c249e96a21d795a639cdfaf338d645c8be9 in / 
# Sat, 01 Feb 2020 16:41:53 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:38:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:38:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:39:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:40:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 01:25:09 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.41.0
# Sun, 02 Feb 2020 01:25:38 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='ad1f8b5199b3b9e231472ed7aa08d2e5d1d539198a15c5b1e53c746aad81d27b' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='6c6c3789dabf12171c7f500e06d21d8004b5318a5083df8b0b02c0e5ef1d017b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='26942c80234bac34b3c1352abbd9187d3e23b43dae3cf56a9f9c1ea8ee53076d' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='27ae12bc294a34e566579deba3e066245d09b8871dc021ef45fc715dced05297' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.21.1/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION;     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:97067fdacc0601fe58a5f782cd09d3c58a214c43b8629a2d92bd7025f46fd265`  
		Last Modified: Sat, 01 Feb 2020 16:47:15 GMT  
		Size: 46.1 MB (46100017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1ac2ac579e53fc74848ab743b53ae2f6e54350989c71359d435c2fef2e5157`  
		Last Modified: Sat, 01 Feb 2020 17:45:45 GMT  
		Size: 10.8 MB (10817587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f7b32e68627ad71130644b1646afb1aa0bcf1f440df145526a73fdbd413f3b`  
		Last Modified: Sat, 01 Feb 2020 17:45:43 GMT  
		Size: 4.6 MB (4561467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b926c1ce2d1cf6b99c32683bf0fd0233d4f71f367d38a16de2ba08e9ecbf1cc2`  
		Last Modified: Sat, 01 Feb 2020 17:46:05 GMT  
		Size: 51.6 MB (51595566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac9b89be3409f23bc9ac380bcfd9f28e0cc2e52b69b8706e0b102211c83abf4`  
		Last Modified: Sat, 01 Feb 2020 17:47:03 GMT  
		Size: 219.9 MB (219925297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69feda6b3fd089c07ee45b4a40f729a67e99bfa21dc5b5eede2fc9efc22d3d01`  
		Last Modified: Sun, 02 Feb 2020 01:29:25 GMT  
		Size: 145.3 MB (145286998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
