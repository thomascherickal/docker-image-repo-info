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
-	[`rust:1.61`](#rust161)
-	[`rust:1.61-alpine`](#rust161-alpine)
-	[`rust:1.61-alpine3.14`](#rust161-alpine314)
-	[`rust:1.61-alpine3.15`](#rust161-alpine315)
-	[`rust:1.61-bullseye`](#rust161-bullseye)
-	[`rust:1.61-buster`](#rust161-buster)
-	[`rust:1.61-slim`](#rust161-slim)
-	[`rust:1.61-slim-bullseye`](#rust161-slim-bullseye)
-	[`rust:1.61-slim-buster`](#rust161-slim-buster)
-	[`rust:1.61.0`](#rust1610)
-	[`rust:1.61.0-alpine`](#rust1610-alpine)
-	[`rust:1.61.0-alpine3.14`](#rust1610-alpine314)
-	[`rust:1.61.0-alpine3.15`](#rust1610-alpine315)
-	[`rust:1.61.0-bullseye`](#rust1610-bullseye)
-	[`rust:1.61.0-buster`](#rust1610-buster)
-	[`rust:1.61.0-slim`](#rust1610-slim)
-	[`rust:1.61.0-slim-bullseye`](#rust1610-slim-bullseye)
-	[`rust:1.61.0-slim-buster`](#rust1610-slim-buster)
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
$ docker pull rust@sha256:7117a2abfcd947cf26bd0e6dc675a3d511036fe5952c0d38e79911e513c5370a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1` - linux; amd64

```console
$ docker pull rust@sha256:9fe1f39bec70576e2bd568fafb194b2a532a6f2928bc0b951ac2c0a69a2be9fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **470.2 MB (470195312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a7fe322d8850b0f32d3cebd5ce588d5c1790c96b27d37aee48bddc124a80aa0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:20:05 GMT
ADD file:68a5d7d0db592625159865110c1b7dcb15cf70ecf71b5fd541ef89584cd734ba in / 
# Wed, 11 May 2022 01:20:05 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:49:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:49:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:50:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 16:17:37 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Wed, 11 May 2022 16:17:52 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:67e8aa6c8bbc76b1f2bccb3864b0887671833b8667dc1f6c965fcb0eac7e6402`  
		Last Modified: Wed, 11 May 2022 01:24:45 GMT  
		Size: 54.9 MB (54945622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627e6c1e105548ea4a08354eea581f137cf368d91aeb0ad47dcb706fca54fd8b`  
		Last Modified: Wed, 11 May 2022 01:57:17 GMT  
		Size: 5.2 MB (5155721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0670968926f6461e3135c82ba2c0ad3ebdedc0d0f41b18bda4a1e41104b8be8a`  
		Last Modified: Wed, 11 May 2022 01:57:18 GMT  
		Size: 10.9 MB (10875052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8b0e20be4b4a332bc3d90b9903a5f3c0664b440fd9f1d2a1db0d4b7e6e826b`  
		Last Modified: Wed, 11 May 2022 01:57:38 GMT  
		Size: 54.6 MB (54578468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b10a3a2784b06bfe0af1493ea2a0fa957ae5e0dc30fcfd1166d2558ba74e4d`  
		Last Modified: Wed, 11 May 2022 01:58:14 GMT  
		Size: 196.6 MB (196562669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283a0d92cdf06eb32299bbf28f78c1618a6163731bcffbc1551510e57e8cb4b9`  
		Last Modified: Wed, 11 May 2022 16:20:50 GMT  
		Size: 148.1 MB (148077780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1` - linux; arm variant v7

```console
$ docker pull rust@sha256:1b59f7d09735e15b0343859d1cb098a1675f013e84347be76936ef9d888fd9e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **467.2 MB (467237488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adc5a024a4724b55a7cba85555cd244b2612ac3057ca98f267dabe0053aeac32`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:48:30 GMT
ADD file:d6545064ea0f75166d59e4d4a2df1e41a3477ae468e558e31f29857336978c0e in / 
# Wed, 11 May 2022 01:48:31 GMT
CMD ["bash"]
# Wed, 11 May 2022 03:21:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:21:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 03:22:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:24:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 May 2022 18:00:44 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 18:01:23 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:ba38f9a6c66968e207a7ada348a2110e3be0ff117e621d9e10ddd7c4becc0d2a`  
		Last Modified: Wed, 11 May 2022 02:03:49 GMT  
		Size: 50.1 MB (50134069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71423015d7b4f718e54ff1561cc06bb4c8357baedc23b49d25fe99cd4b0ae41`  
		Last Modified: Wed, 11 May 2022 03:46:39 GMT  
		Size: 4.9 MB (4924901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8f92194faa0a66e5bd160b229941428f0b0387c6e313e4f1f903c678fbb17e`  
		Last Modified: Wed, 11 May 2022 03:46:41 GMT  
		Size: 10.2 MB (10217886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c410c75a05c2df4ed485cda22fd35206e0ea4b9fbc9f096b11ed5adc6f83fa1c`  
		Last Modified: Wed, 11 May 2022 03:47:32 GMT  
		Size: 50.3 MB (50329744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767978ffc99a492ddd06d37b888a093595a05ac353ceefb2cc01a1322f34164a`  
		Last Modified: Wed, 11 May 2022 03:49:16 GMT  
		Size: 167.0 MB (167042139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3247bc72a5ac57b8481395404128439459da3cbe3d37697e6cce58dc91967469`  
		Last Modified: Thu, 19 May 2022 18:11:31 GMT  
		Size: 184.6 MB (184588749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:0f34bbe3d25473314051f103cf14a43e983500a742512514459dddebcec49acc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **516.4 MB (516393806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4db0c962f51c31164dcd6edf66e1078fa5fa7bd4324918135f1af9e95932bf8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:46:44 GMT
ADD file:239aa42118877a929b2fbfc0d5793fee7815289280affa5286de2459385c0679 in / 
# Wed, 11 May 2022 00:46:44 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:25:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:25:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:25:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:26:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 May 2022 17:58:06 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:58:21 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:3a36574378e6cece2dd3a839e1c0220eaccc4063b61d7481d1a19d3990c1f2c2`  
		Last Modified: Wed, 11 May 2022 00:53:15 GMT  
		Size: 53.6 MB (53634337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61d3345afba43846f3e638752cce2f0d1d47b21cc667ba08b00db10767a4702`  
		Last Modified: Wed, 11 May 2022 01:35:45 GMT  
		Size: 4.9 MB (4938615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e267d6aa58f93a513352a3b46c7addbf9335d7d43bfa4f1df4026d21785181c`  
		Last Modified: Wed, 11 May 2022 01:35:46 GMT  
		Size: 10.7 MB (10656992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f647907d26b879e0d43f6f4f0807f01e4dbdc034edcecbc988f6033cf401becf`  
		Last Modified: Wed, 11 May 2022 01:36:07 GMT  
		Size: 54.7 MB (54672822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0b3e17bdee16cf8bf269a4474bf56713879991bf87ff3bd790aa96a6f00e3c`  
		Last Modified: Wed, 11 May 2022 01:36:46 GMT  
		Size: 189.5 MB (189482172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cba956553646efe774f749ce526b98ebbff7a89a2eea4b21e77ae86ee7de78f`  
		Last Modified: Thu, 19 May 2022 18:03:05 GMT  
		Size: 203.0 MB (203008868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1` - linux; 386

```console
$ docker pull rust@sha256:429ae8c8999946379ab90c480318570fa79e1c1fee0bd8248203a9ca26d1702a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **497.9 MB (497919108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c89e41228cd37377968ac5dc6bbd360636a67126aa6b7a48a3d8e5e8f9f24d7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:38:57 GMT
ADD file:dae3dc662d1327f461e95b84f6f9282f3c4fb51f16ac8f20a5f141951d8436a9 in / 
# Wed, 11 May 2022 01:38:58 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:10:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:10:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 02:11:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:12:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 15:45:42 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Wed, 11 May 2022 15:46:00 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:5ad4f92623738998bc77103ff64344255f842f6e5fe4a846df656351b3c4852f`  
		Last Modified: Wed, 11 May 2022 01:45:53 GMT  
		Size: 55.9 MB (55942833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026e99ab0e4b1d3aec936d04cdf9c04ddc8074f2917b86c02e66d88fcae1e42f`  
		Last Modified: Wed, 11 May 2022 02:21:42 GMT  
		Size: 5.1 MB (5080245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dba083f619f2a2c8cfef4a4e844cf6819c306e225029e62cf7c31c17b0d344`  
		Last Modified: Wed, 11 May 2022 02:21:43 GMT  
		Size: 11.0 MB (11033702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5333a48696af9b52c4219f20b87c5cf9b05764b7c58cd19880e6c5730d1b75`  
		Last Modified: Wed, 11 May 2022 02:22:10 GMT  
		Size: 55.9 MB (55914622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899f353e6896a6f03a5af06a01cea44badeac7062481c294a9d7c1da1859b823`  
		Last Modified: Wed, 11 May 2022 02:22:52 GMT  
		Size: 199.5 MB (199502725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c70e60ad4e506736166da380bdcd6e33bfd1a6a4f654f0f1f21736de86b9d47`  
		Last Modified: Wed, 11 May 2022 15:49:27 GMT  
		Size: 170.4 MB (170444981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-alpine`

```console
$ docker pull rust@sha256:7a917171c2fa060a2665b291820507bca0484efd25811a1c09073b0cfc5cb23d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:1-alpine` - linux; amd64

```console
$ docker pull rust@sha256:e1ddd35b6a802ac8587f8fbc34ce752be20b5c116df2b2f1a90488f0bc3bd439
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.6 MB (249551918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5fbf9bd1849d2598eff6ddedc32b06610905188571179b4a4b0805d6331c549`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:50:48 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 07 Apr 2022 20:22:16 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Thu, 07 Apr 2022 20:22:35 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2113a6fa04a6792c25bda8b467d30b4388d756ab1f526efb6ce7139d464f5b84`  
		Last Modified: Tue, 05 Apr 2022 10:52:45 GMT  
		Size: 42.5 MB (42476793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82ca4327e1d9bb80a8af0bb460d9bef24f8e88470631e2c788f996e91e3d8a7`  
		Last Modified: Thu, 07 Apr 2022 20:27:23 GMT  
		Size: 204.3 MB (204260566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-alpine` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:526dfcfffac3021335f243aabe2b93bf32fd231fbb0e65103266980eedd1e8c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.2 MB (239222115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4049c483a2db267242fac510cf462f66964cbb5e25e512ea43f6648c8e072819`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:18:36 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 19 May 2022 17:59:27 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:59:40 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c79c9d0c9a2cc2bdae9476b20ddb336848888d44ff7d5dfb719ff227ffb79c4`  
		Last Modified: Tue, 05 Apr 2022 07:21:11 GMT  
		Size: 36.1 MB (36073695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d80249e68d74cb54280b56279b2a423d8c0b7682f33bb9a362f716341403763`  
		Last Modified: Thu, 19 May 2022 18:05:57 GMT  
		Size: 200.4 MB (200431943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-alpine3.14`

```console
$ docker pull rust@sha256:dc154448faa074931911a7d85ee984a07786f64f3414978368c764afd6b2a971
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:1-alpine3.14` - linux; amd64

```console
$ docker pull rust@sha256:c4a4a463cd986120a16f1e7e44d77238acc18b31bbdaa66254adb8bde4cb2496
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.4 MB (249419447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a59e129e5e042f57ee01d253e60fafce1011ff98bf3517ab7a1369e32d3242c1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:50:20 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 07 Apr 2022 20:21:52 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Thu, 07 Apr 2022 20:22:12 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77041b2d00354ec0aeef4267546654f2d783ec91f776e89b924b2759dcf3cf7`  
		Last Modified: Tue, 05 Apr 2022 10:52:01 GMT  
		Size: 42.3 MB (42340505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994ac804f5895d53d5a70de8f2d11672e5c6a688fdb5a78f159c3335291914f9`  
		Last Modified: Thu, 07 Apr 2022 20:26:39 GMT  
		Size: 204.3 MB (204260572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:301565f25377b33199f2e8117344416d3db0e6e5fcbe87594838ed22be3bc696
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.1 MB (239070495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3a8e3972791724a8ce0c813fa148fe8456cce8d81a3eab4f9ebd8b79ee56cc2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:18:14 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 19 May 2022 17:59:04 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:59:20 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757084716086a18d818bc8687efebb7931b4f95e66464768dd2f3a724165e5fb`  
		Last Modified: Tue, 05 Apr 2022 07:20:27 GMT  
		Size: 35.9 MB (35921106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7387a7ced2948ec0e416c953e2a8ae1f1fc9955fba656c8a23b60bb29663cc9e`  
		Last Modified: Thu, 19 May 2022 18:05:11 GMT  
		Size: 200.4 MB (200432000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-alpine3.15`

```console
$ docker pull rust@sha256:7a917171c2fa060a2665b291820507bca0484efd25811a1c09073b0cfc5cb23d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:1-alpine3.15` - linux; amd64

```console
$ docker pull rust@sha256:e1ddd35b6a802ac8587f8fbc34ce752be20b5c116df2b2f1a90488f0bc3bd439
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.6 MB (249551918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5fbf9bd1849d2598eff6ddedc32b06610905188571179b4a4b0805d6331c549`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:50:48 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 07 Apr 2022 20:22:16 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Thu, 07 Apr 2022 20:22:35 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2113a6fa04a6792c25bda8b467d30b4388d756ab1f526efb6ce7139d464f5b84`  
		Last Modified: Tue, 05 Apr 2022 10:52:45 GMT  
		Size: 42.5 MB (42476793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82ca4327e1d9bb80a8af0bb460d9bef24f8e88470631e2c788f996e91e3d8a7`  
		Last Modified: Thu, 07 Apr 2022 20:27:23 GMT  
		Size: 204.3 MB (204260566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:526dfcfffac3021335f243aabe2b93bf32fd231fbb0e65103266980eedd1e8c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.2 MB (239222115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4049c483a2db267242fac510cf462f66964cbb5e25e512ea43f6648c8e072819`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:18:36 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 19 May 2022 17:59:27 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:59:40 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c79c9d0c9a2cc2bdae9476b20ddb336848888d44ff7d5dfb719ff227ffb79c4`  
		Last Modified: Tue, 05 Apr 2022 07:21:11 GMT  
		Size: 36.1 MB (36073695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d80249e68d74cb54280b56279b2a423d8c0b7682f33bb9a362f716341403763`  
		Last Modified: Thu, 19 May 2022 18:05:57 GMT  
		Size: 200.4 MB (200431943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-bullseye`

```console
$ docker pull rust@sha256:7117a2abfcd947cf26bd0e6dc675a3d511036fe5952c0d38e79911e513c5370a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-bullseye` - linux; amd64

```console
$ docker pull rust@sha256:9fe1f39bec70576e2bd568fafb194b2a532a6f2928bc0b951ac2c0a69a2be9fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **470.2 MB (470195312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a7fe322d8850b0f32d3cebd5ce588d5c1790c96b27d37aee48bddc124a80aa0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:20:05 GMT
ADD file:68a5d7d0db592625159865110c1b7dcb15cf70ecf71b5fd541ef89584cd734ba in / 
# Wed, 11 May 2022 01:20:05 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:49:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:49:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:50:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 16:17:37 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Wed, 11 May 2022 16:17:52 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:67e8aa6c8bbc76b1f2bccb3864b0887671833b8667dc1f6c965fcb0eac7e6402`  
		Last Modified: Wed, 11 May 2022 01:24:45 GMT  
		Size: 54.9 MB (54945622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627e6c1e105548ea4a08354eea581f137cf368d91aeb0ad47dcb706fca54fd8b`  
		Last Modified: Wed, 11 May 2022 01:57:17 GMT  
		Size: 5.2 MB (5155721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0670968926f6461e3135c82ba2c0ad3ebdedc0d0f41b18bda4a1e41104b8be8a`  
		Last Modified: Wed, 11 May 2022 01:57:18 GMT  
		Size: 10.9 MB (10875052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8b0e20be4b4a332bc3d90b9903a5f3c0664b440fd9f1d2a1db0d4b7e6e826b`  
		Last Modified: Wed, 11 May 2022 01:57:38 GMT  
		Size: 54.6 MB (54578468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b10a3a2784b06bfe0af1493ea2a0fa957ae5e0dc30fcfd1166d2558ba74e4d`  
		Last Modified: Wed, 11 May 2022 01:58:14 GMT  
		Size: 196.6 MB (196562669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283a0d92cdf06eb32299bbf28f78c1618a6163731bcffbc1551510e57e8cb4b9`  
		Last Modified: Wed, 11 May 2022 16:20:50 GMT  
		Size: 148.1 MB (148077780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-bullseye` - linux; arm variant v7

```console
$ docker pull rust@sha256:1b59f7d09735e15b0343859d1cb098a1675f013e84347be76936ef9d888fd9e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **467.2 MB (467237488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adc5a024a4724b55a7cba85555cd244b2612ac3057ca98f267dabe0053aeac32`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:48:30 GMT
ADD file:d6545064ea0f75166d59e4d4a2df1e41a3477ae468e558e31f29857336978c0e in / 
# Wed, 11 May 2022 01:48:31 GMT
CMD ["bash"]
# Wed, 11 May 2022 03:21:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:21:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 03:22:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:24:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 May 2022 18:00:44 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 18:01:23 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:ba38f9a6c66968e207a7ada348a2110e3be0ff117e621d9e10ddd7c4becc0d2a`  
		Last Modified: Wed, 11 May 2022 02:03:49 GMT  
		Size: 50.1 MB (50134069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71423015d7b4f718e54ff1561cc06bb4c8357baedc23b49d25fe99cd4b0ae41`  
		Last Modified: Wed, 11 May 2022 03:46:39 GMT  
		Size: 4.9 MB (4924901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8f92194faa0a66e5bd160b229941428f0b0387c6e313e4f1f903c678fbb17e`  
		Last Modified: Wed, 11 May 2022 03:46:41 GMT  
		Size: 10.2 MB (10217886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c410c75a05c2df4ed485cda22fd35206e0ea4b9fbc9f096b11ed5adc6f83fa1c`  
		Last Modified: Wed, 11 May 2022 03:47:32 GMT  
		Size: 50.3 MB (50329744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767978ffc99a492ddd06d37b888a093595a05ac353ceefb2cc01a1322f34164a`  
		Last Modified: Wed, 11 May 2022 03:49:16 GMT  
		Size: 167.0 MB (167042139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3247bc72a5ac57b8481395404128439459da3cbe3d37697e6cce58dc91967469`  
		Last Modified: Thu, 19 May 2022 18:11:31 GMT  
		Size: 184.6 MB (184588749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-bullseye` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:0f34bbe3d25473314051f103cf14a43e983500a742512514459dddebcec49acc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **516.4 MB (516393806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4db0c962f51c31164dcd6edf66e1078fa5fa7bd4324918135f1af9e95932bf8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:46:44 GMT
ADD file:239aa42118877a929b2fbfc0d5793fee7815289280affa5286de2459385c0679 in / 
# Wed, 11 May 2022 00:46:44 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:25:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:25:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:25:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:26:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 May 2022 17:58:06 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:58:21 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:3a36574378e6cece2dd3a839e1c0220eaccc4063b61d7481d1a19d3990c1f2c2`  
		Last Modified: Wed, 11 May 2022 00:53:15 GMT  
		Size: 53.6 MB (53634337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61d3345afba43846f3e638752cce2f0d1d47b21cc667ba08b00db10767a4702`  
		Last Modified: Wed, 11 May 2022 01:35:45 GMT  
		Size: 4.9 MB (4938615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e267d6aa58f93a513352a3b46c7addbf9335d7d43bfa4f1df4026d21785181c`  
		Last Modified: Wed, 11 May 2022 01:35:46 GMT  
		Size: 10.7 MB (10656992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f647907d26b879e0d43f6f4f0807f01e4dbdc034edcecbc988f6033cf401becf`  
		Last Modified: Wed, 11 May 2022 01:36:07 GMT  
		Size: 54.7 MB (54672822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0b3e17bdee16cf8bf269a4474bf56713879991bf87ff3bd790aa96a6f00e3c`  
		Last Modified: Wed, 11 May 2022 01:36:46 GMT  
		Size: 189.5 MB (189482172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cba956553646efe774f749ce526b98ebbff7a89a2eea4b21e77ae86ee7de78f`  
		Last Modified: Thu, 19 May 2022 18:03:05 GMT  
		Size: 203.0 MB (203008868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-bullseye` - linux; 386

```console
$ docker pull rust@sha256:429ae8c8999946379ab90c480318570fa79e1c1fee0bd8248203a9ca26d1702a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **497.9 MB (497919108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c89e41228cd37377968ac5dc6bbd360636a67126aa6b7a48a3d8e5e8f9f24d7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:38:57 GMT
ADD file:dae3dc662d1327f461e95b84f6f9282f3c4fb51f16ac8f20a5f141951d8436a9 in / 
# Wed, 11 May 2022 01:38:58 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:10:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:10:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 02:11:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:12:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 15:45:42 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Wed, 11 May 2022 15:46:00 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:5ad4f92623738998bc77103ff64344255f842f6e5fe4a846df656351b3c4852f`  
		Last Modified: Wed, 11 May 2022 01:45:53 GMT  
		Size: 55.9 MB (55942833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026e99ab0e4b1d3aec936d04cdf9c04ddc8074f2917b86c02e66d88fcae1e42f`  
		Last Modified: Wed, 11 May 2022 02:21:42 GMT  
		Size: 5.1 MB (5080245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dba083f619f2a2c8cfef4a4e844cf6819c306e225029e62cf7c31c17b0d344`  
		Last Modified: Wed, 11 May 2022 02:21:43 GMT  
		Size: 11.0 MB (11033702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5333a48696af9b52c4219f20b87c5cf9b05764b7c58cd19880e6c5730d1b75`  
		Last Modified: Wed, 11 May 2022 02:22:10 GMT  
		Size: 55.9 MB (55914622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899f353e6896a6f03a5af06a01cea44badeac7062481c294a9d7c1da1859b823`  
		Last Modified: Wed, 11 May 2022 02:22:52 GMT  
		Size: 199.5 MB (199502725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c70e60ad4e506736166da380bdcd6e33bfd1a6a4f654f0f1f21736de86b9d47`  
		Last Modified: Wed, 11 May 2022 15:49:27 GMT  
		Size: 170.4 MB (170444981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-buster`

```console
$ docker pull rust@sha256:66420d8dff60f4f94fc9ee8520193f50d26c69e356c52ed2113ddee8ed3ee1e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-buster` - linux; amd64

```console
$ docker pull rust@sha256:335e517975fc3f1573290c544a1497283dce84670afcb5501791fc138f40854f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **460.7 MB (460695435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b56360f6e8c1b377e4e1d7692cc692b67220afcac641058df0004062d349412e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:20:26 GMT
ADD file:54d60144d251caa916ff50606bc2364131d47d6b10ed83d08c81c647ab56cc40 in / 
# Wed, 11 May 2022 01:20:26 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:50:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:50:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:50:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:51:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 16:16:45 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Wed, 11 May 2022 16:16:59 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:b03a94565ecb6e02edf716307f25a0ea5090e3e2f7acec6a3687b95415378a30`  
		Last Modified: Wed, 11 May 2022 01:25:33 GMT  
		Size: 50.4 MB (50437966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7bcede80b1916d73be58ae0a2af8321770c4ce0c8ada05c39271e292355325`  
		Last Modified: Wed, 11 May 2022 01:58:28 GMT  
		Size: 7.9 MB (7856436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37471fc83c2dc382a8aec5dc1c1f0f2f8156f4df529cd1aea7647cbaee4b25fa`  
		Last Modified: Wed, 11 May 2022 01:58:28 GMT  
		Size: 10.0 MB (9997259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0162432a49c07aa492d3e1031af58a9a9f9b22acde859829434e5a54d019aa1c`  
		Last Modified: Wed, 11 May 2022 01:58:46 GMT  
		Size: 51.8 MB (51843657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee8ddc463fd0224112f41976e81d15dd46444f93185d9cde6203a0185857be2`  
		Last Modified: Wed, 11 May 2022 01:59:19 GMT  
		Size: 192.5 MB (192482405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5ec6530a2ae568c3e10b73d729658f9358962f4d4fc1b9ab79d73ec4fb3436`  
		Last Modified: Wed, 11 May 2022 16:19:31 GMT  
		Size: 148.1 MB (148077712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:fd9d31c4dc31d202d71684c47d09f22505d21c6f58bb8fb9ea8ad2a42dd9e047
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.0 MB (463027085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e30beb4107faddc83b15056987106bf5e40d261ce8c3e764f62bc881e188772c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:49:37 GMT
ADD file:9c75d7f24328b3f84cd700813a0a8ff5af16399f4475d24da9b0a859d584614c in / 
# Wed, 11 May 2022 01:49:38 GMT
CMD ["bash"]
# Wed, 11 May 2022 03:25:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:25:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 03:26:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:28:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 May 2022 17:58:16 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:58:55 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:f328f2671b27c760193a9d82808b176a8a7420205e8eb884e1fee20d2ac57ff0`  
		Last Modified: Wed, 11 May 2022 02:05:20 GMT  
		Size: 45.9 MB (45910176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e554a91160b4bf86ab199d7a5f5f105c5ffecc37b098c4274d98c264f677799`  
		Last Modified: Wed, 11 May 2022 03:49:35 GMT  
		Size: 7.1 MB (7145025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1b07ef419c0604851908ed718983760891b21a649a1b8758b871522e7d3e48`  
		Last Modified: Wed, 11 May 2022 03:49:36 GMT  
		Size: 9.3 MB (9343816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398961d3cf225ff82b93bd457012e308b756c455d1dbe1191bca51a54483f1d7`  
		Last Modified: Wed, 11 May 2022 03:50:19 GMT  
		Size: 47.4 MB (47359230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672070a3841f8c8993724742262e409c973f2ea02773250aff8b7c5bfe81bde6`  
		Last Modified: Wed, 11 May 2022 03:52:03 GMT  
		Size: 168.7 MB (168680126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061ddfe391b623d781b7e0bc3f1f46b681cb0ba8d2fe5efd31138be3e05e30b4`  
		Last Modified: Thu, 19 May 2022 18:06:48 GMT  
		Size: 184.6 MB (184588712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:efa3c3975a4197a5b384d9798b89538424265591c4da905fbc17cd1228c4386d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **506.0 MB (505953047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e47315b8b3fba316e10cf1a807d312f41f096082982190765b4f8bae9cac7d1a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:47:11 GMT
ADD file:5389b77733b44ebc41850baff3ebfc491726af264a745f108d5f16076a0f04ab in / 
# Wed, 11 May 2022 00:47:11 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:26:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:26:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:27:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:28:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 May 2022 17:57:05 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:57:22 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:5528d23e3f315103c99c14258e007a025d09bb4fd587c2d8a32d6dbb6047b891`  
		Last Modified: Wed, 11 May 2022 00:54:09 GMT  
		Size: 49.2 MB (49228300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b2d66a1dbe5960c6de4181ca3512467d3303dfb9cde3d92ecf7a85111cf68b`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 7.7 MB (7719789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9244ac9f9851b43ddc1032930666d339c3a5d9b934e2ca42ecd2e8ef3dd680`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 9.8 MB (9767329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06885dc77f03f05a5f98ceb35e871f027525d932d32027ed9d4ffb0cbd29786c`  
		Last Modified: Wed, 11 May 2022 01:37:21 GMT  
		Size: 52.2 MB (52174787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be89f33c0b133b07e3c53ae901bde6bf63f6a395cdf9c89c263e8d1e625a61cf`  
		Last Modified: Wed, 11 May 2022 01:37:55 GMT  
		Size: 184.1 MB (184054008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3d8265597d91c63bc1303ef37fc2a0650ffe5ef68084a8e38256d7bf63d60f`  
		Last Modified: Thu, 19 May 2022 18:01:26 GMT  
		Size: 203.0 MB (203008834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-buster` - linux; 386

```console
$ docker pull rust@sha256:cf59e8e28f4decd414f74110ad0353f30fad01bf052001e4d4b3d1e25d4efd6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **492.2 MB (492242448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e666158bab1d49cb47d1cb46aa91705753de2c6ca113913d58ce5ab42680d911`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:39:25 GMT
ADD file:03855eb19b36aa184d26264c1416a11ac7661faddae3436aad12661bb4c6e656 in / 
# Wed, 11 May 2022 01:39:26 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:12:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:12:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 02:13:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:14:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 15:44:36 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Wed, 11 May 2022 15:44:57 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:5b096db137216fbea3d646b6cad3959b69b6a1d27ff5f31bd01048df4a7e6c0a`  
		Last Modified: Wed, 11 May 2022 01:46:53 GMT  
		Size: 51.2 MB (51199249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aea31d1a573a95302db6857fc201016b7c6b8f21d0f56e011ec26f49e9d36b6`  
		Last Modified: Wed, 11 May 2022 02:23:08 GMT  
		Size: 8.0 MB (8022259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1841293ac8ab91433085e85c8c899e4324ca8f84a2cf4300cb5410542e39f4`  
		Last Modified: Wed, 11 May 2022 02:23:08 GMT  
		Size: 10.1 MB (10121987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c221acbd6711627d003a42bc75312b3994313814f1ba7a82f10f1e0e37b30b8`  
		Last Modified: Wed, 11 May 2022 02:23:28 GMT  
		Size: 53.4 MB (53442818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d4335971c3c6abcc0cee05c5dc4d86bb28ee87ad0592c808e4454c0579e3ce`  
		Last Modified: Wed, 11 May 2022 02:24:03 GMT  
		Size: 199.0 MB (199011140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93427b1a8630d73a8276d0e8952ddc49154b30b3ad1f78b5ad7cf18ab0abd93a`  
		Last Modified: Wed, 11 May 2022 15:47:59 GMT  
		Size: 170.4 MB (170444995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-slim`

```console
$ docker pull rust@sha256:6a2c53a0fb8f909c0332eaf974667acfb43d017f6ad870361c5baaeb9c09b40a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-slim` - linux; amd64

```console
$ docker pull rust@sha256:334e2416575c89f0e778fe692d7e1de52fdfe8071a1b82005c2c93357cb2fa87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.6 MB (239571414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd2de95a8dc1f3aaa60ddf0112df2d8a1472cd46a457fa458bb6422969807c39`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 16:17:57 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Wed, 11 May 2022 16:18:23 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349f1d9b940a31cb04a2b8c0149fd1139084f54b1fb2ce83a5b86d9c23cbb752`  
		Last Modified: Wed, 11 May 2022 16:21:44 GMT  
		Size: 208.2 MB (208191938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim` - linux; arm variant v7

```console
$ docker pull rust@sha256:637e4a0dcdbbe892de42340ab07af1a2f81cb6df83d40f81b596734a386727fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.4 MB (253447413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4246a64a5c89d0efdd649d037d047eeb0d7c814d2357291c30e81c30bfb7e7c4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:49:07 GMT
ADD file:7c0451fffe8a520c2ab23048948d76bfe0dc0d90298c3d859279ccd8815b84f6 in / 
# Wed, 11 May 2022 01:49:08 GMT
CMD ["bash"]
# Thu, 19 May 2022 18:01:43 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 18:02:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:1a9427b75b1c1db800cae7a9199bb4e508702e6761b17cc904d21441df43016c`  
		Last Modified: Wed, 11 May 2022 02:04:35 GMT  
		Size: 26.6 MB (26575672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3332501bc455d4c889b90983db4f5f72ae1416aaf135f5808f59c60316001ce0`  
		Last Modified: Thu, 19 May 2022 18:14:23 GMT  
		Size: 226.9 MB (226871741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:c24497850afb62c925899b8854fe8c0d5a9c0767145b5cf085e323167dec1eba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.6 MB (288562316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:163110751b432b68a68df23f35c12cd3c30c9ad7992d636e1f539c76abcf59cb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Thu, 19 May 2022 17:58:29 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:58:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3846b6fbdd10a62b50f55e5b616c2b9330ac2eccdc523f652aaa11c94da412a7`  
		Last Modified: Thu, 19 May 2022 18:04:14 GMT  
		Size: 258.5 MB (258496623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim` - linux; 386

```console
$ docker pull rust@sha256:db4d4cd5c20b48773f222cdd354efa8c6bbb873c8625e6af8d310b640990ef1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.4 MB (263392079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b263a284d7b8c23352b7916318acfea63cdfffa633191c5c06692e04541b8631`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:39:14 GMT
ADD file:9eecb0fd311177f9d226e914c411aef49b5de1930e73019d2ee24afed515b5a2 in / 
# Wed, 11 May 2022 01:39:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 15:46:08 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Wed, 11 May 2022 15:46:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:91c5bdbe4bf9f1970dd54ba71e2523649adce4e5240c2ff8a87711bf389ecba3`  
		Last Modified: Wed, 11 May 2022 01:46:25 GMT  
		Size: 32.4 MB (32389776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e2abe277b496c5ea655646e02aeedd052b26bb98861a2aacb50bba3f7d5b51`  
		Last Modified: Wed, 11 May 2022 15:50:51 GMT  
		Size: 231.0 MB (231002303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-slim-bullseye`

```console
$ docker pull rust@sha256:6a2c53a0fb8f909c0332eaf974667acfb43d017f6ad870361c5baaeb9c09b40a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-slim-bullseye` - linux; amd64

```console
$ docker pull rust@sha256:334e2416575c89f0e778fe692d7e1de52fdfe8071a1b82005c2c93357cb2fa87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.6 MB (239571414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd2de95a8dc1f3aaa60ddf0112df2d8a1472cd46a457fa458bb6422969807c39`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 16:17:57 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Wed, 11 May 2022 16:18:23 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349f1d9b940a31cb04a2b8c0149fd1139084f54b1fb2ce83a5b86d9c23cbb752`  
		Last Modified: Wed, 11 May 2022 16:21:44 GMT  
		Size: 208.2 MB (208191938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-bullseye` - linux; arm variant v7

```console
$ docker pull rust@sha256:637e4a0dcdbbe892de42340ab07af1a2f81cb6df83d40f81b596734a386727fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.4 MB (253447413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4246a64a5c89d0efdd649d037d047eeb0d7c814d2357291c30e81c30bfb7e7c4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:49:07 GMT
ADD file:7c0451fffe8a520c2ab23048948d76bfe0dc0d90298c3d859279ccd8815b84f6 in / 
# Wed, 11 May 2022 01:49:08 GMT
CMD ["bash"]
# Thu, 19 May 2022 18:01:43 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 18:02:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:1a9427b75b1c1db800cae7a9199bb4e508702e6761b17cc904d21441df43016c`  
		Last Modified: Wed, 11 May 2022 02:04:35 GMT  
		Size: 26.6 MB (26575672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3332501bc455d4c889b90983db4f5f72ae1416aaf135f5808f59c60316001ce0`  
		Last Modified: Thu, 19 May 2022 18:14:23 GMT  
		Size: 226.9 MB (226871741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:c24497850afb62c925899b8854fe8c0d5a9c0767145b5cf085e323167dec1eba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.6 MB (288562316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:163110751b432b68a68df23f35c12cd3c30c9ad7992d636e1f539c76abcf59cb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Thu, 19 May 2022 17:58:29 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:58:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3846b6fbdd10a62b50f55e5b616c2b9330ac2eccdc523f652aaa11c94da412a7`  
		Last Modified: Thu, 19 May 2022 18:04:14 GMT  
		Size: 258.5 MB (258496623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-bullseye` - linux; 386

```console
$ docker pull rust@sha256:db4d4cd5c20b48773f222cdd354efa8c6bbb873c8625e6af8d310b640990ef1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.4 MB (263392079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b263a284d7b8c23352b7916318acfea63cdfffa633191c5c06692e04541b8631`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:39:14 GMT
ADD file:9eecb0fd311177f9d226e914c411aef49b5de1930e73019d2ee24afed515b5a2 in / 
# Wed, 11 May 2022 01:39:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 15:46:08 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Wed, 11 May 2022 15:46:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:91c5bdbe4bf9f1970dd54ba71e2523649adce4e5240c2ff8a87711bf389ecba3`  
		Last Modified: Wed, 11 May 2022 01:46:25 GMT  
		Size: 32.4 MB (32389776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e2abe277b496c5ea655646e02aeedd052b26bb98861a2aacb50bba3f7d5b51`  
		Last Modified: Wed, 11 May 2022 15:50:51 GMT  
		Size: 231.0 MB (231002303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1-slim-buster`

```console
$ docker pull rust@sha256:8345ef78f92d4b7b3f5542107396f71d42f07a9aa30a2f020828f6d693db6712
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:1-slim-buster` - linux; amd64

```console
$ docker pull rust@sha256:ecf4984a4cbd456d3670449efe63c665bbf850b821c4d3a30a7dee7896d9f1cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.6 MB (220627247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cd1e35201514da9bdc71adeb5f0ad381ce84089c40a6419d02f3a73b6845e96`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 16:17:04 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Wed, 11 May 2022 16:17:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910c9723b9c8224fdc9165793746a7bdef632a394043bf09d8c357918d0d8eeb`  
		Last Modified: Wed, 11 May 2022 16:20:14 GMT  
		Size: 193.5 MB (193486525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:5787cef45a9f13e1dea2638ba8ec7d928a7d6c3e6769eef73355011f9d99f327
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.3 MB (240262048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:979601ce35358bda70bbec9cfa78b0566870036b24dc3a066b2f5e10cbae68f7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:50:13 GMT
ADD file:bccd1898e72cc79621c20ba59061d318521fbd2a8f10806cc3a1561fcbc9daad in / 
# Wed, 11 May 2022 01:50:14 GMT
CMD ["bash"]
# Thu, 19 May 2022 17:59:10 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 18:00:20 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:8f4c08df22a944142862818447616fff8b15d3a7ba383d4eeab678af698c2c43`  
		Last Modified: Wed, 11 May 2022 02:06:00 GMT  
		Size: 22.7 MB (22747864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7445544703dfa3d6936573907d147f14265cf553e666c39769991139c3c5216f`  
		Last Modified: Thu, 19 May 2022 18:09:17 GMT  
		Size: 217.5 MB (217514184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:541f0b63df779aee4eb28f4f2ef5ec9e3b7251be6011cd39f497c8e6472019d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.1 MB (269122908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92aa5b1b5884c8281bde8930fdbac8d2df5495182807435346629bb2a263e5dd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:47:26 GMT
ADD file:2536146c773d09db1a8fbbff00933acc459d8929feb3cff5b93ca4c23b577845 in / 
# Wed, 11 May 2022 00:47:26 GMT
CMD ["bash"]
# Thu, 19 May 2022 17:57:28 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:57:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:383d573fdcf2c6da56fdb61e120549d7bc200471208ca4c7c6605c57a0a87ef6`  
		Last Modified: Wed, 11 May 2022 00:54:36 GMT  
		Size: 25.9 MB (25909014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0503ec1485723fc8953ef8fca5ff5794d54c7f48e60e240180a9a96de34727c7`  
		Last Modified: Thu, 19 May 2022 18:02:19 GMT  
		Size: 243.2 MB (243213894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1-slim-buster` - linux; 386

```console
$ docker pull rust@sha256:03dd42304f522301e06612497c9c34cea732f64d94196fc16f7e18be55696cc9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.2 MB (248236964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a49488bafeb991a838b0f60a1097c2daeb50ef3baf7d3a536b33b99274c502e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:39:41 GMT
ADD file:fc7b00a8a5b0e703ac3ede5e2e51257f5ee709fcd35fee53e7b99d144cd873e4 in / 
# Wed, 11 May 2022 01:39:42 GMT
CMD ["bash"]
# Wed, 11 May 2022 15:45:03 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Wed, 11 May 2022 15:45:35 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:b1c376c64b69c16b8b035dfd04b99bb7769a5afdfb56a1241aa4ec8743e85aa7`  
		Last Modified: Wed, 11 May 2022 01:47:22 GMT  
		Size: 27.8 MB (27799149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6dac1eed3e092c2db915499da260dbc53370448565b8d7dd1a904bc0f736d7a`  
		Last Modified: Wed, 11 May 2022 15:48:47 GMT  
		Size: 220.4 MB (220437815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.61`

```console
$ docker pull rust@sha256:391047085f572cc2437f9fbc0dd8604686c91ae89649101da12c94a14ec4f8b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `rust:1.61` - linux; arm variant v7

```console
$ docker pull rust@sha256:1b59f7d09735e15b0343859d1cb098a1675f013e84347be76936ef9d888fd9e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **467.2 MB (467237488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adc5a024a4724b55a7cba85555cd244b2612ac3057ca98f267dabe0053aeac32`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:48:30 GMT
ADD file:d6545064ea0f75166d59e4d4a2df1e41a3477ae468e558e31f29857336978c0e in / 
# Wed, 11 May 2022 01:48:31 GMT
CMD ["bash"]
# Wed, 11 May 2022 03:21:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:21:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 03:22:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:24:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 May 2022 18:00:44 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 18:01:23 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:ba38f9a6c66968e207a7ada348a2110e3be0ff117e621d9e10ddd7c4becc0d2a`  
		Last Modified: Wed, 11 May 2022 02:03:49 GMT  
		Size: 50.1 MB (50134069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71423015d7b4f718e54ff1561cc06bb4c8357baedc23b49d25fe99cd4b0ae41`  
		Last Modified: Wed, 11 May 2022 03:46:39 GMT  
		Size: 4.9 MB (4924901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8f92194faa0a66e5bd160b229941428f0b0387c6e313e4f1f903c678fbb17e`  
		Last Modified: Wed, 11 May 2022 03:46:41 GMT  
		Size: 10.2 MB (10217886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c410c75a05c2df4ed485cda22fd35206e0ea4b9fbc9f096b11ed5adc6f83fa1c`  
		Last Modified: Wed, 11 May 2022 03:47:32 GMT  
		Size: 50.3 MB (50329744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767978ffc99a492ddd06d37b888a093595a05ac353ceefb2cc01a1322f34164a`  
		Last Modified: Wed, 11 May 2022 03:49:16 GMT  
		Size: 167.0 MB (167042139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3247bc72a5ac57b8481395404128439459da3cbe3d37697e6cce58dc91967469`  
		Last Modified: Thu, 19 May 2022 18:11:31 GMT  
		Size: 184.6 MB (184588749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.61` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:0f34bbe3d25473314051f103cf14a43e983500a742512514459dddebcec49acc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **516.4 MB (516393806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4db0c962f51c31164dcd6edf66e1078fa5fa7bd4324918135f1af9e95932bf8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:46:44 GMT
ADD file:239aa42118877a929b2fbfc0d5793fee7815289280affa5286de2459385c0679 in / 
# Wed, 11 May 2022 00:46:44 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:25:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:25:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:25:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:26:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 May 2022 17:58:06 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:58:21 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:3a36574378e6cece2dd3a839e1c0220eaccc4063b61d7481d1a19d3990c1f2c2`  
		Last Modified: Wed, 11 May 2022 00:53:15 GMT  
		Size: 53.6 MB (53634337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61d3345afba43846f3e638752cce2f0d1d47b21cc667ba08b00db10767a4702`  
		Last Modified: Wed, 11 May 2022 01:35:45 GMT  
		Size: 4.9 MB (4938615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e267d6aa58f93a513352a3b46c7addbf9335d7d43bfa4f1df4026d21785181c`  
		Last Modified: Wed, 11 May 2022 01:35:46 GMT  
		Size: 10.7 MB (10656992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f647907d26b879e0d43f6f4f0807f01e4dbdc034edcecbc988f6033cf401becf`  
		Last Modified: Wed, 11 May 2022 01:36:07 GMT  
		Size: 54.7 MB (54672822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0b3e17bdee16cf8bf269a4474bf56713879991bf87ff3bd790aa96a6f00e3c`  
		Last Modified: Wed, 11 May 2022 01:36:46 GMT  
		Size: 189.5 MB (189482172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cba956553646efe774f749ce526b98ebbff7a89a2eea4b21e77ae86ee7de78f`  
		Last Modified: Thu, 19 May 2022 18:03:05 GMT  
		Size: 203.0 MB (203008868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.61-alpine`

```console
$ docker pull rust@sha256:b53d3ccd8cbbed37065fbb20bc57fdc46ebb5e0cbf729df9a00873db566d30b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `rust:1.61-alpine` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:526dfcfffac3021335f243aabe2b93bf32fd231fbb0e65103266980eedd1e8c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.2 MB (239222115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4049c483a2db267242fac510cf462f66964cbb5e25e512ea43f6648c8e072819`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:18:36 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 19 May 2022 17:59:27 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:59:40 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c79c9d0c9a2cc2bdae9476b20ddb336848888d44ff7d5dfb719ff227ffb79c4`  
		Last Modified: Tue, 05 Apr 2022 07:21:11 GMT  
		Size: 36.1 MB (36073695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d80249e68d74cb54280b56279b2a423d8c0b7682f33bb9a362f716341403763`  
		Last Modified: Thu, 19 May 2022 18:05:57 GMT  
		Size: 200.4 MB (200431943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.61-alpine3.14`

```console
$ docker pull rust@sha256:b8ecdd0e0480b407e4ec6a69b118177ed1ffd197dc099460afc8427a33fde661
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `rust:1.61-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:301565f25377b33199f2e8117344416d3db0e6e5fcbe87594838ed22be3bc696
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.1 MB (239070495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3a8e3972791724a8ce0c813fa148fe8456cce8d81a3eab4f9ebd8b79ee56cc2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:18:14 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 19 May 2022 17:59:04 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:59:20 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757084716086a18d818bc8687efebb7931b4f95e66464768dd2f3a724165e5fb`  
		Last Modified: Tue, 05 Apr 2022 07:20:27 GMT  
		Size: 35.9 MB (35921106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7387a7ced2948ec0e416c953e2a8ae1f1fc9955fba656c8a23b60bb29663cc9e`  
		Last Modified: Thu, 19 May 2022 18:05:11 GMT  
		Size: 200.4 MB (200432000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.61-alpine3.15`

```console
$ docker pull rust@sha256:b53d3ccd8cbbed37065fbb20bc57fdc46ebb5e0cbf729df9a00873db566d30b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `rust:1.61-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:526dfcfffac3021335f243aabe2b93bf32fd231fbb0e65103266980eedd1e8c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.2 MB (239222115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4049c483a2db267242fac510cf462f66964cbb5e25e512ea43f6648c8e072819`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:18:36 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 19 May 2022 17:59:27 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:59:40 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c79c9d0c9a2cc2bdae9476b20ddb336848888d44ff7d5dfb719ff227ffb79c4`  
		Last Modified: Tue, 05 Apr 2022 07:21:11 GMT  
		Size: 36.1 MB (36073695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d80249e68d74cb54280b56279b2a423d8c0b7682f33bb9a362f716341403763`  
		Last Modified: Thu, 19 May 2022 18:05:57 GMT  
		Size: 200.4 MB (200431943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.61-bullseye`

```console
$ docker pull rust@sha256:391047085f572cc2437f9fbc0dd8604686c91ae89649101da12c94a14ec4f8b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `rust:1.61-bullseye` - linux; arm variant v7

```console
$ docker pull rust@sha256:1b59f7d09735e15b0343859d1cb098a1675f013e84347be76936ef9d888fd9e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **467.2 MB (467237488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adc5a024a4724b55a7cba85555cd244b2612ac3057ca98f267dabe0053aeac32`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:48:30 GMT
ADD file:d6545064ea0f75166d59e4d4a2df1e41a3477ae468e558e31f29857336978c0e in / 
# Wed, 11 May 2022 01:48:31 GMT
CMD ["bash"]
# Wed, 11 May 2022 03:21:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:21:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 03:22:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:24:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 May 2022 18:00:44 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 18:01:23 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:ba38f9a6c66968e207a7ada348a2110e3be0ff117e621d9e10ddd7c4becc0d2a`  
		Last Modified: Wed, 11 May 2022 02:03:49 GMT  
		Size: 50.1 MB (50134069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71423015d7b4f718e54ff1561cc06bb4c8357baedc23b49d25fe99cd4b0ae41`  
		Last Modified: Wed, 11 May 2022 03:46:39 GMT  
		Size: 4.9 MB (4924901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8f92194faa0a66e5bd160b229941428f0b0387c6e313e4f1f903c678fbb17e`  
		Last Modified: Wed, 11 May 2022 03:46:41 GMT  
		Size: 10.2 MB (10217886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c410c75a05c2df4ed485cda22fd35206e0ea4b9fbc9f096b11ed5adc6f83fa1c`  
		Last Modified: Wed, 11 May 2022 03:47:32 GMT  
		Size: 50.3 MB (50329744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767978ffc99a492ddd06d37b888a093595a05ac353ceefb2cc01a1322f34164a`  
		Last Modified: Wed, 11 May 2022 03:49:16 GMT  
		Size: 167.0 MB (167042139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3247bc72a5ac57b8481395404128439459da3cbe3d37697e6cce58dc91967469`  
		Last Modified: Thu, 19 May 2022 18:11:31 GMT  
		Size: 184.6 MB (184588749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.61-bullseye` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:0f34bbe3d25473314051f103cf14a43e983500a742512514459dddebcec49acc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **516.4 MB (516393806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4db0c962f51c31164dcd6edf66e1078fa5fa7bd4324918135f1af9e95932bf8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:46:44 GMT
ADD file:239aa42118877a929b2fbfc0d5793fee7815289280affa5286de2459385c0679 in / 
# Wed, 11 May 2022 00:46:44 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:25:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:25:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:25:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:26:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 May 2022 17:58:06 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:58:21 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:3a36574378e6cece2dd3a839e1c0220eaccc4063b61d7481d1a19d3990c1f2c2`  
		Last Modified: Wed, 11 May 2022 00:53:15 GMT  
		Size: 53.6 MB (53634337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61d3345afba43846f3e638752cce2f0d1d47b21cc667ba08b00db10767a4702`  
		Last Modified: Wed, 11 May 2022 01:35:45 GMT  
		Size: 4.9 MB (4938615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e267d6aa58f93a513352a3b46c7addbf9335d7d43bfa4f1df4026d21785181c`  
		Last Modified: Wed, 11 May 2022 01:35:46 GMT  
		Size: 10.7 MB (10656992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f647907d26b879e0d43f6f4f0807f01e4dbdc034edcecbc988f6033cf401becf`  
		Last Modified: Wed, 11 May 2022 01:36:07 GMT  
		Size: 54.7 MB (54672822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0b3e17bdee16cf8bf269a4474bf56713879991bf87ff3bd790aa96a6f00e3c`  
		Last Modified: Wed, 11 May 2022 01:36:46 GMT  
		Size: 189.5 MB (189482172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cba956553646efe774f749ce526b98ebbff7a89a2eea4b21e77ae86ee7de78f`  
		Last Modified: Thu, 19 May 2022 18:03:05 GMT  
		Size: 203.0 MB (203008868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.61-buster`

```console
$ docker pull rust@sha256:2902deb962c94384b26e61829fd6b3180e83d0b5a4dea3e83f281e62d8f1cc04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `rust:1.61-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:fd9d31c4dc31d202d71684c47d09f22505d21c6f58bb8fb9ea8ad2a42dd9e047
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.0 MB (463027085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e30beb4107faddc83b15056987106bf5e40d261ce8c3e764f62bc881e188772c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:49:37 GMT
ADD file:9c75d7f24328b3f84cd700813a0a8ff5af16399f4475d24da9b0a859d584614c in / 
# Wed, 11 May 2022 01:49:38 GMT
CMD ["bash"]
# Wed, 11 May 2022 03:25:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:25:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 03:26:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:28:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 May 2022 17:58:16 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:58:55 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:f328f2671b27c760193a9d82808b176a8a7420205e8eb884e1fee20d2ac57ff0`  
		Last Modified: Wed, 11 May 2022 02:05:20 GMT  
		Size: 45.9 MB (45910176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e554a91160b4bf86ab199d7a5f5f105c5ffecc37b098c4274d98c264f677799`  
		Last Modified: Wed, 11 May 2022 03:49:35 GMT  
		Size: 7.1 MB (7145025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1b07ef419c0604851908ed718983760891b21a649a1b8758b871522e7d3e48`  
		Last Modified: Wed, 11 May 2022 03:49:36 GMT  
		Size: 9.3 MB (9343816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398961d3cf225ff82b93bd457012e308b756c455d1dbe1191bca51a54483f1d7`  
		Last Modified: Wed, 11 May 2022 03:50:19 GMT  
		Size: 47.4 MB (47359230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672070a3841f8c8993724742262e409c973f2ea02773250aff8b7c5bfe81bde6`  
		Last Modified: Wed, 11 May 2022 03:52:03 GMT  
		Size: 168.7 MB (168680126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061ddfe391b623d781b7e0bc3f1f46b681cb0ba8d2fe5efd31138be3e05e30b4`  
		Last Modified: Thu, 19 May 2022 18:06:48 GMT  
		Size: 184.6 MB (184588712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.61-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:efa3c3975a4197a5b384d9798b89538424265591c4da905fbc17cd1228c4386d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **506.0 MB (505953047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e47315b8b3fba316e10cf1a807d312f41f096082982190765b4f8bae9cac7d1a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:47:11 GMT
ADD file:5389b77733b44ebc41850baff3ebfc491726af264a745f108d5f16076a0f04ab in / 
# Wed, 11 May 2022 00:47:11 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:26:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:26:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:27:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:28:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 May 2022 17:57:05 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:57:22 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:5528d23e3f315103c99c14258e007a025d09bb4fd587c2d8a32d6dbb6047b891`  
		Last Modified: Wed, 11 May 2022 00:54:09 GMT  
		Size: 49.2 MB (49228300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b2d66a1dbe5960c6de4181ca3512467d3303dfb9cde3d92ecf7a85111cf68b`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 7.7 MB (7719789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9244ac9f9851b43ddc1032930666d339c3a5d9b934e2ca42ecd2e8ef3dd680`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 9.8 MB (9767329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06885dc77f03f05a5f98ceb35e871f027525d932d32027ed9d4ffb0cbd29786c`  
		Last Modified: Wed, 11 May 2022 01:37:21 GMT  
		Size: 52.2 MB (52174787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be89f33c0b133b07e3c53ae901bde6bf63f6a395cdf9c89c263e8d1e625a61cf`  
		Last Modified: Wed, 11 May 2022 01:37:55 GMT  
		Size: 184.1 MB (184054008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3d8265597d91c63bc1303ef37fc2a0650ffe5ef68084a8e38256d7bf63d60f`  
		Last Modified: Thu, 19 May 2022 18:01:26 GMT  
		Size: 203.0 MB (203008834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.61-slim`

```console
$ docker pull rust@sha256:9fb2fe004423be5e8ec48100fb33c6da30770ed56f9eb73aa1c8dc702426027f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `rust:1.61-slim` - linux; arm variant v7

```console
$ docker pull rust@sha256:637e4a0dcdbbe892de42340ab07af1a2f81cb6df83d40f81b596734a386727fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.4 MB (253447413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4246a64a5c89d0efdd649d037d047eeb0d7c814d2357291c30e81c30bfb7e7c4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:49:07 GMT
ADD file:7c0451fffe8a520c2ab23048948d76bfe0dc0d90298c3d859279ccd8815b84f6 in / 
# Wed, 11 May 2022 01:49:08 GMT
CMD ["bash"]
# Thu, 19 May 2022 18:01:43 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 18:02:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:1a9427b75b1c1db800cae7a9199bb4e508702e6761b17cc904d21441df43016c`  
		Last Modified: Wed, 11 May 2022 02:04:35 GMT  
		Size: 26.6 MB (26575672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3332501bc455d4c889b90983db4f5f72ae1416aaf135f5808f59c60316001ce0`  
		Last Modified: Thu, 19 May 2022 18:14:23 GMT  
		Size: 226.9 MB (226871741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.61-slim` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:c24497850afb62c925899b8854fe8c0d5a9c0767145b5cf085e323167dec1eba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.6 MB (288562316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:163110751b432b68a68df23f35c12cd3c30c9ad7992d636e1f539c76abcf59cb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Thu, 19 May 2022 17:58:29 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:58:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3846b6fbdd10a62b50f55e5b616c2b9330ac2eccdc523f652aaa11c94da412a7`  
		Last Modified: Thu, 19 May 2022 18:04:14 GMT  
		Size: 258.5 MB (258496623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.61-slim-bullseye`

```console
$ docker pull rust@sha256:9fb2fe004423be5e8ec48100fb33c6da30770ed56f9eb73aa1c8dc702426027f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `rust:1.61-slim-bullseye` - linux; arm variant v7

```console
$ docker pull rust@sha256:637e4a0dcdbbe892de42340ab07af1a2f81cb6df83d40f81b596734a386727fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.4 MB (253447413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4246a64a5c89d0efdd649d037d047eeb0d7c814d2357291c30e81c30bfb7e7c4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:49:07 GMT
ADD file:7c0451fffe8a520c2ab23048948d76bfe0dc0d90298c3d859279ccd8815b84f6 in / 
# Wed, 11 May 2022 01:49:08 GMT
CMD ["bash"]
# Thu, 19 May 2022 18:01:43 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 18:02:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:1a9427b75b1c1db800cae7a9199bb4e508702e6761b17cc904d21441df43016c`  
		Last Modified: Wed, 11 May 2022 02:04:35 GMT  
		Size: 26.6 MB (26575672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3332501bc455d4c889b90983db4f5f72ae1416aaf135f5808f59c60316001ce0`  
		Last Modified: Thu, 19 May 2022 18:14:23 GMT  
		Size: 226.9 MB (226871741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.61-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:c24497850afb62c925899b8854fe8c0d5a9c0767145b5cf085e323167dec1eba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.6 MB (288562316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:163110751b432b68a68df23f35c12cd3c30c9ad7992d636e1f539c76abcf59cb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Thu, 19 May 2022 17:58:29 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:58:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3846b6fbdd10a62b50f55e5b616c2b9330ac2eccdc523f652aaa11c94da412a7`  
		Last Modified: Thu, 19 May 2022 18:04:14 GMT  
		Size: 258.5 MB (258496623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.61-slim-buster`

```console
$ docker pull rust@sha256:cd8692e04d98f4750e83895f31d29a0c15c99fb5e65e50f9d3f3ef52e0ae471a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `rust:1.61-slim-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:5787cef45a9f13e1dea2638ba8ec7d928a7d6c3e6769eef73355011f9d99f327
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.3 MB (240262048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:979601ce35358bda70bbec9cfa78b0566870036b24dc3a066b2f5e10cbae68f7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:50:13 GMT
ADD file:bccd1898e72cc79621c20ba59061d318521fbd2a8f10806cc3a1561fcbc9daad in / 
# Wed, 11 May 2022 01:50:14 GMT
CMD ["bash"]
# Thu, 19 May 2022 17:59:10 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 18:00:20 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:8f4c08df22a944142862818447616fff8b15d3a7ba383d4eeab678af698c2c43`  
		Last Modified: Wed, 11 May 2022 02:06:00 GMT  
		Size: 22.7 MB (22747864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7445544703dfa3d6936573907d147f14265cf553e666c39769991139c3c5216f`  
		Last Modified: Thu, 19 May 2022 18:09:17 GMT  
		Size: 217.5 MB (217514184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.61-slim-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:541f0b63df779aee4eb28f4f2ef5ec9e3b7251be6011cd39f497c8e6472019d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.1 MB (269122908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92aa5b1b5884c8281bde8930fdbac8d2df5495182807435346629bb2a263e5dd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:47:26 GMT
ADD file:2536146c773d09db1a8fbbff00933acc459d8929feb3cff5b93ca4c23b577845 in / 
# Wed, 11 May 2022 00:47:26 GMT
CMD ["bash"]
# Thu, 19 May 2022 17:57:28 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:57:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:383d573fdcf2c6da56fdb61e120549d7bc200471208ca4c7c6605c57a0a87ef6`  
		Last Modified: Wed, 11 May 2022 00:54:36 GMT  
		Size: 25.9 MB (25909014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0503ec1485723fc8953ef8fca5ff5794d54c7f48e60e240180a9a96de34727c7`  
		Last Modified: Thu, 19 May 2022 18:02:19 GMT  
		Size: 243.2 MB (243213894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.61.0`

```console
$ docker pull rust@sha256:391047085f572cc2437f9fbc0dd8604686c91ae89649101da12c94a14ec4f8b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `rust:1.61.0` - linux; arm variant v7

```console
$ docker pull rust@sha256:1b59f7d09735e15b0343859d1cb098a1675f013e84347be76936ef9d888fd9e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **467.2 MB (467237488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adc5a024a4724b55a7cba85555cd244b2612ac3057ca98f267dabe0053aeac32`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:48:30 GMT
ADD file:d6545064ea0f75166d59e4d4a2df1e41a3477ae468e558e31f29857336978c0e in / 
# Wed, 11 May 2022 01:48:31 GMT
CMD ["bash"]
# Wed, 11 May 2022 03:21:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:21:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 03:22:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:24:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 May 2022 18:00:44 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 18:01:23 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:ba38f9a6c66968e207a7ada348a2110e3be0ff117e621d9e10ddd7c4becc0d2a`  
		Last Modified: Wed, 11 May 2022 02:03:49 GMT  
		Size: 50.1 MB (50134069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71423015d7b4f718e54ff1561cc06bb4c8357baedc23b49d25fe99cd4b0ae41`  
		Last Modified: Wed, 11 May 2022 03:46:39 GMT  
		Size: 4.9 MB (4924901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8f92194faa0a66e5bd160b229941428f0b0387c6e313e4f1f903c678fbb17e`  
		Last Modified: Wed, 11 May 2022 03:46:41 GMT  
		Size: 10.2 MB (10217886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c410c75a05c2df4ed485cda22fd35206e0ea4b9fbc9f096b11ed5adc6f83fa1c`  
		Last Modified: Wed, 11 May 2022 03:47:32 GMT  
		Size: 50.3 MB (50329744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767978ffc99a492ddd06d37b888a093595a05ac353ceefb2cc01a1322f34164a`  
		Last Modified: Wed, 11 May 2022 03:49:16 GMT  
		Size: 167.0 MB (167042139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3247bc72a5ac57b8481395404128439459da3cbe3d37697e6cce58dc91967469`  
		Last Modified: Thu, 19 May 2022 18:11:31 GMT  
		Size: 184.6 MB (184588749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.61.0` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:0f34bbe3d25473314051f103cf14a43e983500a742512514459dddebcec49acc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **516.4 MB (516393806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4db0c962f51c31164dcd6edf66e1078fa5fa7bd4324918135f1af9e95932bf8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:46:44 GMT
ADD file:239aa42118877a929b2fbfc0d5793fee7815289280affa5286de2459385c0679 in / 
# Wed, 11 May 2022 00:46:44 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:25:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:25:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:25:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:26:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 May 2022 17:58:06 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:58:21 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:3a36574378e6cece2dd3a839e1c0220eaccc4063b61d7481d1a19d3990c1f2c2`  
		Last Modified: Wed, 11 May 2022 00:53:15 GMT  
		Size: 53.6 MB (53634337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61d3345afba43846f3e638752cce2f0d1d47b21cc667ba08b00db10767a4702`  
		Last Modified: Wed, 11 May 2022 01:35:45 GMT  
		Size: 4.9 MB (4938615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e267d6aa58f93a513352a3b46c7addbf9335d7d43bfa4f1df4026d21785181c`  
		Last Modified: Wed, 11 May 2022 01:35:46 GMT  
		Size: 10.7 MB (10656992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f647907d26b879e0d43f6f4f0807f01e4dbdc034edcecbc988f6033cf401becf`  
		Last Modified: Wed, 11 May 2022 01:36:07 GMT  
		Size: 54.7 MB (54672822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0b3e17bdee16cf8bf269a4474bf56713879991bf87ff3bd790aa96a6f00e3c`  
		Last Modified: Wed, 11 May 2022 01:36:46 GMT  
		Size: 189.5 MB (189482172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cba956553646efe774f749ce526b98ebbff7a89a2eea4b21e77ae86ee7de78f`  
		Last Modified: Thu, 19 May 2022 18:03:05 GMT  
		Size: 203.0 MB (203008868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.61.0-alpine`

```console
$ docker pull rust@sha256:b53d3ccd8cbbed37065fbb20bc57fdc46ebb5e0cbf729df9a00873db566d30b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `rust:1.61.0-alpine` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:526dfcfffac3021335f243aabe2b93bf32fd231fbb0e65103266980eedd1e8c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.2 MB (239222115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4049c483a2db267242fac510cf462f66964cbb5e25e512ea43f6648c8e072819`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:18:36 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 19 May 2022 17:59:27 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:59:40 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c79c9d0c9a2cc2bdae9476b20ddb336848888d44ff7d5dfb719ff227ffb79c4`  
		Last Modified: Tue, 05 Apr 2022 07:21:11 GMT  
		Size: 36.1 MB (36073695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d80249e68d74cb54280b56279b2a423d8c0b7682f33bb9a362f716341403763`  
		Last Modified: Thu, 19 May 2022 18:05:57 GMT  
		Size: 200.4 MB (200431943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.61.0-alpine3.14`

```console
$ docker pull rust@sha256:b8ecdd0e0480b407e4ec6a69b118177ed1ffd197dc099460afc8427a33fde661
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `rust:1.61.0-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:301565f25377b33199f2e8117344416d3db0e6e5fcbe87594838ed22be3bc696
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.1 MB (239070495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3a8e3972791724a8ce0c813fa148fe8456cce8d81a3eab4f9ebd8b79ee56cc2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:18:14 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 19 May 2022 17:59:04 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:59:20 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757084716086a18d818bc8687efebb7931b4f95e66464768dd2f3a724165e5fb`  
		Last Modified: Tue, 05 Apr 2022 07:20:27 GMT  
		Size: 35.9 MB (35921106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7387a7ced2948ec0e416c953e2a8ae1f1fc9955fba656c8a23b60bb29663cc9e`  
		Last Modified: Thu, 19 May 2022 18:05:11 GMT  
		Size: 200.4 MB (200432000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.61.0-alpine3.15`

```console
$ docker pull rust@sha256:b53d3ccd8cbbed37065fbb20bc57fdc46ebb5e0cbf729df9a00873db566d30b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `rust:1.61.0-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:526dfcfffac3021335f243aabe2b93bf32fd231fbb0e65103266980eedd1e8c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.2 MB (239222115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4049c483a2db267242fac510cf462f66964cbb5e25e512ea43f6648c8e072819`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:18:36 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 19 May 2022 17:59:27 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:59:40 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c79c9d0c9a2cc2bdae9476b20ddb336848888d44ff7d5dfb719ff227ffb79c4`  
		Last Modified: Tue, 05 Apr 2022 07:21:11 GMT  
		Size: 36.1 MB (36073695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d80249e68d74cb54280b56279b2a423d8c0b7682f33bb9a362f716341403763`  
		Last Modified: Thu, 19 May 2022 18:05:57 GMT  
		Size: 200.4 MB (200431943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.61.0-bullseye`

```console
$ docker pull rust@sha256:391047085f572cc2437f9fbc0dd8604686c91ae89649101da12c94a14ec4f8b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `rust:1.61.0-bullseye` - linux; arm variant v7

```console
$ docker pull rust@sha256:1b59f7d09735e15b0343859d1cb098a1675f013e84347be76936ef9d888fd9e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **467.2 MB (467237488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adc5a024a4724b55a7cba85555cd244b2612ac3057ca98f267dabe0053aeac32`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:48:30 GMT
ADD file:d6545064ea0f75166d59e4d4a2df1e41a3477ae468e558e31f29857336978c0e in / 
# Wed, 11 May 2022 01:48:31 GMT
CMD ["bash"]
# Wed, 11 May 2022 03:21:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:21:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 03:22:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:24:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 May 2022 18:00:44 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 18:01:23 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:ba38f9a6c66968e207a7ada348a2110e3be0ff117e621d9e10ddd7c4becc0d2a`  
		Last Modified: Wed, 11 May 2022 02:03:49 GMT  
		Size: 50.1 MB (50134069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71423015d7b4f718e54ff1561cc06bb4c8357baedc23b49d25fe99cd4b0ae41`  
		Last Modified: Wed, 11 May 2022 03:46:39 GMT  
		Size: 4.9 MB (4924901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8f92194faa0a66e5bd160b229941428f0b0387c6e313e4f1f903c678fbb17e`  
		Last Modified: Wed, 11 May 2022 03:46:41 GMT  
		Size: 10.2 MB (10217886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c410c75a05c2df4ed485cda22fd35206e0ea4b9fbc9f096b11ed5adc6f83fa1c`  
		Last Modified: Wed, 11 May 2022 03:47:32 GMT  
		Size: 50.3 MB (50329744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767978ffc99a492ddd06d37b888a093595a05ac353ceefb2cc01a1322f34164a`  
		Last Modified: Wed, 11 May 2022 03:49:16 GMT  
		Size: 167.0 MB (167042139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3247bc72a5ac57b8481395404128439459da3cbe3d37697e6cce58dc91967469`  
		Last Modified: Thu, 19 May 2022 18:11:31 GMT  
		Size: 184.6 MB (184588749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.61.0-bullseye` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:0f34bbe3d25473314051f103cf14a43e983500a742512514459dddebcec49acc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **516.4 MB (516393806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4db0c962f51c31164dcd6edf66e1078fa5fa7bd4324918135f1af9e95932bf8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:46:44 GMT
ADD file:239aa42118877a929b2fbfc0d5793fee7815289280affa5286de2459385c0679 in / 
# Wed, 11 May 2022 00:46:44 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:25:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:25:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:25:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:26:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 May 2022 17:58:06 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:58:21 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:3a36574378e6cece2dd3a839e1c0220eaccc4063b61d7481d1a19d3990c1f2c2`  
		Last Modified: Wed, 11 May 2022 00:53:15 GMT  
		Size: 53.6 MB (53634337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61d3345afba43846f3e638752cce2f0d1d47b21cc667ba08b00db10767a4702`  
		Last Modified: Wed, 11 May 2022 01:35:45 GMT  
		Size: 4.9 MB (4938615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e267d6aa58f93a513352a3b46c7addbf9335d7d43bfa4f1df4026d21785181c`  
		Last Modified: Wed, 11 May 2022 01:35:46 GMT  
		Size: 10.7 MB (10656992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f647907d26b879e0d43f6f4f0807f01e4dbdc034edcecbc988f6033cf401becf`  
		Last Modified: Wed, 11 May 2022 01:36:07 GMT  
		Size: 54.7 MB (54672822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0b3e17bdee16cf8bf269a4474bf56713879991bf87ff3bd790aa96a6f00e3c`  
		Last Modified: Wed, 11 May 2022 01:36:46 GMT  
		Size: 189.5 MB (189482172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cba956553646efe774f749ce526b98ebbff7a89a2eea4b21e77ae86ee7de78f`  
		Last Modified: Thu, 19 May 2022 18:03:05 GMT  
		Size: 203.0 MB (203008868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.61.0-buster`

```console
$ docker pull rust@sha256:2902deb962c94384b26e61829fd6b3180e83d0b5a4dea3e83f281e62d8f1cc04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `rust:1.61.0-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:fd9d31c4dc31d202d71684c47d09f22505d21c6f58bb8fb9ea8ad2a42dd9e047
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.0 MB (463027085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e30beb4107faddc83b15056987106bf5e40d261ce8c3e764f62bc881e188772c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:49:37 GMT
ADD file:9c75d7f24328b3f84cd700813a0a8ff5af16399f4475d24da9b0a859d584614c in / 
# Wed, 11 May 2022 01:49:38 GMT
CMD ["bash"]
# Wed, 11 May 2022 03:25:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:25:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 03:26:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:28:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 May 2022 17:58:16 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:58:55 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:f328f2671b27c760193a9d82808b176a8a7420205e8eb884e1fee20d2ac57ff0`  
		Last Modified: Wed, 11 May 2022 02:05:20 GMT  
		Size: 45.9 MB (45910176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e554a91160b4bf86ab199d7a5f5f105c5ffecc37b098c4274d98c264f677799`  
		Last Modified: Wed, 11 May 2022 03:49:35 GMT  
		Size: 7.1 MB (7145025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1b07ef419c0604851908ed718983760891b21a649a1b8758b871522e7d3e48`  
		Last Modified: Wed, 11 May 2022 03:49:36 GMT  
		Size: 9.3 MB (9343816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398961d3cf225ff82b93bd457012e308b756c455d1dbe1191bca51a54483f1d7`  
		Last Modified: Wed, 11 May 2022 03:50:19 GMT  
		Size: 47.4 MB (47359230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672070a3841f8c8993724742262e409c973f2ea02773250aff8b7c5bfe81bde6`  
		Last Modified: Wed, 11 May 2022 03:52:03 GMT  
		Size: 168.7 MB (168680126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061ddfe391b623d781b7e0bc3f1f46b681cb0ba8d2fe5efd31138be3e05e30b4`  
		Last Modified: Thu, 19 May 2022 18:06:48 GMT  
		Size: 184.6 MB (184588712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.61.0-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:efa3c3975a4197a5b384d9798b89538424265591c4da905fbc17cd1228c4386d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **506.0 MB (505953047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e47315b8b3fba316e10cf1a807d312f41f096082982190765b4f8bae9cac7d1a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:47:11 GMT
ADD file:5389b77733b44ebc41850baff3ebfc491726af264a745f108d5f16076a0f04ab in / 
# Wed, 11 May 2022 00:47:11 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:26:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:26:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:27:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:28:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 May 2022 17:57:05 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:57:22 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:5528d23e3f315103c99c14258e007a025d09bb4fd587c2d8a32d6dbb6047b891`  
		Last Modified: Wed, 11 May 2022 00:54:09 GMT  
		Size: 49.2 MB (49228300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b2d66a1dbe5960c6de4181ca3512467d3303dfb9cde3d92ecf7a85111cf68b`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 7.7 MB (7719789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9244ac9f9851b43ddc1032930666d339c3a5d9b934e2ca42ecd2e8ef3dd680`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 9.8 MB (9767329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06885dc77f03f05a5f98ceb35e871f027525d932d32027ed9d4ffb0cbd29786c`  
		Last Modified: Wed, 11 May 2022 01:37:21 GMT  
		Size: 52.2 MB (52174787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be89f33c0b133b07e3c53ae901bde6bf63f6a395cdf9c89c263e8d1e625a61cf`  
		Last Modified: Wed, 11 May 2022 01:37:55 GMT  
		Size: 184.1 MB (184054008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3d8265597d91c63bc1303ef37fc2a0650ffe5ef68084a8e38256d7bf63d60f`  
		Last Modified: Thu, 19 May 2022 18:01:26 GMT  
		Size: 203.0 MB (203008834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.61.0-slim`

```console
$ docker pull rust@sha256:9fb2fe004423be5e8ec48100fb33c6da30770ed56f9eb73aa1c8dc702426027f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `rust:1.61.0-slim` - linux; arm variant v7

```console
$ docker pull rust@sha256:637e4a0dcdbbe892de42340ab07af1a2f81cb6df83d40f81b596734a386727fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.4 MB (253447413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4246a64a5c89d0efdd649d037d047eeb0d7c814d2357291c30e81c30bfb7e7c4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:49:07 GMT
ADD file:7c0451fffe8a520c2ab23048948d76bfe0dc0d90298c3d859279ccd8815b84f6 in / 
# Wed, 11 May 2022 01:49:08 GMT
CMD ["bash"]
# Thu, 19 May 2022 18:01:43 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 18:02:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:1a9427b75b1c1db800cae7a9199bb4e508702e6761b17cc904d21441df43016c`  
		Last Modified: Wed, 11 May 2022 02:04:35 GMT  
		Size: 26.6 MB (26575672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3332501bc455d4c889b90983db4f5f72ae1416aaf135f5808f59c60316001ce0`  
		Last Modified: Thu, 19 May 2022 18:14:23 GMT  
		Size: 226.9 MB (226871741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.61.0-slim` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:c24497850afb62c925899b8854fe8c0d5a9c0767145b5cf085e323167dec1eba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.6 MB (288562316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:163110751b432b68a68df23f35c12cd3c30c9ad7992d636e1f539c76abcf59cb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Thu, 19 May 2022 17:58:29 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:58:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3846b6fbdd10a62b50f55e5b616c2b9330ac2eccdc523f652aaa11c94da412a7`  
		Last Modified: Thu, 19 May 2022 18:04:14 GMT  
		Size: 258.5 MB (258496623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.61.0-slim-bullseye`

```console
$ docker pull rust@sha256:9fb2fe004423be5e8ec48100fb33c6da30770ed56f9eb73aa1c8dc702426027f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `rust:1.61.0-slim-bullseye` - linux; arm variant v7

```console
$ docker pull rust@sha256:637e4a0dcdbbe892de42340ab07af1a2f81cb6df83d40f81b596734a386727fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.4 MB (253447413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4246a64a5c89d0efdd649d037d047eeb0d7c814d2357291c30e81c30bfb7e7c4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:49:07 GMT
ADD file:7c0451fffe8a520c2ab23048948d76bfe0dc0d90298c3d859279ccd8815b84f6 in / 
# Wed, 11 May 2022 01:49:08 GMT
CMD ["bash"]
# Thu, 19 May 2022 18:01:43 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 18:02:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:1a9427b75b1c1db800cae7a9199bb4e508702e6761b17cc904d21441df43016c`  
		Last Modified: Wed, 11 May 2022 02:04:35 GMT  
		Size: 26.6 MB (26575672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3332501bc455d4c889b90983db4f5f72ae1416aaf135f5808f59c60316001ce0`  
		Last Modified: Thu, 19 May 2022 18:14:23 GMT  
		Size: 226.9 MB (226871741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.61.0-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:c24497850afb62c925899b8854fe8c0d5a9c0767145b5cf085e323167dec1eba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.6 MB (288562316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:163110751b432b68a68df23f35c12cd3c30c9ad7992d636e1f539c76abcf59cb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Thu, 19 May 2022 17:58:29 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:58:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3846b6fbdd10a62b50f55e5b616c2b9330ac2eccdc523f652aaa11c94da412a7`  
		Last Modified: Thu, 19 May 2022 18:04:14 GMT  
		Size: 258.5 MB (258496623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:1.61.0-slim-buster`

```console
$ docker pull rust@sha256:cd8692e04d98f4750e83895f31d29a0c15c99fb5e65e50f9d3f3ef52e0ae471a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `rust:1.61.0-slim-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:5787cef45a9f13e1dea2638ba8ec7d928a7d6c3e6769eef73355011f9d99f327
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.3 MB (240262048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:979601ce35358bda70bbec9cfa78b0566870036b24dc3a066b2f5e10cbae68f7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:50:13 GMT
ADD file:bccd1898e72cc79621c20ba59061d318521fbd2a8f10806cc3a1561fcbc9daad in / 
# Wed, 11 May 2022 01:50:14 GMT
CMD ["bash"]
# Thu, 19 May 2022 17:59:10 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 18:00:20 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:8f4c08df22a944142862818447616fff8b15d3a7ba383d4eeab678af698c2c43`  
		Last Modified: Wed, 11 May 2022 02:06:00 GMT  
		Size: 22.7 MB (22747864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7445544703dfa3d6936573907d147f14265cf553e666c39769991139c3c5216f`  
		Last Modified: Thu, 19 May 2022 18:09:17 GMT  
		Size: 217.5 MB (217514184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:1.61.0-slim-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:541f0b63df779aee4eb28f4f2ef5ec9e3b7251be6011cd39f497c8e6472019d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.1 MB (269122908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92aa5b1b5884c8281bde8930fdbac8d2df5495182807435346629bb2a263e5dd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:47:26 GMT
ADD file:2536146c773d09db1a8fbbff00933acc459d8929feb3cff5b93ca4c23b577845 in / 
# Wed, 11 May 2022 00:47:26 GMT
CMD ["bash"]
# Thu, 19 May 2022 17:57:28 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:57:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:383d573fdcf2c6da56fdb61e120549d7bc200471208ca4c7c6605c57a0a87ef6`  
		Last Modified: Wed, 11 May 2022 00:54:36 GMT  
		Size: 25.9 MB (25909014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0503ec1485723fc8953ef8fca5ff5794d54c7f48e60e240180a9a96de34727c7`  
		Last Modified: Thu, 19 May 2022 18:02:19 GMT  
		Size: 243.2 MB (243213894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:alpine`

```console
$ docker pull rust@sha256:7a917171c2fa060a2665b291820507bca0484efd25811a1c09073b0cfc5cb23d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:alpine` - linux; amd64

```console
$ docker pull rust@sha256:e1ddd35b6a802ac8587f8fbc34ce752be20b5c116df2b2f1a90488f0bc3bd439
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.6 MB (249551918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5fbf9bd1849d2598eff6ddedc32b06610905188571179b4a4b0805d6331c549`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:50:48 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 07 Apr 2022 20:22:16 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Thu, 07 Apr 2022 20:22:35 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2113a6fa04a6792c25bda8b467d30b4388d756ab1f526efb6ce7139d464f5b84`  
		Last Modified: Tue, 05 Apr 2022 10:52:45 GMT  
		Size: 42.5 MB (42476793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82ca4327e1d9bb80a8af0bb460d9bef24f8e88470631e2c788f996e91e3d8a7`  
		Last Modified: Thu, 07 Apr 2022 20:27:23 GMT  
		Size: 204.3 MB (204260566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:alpine` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:526dfcfffac3021335f243aabe2b93bf32fd231fbb0e65103266980eedd1e8c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.2 MB (239222115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4049c483a2db267242fac510cf462f66964cbb5e25e512ea43f6648c8e072819`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:18:36 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 19 May 2022 17:59:27 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:59:40 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c79c9d0c9a2cc2bdae9476b20ddb336848888d44ff7d5dfb719ff227ffb79c4`  
		Last Modified: Tue, 05 Apr 2022 07:21:11 GMT  
		Size: 36.1 MB (36073695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d80249e68d74cb54280b56279b2a423d8c0b7682f33bb9a362f716341403763`  
		Last Modified: Thu, 19 May 2022 18:05:57 GMT  
		Size: 200.4 MB (200431943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:alpine3.14`

```console
$ docker pull rust@sha256:dc154448faa074931911a7d85ee984a07786f64f3414978368c764afd6b2a971
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:alpine3.14` - linux; amd64

```console
$ docker pull rust@sha256:c4a4a463cd986120a16f1e7e44d77238acc18b31bbdaa66254adb8bde4cb2496
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.4 MB (249419447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a59e129e5e042f57ee01d253e60fafce1011ff98bf3517ab7a1369e32d3242c1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:50:20 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 07 Apr 2022 20:21:52 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Thu, 07 Apr 2022 20:22:12 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77041b2d00354ec0aeef4267546654f2d783ec91f776e89b924b2759dcf3cf7`  
		Last Modified: Tue, 05 Apr 2022 10:52:01 GMT  
		Size: 42.3 MB (42340505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994ac804f5895d53d5a70de8f2d11672e5c6a688fdb5a78f159c3335291914f9`  
		Last Modified: Thu, 07 Apr 2022 20:26:39 GMT  
		Size: 204.3 MB (204260572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:alpine3.14` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:301565f25377b33199f2e8117344416d3db0e6e5fcbe87594838ed22be3bc696
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.1 MB (239070495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3a8e3972791724a8ce0c813fa148fe8456cce8d81a3eab4f9ebd8b79ee56cc2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:18:14 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 19 May 2022 17:59:04 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:59:20 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757084716086a18d818bc8687efebb7931b4f95e66464768dd2f3a724165e5fb`  
		Last Modified: Tue, 05 Apr 2022 07:20:27 GMT  
		Size: 35.9 MB (35921106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7387a7ced2948ec0e416c953e2a8ae1f1fc9955fba656c8a23b60bb29663cc9e`  
		Last Modified: Thu, 19 May 2022 18:05:11 GMT  
		Size: 200.4 MB (200432000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:alpine3.15`

```console
$ docker pull rust@sha256:7a917171c2fa060a2665b291820507bca0484efd25811a1c09073b0cfc5cb23d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rust:alpine3.15` - linux; amd64

```console
$ docker pull rust@sha256:e1ddd35b6a802ac8587f8fbc34ce752be20b5c116df2b2f1a90488f0bc3bd439
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.6 MB (249551918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5fbf9bd1849d2598eff6ddedc32b06610905188571179b4a4b0805d6331c549`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:50:48 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 07 Apr 2022 20:22:16 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Thu, 07 Apr 2022 20:22:35 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2113a6fa04a6792c25bda8b467d30b4388d756ab1f526efb6ce7139d464f5b84`  
		Last Modified: Tue, 05 Apr 2022 10:52:45 GMT  
		Size: 42.5 MB (42476793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82ca4327e1d9bb80a8af0bb460d9bef24f8e88470631e2c788f996e91e3d8a7`  
		Last Modified: Thu, 07 Apr 2022 20:27:23 GMT  
		Size: 204.3 MB (204260566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:alpine3.15` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:526dfcfffac3021335f243aabe2b93bf32fd231fbb0e65103266980eedd1e8c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.2 MB (239222115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4049c483a2db267242fac510cf462f66964cbb5e25e512ea43f6648c8e072819`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:18:36 GMT
RUN apk add --no-cache         ca-certificates         gcc
# Thu, 19 May 2022 17:59:27 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:59:40 GMT
RUN set -eux;     apkArch="$(apk --print-arch)";     case "$apkArch" in         x86_64) rustArch='x86_64-unknown-linux-musl'; rustupSha256='bdf022eb7cba403d0285bb62cbc47211f610caec24589a72af70e1e900663be9' ;;         aarch64) rustArch='aarch64-unknown-linux-musl'; rustupSha256='89ce657fe41e83186f5a6cdca4e0fd40edab4fd41b0f9161ac6241d49fbdbbbe' ;;         *) echo >&2 "unsupported architecture: $apkArch"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c79c9d0c9a2cc2bdae9476b20ddb336848888d44ff7d5dfb719ff227ffb79c4`  
		Last Modified: Tue, 05 Apr 2022 07:21:11 GMT  
		Size: 36.1 MB (36073695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d80249e68d74cb54280b56279b2a423d8c0b7682f33bb9a362f716341403763`  
		Last Modified: Thu, 19 May 2022 18:05:57 GMT  
		Size: 200.4 MB (200431943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:bullseye`

```console
$ docker pull rust@sha256:7117a2abfcd947cf26bd0e6dc675a3d511036fe5952c0d38e79911e513c5370a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:bullseye` - linux; amd64

```console
$ docker pull rust@sha256:9fe1f39bec70576e2bd568fafb194b2a532a6f2928bc0b951ac2c0a69a2be9fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **470.2 MB (470195312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a7fe322d8850b0f32d3cebd5ce588d5c1790c96b27d37aee48bddc124a80aa0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:20:05 GMT
ADD file:68a5d7d0db592625159865110c1b7dcb15cf70ecf71b5fd541ef89584cd734ba in / 
# Wed, 11 May 2022 01:20:05 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:49:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:49:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:50:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 16:17:37 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Wed, 11 May 2022 16:17:52 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:67e8aa6c8bbc76b1f2bccb3864b0887671833b8667dc1f6c965fcb0eac7e6402`  
		Last Modified: Wed, 11 May 2022 01:24:45 GMT  
		Size: 54.9 MB (54945622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627e6c1e105548ea4a08354eea581f137cf368d91aeb0ad47dcb706fca54fd8b`  
		Last Modified: Wed, 11 May 2022 01:57:17 GMT  
		Size: 5.2 MB (5155721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0670968926f6461e3135c82ba2c0ad3ebdedc0d0f41b18bda4a1e41104b8be8a`  
		Last Modified: Wed, 11 May 2022 01:57:18 GMT  
		Size: 10.9 MB (10875052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8b0e20be4b4a332bc3d90b9903a5f3c0664b440fd9f1d2a1db0d4b7e6e826b`  
		Last Modified: Wed, 11 May 2022 01:57:38 GMT  
		Size: 54.6 MB (54578468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b10a3a2784b06bfe0af1493ea2a0fa957ae5e0dc30fcfd1166d2558ba74e4d`  
		Last Modified: Wed, 11 May 2022 01:58:14 GMT  
		Size: 196.6 MB (196562669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283a0d92cdf06eb32299bbf28f78c1618a6163731bcffbc1551510e57e8cb4b9`  
		Last Modified: Wed, 11 May 2022 16:20:50 GMT  
		Size: 148.1 MB (148077780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:bullseye` - linux; arm variant v7

```console
$ docker pull rust@sha256:1b59f7d09735e15b0343859d1cb098a1675f013e84347be76936ef9d888fd9e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **467.2 MB (467237488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adc5a024a4724b55a7cba85555cd244b2612ac3057ca98f267dabe0053aeac32`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:48:30 GMT
ADD file:d6545064ea0f75166d59e4d4a2df1e41a3477ae468e558e31f29857336978c0e in / 
# Wed, 11 May 2022 01:48:31 GMT
CMD ["bash"]
# Wed, 11 May 2022 03:21:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:21:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 03:22:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:24:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 May 2022 18:00:44 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 18:01:23 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:ba38f9a6c66968e207a7ada348a2110e3be0ff117e621d9e10ddd7c4becc0d2a`  
		Last Modified: Wed, 11 May 2022 02:03:49 GMT  
		Size: 50.1 MB (50134069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71423015d7b4f718e54ff1561cc06bb4c8357baedc23b49d25fe99cd4b0ae41`  
		Last Modified: Wed, 11 May 2022 03:46:39 GMT  
		Size: 4.9 MB (4924901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8f92194faa0a66e5bd160b229941428f0b0387c6e313e4f1f903c678fbb17e`  
		Last Modified: Wed, 11 May 2022 03:46:41 GMT  
		Size: 10.2 MB (10217886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c410c75a05c2df4ed485cda22fd35206e0ea4b9fbc9f096b11ed5adc6f83fa1c`  
		Last Modified: Wed, 11 May 2022 03:47:32 GMT  
		Size: 50.3 MB (50329744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767978ffc99a492ddd06d37b888a093595a05ac353ceefb2cc01a1322f34164a`  
		Last Modified: Wed, 11 May 2022 03:49:16 GMT  
		Size: 167.0 MB (167042139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3247bc72a5ac57b8481395404128439459da3cbe3d37697e6cce58dc91967469`  
		Last Modified: Thu, 19 May 2022 18:11:31 GMT  
		Size: 184.6 MB (184588749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:bullseye` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:0f34bbe3d25473314051f103cf14a43e983500a742512514459dddebcec49acc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **516.4 MB (516393806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4db0c962f51c31164dcd6edf66e1078fa5fa7bd4324918135f1af9e95932bf8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:46:44 GMT
ADD file:239aa42118877a929b2fbfc0d5793fee7815289280affa5286de2459385c0679 in / 
# Wed, 11 May 2022 00:46:44 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:25:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:25:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:25:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:26:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 May 2022 17:58:06 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:58:21 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:3a36574378e6cece2dd3a839e1c0220eaccc4063b61d7481d1a19d3990c1f2c2`  
		Last Modified: Wed, 11 May 2022 00:53:15 GMT  
		Size: 53.6 MB (53634337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61d3345afba43846f3e638752cce2f0d1d47b21cc667ba08b00db10767a4702`  
		Last Modified: Wed, 11 May 2022 01:35:45 GMT  
		Size: 4.9 MB (4938615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e267d6aa58f93a513352a3b46c7addbf9335d7d43bfa4f1df4026d21785181c`  
		Last Modified: Wed, 11 May 2022 01:35:46 GMT  
		Size: 10.7 MB (10656992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f647907d26b879e0d43f6f4f0807f01e4dbdc034edcecbc988f6033cf401becf`  
		Last Modified: Wed, 11 May 2022 01:36:07 GMT  
		Size: 54.7 MB (54672822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0b3e17bdee16cf8bf269a4474bf56713879991bf87ff3bd790aa96a6f00e3c`  
		Last Modified: Wed, 11 May 2022 01:36:46 GMT  
		Size: 189.5 MB (189482172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cba956553646efe774f749ce526b98ebbff7a89a2eea4b21e77ae86ee7de78f`  
		Last Modified: Thu, 19 May 2022 18:03:05 GMT  
		Size: 203.0 MB (203008868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:bullseye` - linux; 386

```console
$ docker pull rust@sha256:429ae8c8999946379ab90c480318570fa79e1c1fee0bd8248203a9ca26d1702a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **497.9 MB (497919108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c89e41228cd37377968ac5dc6bbd360636a67126aa6b7a48a3d8e5e8f9f24d7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:38:57 GMT
ADD file:dae3dc662d1327f461e95b84f6f9282f3c4fb51f16ac8f20a5f141951d8436a9 in / 
# Wed, 11 May 2022 01:38:58 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:10:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:10:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 02:11:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:12:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 15:45:42 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Wed, 11 May 2022 15:46:00 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:5ad4f92623738998bc77103ff64344255f842f6e5fe4a846df656351b3c4852f`  
		Last Modified: Wed, 11 May 2022 01:45:53 GMT  
		Size: 55.9 MB (55942833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026e99ab0e4b1d3aec936d04cdf9c04ddc8074f2917b86c02e66d88fcae1e42f`  
		Last Modified: Wed, 11 May 2022 02:21:42 GMT  
		Size: 5.1 MB (5080245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dba083f619f2a2c8cfef4a4e844cf6819c306e225029e62cf7c31c17b0d344`  
		Last Modified: Wed, 11 May 2022 02:21:43 GMT  
		Size: 11.0 MB (11033702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5333a48696af9b52c4219f20b87c5cf9b05764b7c58cd19880e6c5730d1b75`  
		Last Modified: Wed, 11 May 2022 02:22:10 GMT  
		Size: 55.9 MB (55914622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899f353e6896a6f03a5af06a01cea44badeac7062481c294a9d7c1da1859b823`  
		Last Modified: Wed, 11 May 2022 02:22:52 GMT  
		Size: 199.5 MB (199502725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c70e60ad4e506736166da380bdcd6e33bfd1a6a4f654f0f1f21736de86b9d47`  
		Last Modified: Wed, 11 May 2022 15:49:27 GMT  
		Size: 170.4 MB (170444981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:buster`

```console
$ docker pull rust@sha256:66420d8dff60f4f94fc9ee8520193f50d26c69e356c52ed2113ddee8ed3ee1e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:buster` - linux; amd64

```console
$ docker pull rust@sha256:335e517975fc3f1573290c544a1497283dce84670afcb5501791fc138f40854f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **460.7 MB (460695435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b56360f6e8c1b377e4e1d7692cc692b67220afcac641058df0004062d349412e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:20:26 GMT
ADD file:54d60144d251caa916ff50606bc2364131d47d6b10ed83d08c81c647ab56cc40 in / 
# Wed, 11 May 2022 01:20:26 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:50:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:50:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:50:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:51:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 16:16:45 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Wed, 11 May 2022 16:16:59 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:b03a94565ecb6e02edf716307f25a0ea5090e3e2f7acec6a3687b95415378a30`  
		Last Modified: Wed, 11 May 2022 01:25:33 GMT  
		Size: 50.4 MB (50437966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7bcede80b1916d73be58ae0a2af8321770c4ce0c8ada05c39271e292355325`  
		Last Modified: Wed, 11 May 2022 01:58:28 GMT  
		Size: 7.9 MB (7856436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37471fc83c2dc382a8aec5dc1c1f0f2f8156f4df529cd1aea7647cbaee4b25fa`  
		Last Modified: Wed, 11 May 2022 01:58:28 GMT  
		Size: 10.0 MB (9997259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0162432a49c07aa492d3e1031af58a9a9f9b22acde859829434e5a54d019aa1c`  
		Last Modified: Wed, 11 May 2022 01:58:46 GMT  
		Size: 51.8 MB (51843657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee8ddc463fd0224112f41976e81d15dd46444f93185d9cde6203a0185857be2`  
		Last Modified: Wed, 11 May 2022 01:59:19 GMT  
		Size: 192.5 MB (192482405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5ec6530a2ae568c3e10b73d729658f9358962f4d4fc1b9ab79d73ec4fb3436`  
		Last Modified: Wed, 11 May 2022 16:19:31 GMT  
		Size: 148.1 MB (148077712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:fd9d31c4dc31d202d71684c47d09f22505d21c6f58bb8fb9ea8ad2a42dd9e047
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.0 MB (463027085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e30beb4107faddc83b15056987106bf5e40d261ce8c3e764f62bc881e188772c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:49:37 GMT
ADD file:9c75d7f24328b3f84cd700813a0a8ff5af16399f4475d24da9b0a859d584614c in / 
# Wed, 11 May 2022 01:49:38 GMT
CMD ["bash"]
# Wed, 11 May 2022 03:25:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:25:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 03:26:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:28:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 May 2022 17:58:16 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:58:55 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:f328f2671b27c760193a9d82808b176a8a7420205e8eb884e1fee20d2ac57ff0`  
		Last Modified: Wed, 11 May 2022 02:05:20 GMT  
		Size: 45.9 MB (45910176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e554a91160b4bf86ab199d7a5f5f105c5ffecc37b098c4274d98c264f677799`  
		Last Modified: Wed, 11 May 2022 03:49:35 GMT  
		Size: 7.1 MB (7145025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1b07ef419c0604851908ed718983760891b21a649a1b8758b871522e7d3e48`  
		Last Modified: Wed, 11 May 2022 03:49:36 GMT  
		Size: 9.3 MB (9343816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398961d3cf225ff82b93bd457012e308b756c455d1dbe1191bca51a54483f1d7`  
		Last Modified: Wed, 11 May 2022 03:50:19 GMT  
		Size: 47.4 MB (47359230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672070a3841f8c8993724742262e409c973f2ea02773250aff8b7c5bfe81bde6`  
		Last Modified: Wed, 11 May 2022 03:52:03 GMT  
		Size: 168.7 MB (168680126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061ddfe391b623d781b7e0bc3f1f46b681cb0ba8d2fe5efd31138be3e05e30b4`  
		Last Modified: Thu, 19 May 2022 18:06:48 GMT  
		Size: 184.6 MB (184588712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:efa3c3975a4197a5b384d9798b89538424265591c4da905fbc17cd1228c4386d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **506.0 MB (505953047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e47315b8b3fba316e10cf1a807d312f41f096082982190765b4f8bae9cac7d1a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:47:11 GMT
ADD file:5389b77733b44ebc41850baff3ebfc491726af264a745f108d5f16076a0f04ab in / 
# Wed, 11 May 2022 00:47:11 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:26:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:26:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:27:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:28:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 May 2022 17:57:05 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:57:22 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:5528d23e3f315103c99c14258e007a025d09bb4fd587c2d8a32d6dbb6047b891`  
		Last Modified: Wed, 11 May 2022 00:54:09 GMT  
		Size: 49.2 MB (49228300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b2d66a1dbe5960c6de4181ca3512467d3303dfb9cde3d92ecf7a85111cf68b`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 7.7 MB (7719789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9244ac9f9851b43ddc1032930666d339c3a5d9b934e2ca42ecd2e8ef3dd680`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 9.8 MB (9767329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06885dc77f03f05a5f98ceb35e871f027525d932d32027ed9d4ffb0cbd29786c`  
		Last Modified: Wed, 11 May 2022 01:37:21 GMT  
		Size: 52.2 MB (52174787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be89f33c0b133b07e3c53ae901bde6bf63f6a395cdf9c89c263e8d1e625a61cf`  
		Last Modified: Wed, 11 May 2022 01:37:55 GMT  
		Size: 184.1 MB (184054008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3d8265597d91c63bc1303ef37fc2a0650ffe5ef68084a8e38256d7bf63d60f`  
		Last Modified: Thu, 19 May 2022 18:01:26 GMT  
		Size: 203.0 MB (203008834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:buster` - linux; 386

```console
$ docker pull rust@sha256:cf59e8e28f4decd414f74110ad0353f30fad01bf052001e4d4b3d1e25d4efd6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **492.2 MB (492242448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e666158bab1d49cb47d1cb46aa91705753de2c6ca113913d58ce5ab42680d911`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:39:25 GMT
ADD file:03855eb19b36aa184d26264c1416a11ac7661faddae3436aad12661bb4c6e656 in / 
# Wed, 11 May 2022 01:39:26 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:12:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:12:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 02:13:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:14:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 15:44:36 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Wed, 11 May 2022 15:44:57 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:5b096db137216fbea3d646b6cad3959b69b6a1d27ff5f31bd01048df4a7e6c0a`  
		Last Modified: Wed, 11 May 2022 01:46:53 GMT  
		Size: 51.2 MB (51199249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aea31d1a573a95302db6857fc201016b7c6b8f21d0f56e011ec26f49e9d36b6`  
		Last Modified: Wed, 11 May 2022 02:23:08 GMT  
		Size: 8.0 MB (8022259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1841293ac8ab91433085e85c8c899e4324ca8f84a2cf4300cb5410542e39f4`  
		Last Modified: Wed, 11 May 2022 02:23:08 GMT  
		Size: 10.1 MB (10121987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c221acbd6711627d003a42bc75312b3994313814f1ba7a82f10f1e0e37b30b8`  
		Last Modified: Wed, 11 May 2022 02:23:28 GMT  
		Size: 53.4 MB (53442818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d4335971c3c6abcc0cee05c5dc4d86bb28ee87ad0592c808e4454c0579e3ce`  
		Last Modified: Wed, 11 May 2022 02:24:03 GMT  
		Size: 199.0 MB (199011140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93427b1a8630d73a8276d0e8952ddc49154b30b3ad1f78b5ad7cf18ab0abd93a`  
		Last Modified: Wed, 11 May 2022 15:47:59 GMT  
		Size: 170.4 MB (170444995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:latest`

```console
$ docker pull rust@sha256:7117a2abfcd947cf26bd0e6dc675a3d511036fe5952c0d38e79911e513c5370a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:latest` - linux; amd64

```console
$ docker pull rust@sha256:9fe1f39bec70576e2bd568fafb194b2a532a6f2928bc0b951ac2c0a69a2be9fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **470.2 MB (470195312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a7fe322d8850b0f32d3cebd5ce588d5c1790c96b27d37aee48bddc124a80aa0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:20:05 GMT
ADD file:68a5d7d0db592625159865110c1b7dcb15cf70ecf71b5fd541ef89584cd734ba in / 
# Wed, 11 May 2022 01:20:05 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:49:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:49:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:50:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 16:17:37 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Wed, 11 May 2022 16:17:52 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:67e8aa6c8bbc76b1f2bccb3864b0887671833b8667dc1f6c965fcb0eac7e6402`  
		Last Modified: Wed, 11 May 2022 01:24:45 GMT  
		Size: 54.9 MB (54945622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627e6c1e105548ea4a08354eea581f137cf368d91aeb0ad47dcb706fca54fd8b`  
		Last Modified: Wed, 11 May 2022 01:57:17 GMT  
		Size: 5.2 MB (5155721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0670968926f6461e3135c82ba2c0ad3ebdedc0d0f41b18bda4a1e41104b8be8a`  
		Last Modified: Wed, 11 May 2022 01:57:18 GMT  
		Size: 10.9 MB (10875052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8b0e20be4b4a332bc3d90b9903a5f3c0664b440fd9f1d2a1db0d4b7e6e826b`  
		Last Modified: Wed, 11 May 2022 01:57:38 GMT  
		Size: 54.6 MB (54578468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b10a3a2784b06bfe0af1493ea2a0fa957ae5e0dc30fcfd1166d2558ba74e4d`  
		Last Modified: Wed, 11 May 2022 01:58:14 GMT  
		Size: 196.6 MB (196562669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283a0d92cdf06eb32299bbf28f78c1618a6163731bcffbc1551510e57e8cb4b9`  
		Last Modified: Wed, 11 May 2022 16:20:50 GMT  
		Size: 148.1 MB (148077780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:latest` - linux; arm variant v7

```console
$ docker pull rust@sha256:1b59f7d09735e15b0343859d1cb098a1675f013e84347be76936ef9d888fd9e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **467.2 MB (467237488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adc5a024a4724b55a7cba85555cd244b2612ac3057ca98f267dabe0053aeac32`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:48:30 GMT
ADD file:d6545064ea0f75166d59e4d4a2df1e41a3477ae468e558e31f29857336978c0e in / 
# Wed, 11 May 2022 01:48:31 GMT
CMD ["bash"]
# Wed, 11 May 2022 03:21:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:21:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 03:22:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:24:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 May 2022 18:00:44 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 18:01:23 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:ba38f9a6c66968e207a7ada348a2110e3be0ff117e621d9e10ddd7c4becc0d2a`  
		Last Modified: Wed, 11 May 2022 02:03:49 GMT  
		Size: 50.1 MB (50134069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71423015d7b4f718e54ff1561cc06bb4c8357baedc23b49d25fe99cd4b0ae41`  
		Last Modified: Wed, 11 May 2022 03:46:39 GMT  
		Size: 4.9 MB (4924901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8f92194faa0a66e5bd160b229941428f0b0387c6e313e4f1f903c678fbb17e`  
		Last Modified: Wed, 11 May 2022 03:46:41 GMT  
		Size: 10.2 MB (10217886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c410c75a05c2df4ed485cda22fd35206e0ea4b9fbc9f096b11ed5adc6f83fa1c`  
		Last Modified: Wed, 11 May 2022 03:47:32 GMT  
		Size: 50.3 MB (50329744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767978ffc99a492ddd06d37b888a093595a05ac353ceefb2cc01a1322f34164a`  
		Last Modified: Wed, 11 May 2022 03:49:16 GMT  
		Size: 167.0 MB (167042139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3247bc72a5ac57b8481395404128439459da3cbe3d37697e6cce58dc91967469`  
		Last Modified: Thu, 19 May 2022 18:11:31 GMT  
		Size: 184.6 MB (184588749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:latest` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:0f34bbe3d25473314051f103cf14a43e983500a742512514459dddebcec49acc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **516.4 MB (516393806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4db0c962f51c31164dcd6edf66e1078fa5fa7bd4324918135f1af9e95932bf8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:46:44 GMT
ADD file:239aa42118877a929b2fbfc0d5793fee7815289280affa5286de2459385c0679 in / 
# Wed, 11 May 2022 00:46:44 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:25:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:25:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:25:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:26:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 May 2022 17:58:06 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:58:21 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:3a36574378e6cece2dd3a839e1c0220eaccc4063b61d7481d1a19d3990c1f2c2`  
		Last Modified: Wed, 11 May 2022 00:53:15 GMT  
		Size: 53.6 MB (53634337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61d3345afba43846f3e638752cce2f0d1d47b21cc667ba08b00db10767a4702`  
		Last Modified: Wed, 11 May 2022 01:35:45 GMT  
		Size: 4.9 MB (4938615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e267d6aa58f93a513352a3b46c7addbf9335d7d43bfa4f1df4026d21785181c`  
		Last Modified: Wed, 11 May 2022 01:35:46 GMT  
		Size: 10.7 MB (10656992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f647907d26b879e0d43f6f4f0807f01e4dbdc034edcecbc988f6033cf401becf`  
		Last Modified: Wed, 11 May 2022 01:36:07 GMT  
		Size: 54.7 MB (54672822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0b3e17bdee16cf8bf269a4474bf56713879991bf87ff3bd790aa96a6f00e3c`  
		Last Modified: Wed, 11 May 2022 01:36:46 GMT  
		Size: 189.5 MB (189482172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cba956553646efe774f749ce526b98ebbff7a89a2eea4b21e77ae86ee7de78f`  
		Last Modified: Thu, 19 May 2022 18:03:05 GMT  
		Size: 203.0 MB (203008868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:latest` - linux; 386

```console
$ docker pull rust@sha256:429ae8c8999946379ab90c480318570fa79e1c1fee0bd8248203a9ca26d1702a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **497.9 MB (497919108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c89e41228cd37377968ac5dc6bbd360636a67126aa6b7a48a3d8e5e8f9f24d7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:38:57 GMT
ADD file:dae3dc662d1327f461e95b84f6f9282f3c4fb51f16ac8f20a5f141951d8436a9 in / 
# Wed, 11 May 2022 01:38:58 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:10:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:10:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 02:11:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:12:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 15:45:42 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Wed, 11 May 2022 15:46:00 GMT
RUN set -eux;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;
```

-	Layers:
	-	`sha256:5ad4f92623738998bc77103ff64344255f842f6e5fe4a846df656351b3c4852f`  
		Last Modified: Wed, 11 May 2022 01:45:53 GMT  
		Size: 55.9 MB (55942833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026e99ab0e4b1d3aec936d04cdf9c04ddc8074f2917b86c02e66d88fcae1e42f`  
		Last Modified: Wed, 11 May 2022 02:21:42 GMT  
		Size: 5.1 MB (5080245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dba083f619f2a2c8cfef4a4e844cf6819c306e225029e62cf7c31c17b0d344`  
		Last Modified: Wed, 11 May 2022 02:21:43 GMT  
		Size: 11.0 MB (11033702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5333a48696af9b52c4219f20b87c5cf9b05764b7c58cd19880e6c5730d1b75`  
		Last Modified: Wed, 11 May 2022 02:22:10 GMT  
		Size: 55.9 MB (55914622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899f353e6896a6f03a5af06a01cea44badeac7062481c294a9d7c1da1859b823`  
		Last Modified: Wed, 11 May 2022 02:22:52 GMT  
		Size: 199.5 MB (199502725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c70e60ad4e506736166da380bdcd6e33bfd1a6a4f654f0f1f21736de86b9d47`  
		Last Modified: Wed, 11 May 2022 15:49:27 GMT  
		Size: 170.4 MB (170444981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:slim`

```console
$ docker pull rust@sha256:6a2c53a0fb8f909c0332eaf974667acfb43d017f6ad870361c5baaeb9c09b40a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:slim` - linux; amd64

```console
$ docker pull rust@sha256:334e2416575c89f0e778fe692d7e1de52fdfe8071a1b82005c2c93357cb2fa87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.6 MB (239571414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd2de95a8dc1f3aaa60ddf0112df2d8a1472cd46a457fa458bb6422969807c39`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 16:17:57 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Wed, 11 May 2022 16:18:23 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349f1d9b940a31cb04a2b8c0149fd1139084f54b1fb2ce83a5b86d9c23cbb752`  
		Last Modified: Wed, 11 May 2022 16:21:44 GMT  
		Size: 208.2 MB (208191938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim` - linux; arm variant v7

```console
$ docker pull rust@sha256:637e4a0dcdbbe892de42340ab07af1a2f81cb6df83d40f81b596734a386727fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.4 MB (253447413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4246a64a5c89d0efdd649d037d047eeb0d7c814d2357291c30e81c30bfb7e7c4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:49:07 GMT
ADD file:7c0451fffe8a520c2ab23048948d76bfe0dc0d90298c3d859279ccd8815b84f6 in / 
# Wed, 11 May 2022 01:49:08 GMT
CMD ["bash"]
# Thu, 19 May 2022 18:01:43 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 18:02:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:1a9427b75b1c1db800cae7a9199bb4e508702e6761b17cc904d21441df43016c`  
		Last Modified: Wed, 11 May 2022 02:04:35 GMT  
		Size: 26.6 MB (26575672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3332501bc455d4c889b90983db4f5f72ae1416aaf135f5808f59c60316001ce0`  
		Last Modified: Thu, 19 May 2022 18:14:23 GMT  
		Size: 226.9 MB (226871741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:c24497850afb62c925899b8854fe8c0d5a9c0767145b5cf085e323167dec1eba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.6 MB (288562316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:163110751b432b68a68df23f35c12cd3c30c9ad7992d636e1f539c76abcf59cb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Thu, 19 May 2022 17:58:29 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:58:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3846b6fbdd10a62b50f55e5b616c2b9330ac2eccdc523f652aaa11c94da412a7`  
		Last Modified: Thu, 19 May 2022 18:04:14 GMT  
		Size: 258.5 MB (258496623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim` - linux; 386

```console
$ docker pull rust@sha256:db4d4cd5c20b48773f222cdd354efa8c6bbb873c8625e6af8d310b640990ef1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.4 MB (263392079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b263a284d7b8c23352b7916318acfea63cdfffa633191c5c06692e04541b8631`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:39:14 GMT
ADD file:9eecb0fd311177f9d226e914c411aef49b5de1930e73019d2ee24afed515b5a2 in / 
# Wed, 11 May 2022 01:39:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 15:46:08 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Wed, 11 May 2022 15:46:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:91c5bdbe4bf9f1970dd54ba71e2523649adce4e5240c2ff8a87711bf389ecba3`  
		Last Modified: Wed, 11 May 2022 01:46:25 GMT  
		Size: 32.4 MB (32389776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e2abe277b496c5ea655646e02aeedd052b26bb98861a2aacb50bba3f7d5b51`  
		Last Modified: Wed, 11 May 2022 15:50:51 GMT  
		Size: 231.0 MB (231002303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:slim-bullseye`

```console
$ docker pull rust@sha256:6a2c53a0fb8f909c0332eaf974667acfb43d017f6ad870361c5baaeb9c09b40a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:slim-bullseye` - linux; amd64

```console
$ docker pull rust@sha256:334e2416575c89f0e778fe692d7e1de52fdfe8071a1b82005c2c93357cb2fa87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.6 MB (239571414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd2de95a8dc1f3aaa60ddf0112df2d8a1472cd46a457fa458bb6422969807c39`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 16:17:57 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Wed, 11 May 2022 16:18:23 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349f1d9b940a31cb04a2b8c0149fd1139084f54b1fb2ce83a5b86d9c23cbb752`  
		Last Modified: Wed, 11 May 2022 16:21:44 GMT  
		Size: 208.2 MB (208191938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-bullseye` - linux; arm variant v7

```console
$ docker pull rust@sha256:637e4a0dcdbbe892de42340ab07af1a2f81cb6df83d40f81b596734a386727fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.4 MB (253447413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4246a64a5c89d0efdd649d037d047eeb0d7c814d2357291c30e81c30bfb7e7c4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:49:07 GMT
ADD file:7c0451fffe8a520c2ab23048948d76bfe0dc0d90298c3d859279ccd8815b84f6 in / 
# Wed, 11 May 2022 01:49:08 GMT
CMD ["bash"]
# Thu, 19 May 2022 18:01:43 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 18:02:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:1a9427b75b1c1db800cae7a9199bb4e508702e6761b17cc904d21441df43016c`  
		Last Modified: Wed, 11 May 2022 02:04:35 GMT  
		Size: 26.6 MB (26575672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3332501bc455d4c889b90983db4f5f72ae1416aaf135f5808f59c60316001ce0`  
		Last Modified: Thu, 19 May 2022 18:14:23 GMT  
		Size: 226.9 MB (226871741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:c24497850afb62c925899b8854fe8c0d5a9c0767145b5cf085e323167dec1eba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.6 MB (288562316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:163110751b432b68a68df23f35c12cd3c30c9ad7992d636e1f539c76abcf59cb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Thu, 19 May 2022 17:58:29 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:58:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3846b6fbdd10a62b50f55e5b616c2b9330ac2eccdc523f652aaa11c94da412a7`  
		Last Modified: Thu, 19 May 2022 18:04:14 GMT  
		Size: 258.5 MB (258496623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-bullseye` - linux; 386

```console
$ docker pull rust@sha256:db4d4cd5c20b48773f222cdd354efa8c6bbb873c8625e6af8d310b640990ef1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.4 MB (263392079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b263a284d7b8c23352b7916318acfea63cdfffa633191c5c06692e04541b8631`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:39:14 GMT
ADD file:9eecb0fd311177f9d226e914c411aef49b5de1930e73019d2ee24afed515b5a2 in / 
# Wed, 11 May 2022 01:39:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 15:46:08 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Wed, 11 May 2022 15:46:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:91c5bdbe4bf9f1970dd54ba71e2523649adce4e5240c2ff8a87711bf389ecba3`  
		Last Modified: Wed, 11 May 2022 01:46:25 GMT  
		Size: 32.4 MB (32389776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e2abe277b496c5ea655646e02aeedd052b26bb98861a2aacb50bba3f7d5b51`  
		Last Modified: Wed, 11 May 2022 15:50:51 GMT  
		Size: 231.0 MB (231002303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rust:slim-buster`

```console
$ docker pull rust@sha256:8345ef78f92d4b7b3f5542107396f71d42f07a9aa30a2f020828f6d693db6712
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `rust:slim-buster` - linux; amd64

```console
$ docker pull rust@sha256:ecf4984a4cbd456d3670449efe63c665bbf850b821c4d3a30a7dee7896d9f1cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.6 MB (220627247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cd1e35201514da9bdc71adeb5f0ad381ce84089c40a6419d02f3a73b6845e96`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 16:17:04 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Wed, 11 May 2022 16:17:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910c9723b9c8224fdc9165793746a7bdef632a394043bf09d8c357918d0d8eeb`  
		Last Modified: Wed, 11 May 2022 16:20:14 GMT  
		Size: 193.5 MB (193486525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-buster` - linux; arm variant v7

```console
$ docker pull rust@sha256:5787cef45a9f13e1dea2638ba8ec7d928a7d6c3e6769eef73355011f9d99f327
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.3 MB (240262048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:979601ce35358bda70bbec9cfa78b0566870036b24dc3a066b2f5e10cbae68f7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:50:13 GMT
ADD file:bccd1898e72cc79621c20ba59061d318521fbd2a8f10806cc3a1561fcbc9daad in / 
# Wed, 11 May 2022 01:50:14 GMT
CMD ["bash"]
# Thu, 19 May 2022 17:59:10 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 18:00:20 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:8f4c08df22a944142862818447616fff8b15d3a7ba383d4eeab678af698c2c43`  
		Last Modified: Wed, 11 May 2022 02:06:00 GMT  
		Size: 22.7 MB (22747864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7445544703dfa3d6936573907d147f14265cf553e666c39769991139c3c5216f`  
		Last Modified: Thu, 19 May 2022 18:09:17 GMT  
		Size: 217.5 MB (217514184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-buster` - linux; arm64 variant v8

```console
$ docker pull rust@sha256:541f0b63df779aee4eb28f4f2ef5ec9e3b7251be6011cd39f497c8e6472019d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.1 MB (269122908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92aa5b1b5884c8281bde8930fdbac8d2df5495182807435346629bb2a263e5dd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:47:26 GMT
ADD file:2536146c773d09db1a8fbbff00933acc459d8929feb3cff5b93ca4c23b577845 in / 
# Wed, 11 May 2022 00:47:26 GMT
CMD ["bash"]
# Thu, 19 May 2022 17:57:28 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.61.0
# Thu, 19 May 2022 17:57:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:383d573fdcf2c6da56fdb61e120549d7bc200471208ca4c7c6605c57a0a87ef6`  
		Last Modified: Wed, 11 May 2022 00:54:36 GMT  
		Size: 25.9 MB (25909014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0503ec1485723fc8953ef8fca5ff5794d54c7f48e60e240180a9a96de34727c7`  
		Last Modified: Thu, 19 May 2022 18:02:19 GMT  
		Size: 243.2 MB (243213894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rust:slim-buster` - linux; 386

```console
$ docker pull rust@sha256:03dd42304f522301e06612497c9c34cea732f64d94196fc16f7e18be55696cc9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.2 MB (248236964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a49488bafeb991a838b0f60a1097c2daeb50ef3baf7d3a536b33b99274c502e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:39:41 GMT
ADD file:fc7b00a8a5b0e703ac3ede5e2e51257f5ee709fcd35fee53e7b99d144cd873e4 in / 
# Wed, 11 May 2022 01:39:42 GMT
CMD ["bash"]
# Wed, 11 May 2022 15:45:03 GMT
ENV RUSTUP_HOME=/usr/local/rustup CARGO_HOME=/usr/local/cargo PATH=/usr/local/cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin RUST_VERSION=1.60.0
# Wed, 11 May 2022 15:45:35 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         gcc         libc6-dev         wget         ;     dpkgArch="$(dpkg --print-architecture)";     case "${dpkgArch##*-}" in         amd64) rustArch='x86_64-unknown-linux-gnu'; rustupSha256='3dc5ef50861ee18657f9db2eeb7392f9c2a6c95c90ab41e45ab4ca71476b4338' ;;         armhf) rustArch='armv7-unknown-linux-gnueabihf'; rustupSha256='67777ac3bc17277102f2ed73fd5f14c51f4ca5963adadf7f174adf4ebc38747b' ;;         arm64) rustArch='aarch64-unknown-linux-gnu'; rustupSha256='32a1532f7cef072a667bac53f1a5542c99666c4071af0c9549795bbdb2069ec1' ;;         i386) rustArch='i686-unknown-linux-gnu'; rustupSha256='e50d1deb99048bc5782a0200aa33e4eea70747d49dffdc9d06812fd22a372515' ;;         *) echo >&2 "unsupported architecture: ${dpkgArch}"; exit 1 ;;     esac;     url="https://static.rust-lang.org/rustup/archive/1.24.3/${rustArch}/rustup-init";     wget "$url";     echo "${rustupSha256} *rustup-init" | sha256sum -c -;     chmod +x rustup-init;     ./rustup-init -y --no-modify-path --profile minimal --default-toolchain $RUST_VERSION --default-host ${rustArch};     rm rustup-init;     chmod -R a+w $RUSTUP_HOME $CARGO_HOME;     rustup --version;     cargo --version;     rustc --version;     apt-get remove -y --auto-remove         wget         ;     rm -rf /var/lib/apt/lists/*;
```

-	Layers:
	-	`sha256:b1c376c64b69c16b8b035dfd04b99bb7769a5afdfb56a1241aa4ec8743e85aa7`  
		Last Modified: Wed, 11 May 2022 01:47:22 GMT  
		Size: 27.8 MB (27799149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6dac1eed3e092c2db915499da260dbc53370448565b8d7dd1a904bc0f736d7a`  
		Last Modified: Wed, 11 May 2022 15:48:47 GMT  
		Size: 220.4 MB (220437815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
