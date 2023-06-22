<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `irssi`

-	[`irssi:1`](#irssi1)
-	[`irssi:1-alpine`](#irssi1-alpine)
-	[`irssi:1-alpine3.18`](#irssi1-alpine318)
-	[`irssi:1-bookworm`](#irssi1-bookworm)
-	[`irssi:1.4`](#irssi14)
-	[`irssi:1.4-alpine`](#irssi14-alpine)
-	[`irssi:1.4-alpine3.18`](#irssi14-alpine318)
-	[`irssi:1.4-bookworm`](#irssi14-bookworm)
-	[`irssi:1.4.4`](#irssi144)
-	[`irssi:1.4.4-alpine`](#irssi144-alpine)
-	[`irssi:1.4.4-alpine3.18`](#irssi144-alpine318)
-	[`irssi:1.4.4-bookworm`](#irssi144-bookworm)
-	[`irssi:alpine`](#irssialpine)
-	[`irssi:alpine3.18`](#irssialpine318)
-	[`irssi:bookworm`](#irssibookworm)
-	[`irssi:latest`](#irssilatest)

## `irssi:1`

```console
$ docker pull irssi@sha256:14481b64cd4dc6c9a9f26629b698c88886eff923a6e4f296516508939c73333c
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

### `irssi:1` - linux; amd64

```console
$ docker pull irssi@sha256:1fda0af19ea9f808bab9108bb4b4528d6f36297ae226f7e17ebb2510aebbe39c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.4 MB (51353812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3240c2b2def4b35f616344709cdf6120faa7bdfb9973ce8e2100aa3905f16bfb`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:04:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:04:35 GMT
ENV HOME=/home/user
# Tue, 13 Jun 2023 07:04:36 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 13 Jun 2023 07:04:36 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 07:04:36 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 13 Jun 2023 07:05:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 13 Jun 2023 07:05:25 GMT
WORKDIR /home/user
# Tue, 13 Jun 2023 07:05:25 GMT
USER user
# Tue, 13 Jun 2023 07:05:25 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fa339e2e18ca8ee7894660c0b14e3f7ca734b3aeee8e2304b3e8c2563845ce`  
		Last Modified: Tue, 13 Jun 2023 07:05:49 GMT  
		Size: 15.5 MB (15457449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d616343ca0282e2d024ff05930f8eede4a1b1def9f5c9d7c706e5589fcfe44`  
		Last Modified: Tue, 13 Jun 2023 07:05:46 GMT  
		Size: 4.2 KB (4202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24ca3bf390591ce5506aa13625a97a7e80eb5fa1f34b25e33a9bdbfef4a1589`  
		Last Modified: Tue, 13 Jun 2023 07:05:47 GMT  
		Size: 4.5 MB (4474751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm variant v5

```console
$ docker pull irssi@sha256:ec8e8fb46b70710ad03ffd0b0437286a0ec119c785edb791566d4534b21abf23
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70391870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb94ca655a3ecc2baf5113690a7bfa622f05cc2c362c9383c0a9bcfd736acf7d`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:48:31 GMT
ADD file:54a716f17b23e4fa49d1d5c0a7f63becc295873c116d19bb4753d34f1ca6affb in / 
# Mon, 12 Jun 2023 23:48:31 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 00:48:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 00:48:44 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:48:44 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:48:45 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:48:45 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:49:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 00:49:43 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:49:43 GMT
USER user
# Thu, 22 Jun 2023 00:49:43 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:70c60174b18d99741c33011138b5abf2f4d8eca0384521ccb43db3612078e36f`  
		Last Modified: Mon, 12 Jun 2023 23:51:26 GMT  
		Size: 27.0 MB (26982142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2fce51156cf8962c69bb6b4557b25c7c07264ce1ae06bcea0709030ed202ab`  
		Last Modified: Thu, 22 Jun 2023 00:50:07 GMT  
		Size: 17.1 MB (17083367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78197c8422a93eb658c23dff5d622f2d4f7524f184ddec1d7eda45e518c4354f`  
		Last Modified: Thu, 22 Jun 2023 00:50:03 GMT  
		Size: 3.4 KB (3370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4257c989a7f7bddb1161416c0d8ad56a66c61b37802ca313fea85633c9511567`  
		Last Modified: Thu, 22 Jun 2023 00:50:08 GMT  
		Size: 26.3 MB (26322991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm variant v7

```console
$ docker pull irssi@sha256:6b07201205f1936d606641ab462c40bcb52da3a8867b54d3c275685eeeb90ecb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45156187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0bc29edfecb98551b42621135d0e6a9a8df4e4eaf154137cf368ede533f1ceb`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:47 GMT
ADD file:319a24b7e30fc548f9dcf48ad6cee469e8bf7e89c67901cf3851e41e75693489 in / 
# Mon, 12 Jun 2023 23:58:47 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 17:16:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 17:16:56 GMT
ENV HOME=/home/user
# Tue, 13 Jun 2023 17:16:57 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 13 Jun 2023 17:16:57 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 17:16:57 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 13 Jun 2023 17:17:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 13 Jun 2023 17:17:44 GMT
WORKDIR /home/user
# Tue, 13 Jun 2023 17:17:45 GMT
USER user
# Tue, 13 Jun 2023 17:17:45 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b7c295cb849275e211d18b720d2349cc84c0038be1a362aca4765ceb3342043c`  
		Last Modified: Tue, 13 Jun 2023 00:04:24 GMT  
		Size: 26.6 MB (26578690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849490fbc07826e4ba5d7341723cfc86674072f6dea1fef7ee6c95a2d47f94ea`  
		Last Modified: Tue, 13 Jun 2023 17:18:12 GMT  
		Size: 14.4 MB (14385956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2ac9297b563c1cb4c92586f2e565024907221ef118e14789c48461ec982ce1`  
		Last Modified: Tue, 13 Jun 2023 17:18:08 GMT  
		Size: 4.2 KB (4190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0386945f81bf6c09429e43066eab30120446fd066a8e3d3450bf756774b9bad2`  
		Last Modified: Tue, 13 Jun 2023 17:18:09 GMT  
		Size: 4.2 MB (4187351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:266e75793b01d3790ac03073281aa85091694092f5da2a74804a57096c65e8cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74817663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2788ad4db80732ee28509ee691fff308c9dbf05d0f10c8264187cf487aea3e8`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:13 GMT
ADD file:f75c3fe22fec548b35a86a9a5802fdc97497f5d253cf630d65f13282169d3f3f in / 
# Mon, 12 Jun 2023 23:40:14 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 00:59:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 00:59:33 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:59:34 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:59:34 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:59:34 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:00:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 01:00:22 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:00:22 GMT
USER user
# Thu, 22 Jun 2023 01:00:23 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:95039a22a7cc3ae41d71f075e6e09e91e8da850fb5f80aba2f4a09f254520539`  
		Last Modified: Mon, 12 Jun 2023 23:44:08 GMT  
		Size: 29.2 MB (29152534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07791bb7d3b8da337cb7da387519554fbdb05d5d18a9015f7fd00751b524b4c6`  
		Last Modified: Thu, 22 Jun 2023 01:01:08 GMT  
		Size: 18.0 MB (18024086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b6d1cc205388e8478b3e53f9a0bd93b14aeac4315990aac3ad7b6d885c9ebe`  
		Last Modified: Thu, 22 Jun 2023 01:01:05 GMT  
		Size: 3.4 KB (3371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93207a63a416b94a1d0f7cf4c0794018f105ecd47ec4d24bc1ccf38d3269c5e`  
		Last Modified: Thu, 22 Jun 2023 01:01:09 GMT  
		Size: 27.6 MB (27637672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; 386

```console
$ docker pull irssi@sha256:0189dd47eeb861dff6aae81b129a397bf423c30f9d10edafdfe0f60eabbacecf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76490983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4845371b0a05c37bd8b6d4f60b11c9829ab2a362e65e8f85033cd78c89200eb8`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:20 GMT
ADD file:c7ecc5e2bed99e2cbca26f9f4247cd9bc399749556f4084e9357a9b00bb80530 in / 
# Mon, 12 Jun 2023 23:39:20 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 00:52:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 00:52:29 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:52:29 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:52:29 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:52:30 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:53:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 00:53:34 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:53:34 GMT
USER user
# Thu, 22 Jun 2023 00:53:34 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:82a41d17956dd7c8ebb39c9ce936fd26841bdbec98d0a185e3db8154b352edff`  
		Last Modified: Mon, 12 Jun 2023 23:46:21 GMT  
		Size: 30.1 MB (30140741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb531271cfa6ef221334ee9305eae83f672ba29341a2024e4520dbf81b6aa8f`  
		Last Modified: Thu, 22 Jun 2023 00:54:50 GMT  
		Size: 17.8 MB (17783961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9dc41e70935097ed849f2b07b7ad815928f38688133be530d26cacf20f94040`  
		Last Modified: Thu, 22 Jun 2023 00:54:44 GMT  
		Size: 3.4 KB (3367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6bf06950cb921c0ef76ebc588fa3c5a0b713fdfa45199468d58e625ada6e6a9`  
		Last Modified: Thu, 22 Jun 2023 00:54:51 GMT  
		Size: 28.6 MB (28562914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; mips64le

```console
$ docker pull irssi@sha256:fcad96467ecda441065d8062d7deffe2231cf5473de7f214932098cb7469b642
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.4 MB (48376311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:385baa614e97ceda4073810d1f47b470ba54a00c18ced3b057f8f8a21f9688cd`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Jun 2023 00:10:34 GMT
ADD file:4d5c7737e954f157e3d7ea47cc1814c46ec5c753a3d5d828ad9614969b572253 in / 
# Tue, 13 Jun 2023 00:10:38 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 14:58:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 14:58:45 GMT
ENV HOME=/home/user
# Tue, 13 Jun 2023 14:58:52 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 13 Jun 2023 14:58:55 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 14:58:58 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 13 Jun 2023 15:02:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 13 Jun 2023 15:02:56 GMT
WORKDIR /home/user
# Tue, 13 Jun 2023 15:02:59 GMT
USER user
# Tue, 13 Jun 2023 15:03:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:61bd6562a93acd0a3b327321e5465408e1d921b3ce1fb4fe353633330c3ede91`  
		Last Modified: Tue, 13 Jun 2023 00:23:53 GMT  
		Size: 29.6 MB (29634422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cd3adcf928d62813a219ad0c5c5c8015b780b4a6b4bb1ded47ae7f4e77036b`  
		Last Modified: Tue, 13 Jun 2023 15:03:43 GMT  
		Size: 14.4 MB (14421797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b360405355f5536c6ebb3ed5466c97a155165087081278fd8326b9c6a618e41c`  
		Last Modified: Tue, 13 Jun 2023 15:03:30 GMT  
		Size: 4.1 KB (4066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cf810f1b3cb9d35488e456c3cd9a56a60af589307368bb89a24c740fc94727`  
		Last Modified: Tue, 13 Jun 2023 15:03:33 GMT  
		Size: 4.3 MB (4316026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; ppc64le

```console
$ docker pull irssi@sha256:2c84f21d14766ef5faf43cbde7d5d21da7fbb7380ad823f06c9ffe0e6af8246f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55734024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39a07dc4dd7e0a6d1e413452909230f2fef5affd9aa6aad211c12e99096995bf`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:18:20 GMT
ADD file:b17eabe509462fa1a2e4c5421e877e3e4149085e3da07a421a66c7b06566c457 in / 
# Mon, 12 Jun 2023 23:18:22 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 08:47:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 08:47:07 GMT
ENV HOME=/home/user
# Tue, 13 Jun 2023 08:47:08 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 13 Jun 2023 08:47:08 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 08:47:08 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 13 Jun 2023 08:48:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 13 Jun 2023 08:48:26 GMT
WORKDIR /home/user
# Tue, 13 Jun 2023 08:48:26 GMT
USER user
# Tue, 13 Jun 2023 08:48:26 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2973ac0be4a80a6cecbb73370e92810a6f67a98e12e61b3044aa63a322dab03a`  
		Last Modified: Mon, 12 Jun 2023 23:25:03 GMT  
		Size: 35.3 MB (35290790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc5bd67d599f4e07b6f68f09a02d378eac43824b1a4cda56b24bc1c51d7c5ee`  
		Last Modified: Tue, 13 Jun 2023 08:48:45 GMT  
		Size: 15.8 MB (15756316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382a2c88702295eea22c668bccd54ea16eae65ffa15581e3bc67235a3c431e1b`  
		Last Modified: Tue, 13 Jun 2023 08:48:40 GMT  
		Size: 4.2 KB (4204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0199a0ffe4039f498bae34b531ebd5b5c6cdfa729e2233e3f5ca444d92962e`  
		Last Modified: Tue, 13 Jun 2023 08:48:41 GMT  
		Size: 4.7 MB (4682714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; s390x

```console
$ docker pull irssi@sha256:e400a68cd9ed507fdcb70211f4e758d4ab1abe4cbee7d36f701992e245230b72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50165469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20e837351a85c5d1ad2a54b291f29efa67fb03ba9dc35ea6662bdfc54510e130`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Jun 2023 04:30:13 GMT
ADD file:558e8c34e969d458ce6bf4207d9c0fe05d2e67d3457c1d5689666749e82ef2ab in / 
# Tue, 13 Jun 2023 04:30:14 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 20:32:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 20:32:02 GMT
ENV HOME=/home/user
# Tue, 13 Jun 2023 20:32:03 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 13 Jun 2023 20:32:03 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 20:32:03 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 13 Jun 2023 20:32:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 13 Jun 2023 20:32:36 GMT
WORKDIR /home/user
# Tue, 13 Jun 2023 20:32:36 GMT
USER user
# Tue, 13 Jun 2023 20:32:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6a752e2308c741009b6f5a88a8ea6764b96ebe7f544197912d8ef9a3ec8c8763`  
		Last Modified: Tue, 13 Jun 2023 04:34:49 GMT  
		Size: 29.7 MB (29652514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8801b0ffac290f142720ddaa925d39bcd3618f1c130f5a0497634f2efa2d16d7`  
		Last Modified: Tue, 13 Jun 2023 20:33:03 GMT  
		Size: 15.8 MB (15757517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11c128c370af2f7eac6f07cfb2de9128c708f7328806131725ec7b950c46718`  
		Last Modified: Tue, 13 Jun 2023 20:33:00 GMT  
		Size: 4.2 KB (4206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a967901fa87998ad3b8800f8eb690db5ce84ded9e821210ddeda55901e488136`  
		Last Modified: Tue, 13 Jun 2023 20:33:01 GMT  
		Size: 4.8 MB (4751232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1-alpine`

```console
$ docker pull irssi@sha256:554d2243f8a34d09fa6a15bf3304eba7030550de34bdfa653b497cd752f287ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `irssi:1-alpine` - linux; amd64

```console
$ docker pull irssi@sha256:df33162f0e50c52c10cbc95a42f1cb42a89705f6c83ffd7afd7cbec9443a8f8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18276585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f1af4d2f8b92472032db235e289cb9962144969514aff20659771cbd821edea`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 05:44:22 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 15 Jun 2023 05:44:22 GMT
ENV HOME=/home/user
# Thu, 15 Jun 2023 05:44:23 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 15 Jun 2023 05:44:23 GMT
ENV LANG=C.UTF-8
# Thu, 15 Jun 2023 05:44:23 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 15 Jun 2023 05:44:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 15 Jun 2023 05:44:42 GMT
WORKDIR /home/user
# Thu, 15 Jun 2023 05:44:42 GMT
USER user
# Thu, 15 Jun 2023 05:44:42 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16db5ccbd16300cfe3a0c9f34b1f542069afdc21f717b410fae474a86e85c61f`  
		Last Modified: Thu, 15 Jun 2023 05:44:58 GMT  
		Size: 9.7 MB (9730952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d12740aa5ddf98127801ec314bbae032c68524b23c82d8e1e35a4a1ee5343e7`  
		Last Modified: Thu, 15 Jun 2023 05:44:57 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87af7c88801970c57df2d16564333d097ce75a779c2f1d3efe0b0a4a6683bb96`  
		Last Modified: Thu, 15 Jun 2023 05:44:58 GMT  
		Size: 5.2 MB (5169637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:bb597fb239a0bd0ab274a3954a976e7a8bd496662eeb66a9ea540606d3d8de35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17261761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcd756feb5566228922fc9f7d0e3904d76d421749b294dd3a4643d1c7274f5c7`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 00:58:29 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 00:58:31 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:58:32 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:58:32 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:58:32 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:58:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 00:58:52 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:58:52 GMT
USER user
# Thu, 22 Jun 2023 00:58:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da40b022b0296d6aa3db9bdeeb4c2e75c57f15429e1b6af2b7027548372ca8b`  
		Last Modified: Thu, 22 Jun 2023 00:59:06 GMT  
		Size: 8.9 MB (8873416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b96767a0ecd78f7941b675b0af4b50cbecb0d5152dab111a5a441594ae6603`  
		Last Modified: Thu, 22 Jun 2023 00:59:03 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b501eb48ba4f12d62b8aea88131359fb8f39cb356fac11d0259549db8e77d8`  
		Last Modified: Thu, 22 Jun 2023 00:59:04 GMT  
		Size: 5.2 MB (5243707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:0b986f46e3300def597e471838a101aa352def1ae0b5f7f9f42c97dfbd11b83b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16562586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1d80e6235adbd2367ceeee4bb15c7b1e544f7a8e7fee19f67d6676360de3ebd`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:20 GMT
ADD file:5e92075a8d9a5898d661caf9c2be8a83fb25742251b4ebdc0c3d448a6dc58e4a in / 
# Wed, 14 Jun 2023 22:36:20 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 02:36:44 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 15 Jun 2023 02:36:44 GMT
ENV HOME=/home/user
# Thu, 15 Jun 2023 02:36:44 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 15 Jun 2023 02:36:45 GMT
ENV LANG=C.UTF-8
# Thu, 15 Jun 2023 02:36:45 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 15 Jun 2023 02:37:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 15 Jun 2023 02:37:02 GMT
WORKDIR /home/user
# Thu, 15 Jun 2023 02:37:03 GMT
USER user
# Thu, 15 Jun 2023 02:37:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f929d112168394cf1fbe294a86fbe5173dd92df4daac8cb09437b17dfc5df802`  
		Last Modified: Wed, 14 Jun 2023 22:37:01 GMT  
		Size: 2.9 MB (2868554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19564852001304e25333fcaab3ff6b786fa9b4fd00951a0de7f21590421663c0`  
		Last Modified: Thu, 15 Jun 2023 02:37:17 GMT  
		Size: 8.9 MB (8862221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e9266e16eb957d32cfe744ce2a3e2816dcf23785557fc6f7a16823a7ca1555`  
		Last Modified: Thu, 15 Jun 2023 02:37:14 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7eca2cc340821a140c2b4125d47f2e4ede76abc67c397ae6956bd9f4fcab86`  
		Last Modified: Thu, 15 Jun 2023 02:37:15 GMT  
		Size: 4.8 MB (4830526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:22b4938b5405529664397a96505be6a0a68216bc5e4dfd1a21212650e8767e73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18305951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f25464e2094646ab0d15f3b07d9f086640cf1fe1514bbde35957288c200e8ce`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:00:36 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:00:36 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:00:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:00:37 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:00:37 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:00:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:00:49 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:00:49 GMT
USER user
# Thu, 22 Jun 2023 01:00:49 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f2b2cec23be63b100192d36d65457ca5a26f7eea16d8e43ade7f2a71b93ae6`  
		Last Modified: Thu, 22 Jun 2023 01:01:31 GMT  
		Size: 9.7 MB (9666778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f96463864962e4e3fb7c345cfbcf0bec7c4339f64ac2033fdc156dad9ef918`  
		Last Modified: Thu, 22 Jun 2023 01:01:29 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795ebb03672fc4e273a972202f51cdb3b57a46535e2e027c0ec705d277af2c6e`  
		Last Modified: Thu, 22 Jun 2023 01:01:30 GMT  
		Size: 5.3 MB (5308640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; 386

```console
$ docker pull irssi@sha256:fddae328f37731c13d5bf17a3946f5cd460fa8a1877b2c4eefcd83b0dd7b543a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.5 MB (17544572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b0dbc2e51d5bf9a3b7bd5cd8d2f1e40fa598f375d7750df018959bc790c1eb5`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:22 GMT
ADD file:94bec00e2c0c7f47c81ec4355a29ca23a81b439797d037b1a5a455f36a25dab4 in / 
# Wed, 14 Jun 2023 22:33:22 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 00:53:45 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 00:53:45 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:53:46 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:53:46 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:53:46 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:54:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 00:54:19 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:54:19 GMT
USER user
# Thu, 22 Jun 2023 00:54:19 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b3f50075abd13aad1cb7d8c1427aa59d7fcac88f3690d3f9c3efdbec80fd0856`  
		Last Modified: Wed, 14 Jun 2023 22:33:48 GMT  
		Size: 3.2 MB (3233951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af01bb2560a285c7c3f49f618c91cddeddaae06f68de1d63318a35d08ddd335`  
		Last Modified: Thu, 22 Jun 2023 00:55:14 GMT  
		Size: 8.9 MB (8896518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400b4f5222097fceb2802b1b4c86df1e17d9c756033d35b1bbe932496bb67d55`  
		Last Modified: Thu, 22 Jun 2023 00:55:11 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4f83428ff29063f3abf5ecdcdade0657f4c35089baf0e5a17abf0284dde4e9`  
		Last Modified: Thu, 22 Jun 2023 00:55:13 GMT  
		Size: 5.4 MB (5412820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:edbac3bc69ae83f6a98c2aad44f19c80a109631cb22bd3fa7f0c500242c62faf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18484325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e94c29de632503a0823c113d66340f5bc25c0af8ef7e8bff75880144aa1c2f0`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:56 GMT
ADD file:1c25b0be52aae22767603d9404fb777e27c5dd1bcd627221aac7517ac1bce1e3 in / 
# Thu, 15 Jun 2023 00:39:57 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 02:12:08 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 15 Jun 2023 02:12:09 GMT
ENV HOME=/home/user
# Thu, 15 Jun 2023 02:12:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 15 Jun 2023 02:12:10 GMT
ENV LANG=C.UTF-8
# Thu, 15 Jun 2023 02:12:11 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 15 Jun 2023 02:12:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 15 Jun 2023 02:12:35 GMT
WORKDIR /home/user
# Thu, 15 Jun 2023 02:12:35 GMT
USER user
# Thu, 15 Jun 2023 02:12:35 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8436307590cda5ccded8a952bb1d66684f8700d07029527293dd695eac6fabc9`  
		Last Modified: Thu, 15 Jun 2023 00:40:39 GMT  
		Size: 3.4 MB (3389905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864111a1d0261ae544596480b7c499eeaf06cbbe1bc28790c10c4f7c970266cc`  
		Last Modified: Thu, 15 Jun 2023 02:12:54 GMT  
		Size: 9.8 MB (9819563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0ad87a302112668f0b2d1aa81c90fea805716562d224e498f265e8fbc40ed9`  
		Last Modified: Thu, 15 Jun 2023 02:12:51 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc50b4b50b6a0ce01de8d1e1e0c6e619054efd5e6110152ccb85f0d07e940776`  
		Last Modified: Thu, 15 Jun 2023 02:12:52 GMT  
		Size: 5.3 MB (5273573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:dbf8a6d36f09f574725d7cc6f6284a867c447eb0ca83eb1cc60b6f88c1cc23c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18463228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ac2b28856e91692db99f7d4ddc3224676a32846026bfd08d2ee7c118a4f36f9`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 15 Jun 2023 05:19:50 GMT
ADD file:8ad8a62cf274ba5a6568f68473359114136cb5c7704bfdfce6c38efef3081782 in / 
# Thu, 15 Jun 2023 05:19:51 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 07:28:51 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 16 Jun 2023 07:28:52 GMT
ENV HOME=/home/user
# Fri, 16 Jun 2023 07:28:53 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 16 Jun 2023 07:28:54 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 07:28:54 GMT
ENV IRSSI_VERSION=1.4.4
# Fri, 16 Jun 2023 07:29:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 16 Jun 2023 07:29:18 GMT
WORKDIR /home/user
# Fri, 16 Jun 2023 07:29:18 GMT
USER user
# Fri, 16 Jun 2023 07:29:18 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:eb857838eb854a669f87c5df4d936d905fb3129287a93ef485da9454c11d83cd`  
		Last Modified: Thu, 15 Jun 2023 05:30:48 GMT  
		Size: 3.2 MB (3174898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7aaa04f45ef848c1c2f0c93b981862cc5a7e75fa94769dc25fa6e6c90124bb7`  
		Last Modified: Fri, 16 Jun 2023 07:33:42 GMT  
		Size: 10.2 MB (10161596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5466510fd4b694305a4d3e46080afb8ed895bded299c98d7284313b5de554715`  
		Last Modified: Fri, 16 Jun 2023 07:33:40 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd30109dad033bd844acba0eb497941214a16aadd9b6dd7d208ec1550930aaca`  
		Last Modified: Fri, 16 Jun 2023 07:33:41 GMT  
		Size: 5.1 MB (5125449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1-alpine3.18`

```console
$ docker pull irssi@sha256:fe09fe14dfdb8a3d17a7a8d6c2c13e3f8ddfbff09793154369dd58443fc9ade1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `irssi:1-alpine3.18` - linux; arm variant v6

```console
$ docker pull irssi@sha256:bb597fb239a0bd0ab274a3954a976e7a8bd496662eeb66a9ea540606d3d8de35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17261761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcd756feb5566228922fc9f7d0e3904d76d421749b294dd3a4643d1c7274f5c7`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 00:58:29 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 00:58:31 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:58:32 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:58:32 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:58:32 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:58:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 00:58:52 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:58:52 GMT
USER user
# Thu, 22 Jun 2023 00:58:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da40b022b0296d6aa3db9bdeeb4c2e75c57f15429e1b6af2b7027548372ca8b`  
		Last Modified: Thu, 22 Jun 2023 00:59:06 GMT  
		Size: 8.9 MB (8873416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b96767a0ecd78f7941b675b0af4b50cbecb0d5152dab111a5a441594ae6603`  
		Last Modified: Thu, 22 Jun 2023 00:59:03 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b501eb48ba4f12d62b8aea88131359fb8f39cb356fac11d0259549db8e77d8`  
		Last Modified: Thu, 22 Jun 2023 00:59:04 GMT  
		Size: 5.2 MB (5243707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:22b4938b5405529664397a96505be6a0a68216bc5e4dfd1a21212650e8767e73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18305951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f25464e2094646ab0d15f3b07d9f086640cf1fe1514bbde35957288c200e8ce`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:00:36 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:00:36 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:00:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:00:37 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:00:37 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:00:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:00:49 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:00:49 GMT
USER user
# Thu, 22 Jun 2023 01:00:49 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f2b2cec23be63b100192d36d65457ca5a26f7eea16d8e43ade7f2a71b93ae6`  
		Last Modified: Thu, 22 Jun 2023 01:01:31 GMT  
		Size: 9.7 MB (9666778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f96463864962e4e3fb7c345cfbcf0bec7c4339f64ac2033fdc156dad9ef918`  
		Last Modified: Thu, 22 Jun 2023 01:01:29 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795ebb03672fc4e273a972202f51cdb3b57a46535e2e027c0ec705d277af2c6e`  
		Last Modified: Thu, 22 Jun 2023 01:01:30 GMT  
		Size: 5.3 MB (5308640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine3.18` - linux; 386

```console
$ docker pull irssi@sha256:fddae328f37731c13d5bf17a3946f5cd460fa8a1877b2c4eefcd83b0dd7b543a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.5 MB (17544572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b0dbc2e51d5bf9a3b7bd5cd8d2f1e40fa598f375d7750df018959bc790c1eb5`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:22 GMT
ADD file:94bec00e2c0c7f47c81ec4355a29ca23a81b439797d037b1a5a455f36a25dab4 in / 
# Wed, 14 Jun 2023 22:33:22 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 00:53:45 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 00:53:45 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:53:46 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:53:46 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:53:46 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:54:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 00:54:19 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:54:19 GMT
USER user
# Thu, 22 Jun 2023 00:54:19 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b3f50075abd13aad1cb7d8c1427aa59d7fcac88f3690d3f9c3efdbec80fd0856`  
		Last Modified: Wed, 14 Jun 2023 22:33:48 GMT  
		Size: 3.2 MB (3233951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af01bb2560a285c7c3f49f618c91cddeddaae06f68de1d63318a35d08ddd335`  
		Last Modified: Thu, 22 Jun 2023 00:55:14 GMT  
		Size: 8.9 MB (8896518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400b4f5222097fceb2802b1b4c86df1e17d9c756033d35b1bbe932496bb67d55`  
		Last Modified: Thu, 22 Jun 2023 00:55:11 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4f83428ff29063f3abf5ecdcdade0657f4c35089baf0e5a17abf0284dde4e9`  
		Last Modified: Thu, 22 Jun 2023 00:55:13 GMT  
		Size: 5.4 MB (5412820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1-bookworm`

```console
$ docker pull irssi@sha256:3411a7a810e2ca8428f42cdd8111263294957fa5200720bd10e411922e759d74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386

### `irssi:1-bookworm` - linux; arm variant v5

```console
$ docker pull irssi@sha256:ec8e8fb46b70710ad03ffd0b0437286a0ec119c785edb791566d4534b21abf23
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70391870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb94ca655a3ecc2baf5113690a7bfa622f05cc2c362c9383c0a9bcfd736acf7d`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:48:31 GMT
ADD file:54a716f17b23e4fa49d1d5c0a7f63becc295873c116d19bb4753d34f1ca6affb in / 
# Mon, 12 Jun 2023 23:48:31 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 00:48:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 00:48:44 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:48:44 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:48:45 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:48:45 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:49:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 00:49:43 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:49:43 GMT
USER user
# Thu, 22 Jun 2023 00:49:43 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:70c60174b18d99741c33011138b5abf2f4d8eca0384521ccb43db3612078e36f`  
		Last Modified: Mon, 12 Jun 2023 23:51:26 GMT  
		Size: 27.0 MB (26982142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2fce51156cf8962c69bb6b4557b25c7c07264ce1ae06bcea0709030ed202ab`  
		Last Modified: Thu, 22 Jun 2023 00:50:07 GMT  
		Size: 17.1 MB (17083367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78197c8422a93eb658c23dff5d622f2d4f7524f184ddec1d7eda45e518c4354f`  
		Last Modified: Thu, 22 Jun 2023 00:50:03 GMT  
		Size: 3.4 KB (3370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4257c989a7f7bddb1161416c0d8ad56a66c61b37802ca313fea85633c9511567`  
		Last Modified: Thu, 22 Jun 2023 00:50:08 GMT  
		Size: 26.3 MB (26322991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-bookworm` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:266e75793b01d3790ac03073281aa85091694092f5da2a74804a57096c65e8cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74817663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2788ad4db80732ee28509ee691fff308c9dbf05d0f10c8264187cf487aea3e8`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:13 GMT
ADD file:f75c3fe22fec548b35a86a9a5802fdc97497f5d253cf630d65f13282169d3f3f in / 
# Mon, 12 Jun 2023 23:40:14 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 00:59:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 00:59:33 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:59:34 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:59:34 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:59:34 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:00:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 01:00:22 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:00:22 GMT
USER user
# Thu, 22 Jun 2023 01:00:23 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:95039a22a7cc3ae41d71f075e6e09e91e8da850fb5f80aba2f4a09f254520539`  
		Last Modified: Mon, 12 Jun 2023 23:44:08 GMT  
		Size: 29.2 MB (29152534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07791bb7d3b8da337cb7da387519554fbdb05d5d18a9015f7fd00751b524b4c6`  
		Last Modified: Thu, 22 Jun 2023 01:01:08 GMT  
		Size: 18.0 MB (18024086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b6d1cc205388e8478b3e53f9a0bd93b14aeac4315990aac3ad7b6d885c9ebe`  
		Last Modified: Thu, 22 Jun 2023 01:01:05 GMT  
		Size: 3.4 KB (3371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93207a63a416b94a1d0f7cf4c0794018f105ecd47ec4d24bc1ccf38d3269c5e`  
		Last Modified: Thu, 22 Jun 2023 01:01:09 GMT  
		Size: 27.6 MB (27637672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-bookworm` - linux; 386

```console
$ docker pull irssi@sha256:0189dd47eeb861dff6aae81b129a397bf423c30f9d10edafdfe0f60eabbacecf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76490983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4845371b0a05c37bd8b6d4f60b11c9829ab2a362e65e8f85033cd78c89200eb8`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:20 GMT
ADD file:c7ecc5e2bed99e2cbca26f9f4247cd9bc399749556f4084e9357a9b00bb80530 in / 
# Mon, 12 Jun 2023 23:39:20 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 00:52:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 00:52:29 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:52:29 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:52:29 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:52:30 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:53:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 00:53:34 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:53:34 GMT
USER user
# Thu, 22 Jun 2023 00:53:34 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:82a41d17956dd7c8ebb39c9ce936fd26841bdbec98d0a185e3db8154b352edff`  
		Last Modified: Mon, 12 Jun 2023 23:46:21 GMT  
		Size: 30.1 MB (30140741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb531271cfa6ef221334ee9305eae83f672ba29341a2024e4520dbf81b6aa8f`  
		Last Modified: Thu, 22 Jun 2023 00:54:50 GMT  
		Size: 17.8 MB (17783961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9dc41e70935097ed849f2b07b7ad815928f38688133be530d26cacf20f94040`  
		Last Modified: Thu, 22 Jun 2023 00:54:44 GMT  
		Size: 3.4 KB (3367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6bf06950cb921c0ef76ebc588fa3c5a0b713fdfa45199468d58e625ada6e6a9`  
		Last Modified: Thu, 22 Jun 2023 00:54:51 GMT  
		Size: 28.6 MB (28562914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4`

```console
$ docker pull irssi@sha256:14481b64cd4dc6c9a9f26629b698c88886eff923a6e4f296516508939c73333c
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

### `irssi:1.4` - linux; amd64

```console
$ docker pull irssi@sha256:1fda0af19ea9f808bab9108bb4b4528d6f36297ae226f7e17ebb2510aebbe39c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.4 MB (51353812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3240c2b2def4b35f616344709cdf6120faa7bdfb9973ce8e2100aa3905f16bfb`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:04:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:04:35 GMT
ENV HOME=/home/user
# Tue, 13 Jun 2023 07:04:36 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 13 Jun 2023 07:04:36 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 07:04:36 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 13 Jun 2023 07:05:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 13 Jun 2023 07:05:25 GMT
WORKDIR /home/user
# Tue, 13 Jun 2023 07:05:25 GMT
USER user
# Tue, 13 Jun 2023 07:05:25 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fa339e2e18ca8ee7894660c0b14e3f7ca734b3aeee8e2304b3e8c2563845ce`  
		Last Modified: Tue, 13 Jun 2023 07:05:49 GMT  
		Size: 15.5 MB (15457449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d616343ca0282e2d024ff05930f8eede4a1b1def9f5c9d7c706e5589fcfe44`  
		Last Modified: Tue, 13 Jun 2023 07:05:46 GMT  
		Size: 4.2 KB (4202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24ca3bf390591ce5506aa13625a97a7e80eb5fa1f34b25e33a9bdbfef4a1589`  
		Last Modified: Tue, 13 Jun 2023 07:05:47 GMT  
		Size: 4.5 MB (4474751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; arm variant v5

```console
$ docker pull irssi@sha256:ec8e8fb46b70710ad03ffd0b0437286a0ec119c785edb791566d4534b21abf23
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70391870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb94ca655a3ecc2baf5113690a7bfa622f05cc2c362c9383c0a9bcfd736acf7d`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:48:31 GMT
ADD file:54a716f17b23e4fa49d1d5c0a7f63becc295873c116d19bb4753d34f1ca6affb in / 
# Mon, 12 Jun 2023 23:48:31 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 00:48:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 00:48:44 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:48:44 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:48:45 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:48:45 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:49:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 00:49:43 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:49:43 GMT
USER user
# Thu, 22 Jun 2023 00:49:43 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:70c60174b18d99741c33011138b5abf2f4d8eca0384521ccb43db3612078e36f`  
		Last Modified: Mon, 12 Jun 2023 23:51:26 GMT  
		Size: 27.0 MB (26982142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2fce51156cf8962c69bb6b4557b25c7c07264ce1ae06bcea0709030ed202ab`  
		Last Modified: Thu, 22 Jun 2023 00:50:07 GMT  
		Size: 17.1 MB (17083367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78197c8422a93eb658c23dff5d622f2d4f7524f184ddec1d7eda45e518c4354f`  
		Last Modified: Thu, 22 Jun 2023 00:50:03 GMT  
		Size: 3.4 KB (3370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4257c989a7f7bddb1161416c0d8ad56a66c61b37802ca313fea85633c9511567`  
		Last Modified: Thu, 22 Jun 2023 00:50:08 GMT  
		Size: 26.3 MB (26322991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; arm variant v7

```console
$ docker pull irssi@sha256:6b07201205f1936d606641ab462c40bcb52da3a8867b54d3c275685eeeb90ecb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45156187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0bc29edfecb98551b42621135d0e6a9a8df4e4eaf154137cf368ede533f1ceb`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:47 GMT
ADD file:319a24b7e30fc548f9dcf48ad6cee469e8bf7e89c67901cf3851e41e75693489 in / 
# Mon, 12 Jun 2023 23:58:47 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 17:16:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 17:16:56 GMT
ENV HOME=/home/user
# Tue, 13 Jun 2023 17:16:57 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 13 Jun 2023 17:16:57 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 17:16:57 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 13 Jun 2023 17:17:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 13 Jun 2023 17:17:44 GMT
WORKDIR /home/user
# Tue, 13 Jun 2023 17:17:45 GMT
USER user
# Tue, 13 Jun 2023 17:17:45 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b7c295cb849275e211d18b720d2349cc84c0038be1a362aca4765ceb3342043c`  
		Last Modified: Tue, 13 Jun 2023 00:04:24 GMT  
		Size: 26.6 MB (26578690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849490fbc07826e4ba5d7341723cfc86674072f6dea1fef7ee6c95a2d47f94ea`  
		Last Modified: Tue, 13 Jun 2023 17:18:12 GMT  
		Size: 14.4 MB (14385956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2ac9297b563c1cb4c92586f2e565024907221ef118e14789c48461ec982ce1`  
		Last Modified: Tue, 13 Jun 2023 17:18:08 GMT  
		Size: 4.2 KB (4190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0386945f81bf6c09429e43066eab30120446fd066a8e3d3450bf756774b9bad2`  
		Last Modified: Tue, 13 Jun 2023 17:18:09 GMT  
		Size: 4.2 MB (4187351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:266e75793b01d3790ac03073281aa85091694092f5da2a74804a57096c65e8cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74817663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2788ad4db80732ee28509ee691fff308c9dbf05d0f10c8264187cf487aea3e8`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:13 GMT
ADD file:f75c3fe22fec548b35a86a9a5802fdc97497f5d253cf630d65f13282169d3f3f in / 
# Mon, 12 Jun 2023 23:40:14 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 00:59:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 00:59:33 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:59:34 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:59:34 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:59:34 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:00:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 01:00:22 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:00:22 GMT
USER user
# Thu, 22 Jun 2023 01:00:23 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:95039a22a7cc3ae41d71f075e6e09e91e8da850fb5f80aba2f4a09f254520539`  
		Last Modified: Mon, 12 Jun 2023 23:44:08 GMT  
		Size: 29.2 MB (29152534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07791bb7d3b8da337cb7da387519554fbdb05d5d18a9015f7fd00751b524b4c6`  
		Last Modified: Thu, 22 Jun 2023 01:01:08 GMT  
		Size: 18.0 MB (18024086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b6d1cc205388e8478b3e53f9a0bd93b14aeac4315990aac3ad7b6d885c9ebe`  
		Last Modified: Thu, 22 Jun 2023 01:01:05 GMT  
		Size: 3.4 KB (3371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93207a63a416b94a1d0f7cf4c0794018f105ecd47ec4d24bc1ccf38d3269c5e`  
		Last Modified: Thu, 22 Jun 2023 01:01:09 GMT  
		Size: 27.6 MB (27637672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; 386

```console
$ docker pull irssi@sha256:0189dd47eeb861dff6aae81b129a397bf423c30f9d10edafdfe0f60eabbacecf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76490983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4845371b0a05c37bd8b6d4f60b11c9829ab2a362e65e8f85033cd78c89200eb8`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:20 GMT
ADD file:c7ecc5e2bed99e2cbca26f9f4247cd9bc399749556f4084e9357a9b00bb80530 in / 
# Mon, 12 Jun 2023 23:39:20 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 00:52:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 00:52:29 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:52:29 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:52:29 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:52:30 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:53:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 00:53:34 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:53:34 GMT
USER user
# Thu, 22 Jun 2023 00:53:34 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:82a41d17956dd7c8ebb39c9ce936fd26841bdbec98d0a185e3db8154b352edff`  
		Last Modified: Mon, 12 Jun 2023 23:46:21 GMT  
		Size: 30.1 MB (30140741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb531271cfa6ef221334ee9305eae83f672ba29341a2024e4520dbf81b6aa8f`  
		Last Modified: Thu, 22 Jun 2023 00:54:50 GMT  
		Size: 17.8 MB (17783961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9dc41e70935097ed849f2b07b7ad815928f38688133be530d26cacf20f94040`  
		Last Modified: Thu, 22 Jun 2023 00:54:44 GMT  
		Size: 3.4 KB (3367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6bf06950cb921c0ef76ebc588fa3c5a0b713fdfa45199468d58e625ada6e6a9`  
		Last Modified: Thu, 22 Jun 2023 00:54:51 GMT  
		Size: 28.6 MB (28562914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; mips64le

```console
$ docker pull irssi@sha256:fcad96467ecda441065d8062d7deffe2231cf5473de7f214932098cb7469b642
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.4 MB (48376311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:385baa614e97ceda4073810d1f47b470ba54a00c18ced3b057f8f8a21f9688cd`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Jun 2023 00:10:34 GMT
ADD file:4d5c7737e954f157e3d7ea47cc1814c46ec5c753a3d5d828ad9614969b572253 in / 
# Tue, 13 Jun 2023 00:10:38 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 14:58:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 14:58:45 GMT
ENV HOME=/home/user
# Tue, 13 Jun 2023 14:58:52 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 13 Jun 2023 14:58:55 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 14:58:58 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 13 Jun 2023 15:02:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 13 Jun 2023 15:02:56 GMT
WORKDIR /home/user
# Tue, 13 Jun 2023 15:02:59 GMT
USER user
# Tue, 13 Jun 2023 15:03:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:61bd6562a93acd0a3b327321e5465408e1d921b3ce1fb4fe353633330c3ede91`  
		Last Modified: Tue, 13 Jun 2023 00:23:53 GMT  
		Size: 29.6 MB (29634422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cd3adcf928d62813a219ad0c5c5c8015b780b4a6b4bb1ded47ae7f4e77036b`  
		Last Modified: Tue, 13 Jun 2023 15:03:43 GMT  
		Size: 14.4 MB (14421797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b360405355f5536c6ebb3ed5466c97a155165087081278fd8326b9c6a618e41c`  
		Last Modified: Tue, 13 Jun 2023 15:03:30 GMT  
		Size: 4.1 KB (4066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cf810f1b3cb9d35488e456c3cd9a56a60af589307368bb89a24c740fc94727`  
		Last Modified: Tue, 13 Jun 2023 15:03:33 GMT  
		Size: 4.3 MB (4316026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; ppc64le

```console
$ docker pull irssi@sha256:2c84f21d14766ef5faf43cbde7d5d21da7fbb7380ad823f06c9ffe0e6af8246f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55734024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39a07dc4dd7e0a6d1e413452909230f2fef5affd9aa6aad211c12e99096995bf`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:18:20 GMT
ADD file:b17eabe509462fa1a2e4c5421e877e3e4149085e3da07a421a66c7b06566c457 in / 
# Mon, 12 Jun 2023 23:18:22 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 08:47:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 08:47:07 GMT
ENV HOME=/home/user
# Tue, 13 Jun 2023 08:47:08 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 13 Jun 2023 08:47:08 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 08:47:08 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 13 Jun 2023 08:48:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 13 Jun 2023 08:48:26 GMT
WORKDIR /home/user
# Tue, 13 Jun 2023 08:48:26 GMT
USER user
# Tue, 13 Jun 2023 08:48:26 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2973ac0be4a80a6cecbb73370e92810a6f67a98e12e61b3044aa63a322dab03a`  
		Last Modified: Mon, 12 Jun 2023 23:25:03 GMT  
		Size: 35.3 MB (35290790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc5bd67d599f4e07b6f68f09a02d378eac43824b1a4cda56b24bc1c51d7c5ee`  
		Last Modified: Tue, 13 Jun 2023 08:48:45 GMT  
		Size: 15.8 MB (15756316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382a2c88702295eea22c668bccd54ea16eae65ffa15581e3bc67235a3c431e1b`  
		Last Modified: Tue, 13 Jun 2023 08:48:40 GMT  
		Size: 4.2 KB (4204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0199a0ffe4039f498bae34b531ebd5b5c6cdfa729e2233e3f5ca444d92962e`  
		Last Modified: Tue, 13 Jun 2023 08:48:41 GMT  
		Size: 4.7 MB (4682714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; s390x

```console
$ docker pull irssi@sha256:e400a68cd9ed507fdcb70211f4e758d4ab1abe4cbee7d36f701992e245230b72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50165469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20e837351a85c5d1ad2a54b291f29efa67fb03ba9dc35ea6662bdfc54510e130`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Jun 2023 04:30:13 GMT
ADD file:558e8c34e969d458ce6bf4207d9c0fe05d2e67d3457c1d5689666749e82ef2ab in / 
# Tue, 13 Jun 2023 04:30:14 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 20:32:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 20:32:02 GMT
ENV HOME=/home/user
# Tue, 13 Jun 2023 20:32:03 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 13 Jun 2023 20:32:03 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 20:32:03 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 13 Jun 2023 20:32:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 13 Jun 2023 20:32:36 GMT
WORKDIR /home/user
# Tue, 13 Jun 2023 20:32:36 GMT
USER user
# Tue, 13 Jun 2023 20:32:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6a752e2308c741009b6f5a88a8ea6764b96ebe7f544197912d8ef9a3ec8c8763`  
		Last Modified: Tue, 13 Jun 2023 04:34:49 GMT  
		Size: 29.7 MB (29652514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8801b0ffac290f142720ddaa925d39bcd3618f1c130f5a0497634f2efa2d16d7`  
		Last Modified: Tue, 13 Jun 2023 20:33:03 GMT  
		Size: 15.8 MB (15757517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11c128c370af2f7eac6f07cfb2de9128c708f7328806131725ec7b950c46718`  
		Last Modified: Tue, 13 Jun 2023 20:33:00 GMT  
		Size: 4.2 KB (4206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a967901fa87998ad3b8800f8eb690db5ce84ded9e821210ddeda55901e488136`  
		Last Modified: Tue, 13 Jun 2023 20:33:01 GMT  
		Size: 4.8 MB (4751232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4-alpine`

```console
$ docker pull irssi@sha256:554d2243f8a34d09fa6a15bf3304eba7030550de34bdfa653b497cd752f287ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `irssi:1.4-alpine` - linux; amd64

```console
$ docker pull irssi@sha256:df33162f0e50c52c10cbc95a42f1cb42a89705f6c83ffd7afd7cbec9443a8f8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18276585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f1af4d2f8b92472032db235e289cb9962144969514aff20659771cbd821edea`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 05:44:22 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 15 Jun 2023 05:44:22 GMT
ENV HOME=/home/user
# Thu, 15 Jun 2023 05:44:23 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 15 Jun 2023 05:44:23 GMT
ENV LANG=C.UTF-8
# Thu, 15 Jun 2023 05:44:23 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 15 Jun 2023 05:44:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 15 Jun 2023 05:44:42 GMT
WORKDIR /home/user
# Thu, 15 Jun 2023 05:44:42 GMT
USER user
# Thu, 15 Jun 2023 05:44:42 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16db5ccbd16300cfe3a0c9f34b1f542069afdc21f717b410fae474a86e85c61f`  
		Last Modified: Thu, 15 Jun 2023 05:44:58 GMT  
		Size: 9.7 MB (9730952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d12740aa5ddf98127801ec314bbae032c68524b23c82d8e1e35a4a1ee5343e7`  
		Last Modified: Thu, 15 Jun 2023 05:44:57 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87af7c88801970c57df2d16564333d097ce75a779c2f1d3efe0b0a4a6683bb96`  
		Last Modified: Thu, 15 Jun 2023 05:44:58 GMT  
		Size: 5.2 MB (5169637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:bb597fb239a0bd0ab274a3954a976e7a8bd496662eeb66a9ea540606d3d8de35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17261761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcd756feb5566228922fc9f7d0e3904d76d421749b294dd3a4643d1c7274f5c7`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 00:58:29 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 00:58:31 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:58:32 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:58:32 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:58:32 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:58:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 00:58:52 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:58:52 GMT
USER user
# Thu, 22 Jun 2023 00:58:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da40b022b0296d6aa3db9bdeeb4c2e75c57f15429e1b6af2b7027548372ca8b`  
		Last Modified: Thu, 22 Jun 2023 00:59:06 GMT  
		Size: 8.9 MB (8873416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b96767a0ecd78f7941b675b0af4b50cbecb0d5152dab111a5a441594ae6603`  
		Last Modified: Thu, 22 Jun 2023 00:59:03 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b501eb48ba4f12d62b8aea88131359fb8f39cb356fac11d0259549db8e77d8`  
		Last Modified: Thu, 22 Jun 2023 00:59:04 GMT  
		Size: 5.2 MB (5243707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:0b986f46e3300def597e471838a101aa352def1ae0b5f7f9f42c97dfbd11b83b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16562586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1d80e6235adbd2367ceeee4bb15c7b1e544f7a8e7fee19f67d6676360de3ebd`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:20 GMT
ADD file:5e92075a8d9a5898d661caf9c2be8a83fb25742251b4ebdc0c3d448a6dc58e4a in / 
# Wed, 14 Jun 2023 22:36:20 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 02:36:44 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 15 Jun 2023 02:36:44 GMT
ENV HOME=/home/user
# Thu, 15 Jun 2023 02:36:44 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 15 Jun 2023 02:36:45 GMT
ENV LANG=C.UTF-8
# Thu, 15 Jun 2023 02:36:45 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 15 Jun 2023 02:37:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 15 Jun 2023 02:37:02 GMT
WORKDIR /home/user
# Thu, 15 Jun 2023 02:37:03 GMT
USER user
# Thu, 15 Jun 2023 02:37:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f929d112168394cf1fbe294a86fbe5173dd92df4daac8cb09437b17dfc5df802`  
		Last Modified: Wed, 14 Jun 2023 22:37:01 GMT  
		Size: 2.9 MB (2868554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19564852001304e25333fcaab3ff6b786fa9b4fd00951a0de7f21590421663c0`  
		Last Modified: Thu, 15 Jun 2023 02:37:17 GMT  
		Size: 8.9 MB (8862221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e9266e16eb957d32cfe744ce2a3e2816dcf23785557fc6f7a16823a7ca1555`  
		Last Modified: Thu, 15 Jun 2023 02:37:14 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7eca2cc340821a140c2b4125d47f2e4ede76abc67c397ae6956bd9f4fcab86`  
		Last Modified: Thu, 15 Jun 2023 02:37:15 GMT  
		Size: 4.8 MB (4830526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:22b4938b5405529664397a96505be6a0a68216bc5e4dfd1a21212650e8767e73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18305951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f25464e2094646ab0d15f3b07d9f086640cf1fe1514bbde35957288c200e8ce`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:00:36 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:00:36 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:00:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:00:37 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:00:37 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:00:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:00:49 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:00:49 GMT
USER user
# Thu, 22 Jun 2023 01:00:49 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f2b2cec23be63b100192d36d65457ca5a26f7eea16d8e43ade7f2a71b93ae6`  
		Last Modified: Thu, 22 Jun 2023 01:01:31 GMT  
		Size: 9.7 MB (9666778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f96463864962e4e3fb7c345cfbcf0bec7c4339f64ac2033fdc156dad9ef918`  
		Last Modified: Thu, 22 Jun 2023 01:01:29 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795ebb03672fc4e273a972202f51cdb3b57a46535e2e027c0ec705d277af2c6e`  
		Last Modified: Thu, 22 Jun 2023 01:01:30 GMT  
		Size: 5.3 MB (5308640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine` - linux; 386

```console
$ docker pull irssi@sha256:fddae328f37731c13d5bf17a3946f5cd460fa8a1877b2c4eefcd83b0dd7b543a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.5 MB (17544572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b0dbc2e51d5bf9a3b7bd5cd8d2f1e40fa598f375d7750df018959bc790c1eb5`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:22 GMT
ADD file:94bec00e2c0c7f47c81ec4355a29ca23a81b439797d037b1a5a455f36a25dab4 in / 
# Wed, 14 Jun 2023 22:33:22 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 00:53:45 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 00:53:45 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:53:46 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:53:46 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:53:46 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:54:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 00:54:19 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:54:19 GMT
USER user
# Thu, 22 Jun 2023 00:54:19 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b3f50075abd13aad1cb7d8c1427aa59d7fcac88f3690d3f9c3efdbec80fd0856`  
		Last Modified: Wed, 14 Jun 2023 22:33:48 GMT  
		Size: 3.2 MB (3233951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af01bb2560a285c7c3f49f618c91cddeddaae06f68de1d63318a35d08ddd335`  
		Last Modified: Thu, 22 Jun 2023 00:55:14 GMT  
		Size: 8.9 MB (8896518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400b4f5222097fceb2802b1b4c86df1e17d9c756033d35b1bbe932496bb67d55`  
		Last Modified: Thu, 22 Jun 2023 00:55:11 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4f83428ff29063f3abf5ecdcdade0657f4c35089baf0e5a17abf0284dde4e9`  
		Last Modified: Thu, 22 Jun 2023 00:55:13 GMT  
		Size: 5.4 MB (5412820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:edbac3bc69ae83f6a98c2aad44f19c80a109631cb22bd3fa7f0c500242c62faf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18484325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e94c29de632503a0823c113d66340f5bc25c0af8ef7e8bff75880144aa1c2f0`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:56 GMT
ADD file:1c25b0be52aae22767603d9404fb777e27c5dd1bcd627221aac7517ac1bce1e3 in / 
# Thu, 15 Jun 2023 00:39:57 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 02:12:08 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 15 Jun 2023 02:12:09 GMT
ENV HOME=/home/user
# Thu, 15 Jun 2023 02:12:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 15 Jun 2023 02:12:10 GMT
ENV LANG=C.UTF-8
# Thu, 15 Jun 2023 02:12:11 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 15 Jun 2023 02:12:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 15 Jun 2023 02:12:35 GMT
WORKDIR /home/user
# Thu, 15 Jun 2023 02:12:35 GMT
USER user
# Thu, 15 Jun 2023 02:12:35 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8436307590cda5ccded8a952bb1d66684f8700d07029527293dd695eac6fabc9`  
		Last Modified: Thu, 15 Jun 2023 00:40:39 GMT  
		Size: 3.4 MB (3389905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864111a1d0261ae544596480b7c499eeaf06cbbe1bc28790c10c4f7c970266cc`  
		Last Modified: Thu, 15 Jun 2023 02:12:54 GMT  
		Size: 9.8 MB (9819563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0ad87a302112668f0b2d1aa81c90fea805716562d224e498f265e8fbc40ed9`  
		Last Modified: Thu, 15 Jun 2023 02:12:51 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc50b4b50b6a0ce01de8d1e1e0c6e619054efd5e6110152ccb85f0d07e940776`  
		Last Modified: Thu, 15 Jun 2023 02:12:52 GMT  
		Size: 5.3 MB (5273573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:dbf8a6d36f09f574725d7cc6f6284a867c447eb0ca83eb1cc60b6f88c1cc23c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18463228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ac2b28856e91692db99f7d4ddc3224676a32846026bfd08d2ee7c118a4f36f9`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 15 Jun 2023 05:19:50 GMT
ADD file:8ad8a62cf274ba5a6568f68473359114136cb5c7704bfdfce6c38efef3081782 in / 
# Thu, 15 Jun 2023 05:19:51 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 07:28:51 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 16 Jun 2023 07:28:52 GMT
ENV HOME=/home/user
# Fri, 16 Jun 2023 07:28:53 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 16 Jun 2023 07:28:54 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 07:28:54 GMT
ENV IRSSI_VERSION=1.4.4
# Fri, 16 Jun 2023 07:29:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 16 Jun 2023 07:29:18 GMT
WORKDIR /home/user
# Fri, 16 Jun 2023 07:29:18 GMT
USER user
# Fri, 16 Jun 2023 07:29:18 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:eb857838eb854a669f87c5df4d936d905fb3129287a93ef485da9454c11d83cd`  
		Last Modified: Thu, 15 Jun 2023 05:30:48 GMT  
		Size: 3.2 MB (3174898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7aaa04f45ef848c1c2f0c93b981862cc5a7e75fa94769dc25fa6e6c90124bb7`  
		Last Modified: Fri, 16 Jun 2023 07:33:42 GMT  
		Size: 10.2 MB (10161596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5466510fd4b694305a4d3e46080afb8ed895bded299c98d7284313b5de554715`  
		Last Modified: Fri, 16 Jun 2023 07:33:40 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd30109dad033bd844acba0eb497941214a16aadd9b6dd7d208ec1550930aaca`  
		Last Modified: Fri, 16 Jun 2023 07:33:41 GMT  
		Size: 5.1 MB (5125449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4-alpine3.18`

```console
$ docker pull irssi@sha256:fe09fe14dfdb8a3d17a7a8d6c2c13e3f8ddfbff09793154369dd58443fc9ade1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `irssi:1.4-alpine3.18` - linux; arm variant v6

```console
$ docker pull irssi@sha256:bb597fb239a0bd0ab274a3954a976e7a8bd496662eeb66a9ea540606d3d8de35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17261761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcd756feb5566228922fc9f7d0e3904d76d421749b294dd3a4643d1c7274f5c7`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 00:58:29 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 00:58:31 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:58:32 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:58:32 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:58:32 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:58:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 00:58:52 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:58:52 GMT
USER user
# Thu, 22 Jun 2023 00:58:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da40b022b0296d6aa3db9bdeeb4c2e75c57f15429e1b6af2b7027548372ca8b`  
		Last Modified: Thu, 22 Jun 2023 00:59:06 GMT  
		Size: 8.9 MB (8873416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b96767a0ecd78f7941b675b0af4b50cbecb0d5152dab111a5a441594ae6603`  
		Last Modified: Thu, 22 Jun 2023 00:59:03 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b501eb48ba4f12d62b8aea88131359fb8f39cb356fac11d0259549db8e77d8`  
		Last Modified: Thu, 22 Jun 2023 00:59:04 GMT  
		Size: 5.2 MB (5243707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:22b4938b5405529664397a96505be6a0a68216bc5e4dfd1a21212650e8767e73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18305951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f25464e2094646ab0d15f3b07d9f086640cf1fe1514bbde35957288c200e8ce`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:00:36 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:00:36 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:00:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:00:37 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:00:37 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:00:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:00:49 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:00:49 GMT
USER user
# Thu, 22 Jun 2023 01:00:49 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f2b2cec23be63b100192d36d65457ca5a26f7eea16d8e43ade7f2a71b93ae6`  
		Last Modified: Thu, 22 Jun 2023 01:01:31 GMT  
		Size: 9.7 MB (9666778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f96463864962e4e3fb7c345cfbcf0bec7c4339f64ac2033fdc156dad9ef918`  
		Last Modified: Thu, 22 Jun 2023 01:01:29 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795ebb03672fc4e273a972202f51cdb3b57a46535e2e027c0ec705d277af2c6e`  
		Last Modified: Thu, 22 Jun 2023 01:01:30 GMT  
		Size: 5.3 MB (5308640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine3.18` - linux; 386

```console
$ docker pull irssi@sha256:fddae328f37731c13d5bf17a3946f5cd460fa8a1877b2c4eefcd83b0dd7b543a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.5 MB (17544572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b0dbc2e51d5bf9a3b7bd5cd8d2f1e40fa598f375d7750df018959bc790c1eb5`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:22 GMT
ADD file:94bec00e2c0c7f47c81ec4355a29ca23a81b439797d037b1a5a455f36a25dab4 in / 
# Wed, 14 Jun 2023 22:33:22 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 00:53:45 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 00:53:45 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:53:46 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:53:46 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:53:46 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:54:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 00:54:19 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:54:19 GMT
USER user
# Thu, 22 Jun 2023 00:54:19 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b3f50075abd13aad1cb7d8c1427aa59d7fcac88f3690d3f9c3efdbec80fd0856`  
		Last Modified: Wed, 14 Jun 2023 22:33:48 GMT  
		Size: 3.2 MB (3233951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af01bb2560a285c7c3f49f618c91cddeddaae06f68de1d63318a35d08ddd335`  
		Last Modified: Thu, 22 Jun 2023 00:55:14 GMT  
		Size: 8.9 MB (8896518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400b4f5222097fceb2802b1b4c86df1e17d9c756033d35b1bbe932496bb67d55`  
		Last Modified: Thu, 22 Jun 2023 00:55:11 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4f83428ff29063f3abf5ecdcdade0657f4c35089baf0e5a17abf0284dde4e9`  
		Last Modified: Thu, 22 Jun 2023 00:55:13 GMT  
		Size: 5.4 MB (5412820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4-bookworm`

```console
$ docker pull irssi@sha256:3411a7a810e2ca8428f42cdd8111263294957fa5200720bd10e411922e759d74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386

### `irssi:1.4-bookworm` - linux; arm variant v5

```console
$ docker pull irssi@sha256:ec8e8fb46b70710ad03ffd0b0437286a0ec119c785edb791566d4534b21abf23
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70391870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb94ca655a3ecc2baf5113690a7bfa622f05cc2c362c9383c0a9bcfd736acf7d`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:48:31 GMT
ADD file:54a716f17b23e4fa49d1d5c0a7f63becc295873c116d19bb4753d34f1ca6affb in / 
# Mon, 12 Jun 2023 23:48:31 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 00:48:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 00:48:44 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:48:44 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:48:45 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:48:45 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:49:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 00:49:43 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:49:43 GMT
USER user
# Thu, 22 Jun 2023 00:49:43 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:70c60174b18d99741c33011138b5abf2f4d8eca0384521ccb43db3612078e36f`  
		Last Modified: Mon, 12 Jun 2023 23:51:26 GMT  
		Size: 27.0 MB (26982142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2fce51156cf8962c69bb6b4557b25c7c07264ce1ae06bcea0709030ed202ab`  
		Last Modified: Thu, 22 Jun 2023 00:50:07 GMT  
		Size: 17.1 MB (17083367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78197c8422a93eb658c23dff5d622f2d4f7524f184ddec1d7eda45e518c4354f`  
		Last Modified: Thu, 22 Jun 2023 00:50:03 GMT  
		Size: 3.4 KB (3370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4257c989a7f7bddb1161416c0d8ad56a66c61b37802ca313fea85633c9511567`  
		Last Modified: Thu, 22 Jun 2023 00:50:08 GMT  
		Size: 26.3 MB (26322991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-bookworm` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:266e75793b01d3790ac03073281aa85091694092f5da2a74804a57096c65e8cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74817663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2788ad4db80732ee28509ee691fff308c9dbf05d0f10c8264187cf487aea3e8`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:13 GMT
ADD file:f75c3fe22fec548b35a86a9a5802fdc97497f5d253cf630d65f13282169d3f3f in / 
# Mon, 12 Jun 2023 23:40:14 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 00:59:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 00:59:33 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:59:34 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:59:34 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:59:34 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:00:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 01:00:22 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:00:22 GMT
USER user
# Thu, 22 Jun 2023 01:00:23 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:95039a22a7cc3ae41d71f075e6e09e91e8da850fb5f80aba2f4a09f254520539`  
		Last Modified: Mon, 12 Jun 2023 23:44:08 GMT  
		Size: 29.2 MB (29152534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07791bb7d3b8da337cb7da387519554fbdb05d5d18a9015f7fd00751b524b4c6`  
		Last Modified: Thu, 22 Jun 2023 01:01:08 GMT  
		Size: 18.0 MB (18024086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b6d1cc205388e8478b3e53f9a0bd93b14aeac4315990aac3ad7b6d885c9ebe`  
		Last Modified: Thu, 22 Jun 2023 01:01:05 GMT  
		Size: 3.4 KB (3371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93207a63a416b94a1d0f7cf4c0794018f105ecd47ec4d24bc1ccf38d3269c5e`  
		Last Modified: Thu, 22 Jun 2023 01:01:09 GMT  
		Size: 27.6 MB (27637672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-bookworm` - linux; 386

```console
$ docker pull irssi@sha256:0189dd47eeb861dff6aae81b129a397bf423c30f9d10edafdfe0f60eabbacecf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76490983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4845371b0a05c37bd8b6d4f60b11c9829ab2a362e65e8f85033cd78c89200eb8`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:20 GMT
ADD file:c7ecc5e2bed99e2cbca26f9f4247cd9bc399749556f4084e9357a9b00bb80530 in / 
# Mon, 12 Jun 2023 23:39:20 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 00:52:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 00:52:29 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:52:29 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:52:29 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:52:30 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:53:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 00:53:34 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:53:34 GMT
USER user
# Thu, 22 Jun 2023 00:53:34 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:82a41d17956dd7c8ebb39c9ce936fd26841bdbec98d0a185e3db8154b352edff`  
		Last Modified: Mon, 12 Jun 2023 23:46:21 GMT  
		Size: 30.1 MB (30140741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb531271cfa6ef221334ee9305eae83f672ba29341a2024e4520dbf81b6aa8f`  
		Last Modified: Thu, 22 Jun 2023 00:54:50 GMT  
		Size: 17.8 MB (17783961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9dc41e70935097ed849f2b07b7ad815928f38688133be530d26cacf20f94040`  
		Last Modified: Thu, 22 Jun 2023 00:54:44 GMT  
		Size: 3.4 KB (3367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6bf06950cb921c0ef76ebc588fa3c5a0b713fdfa45199468d58e625ada6e6a9`  
		Last Modified: Thu, 22 Jun 2023 00:54:51 GMT  
		Size: 28.6 MB (28562914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4.4`

```console
$ docker pull irssi@sha256:14481b64cd4dc6c9a9f26629b698c88886eff923a6e4f296516508939c73333c
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

### `irssi:1.4.4` - linux; amd64

```console
$ docker pull irssi@sha256:1fda0af19ea9f808bab9108bb4b4528d6f36297ae226f7e17ebb2510aebbe39c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.4 MB (51353812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3240c2b2def4b35f616344709cdf6120faa7bdfb9973ce8e2100aa3905f16bfb`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:04:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:04:35 GMT
ENV HOME=/home/user
# Tue, 13 Jun 2023 07:04:36 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 13 Jun 2023 07:04:36 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 07:04:36 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 13 Jun 2023 07:05:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 13 Jun 2023 07:05:25 GMT
WORKDIR /home/user
# Tue, 13 Jun 2023 07:05:25 GMT
USER user
# Tue, 13 Jun 2023 07:05:25 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fa339e2e18ca8ee7894660c0b14e3f7ca734b3aeee8e2304b3e8c2563845ce`  
		Last Modified: Tue, 13 Jun 2023 07:05:49 GMT  
		Size: 15.5 MB (15457449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d616343ca0282e2d024ff05930f8eede4a1b1def9f5c9d7c706e5589fcfe44`  
		Last Modified: Tue, 13 Jun 2023 07:05:46 GMT  
		Size: 4.2 KB (4202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24ca3bf390591ce5506aa13625a97a7e80eb5fa1f34b25e33a9bdbfef4a1589`  
		Last Modified: Tue, 13 Jun 2023 07:05:47 GMT  
		Size: 4.5 MB (4474751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.4` - linux; arm variant v5

```console
$ docker pull irssi@sha256:ec8e8fb46b70710ad03ffd0b0437286a0ec119c785edb791566d4534b21abf23
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70391870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb94ca655a3ecc2baf5113690a7bfa622f05cc2c362c9383c0a9bcfd736acf7d`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:48:31 GMT
ADD file:54a716f17b23e4fa49d1d5c0a7f63becc295873c116d19bb4753d34f1ca6affb in / 
# Mon, 12 Jun 2023 23:48:31 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 00:48:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 00:48:44 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:48:44 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:48:45 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:48:45 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:49:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 00:49:43 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:49:43 GMT
USER user
# Thu, 22 Jun 2023 00:49:43 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:70c60174b18d99741c33011138b5abf2f4d8eca0384521ccb43db3612078e36f`  
		Last Modified: Mon, 12 Jun 2023 23:51:26 GMT  
		Size: 27.0 MB (26982142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2fce51156cf8962c69bb6b4557b25c7c07264ce1ae06bcea0709030ed202ab`  
		Last Modified: Thu, 22 Jun 2023 00:50:07 GMT  
		Size: 17.1 MB (17083367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78197c8422a93eb658c23dff5d622f2d4f7524f184ddec1d7eda45e518c4354f`  
		Last Modified: Thu, 22 Jun 2023 00:50:03 GMT  
		Size: 3.4 KB (3370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4257c989a7f7bddb1161416c0d8ad56a66c61b37802ca313fea85633c9511567`  
		Last Modified: Thu, 22 Jun 2023 00:50:08 GMT  
		Size: 26.3 MB (26322991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.4` - linux; arm variant v7

```console
$ docker pull irssi@sha256:6b07201205f1936d606641ab462c40bcb52da3a8867b54d3c275685eeeb90ecb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45156187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0bc29edfecb98551b42621135d0e6a9a8df4e4eaf154137cf368ede533f1ceb`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:47 GMT
ADD file:319a24b7e30fc548f9dcf48ad6cee469e8bf7e89c67901cf3851e41e75693489 in / 
# Mon, 12 Jun 2023 23:58:47 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 17:16:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 17:16:56 GMT
ENV HOME=/home/user
# Tue, 13 Jun 2023 17:16:57 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 13 Jun 2023 17:16:57 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 17:16:57 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 13 Jun 2023 17:17:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 13 Jun 2023 17:17:44 GMT
WORKDIR /home/user
# Tue, 13 Jun 2023 17:17:45 GMT
USER user
# Tue, 13 Jun 2023 17:17:45 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b7c295cb849275e211d18b720d2349cc84c0038be1a362aca4765ceb3342043c`  
		Last Modified: Tue, 13 Jun 2023 00:04:24 GMT  
		Size: 26.6 MB (26578690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849490fbc07826e4ba5d7341723cfc86674072f6dea1fef7ee6c95a2d47f94ea`  
		Last Modified: Tue, 13 Jun 2023 17:18:12 GMT  
		Size: 14.4 MB (14385956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2ac9297b563c1cb4c92586f2e565024907221ef118e14789c48461ec982ce1`  
		Last Modified: Tue, 13 Jun 2023 17:18:08 GMT  
		Size: 4.2 KB (4190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0386945f81bf6c09429e43066eab30120446fd066a8e3d3450bf756774b9bad2`  
		Last Modified: Tue, 13 Jun 2023 17:18:09 GMT  
		Size: 4.2 MB (4187351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.4` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:266e75793b01d3790ac03073281aa85091694092f5da2a74804a57096c65e8cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74817663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2788ad4db80732ee28509ee691fff308c9dbf05d0f10c8264187cf487aea3e8`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:13 GMT
ADD file:f75c3fe22fec548b35a86a9a5802fdc97497f5d253cf630d65f13282169d3f3f in / 
# Mon, 12 Jun 2023 23:40:14 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 00:59:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 00:59:33 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:59:34 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:59:34 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:59:34 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:00:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 01:00:22 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:00:22 GMT
USER user
# Thu, 22 Jun 2023 01:00:23 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:95039a22a7cc3ae41d71f075e6e09e91e8da850fb5f80aba2f4a09f254520539`  
		Last Modified: Mon, 12 Jun 2023 23:44:08 GMT  
		Size: 29.2 MB (29152534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07791bb7d3b8da337cb7da387519554fbdb05d5d18a9015f7fd00751b524b4c6`  
		Last Modified: Thu, 22 Jun 2023 01:01:08 GMT  
		Size: 18.0 MB (18024086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b6d1cc205388e8478b3e53f9a0bd93b14aeac4315990aac3ad7b6d885c9ebe`  
		Last Modified: Thu, 22 Jun 2023 01:01:05 GMT  
		Size: 3.4 KB (3371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93207a63a416b94a1d0f7cf4c0794018f105ecd47ec4d24bc1ccf38d3269c5e`  
		Last Modified: Thu, 22 Jun 2023 01:01:09 GMT  
		Size: 27.6 MB (27637672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.4` - linux; 386

```console
$ docker pull irssi@sha256:0189dd47eeb861dff6aae81b129a397bf423c30f9d10edafdfe0f60eabbacecf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76490983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4845371b0a05c37bd8b6d4f60b11c9829ab2a362e65e8f85033cd78c89200eb8`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:20 GMT
ADD file:c7ecc5e2bed99e2cbca26f9f4247cd9bc399749556f4084e9357a9b00bb80530 in / 
# Mon, 12 Jun 2023 23:39:20 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 00:52:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 00:52:29 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:52:29 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:52:29 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:52:30 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:53:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 00:53:34 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:53:34 GMT
USER user
# Thu, 22 Jun 2023 00:53:34 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:82a41d17956dd7c8ebb39c9ce936fd26841bdbec98d0a185e3db8154b352edff`  
		Last Modified: Mon, 12 Jun 2023 23:46:21 GMT  
		Size: 30.1 MB (30140741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb531271cfa6ef221334ee9305eae83f672ba29341a2024e4520dbf81b6aa8f`  
		Last Modified: Thu, 22 Jun 2023 00:54:50 GMT  
		Size: 17.8 MB (17783961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9dc41e70935097ed849f2b07b7ad815928f38688133be530d26cacf20f94040`  
		Last Modified: Thu, 22 Jun 2023 00:54:44 GMT  
		Size: 3.4 KB (3367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6bf06950cb921c0ef76ebc588fa3c5a0b713fdfa45199468d58e625ada6e6a9`  
		Last Modified: Thu, 22 Jun 2023 00:54:51 GMT  
		Size: 28.6 MB (28562914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.4` - linux; mips64le

```console
$ docker pull irssi@sha256:fcad96467ecda441065d8062d7deffe2231cf5473de7f214932098cb7469b642
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.4 MB (48376311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:385baa614e97ceda4073810d1f47b470ba54a00c18ced3b057f8f8a21f9688cd`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Jun 2023 00:10:34 GMT
ADD file:4d5c7737e954f157e3d7ea47cc1814c46ec5c753a3d5d828ad9614969b572253 in / 
# Tue, 13 Jun 2023 00:10:38 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 14:58:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 14:58:45 GMT
ENV HOME=/home/user
# Tue, 13 Jun 2023 14:58:52 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 13 Jun 2023 14:58:55 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 14:58:58 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 13 Jun 2023 15:02:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 13 Jun 2023 15:02:56 GMT
WORKDIR /home/user
# Tue, 13 Jun 2023 15:02:59 GMT
USER user
# Tue, 13 Jun 2023 15:03:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:61bd6562a93acd0a3b327321e5465408e1d921b3ce1fb4fe353633330c3ede91`  
		Last Modified: Tue, 13 Jun 2023 00:23:53 GMT  
		Size: 29.6 MB (29634422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cd3adcf928d62813a219ad0c5c5c8015b780b4a6b4bb1ded47ae7f4e77036b`  
		Last Modified: Tue, 13 Jun 2023 15:03:43 GMT  
		Size: 14.4 MB (14421797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b360405355f5536c6ebb3ed5466c97a155165087081278fd8326b9c6a618e41c`  
		Last Modified: Tue, 13 Jun 2023 15:03:30 GMT  
		Size: 4.1 KB (4066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cf810f1b3cb9d35488e456c3cd9a56a60af589307368bb89a24c740fc94727`  
		Last Modified: Tue, 13 Jun 2023 15:03:33 GMT  
		Size: 4.3 MB (4316026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.4` - linux; ppc64le

```console
$ docker pull irssi@sha256:2c84f21d14766ef5faf43cbde7d5d21da7fbb7380ad823f06c9ffe0e6af8246f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55734024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39a07dc4dd7e0a6d1e413452909230f2fef5affd9aa6aad211c12e99096995bf`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:18:20 GMT
ADD file:b17eabe509462fa1a2e4c5421e877e3e4149085e3da07a421a66c7b06566c457 in / 
# Mon, 12 Jun 2023 23:18:22 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 08:47:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 08:47:07 GMT
ENV HOME=/home/user
# Tue, 13 Jun 2023 08:47:08 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 13 Jun 2023 08:47:08 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 08:47:08 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 13 Jun 2023 08:48:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 13 Jun 2023 08:48:26 GMT
WORKDIR /home/user
# Tue, 13 Jun 2023 08:48:26 GMT
USER user
# Tue, 13 Jun 2023 08:48:26 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2973ac0be4a80a6cecbb73370e92810a6f67a98e12e61b3044aa63a322dab03a`  
		Last Modified: Mon, 12 Jun 2023 23:25:03 GMT  
		Size: 35.3 MB (35290790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc5bd67d599f4e07b6f68f09a02d378eac43824b1a4cda56b24bc1c51d7c5ee`  
		Last Modified: Tue, 13 Jun 2023 08:48:45 GMT  
		Size: 15.8 MB (15756316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382a2c88702295eea22c668bccd54ea16eae65ffa15581e3bc67235a3c431e1b`  
		Last Modified: Tue, 13 Jun 2023 08:48:40 GMT  
		Size: 4.2 KB (4204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0199a0ffe4039f498bae34b531ebd5b5c6cdfa729e2233e3f5ca444d92962e`  
		Last Modified: Tue, 13 Jun 2023 08:48:41 GMT  
		Size: 4.7 MB (4682714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.4` - linux; s390x

```console
$ docker pull irssi@sha256:e400a68cd9ed507fdcb70211f4e758d4ab1abe4cbee7d36f701992e245230b72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50165469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20e837351a85c5d1ad2a54b291f29efa67fb03ba9dc35ea6662bdfc54510e130`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Jun 2023 04:30:13 GMT
ADD file:558e8c34e969d458ce6bf4207d9c0fe05d2e67d3457c1d5689666749e82ef2ab in / 
# Tue, 13 Jun 2023 04:30:14 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 20:32:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 20:32:02 GMT
ENV HOME=/home/user
# Tue, 13 Jun 2023 20:32:03 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 13 Jun 2023 20:32:03 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 20:32:03 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 13 Jun 2023 20:32:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 13 Jun 2023 20:32:36 GMT
WORKDIR /home/user
# Tue, 13 Jun 2023 20:32:36 GMT
USER user
# Tue, 13 Jun 2023 20:32:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6a752e2308c741009b6f5a88a8ea6764b96ebe7f544197912d8ef9a3ec8c8763`  
		Last Modified: Tue, 13 Jun 2023 04:34:49 GMT  
		Size: 29.7 MB (29652514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8801b0ffac290f142720ddaa925d39bcd3618f1c130f5a0497634f2efa2d16d7`  
		Last Modified: Tue, 13 Jun 2023 20:33:03 GMT  
		Size: 15.8 MB (15757517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11c128c370af2f7eac6f07cfb2de9128c708f7328806131725ec7b950c46718`  
		Last Modified: Tue, 13 Jun 2023 20:33:00 GMT  
		Size: 4.2 KB (4206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a967901fa87998ad3b8800f8eb690db5ce84ded9e821210ddeda55901e488136`  
		Last Modified: Tue, 13 Jun 2023 20:33:01 GMT  
		Size: 4.8 MB (4751232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4.4-alpine`

```console
$ docker pull irssi@sha256:554d2243f8a34d09fa6a15bf3304eba7030550de34bdfa653b497cd752f287ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `irssi:1.4.4-alpine` - linux; amd64

```console
$ docker pull irssi@sha256:df33162f0e50c52c10cbc95a42f1cb42a89705f6c83ffd7afd7cbec9443a8f8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18276585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f1af4d2f8b92472032db235e289cb9962144969514aff20659771cbd821edea`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 05:44:22 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 15 Jun 2023 05:44:22 GMT
ENV HOME=/home/user
# Thu, 15 Jun 2023 05:44:23 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 15 Jun 2023 05:44:23 GMT
ENV LANG=C.UTF-8
# Thu, 15 Jun 2023 05:44:23 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 15 Jun 2023 05:44:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 15 Jun 2023 05:44:42 GMT
WORKDIR /home/user
# Thu, 15 Jun 2023 05:44:42 GMT
USER user
# Thu, 15 Jun 2023 05:44:42 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16db5ccbd16300cfe3a0c9f34b1f542069afdc21f717b410fae474a86e85c61f`  
		Last Modified: Thu, 15 Jun 2023 05:44:58 GMT  
		Size: 9.7 MB (9730952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d12740aa5ddf98127801ec314bbae032c68524b23c82d8e1e35a4a1ee5343e7`  
		Last Modified: Thu, 15 Jun 2023 05:44:57 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87af7c88801970c57df2d16564333d097ce75a779c2f1d3efe0b0a4a6683bb96`  
		Last Modified: Thu, 15 Jun 2023 05:44:58 GMT  
		Size: 5.2 MB (5169637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.4-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:bb597fb239a0bd0ab274a3954a976e7a8bd496662eeb66a9ea540606d3d8de35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17261761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcd756feb5566228922fc9f7d0e3904d76d421749b294dd3a4643d1c7274f5c7`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 00:58:29 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 00:58:31 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:58:32 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:58:32 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:58:32 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:58:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 00:58:52 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:58:52 GMT
USER user
# Thu, 22 Jun 2023 00:58:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da40b022b0296d6aa3db9bdeeb4c2e75c57f15429e1b6af2b7027548372ca8b`  
		Last Modified: Thu, 22 Jun 2023 00:59:06 GMT  
		Size: 8.9 MB (8873416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b96767a0ecd78f7941b675b0af4b50cbecb0d5152dab111a5a441594ae6603`  
		Last Modified: Thu, 22 Jun 2023 00:59:03 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b501eb48ba4f12d62b8aea88131359fb8f39cb356fac11d0259549db8e77d8`  
		Last Modified: Thu, 22 Jun 2023 00:59:04 GMT  
		Size: 5.2 MB (5243707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.4-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:0b986f46e3300def597e471838a101aa352def1ae0b5f7f9f42c97dfbd11b83b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16562586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1d80e6235adbd2367ceeee4bb15c7b1e544f7a8e7fee19f67d6676360de3ebd`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:20 GMT
ADD file:5e92075a8d9a5898d661caf9c2be8a83fb25742251b4ebdc0c3d448a6dc58e4a in / 
# Wed, 14 Jun 2023 22:36:20 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 02:36:44 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 15 Jun 2023 02:36:44 GMT
ENV HOME=/home/user
# Thu, 15 Jun 2023 02:36:44 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 15 Jun 2023 02:36:45 GMT
ENV LANG=C.UTF-8
# Thu, 15 Jun 2023 02:36:45 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 15 Jun 2023 02:37:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 15 Jun 2023 02:37:02 GMT
WORKDIR /home/user
# Thu, 15 Jun 2023 02:37:03 GMT
USER user
# Thu, 15 Jun 2023 02:37:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f929d112168394cf1fbe294a86fbe5173dd92df4daac8cb09437b17dfc5df802`  
		Last Modified: Wed, 14 Jun 2023 22:37:01 GMT  
		Size: 2.9 MB (2868554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19564852001304e25333fcaab3ff6b786fa9b4fd00951a0de7f21590421663c0`  
		Last Modified: Thu, 15 Jun 2023 02:37:17 GMT  
		Size: 8.9 MB (8862221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e9266e16eb957d32cfe744ce2a3e2816dcf23785557fc6f7a16823a7ca1555`  
		Last Modified: Thu, 15 Jun 2023 02:37:14 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7eca2cc340821a140c2b4125d47f2e4ede76abc67c397ae6956bd9f4fcab86`  
		Last Modified: Thu, 15 Jun 2023 02:37:15 GMT  
		Size: 4.8 MB (4830526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.4-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:22b4938b5405529664397a96505be6a0a68216bc5e4dfd1a21212650e8767e73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18305951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f25464e2094646ab0d15f3b07d9f086640cf1fe1514bbde35957288c200e8ce`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:00:36 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:00:36 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:00:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:00:37 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:00:37 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:00:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:00:49 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:00:49 GMT
USER user
# Thu, 22 Jun 2023 01:00:49 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f2b2cec23be63b100192d36d65457ca5a26f7eea16d8e43ade7f2a71b93ae6`  
		Last Modified: Thu, 22 Jun 2023 01:01:31 GMT  
		Size: 9.7 MB (9666778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f96463864962e4e3fb7c345cfbcf0bec7c4339f64ac2033fdc156dad9ef918`  
		Last Modified: Thu, 22 Jun 2023 01:01:29 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795ebb03672fc4e273a972202f51cdb3b57a46535e2e027c0ec705d277af2c6e`  
		Last Modified: Thu, 22 Jun 2023 01:01:30 GMT  
		Size: 5.3 MB (5308640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.4-alpine` - linux; 386

```console
$ docker pull irssi@sha256:fddae328f37731c13d5bf17a3946f5cd460fa8a1877b2c4eefcd83b0dd7b543a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.5 MB (17544572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b0dbc2e51d5bf9a3b7bd5cd8d2f1e40fa598f375d7750df018959bc790c1eb5`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:22 GMT
ADD file:94bec00e2c0c7f47c81ec4355a29ca23a81b439797d037b1a5a455f36a25dab4 in / 
# Wed, 14 Jun 2023 22:33:22 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 00:53:45 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 00:53:45 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:53:46 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:53:46 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:53:46 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:54:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 00:54:19 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:54:19 GMT
USER user
# Thu, 22 Jun 2023 00:54:19 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b3f50075abd13aad1cb7d8c1427aa59d7fcac88f3690d3f9c3efdbec80fd0856`  
		Last Modified: Wed, 14 Jun 2023 22:33:48 GMT  
		Size: 3.2 MB (3233951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af01bb2560a285c7c3f49f618c91cddeddaae06f68de1d63318a35d08ddd335`  
		Last Modified: Thu, 22 Jun 2023 00:55:14 GMT  
		Size: 8.9 MB (8896518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400b4f5222097fceb2802b1b4c86df1e17d9c756033d35b1bbe932496bb67d55`  
		Last Modified: Thu, 22 Jun 2023 00:55:11 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4f83428ff29063f3abf5ecdcdade0657f4c35089baf0e5a17abf0284dde4e9`  
		Last Modified: Thu, 22 Jun 2023 00:55:13 GMT  
		Size: 5.4 MB (5412820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.4-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:edbac3bc69ae83f6a98c2aad44f19c80a109631cb22bd3fa7f0c500242c62faf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18484325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e94c29de632503a0823c113d66340f5bc25c0af8ef7e8bff75880144aa1c2f0`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:56 GMT
ADD file:1c25b0be52aae22767603d9404fb777e27c5dd1bcd627221aac7517ac1bce1e3 in / 
# Thu, 15 Jun 2023 00:39:57 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 02:12:08 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 15 Jun 2023 02:12:09 GMT
ENV HOME=/home/user
# Thu, 15 Jun 2023 02:12:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 15 Jun 2023 02:12:10 GMT
ENV LANG=C.UTF-8
# Thu, 15 Jun 2023 02:12:11 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 15 Jun 2023 02:12:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 15 Jun 2023 02:12:35 GMT
WORKDIR /home/user
# Thu, 15 Jun 2023 02:12:35 GMT
USER user
# Thu, 15 Jun 2023 02:12:35 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8436307590cda5ccded8a952bb1d66684f8700d07029527293dd695eac6fabc9`  
		Last Modified: Thu, 15 Jun 2023 00:40:39 GMT  
		Size: 3.4 MB (3389905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864111a1d0261ae544596480b7c499eeaf06cbbe1bc28790c10c4f7c970266cc`  
		Last Modified: Thu, 15 Jun 2023 02:12:54 GMT  
		Size: 9.8 MB (9819563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0ad87a302112668f0b2d1aa81c90fea805716562d224e498f265e8fbc40ed9`  
		Last Modified: Thu, 15 Jun 2023 02:12:51 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc50b4b50b6a0ce01de8d1e1e0c6e619054efd5e6110152ccb85f0d07e940776`  
		Last Modified: Thu, 15 Jun 2023 02:12:52 GMT  
		Size: 5.3 MB (5273573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.4-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:dbf8a6d36f09f574725d7cc6f6284a867c447eb0ca83eb1cc60b6f88c1cc23c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18463228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ac2b28856e91692db99f7d4ddc3224676a32846026bfd08d2ee7c118a4f36f9`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 15 Jun 2023 05:19:50 GMT
ADD file:8ad8a62cf274ba5a6568f68473359114136cb5c7704bfdfce6c38efef3081782 in / 
# Thu, 15 Jun 2023 05:19:51 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 07:28:51 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 16 Jun 2023 07:28:52 GMT
ENV HOME=/home/user
# Fri, 16 Jun 2023 07:28:53 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 16 Jun 2023 07:28:54 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 07:28:54 GMT
ENV IRSSI_VERSION=1.4.4
# Fri, 16 Jun 2023 07:29:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 16 Jun 2023 07:29:18 GMT
WORKDIR /home/user
# Fri, 16 Jun 2023 07:29:18 GMT
USER user
# Fri, 16 Jun 2023 07:29:18 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:eb857838eb854a669f87c5df4d936d905fb3129287a93ef485da9454c11d83cd`  
		Last Modified: Thu, 15 Jun 2023 05:30:48 GMT  
		Size: 3.2 MB (3174898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7aaa04f45ef848c1c2f0c93b981862cc5a7e75fa94769dc25fa6e6c90124bb7`  
		Last Modified: Fri, 16 Jun 2023 07:33:42 GMT  
		Size: 10.2 MB (10161596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5466510fd4b694305a4d3e46080afb8ed895bded299c98d7284313b5de554715`  
		Last Modified: Fri, 16 Jun 2023 07:33:40 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd30109dad033bd844acba0eb497941214a16aadd9b6dd7d208ec1550930aaca`  
		Last Modified: Fri, 16 Jun 2023 07:33:41 GMT  
		Size: 5.1 MB (5125449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4.4-alpine3.18`

```console
$ docker pull irssi@sha256:fe09fe14dfdb8a3d17a7a8d6c2c13e3f8ddfbff09793154369dd58443fc9ade1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `irssi:1.4.4-alpine3.18` - linux; arm variant v6

```console
$ docker pull irssi@sha256:bb597fb239a0bd0ab274a3954a976e7a8bd496662eeb66a9ea540606d3d8de35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17261761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcd756feb5566228922fc9f7d0e3904d76d421749b294dd3a4643d1c7274f5c7`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 00:58:29 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 00:58:31 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:58:32 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:58:32 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:58:32 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:58:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 00:58:52 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:58:52 GMT
USER user
# Thu, 22 Jun 2023 00:58:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da40b022b0296d6aa3db9bdeeb4c2e75c57f15429e1b6af2b7027548372ca8b`  
		Last Modified: Thu, 22 Jun 2023 00:59:06 GMT  
		Size: 8.9 MB (8873416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b96767a0ecd78f7941b675b0af4b50cbecb0d5152dab111a5a441594ae6603`  
		Last Modified: Thu, 22 Jun 2023 00:59:03 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b501eb48ba4f12d62b8aea88131359fb8f39cb356fac11d0259549db8e77d8`  
		Last Modified: Thu, 22 Jun 2023 00:59:04 GMT  
		Size: 5.2 MB (5243707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.4-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:22b4938b5405529664397a96505be6a0a68216bc5e4dfd1a21212650e8767e73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18305951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f25464e2094646ab0d15f3b07d9f086640cf1fe1514bbde35957288c200e8ce`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:00:36 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:00:36 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:00:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:00:37 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:00:37 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:00:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:00:49 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:00:49 GMT
USER user
# Thu, 22 Jun 2023 01:00:49 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f2b2cec23be63b100192d36d65457ca5a26f7eea16d8e43ade7f2a71b93ae6`  
		Last Modified: Thu, 22 Jun 2023 01:01:31 GMT  
		Size: 9.7 MB (9666778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f96463864962e4e3fb7c345cfbcf0bec7c4339f64ac2033fdc156dad9ef918`  
		Last Modified: Thu, 22 Jun 2023 01:01:29 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795ebb03672fc4e273a972202f51cdb3b57a46535e2e027c0ec705d277af2c6e`  
		Last Modified: Thu, 22 Jun 2023 01:01:30 GMT  
		Size: 5.3 MB (5308640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.4-alpine3.18` - linux; 386

```console
$ docker pull irssi@sha256:fddae328f37731c13d5bf17a3946f5cd460fa8a1877b2c4eefcd83b0dd7b543a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.5 MB (17544572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b0dbc2e51d5bf9a3b7bd5cd8d2f1e40fa598f375d7750df018959bc790c1eb5`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:22 GMT
ADD file:94bec00e2c0c7f47c81ec4355a29ca23a81b439797d037b1a5a455f36a25dab4 in / 
# Wed, 14 Jun 2023 22:33:22 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 00:53:45 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 00:53:45 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:53:46 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:53:46 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:53:46 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:54:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 00:54:19 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:54:19 GMT
USER user
# Thu, 22 Jun 2023 00:54:19 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b3f50075abd13aad1cb7d8c1427aa59d7fcac88f3690d3f9c3efdbec80fd0856`  
		Last Modified: Wed, 14 Jun 2023 22:33:48 GMT  
		Size: 3.2 MB (3233951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af01bb2560a285c7c3f49f618c91cddeddaae06f68de1d63318a35d08ddd335`  
		Last Modified: Thu, 22 Jun 2023 00:55:14 GMT  
		Size: 8.9 MB (8896518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400b4f5222097fceb2802b1b4c86df1e17d9c756033d35b1bbe932496bb67d55`  
		Last Modified: Thu, 22 Jun 2023 00:55:11 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4f83428ff29063f3abf5ecdcdade0657f4c35089baf0e5a17abf0284dde4e9`  
		Last Modified: Thu, 22 Jun 2023 00:55:13 GMT  
		Size: 5.4 MB (5412820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4.4-bookworm`

```console
$ docker pull irssi@sha256:3411a7a810e2ca8428f42cdd8111263294957fa5200720bd10e411922e759d74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386

### `irssi:1.4.4-bookworm` - linux; arm variant v5

```console
$ docker pull irssi@sha256:ec8e8fb46b70710ad03ffd0b0437286a0ec119c785edb791566d4534b21abf23
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70391870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb94ca655a3ecc2baf5113690a7bfa622f05cc2c362c9383c0a9bcfd736acf7d`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:48:31 GMT
ADD file:54a716f17b23e4fa49d1d5c0a7f63becc295873c116d19bb4753d34f1ca6affb in / 
# Mon, 12 Jun 2023 23:48:31 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 00:48:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 00:48:44 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:48:44 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:48:45 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:48:45 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:49:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 00:49:43 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:49:43 GMT
USER user
# Thu, 22 Jun 2023 00:49:43 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:70c60174b18d99741c33011138b5abf2f4d8eca0384521ccb43db3612078e36f`  
		Last Modified: Mon, 12 Jun 2023 23:51:26 GMT  
		Size: 27.0 MB (26982142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2fce51156cf8962c69bb6b4557b25c7c07264ce1ae06bcea0709030ed202ab`  
		Last Modified: Thu, 22 Jun 2023 00:50:07 GMT  
		Size: 17.1 MB (17083367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78197c8422a93eb658c23dff5d622f2d4f7524f184ddec1d7eda45e518c4354f`  
		Last Modified: Thu, 22 Jun 2023 00:50:03 GMT  
		Size: 3.4 KB (3370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4257c989a7f7bddb1161416c0d8ad56a66c61b37802ca313fea85633c9511567`  
		Last Modified: Thu, 22 Jun 2023 00:50:08 GMT  
		Size: 26.3 MB (26322991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.4-bookworm` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:266e75793b01d3790ac03073281aa85091694092f5da2a74804a57096c65e8cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74817663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2788ad4db80732ee28509ee691fff308c9dbf05d0f10c8264187cf487aea3e8`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:13 GMT
ADD file:f75c3fe22fec548b35a86a9a5802fdc97497f5d253cf630d65f13282169d3f3f in / 
# Mon, 12 Jun 2023 23:40:14 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 00:59:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 00:59:33 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:59:34 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:59:34 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:59:34 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:00:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 01:00:22 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:00:22 GMT
USER user
# Thu, 22 Jun 2023 01:00:23 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:95039a22a7cc3ae41d71f075e6e09e91e8da850fb5f80aba2f4a09f254520539`  
		Last Modified: Mon, 12 Jun 2023 23:44:08 GMT  
		Size: 29.2 MB (29152534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07791bb7d3b8da337cb7da387519554fbdb05d5d18a9015f7fd00751b524b4c6`  
		Last Modified: Thu, 22 Jun 2023 01:01:08 GMT  
		Size: 18.0 MB (18024086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b6d1cc205388e8478b3e53f9a0bd93b14aeac4315990aac3ad7b6d885c9ebe`  
		Last Modified: Thu, 22 Jun 2023 01:01:05 GMT  
		Size: 3.4 KB (3371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93207a63a416b94a1d0f7cf4c0794018f105ecd47ec4d24bc1ccf38d3269c5e`  
		Last Modified: Thu, 22 Jun 2023 01:01:09 GMT  
		Size: 27.6 MB (27637672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.4-bookworm` - linux; 386

```console
$ docker pull irssi@sha256:0189dd47eeb861dff6aae81b129a397bf423c30f9d10edafdfe0f60eabbacecf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76490983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4845371b0a05c37bd8b6d4f60b11c9829ab2a362e65e8f85033cd78c89200eb8`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:20 GMT
ADD file:c7ecc5e2bed99e2cbca26f9f4247cd9bc399749556f4084e9357a9b00bb80530 in / 
# Mon, 12 Jun 2023 23:39:20 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 00:52:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 00:52:29 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:52:29 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:52:29 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:52:30 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:53:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 00:53:34 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:53:34 GMT
USER user
# Thu, 22 Jun 2023 00:53:34 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:82a41d17956dd7c8ebb39c9ce936fd26841bdbec98d0a185e3db8154b352edff`  
		Last Modified: Mon, 12 Jun 2023 23:46:21 GMT  
		Size: 30.1 MB (30140741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb531271cfa6ef221334ee9305eae83f672ba29341a2024e4520dbf81b6aa8f`  
		Last Modified: Thu, 22 Jun 2023 00:54:50 GMT  
		Size: 17.8 MB (17783961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9dc41e70935097ed849f2b07b7ad815928f38688133be530d26cacf20f94040`  
		Last Modified: Thu, 22 Jun 2023 00:54:44 GMT  
		Size: 3.4 KB (3367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6bf06950cb921c0ef76ebc588fa3c5a0b713fdfa45199468d58e625ada6e6a9`  
		Last Modified: Thu, 22 Jun 2023 00:54:51 GMT  
		Size: 28.6 MB (28562914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:alpine`

```console
$ docker pull irssi@sha256:554d2243f8a34d09fa6a15bf3304eba7030550de34bdfa653b497cd752f287ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `irssi:alpine` - linux; amd64

```console
$ docker pull irssi@sha256:df33162f0e50c52c10cbc95a42f1cb42a89705f6c83ffd7afd7cbec9443a8f8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18276585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f1af4d2f8b92472032db235e289cb9962144969514aff20659771cbd821edea`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 05:44:22 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 15 Jun 2023 05:44:22 GMT
ENV HOME=/home/user
# Thu, 15 Jun 2023 05:44:23 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 15 Jun 2023 05:44:23 GMT
ENV LANG=C.UTF-8
# Thu, 15 Jun 2023 05:44:23 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 15 Jun 2023 05:44:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 15 Jun 2023 05:44:42 GMT
WORKDIR /home/user
# Thu, 15 Jun 2023 05:44:42 GMT
USER user
# Thu, 15 Jun 2023 05:44:42 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16db5ccbd16300cfe3a0c9f34b1f542069afdc21f717b410fae474a86e85c61f`  
		Last Modified: Thu, 15 Jun 2023 05:44:58 GMT  
		Size: 9.7 MB (9730952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d12740aa5ddf98127801ec314bbae032c68524b23c82d8e1e35a4a1ee5343e7`  
		Last Modified: Thu, 15 Jun 2023 05:44:57 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87af7c88801970c57df2d16564333d097ce75a779c2f1d3efe0b0a4a6683bb96`  
		Last Modified: Thu, 15 Jun 2023 05:44:58 GMT  
		Size: 5.2 MB (5169637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:bb597fb239a0bd0ab274a3954a976e7a8bd496662eeb66a9ea540606d3d8de35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17261761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcd756feb5566228922fc9f7d0e3904d76d421749b294dd3a4643d1c7274f5c7`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 00:58:29 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 00:58:31 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:58:32 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:58:32 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:58:32 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:58:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 00:58:52 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:58:52 GMT
USER user
# Thu, 22 Jun 2023 00:58:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da40b022b0296d6aa3db9bdeeb4c2e75c57f15429e1b6af2b7027548372ca8b`  
		Last Modified: Thu, 22 Jun 2023 00:59:06 GMT  
		Size: 8.9 MB (8873416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b96767a0ecd78f7941b675b0af4b50cbecb0d5152dab111a5a441594ae6603`  
		Last Modified: Thu, 22 Jun 2023 00:59:03 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b501eb48ba4f12d62b8aea88131359fb8f39cb356fac11d0259549db8e77d8`  
		Last Modified: Thu, 22 Jun 2023 00:59:04 GMT  
		Size: 5.2 MB (5243707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:0b986f46e3300def597e471838a101aa352def1ae0b5f7f9f42c97dfbd11b83b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16562586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1d80e6235adbd2367ceeee4bb15c7b1e544f7a8e7fee19f67d6676360de3ebd`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:20 GMT
ADD file:5e92075a8d9a5898d661caf9c2be8a83fb25742251b4ebdc0c3d448a6dc58e4a in / 
# Wed, 14 Jun 2023 22:36:20 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 02:36:44 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 15 Jun 2023 02:36:44 GMT
ENV HOME=/home/user
# Thu, 15 Jun 2023 02:36:44 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 15 Jun 2023 02:36:45 GMT
ENV LANG=C.UTF-8
# Thu, 15 Jun 2023 02:36:45 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 15 Jun 2023 02:37:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 15 Jun 2023 02:37:02 GMT
WORKDIR /home/user
# Thu, 15 Jun 2023 02:37:03 GMT
USER user
# Thu, 15 Jun 2023 02:37:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f929d112168394cf1fbe294a86fbe5173dd92df4daac8cb09437b17dfc5df802`  
		Last Modified: Wed, 14 Jun 2023 22:37:01 GMT  
		Size: 2.9 MB (2868554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19564852001304e25333fcaab3ff6b786fa9b4fd00951a0de7f21590421663c0`  
		Last Modified: Thu, 15 Jun 2023 02:37:17 GMT  
		Size: 8.9 MB (8862221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e9266e16eb957d32cfe744ce2a3e2816dcf23785557fc6f7a16823a7ca1555`  
		Last Modified: Thu, 15 Jun 2023 02:37:14 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7eca2cc340821a140c2b4125d47f2e4ede76abc67c397ae6956bd9f4fcab86`  
		Last Modified: Thu, 15 Jun 2023 02:37:15 GMT  
		Size: 4.8 MB (4830526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:22b4938b5405529664397a96505be6a0a68216bc5e4dfd1a21212650e8767e73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18305951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f25464e2094646ab0d15f3b07d9f086640cf1fe1514bbde35957288c200e8ce`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:00:36 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:00:36 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:00:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:00:37 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:00:37 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:00:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:00:49 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:00:49 GMT
USER user
# Thu, 22 Jun 2023 01:00:49 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f2b2cec23be63b100192d36d65457ca5a26f7eea16d8e43ade7f2a71b93ae6`  
		Last Modified: Thu, 22 Jun 2023 01:01:31 GMT  
		Size: 9.7 MB (9666778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f96463864962e4e3fb7c345cfbcf0bec7c4339f64ac2033fdc156dad9ef918`  
		Last Modified: Thu, 22 Jun 2023 01:01:29 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795ebb03672fc4e273a972202f51cdb3b57a46535e2e027c0ec705d277af2c6e`  
		Last Modified: Thu, 22 Jun 2023 01:01:30 GMT  
		Size: 5.3 MB (5308640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; 386

```console
$ docker pull irssi@sha256:fddae328f37731c13d5bf17a3946f5cd460fa8a1877b2c4eefcd83b0dd7b543a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.5 MB (17544572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b0dbc2e51d5bf9a3b7bd5cd8d2f1e40fa598f375d7750df018959bc790c1eb5`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:22 GMT
ADD file:94bec00e2c0c7f47c81ec4355a29ca23a81b439797d037b1a5a455f36a25dab4 in / 
# Wed, 14 Jun 2023 22:33:22 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 00:53:45 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 00:53:45 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:53:46 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:53:46 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:53:46 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:54:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 00:54:19 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:54:19 GMT
USER user
# Thu, 22 Jun 2023 00:54:19 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b3f50075abd13aad1cb7d8c1427aa59d7fcac88f3690d3f9c3efdbec80fd0856`  
		Last Modified: Wed, 14 Jun 2023 22:33:48 GMT  
		Size: 3.2 MB (3233951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af01bb2560a285c7c3f49f618c91cddeddaae06f68de1d63318a35d08ddd335`  
		Last Modified: Thu, 22 Jun 2023 00:55:14 GMT  
		Size: 8.9 MB (8896518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400b4f5222097fceb2802b1b4c86df1e17d9c756033d35b1bbe932496bb67d55`  
		Last Modified: Thu, 22 Jun 2023 00:55:11 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4f83428ff29063f3abf5ecdcdade0657f4c35089baf0e5a17abf0284dde4e9`  
		Last Modified: Thu, 22 Jun 2023 00:55:13 GMT  
		Size: 5.4 MB (5412820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:edbac3bc69ae83f6a98c2aad44f19c80a109631cb22bd3fa7f0c500242c62faf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18484325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e94c29de632503a0823c113d66340f5bc25c0af8ef7e8bff75880144aa1c2f0`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:56 GMT
ADD file:1c25b0be52aae22767603d9404fb777e27c5dd1bcd627221aac7517ac1bce1e3 in / 
# Thu, 15 Jun 2023 00:39:57 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 02:12:08 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 15 Jun 2023 02:12:09 GMT
ENV HOME=/home/user
# Thu, 15 Jun 2023 02:12:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 15 Jun 2023 02:12:10 GMT
ENV LANG=C.UTF-8
# Thu, 15 Jun 2023 02:12:11 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 15 Jun 2023 02:12:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 15 Jun 2023 02:12:35 GMT
WORKDIR /home/user
# Thu, 15 Jun 2023 02:12:35 GMT
USER user
# Thu, 15 Jun 2023 02:12:35 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8436307590cda5ccded8a952bb1d66684f8700d07029527293dd695eac6fabc9`  
		Last Modified: Thu, 15 Jun 2023 00:40:39 GMT  
		Size: 3.4 MB (3389905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864111a1d0261ae544596480b7c499eeaf06cbbe1bc28790c10c4f7c970266cc`  
		Last Modified: Thu, 15 Jun 2023 02:12:54 GMT  
		Size: 9.8 MB (9819563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0ad87a302112668f0b2d1aa81c90fea805716562d224e498f265e8fbc40ed9`  
		Last Modified: Thu, 15 Jun 2023 02:12:51 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc50b4b50b6a0ce01de8d1e1e0c6e619054efd5e6110152ccb85f0d07e940776`  
		Last Modified: Thu, 15 Jun 2023 02:12:52 GMT  
		Size: 5.3 MB (5273573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; s390x

```console
$ docker pull irssi@sha256:dbf8a6d36f09f574725d7cc6f6284a867c447eb0ca83eb1cc60b6f88c1cc23c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18463228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ac2b28856e91692db99f7d4ddc3224676a32846026bfd08d2ee7c118a4f36f9`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 15 Jun 2023 05:19:50 GMT
ADD file:8ad8a62cf274ba5a6568f68473359114136cb5c7704bfdfce6c38efef3081782 in / 
# Thu, 15 Jun 2023 05:19:51 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 07:28:51 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 16 Jun 2023 07:28:52 GMT
ENV HOME=/home/user
# Fri, 16 Jun 2023 07:28:53 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 16 Jun 2023 07:28:54 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 07:28:54 GMT
ENV IRSSI_VERSION=1.4.4
# Fri, 16 Jun 2023 07:29:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 16 Jun 2023 07:29:18 GMT
WORKDIR /home/user
# Fri, 16 Jun 2023 07:29:18 GMT
USER user
# Fri, 16 Jun 2023 07:29:18 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:eb857838eb854a669f87c5df4d936d905fb3129287a93ef485da9454c11d83cd`  
		Last Modified: Thu, 15 Jun 2023 05:30:48 GMT  
		Size: 3.2 MB (3174898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7aaa04f45ef848c1c2f0c93b981862cc5a7e75fa94769dc25fa6e6c90124bb7`  
		Last Modified: Fri, 16 Jun 2023 07:33:42 GMT  
		Size: 10.2 MB (10161596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5466510fd4b694305a4d3e46080afb8ed895bded299c98d7284313b5de554715`  
		Last Modified: Fri, 16 Jun 2023 07:33:40 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd30109dad033bd844acba0eb497941214a16aadd9b6dd7d208ec1550930aaca`  
		Last Modified: Fri, 16 Jun 2023 07:33:41 GMT  
		Size: 5.1 MB (5125449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:alpine3.18`

```console
$ docker pull irssi@sha256:fe09fe14dfdb8a3d17a7a8d6c2c13e3f8ddfbff09793154369dd58443fc9ade1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `irssi:alpine3.18` - linux; arm variant v6

```console
$ docker pull irssi@sha256:bb597fb239a0bd0ab274a3954a976e7a8bd496662eeb66a9ea540606d3d8de35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17261761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcd756feb5566228922fc9f7d0e3904d76d421749b294dd3a4643d1c7274f5c7`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 00:58:29 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 00:58:31 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:58:32 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:58:32 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:58:32 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:58:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 00:58:52 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:58:52 GMT
USER user
# Thu, 22 Jun 2023 00:58:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da40b022b0296d6aa3db9bdeeb4c2e75c57f15429e1b6af2b7027548372ca8b`  
		Last Modified: Thu, 22 Jun 2023 00:59:06 GMT  
		Size: 8.9 MB (8873416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b96767a0ecd78f7941b675b0af4b50cbecb0d5152dab111a5a441594ae6603`  
		Last Modified: Thu, 22 Jun 2023 00:59:03 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b501eb48ba4f12d62b8aea88131359fb8f39cb356fac11d0259549db8e77d8`  
		Last Modified: Thu, 22 Jun 2023 00:59:04 GMT  
		Size: 5.2 MB (5243707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine3.18` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:22b4938b5405529664397a96505be6a0a68216bc5e4dfd1a21212650e8767e73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18305951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f25464e2094646ab0d15f3b07d9f086640cf1fe1514bbde35957288c200e8ce`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:00:36 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:00:36 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:00:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:00:37 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:00:37 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:00:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:00:49 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:00:49 GMT
USER user
# Thu, 22 Jun 2023 01:00:49 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f2b2cec23be63b100192d36d65457ca5a26f7eea16d8e43ade7f2a71b93ae6`  
		Last Modified: Thu, 22 Jun 2023 01:01:31 GMT  
		Size: 9.7 MB (9666778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f96463864962e4e3fb7c345cfbcf0bec7c4339f64ac2033fdc156dad9ef918`  
		Last Modified: Thu, 22 Jun 2023 01:01:29 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795ebb03672fc4e273a972202f51cdb3b57a46535e2e027c0ec705d277af2c6e`  
		Last Modified: Thu, 22 Jun 2023 01:01:30 GMT  
		Size: 5.3 MB (5308640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine3.18` - linux; 386

```console
$ docker pull irssi@sha256:fddae328f37731c13d5bf17a3946f5cd460fa8a1877b2c4eefcd83b0dd7b543a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.5 MB (17544572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b0dbc2e51d5bf9a3b7bd5cd8d2f1e40fa598f375d7750df018959bc790c1eb5`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:22 GMT
ADD file:94bec00e2c0c7f47c81ec4355a29ca23a81b439797d037b1a5a455f36a25dab4 in / 
# Wed, 14 Jun 2023 22:33:22 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 00:53:45 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 00:53:45 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:53:46 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:53:46 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:53:46 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:54:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 00:54:19 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:54:19 GMT
USER user
# Thu, 22 Jun 2023 00:54:19 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b3f50075abd13aad1cb7d8c1427aa59d7fcac88f3690d3f9c3efdbec80fd0856`  
		Last Modified: Wed, 14 Jun 2023 22:33:48 GMT  
		Size: 3.2 MB (3233951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af01bb2560a285c7c3f49f618c91cddeddaae06f68de1d63318a35d08ddd335`  
		Last Modified: Thu, 22 Jun 2023 00:55:14 GMT  
		Size: 8.9 MB (8896518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400b4f5222097fceb2802b1b4c86df1e17d9c756033d35b1bbe932496bb67d55`  
		Last Modified: Thu, 22 Jun 2023 00:55:11 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4f83428ff29063f3abf5ecdcdade0657f4c35089baf0e5a17abf0284dde4e9`  
		Last Modified: Thu, 22 Jun 2023 00:55:13 GMT  
		Size: 5.4 MB (5412820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:bookworm`

```console
$ docker pull irssi@sha256:3411a7a810e2ca8428f42cdd8111263294957fa5200720bd10e411922e759d74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386

### `irssi:bookworm` - linux; arm variant v5

```console
$ docker pull irssi@sha256:ec8e8fb46b70710ad03ffd0b0437286a0ec119c785edb791566d4534b21abf23
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70391870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb94ca655a3ecc2baf5113690a7bfa622f05cc2c362c9383c0a9bcfd736acf7d`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:48:31 GMT
ADD file:54a716f17b23e4fa49d1d5c0a7f63becc295873c116d19bb4753d34f1ca6affb in / 
# Mon, 12 Jun 2023 23:48:31 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 00:48:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 00:48:44 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:48:44 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:48:45 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:48:45 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:49:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 00:49:43 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:49:43 GMT
USER user
# Thu, 22 Jun 2023 00:49:43 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:70c60174b18d99741c33011138b5abf2f4d8eca0384521ccb43db3612078e36f`  
		Last Modified: Mon, 12 Jun 2023 23:51:26 GMT  
		Size: 27.0 MB (26982142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2fce51156cf8962c69bb6b4557b25c7c07264ce1ae06bcea0709030ed202ab`  
		Last Modified: Thu, 22 Jun 2023 00:50:07 GMT  
		Size: 17.1 MB (17083367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78197c8422a93eb658c23dff5d622f2d4f7524f184ddec1d7eda45e518c4354f`  
		Last Modified: Thu, 22 Jun 2023 00:50:03 GMT  
		Size: 3.4 KB (3370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4257c989a7f7bddb1161416c0d8ad56a66c61b37802ca313fea85633c9511567`  
		Last Modified: Thu, 22 Jun 2023 00:50:08 GMT  
		Size: 26.3 MB (26322991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:bookworm` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:266e75793b01d3790ac03073281aa85091694092f5da2a74804a57096c65e8cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74817663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2788ad4db80732ee28509ee691fff308c9dbf05d0f10c8264187cf487aea3e8`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:13 GMT
ADD file:f75c3fe22fec548b35a86a9a5802fdc97497f5d253cf630d65f13282169d3f3f in / 
# Mon, 12 Jun 2023 23:40:14 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 00:59:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 00:59:33 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:59:34 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:59:34 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:59:34 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:00:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 01:00:22 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:00:22 GMT
USER user
# Thu, 22 Jun 2023 01:00:23 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:95039a22a7cc3ae41d71f075e6e09e91e8da850fb5f80aba2f4a09f254520539`  
		Last Modified: Mon, 12 Jun 2023 23:44:08 GMT  
		Size: 29.2 MB (29152534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07791bb7d3b8da337cb7da387519554fbdb05d5d18a9015f7fd00751b524b4c6`  
		Last Modified: Thu, 22 Jun 2023 01:01:08 GMT  
		Size: 18.0 MB (18024086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b6d1cc205388e8478b3e53f9a0bd93b14aeac4315990aac3ad7b6d885c9ebe`  
		Last Modified: Thu, 22 Jun 2023 01:01:05 GMT  
		Size: 3.4 KB (3371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93207a63a416b94a1d0f7cf4c0794018f105ecd47ec4d24bc1ccf38d3269c5e`  
		Last Modified: Thu, 22 Jun 2023 01:01:09 GMT  
		Size: 27.6 MB (27637672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:bookworm` - linux; 386

```console
$ docker pull irssi@sha256:0189dd47eeb861dff6aae81b129a397bf423c30f9d10edafdfe0f60eabbacecf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76490983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4845371b0a05c37bd8b6d4f60b11c9829ab2a362e65e8f85033cd78c89200eb8`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:20 GMT
ADD file:c7ecc5e2bed99e2cbca26f9f4247cd9bc399749556f4084e9357a9b00bb80530 in / 
# Mon, 12 Jun 2023 23:39:20 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 00:52:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 00:52:29 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:52:29 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:52:29 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:52:30 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:53:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 00:53:34 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:53:34 GMT
USER user
# Thu, 22 Jun 2023 00:53:34 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:82a41d17956dd7c8ebb39c9ce936fd26841bdbec98d0a185e3db8154b352edff`  
		Last Modified: Mon, 12 Jun 2023 23:46:21 GMT  
		Size: 30.1 MB (30140741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb531271cfa6ef221334ee9305eae83f672ba29341a2024e4520dbf81b6aa8f`  
		Last Modified: Thu, 22 Jun 2023 00:54:50 GMT  
		Size: 17.8 MB (17783961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9dc41e70935097ed849f2b07b7ad815928f38688133be530d26cacf20f94040`  
		Last Modified: Thu, 22 Jun 2023 00:54:44 GMT  
		Size: 3.4 KB (3367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6bf06950cb921c0ef76ebc588fa3c5a0b713fdfa45199468d58e625ada6e6a9`  
		Last Modified: Thu, 22 Jun 2023 00:54:51 GMT  
		Size: 28.6 MB (28562914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:latest`

```console
$ docker pull irssi@sha256:14481b64cd4dc6c9a9f26629b698c88886eff923a6e4f296516508939c73333c
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

### `irssi:latest` - linux; amd64

```console
$ docker pull irssi@sha256:1fda0af19ea9f808bab9108bb4b4528d6f36297ae226f7e17ebb2510aebbe39c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.4 MB (51353812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3240c2b2def4b35f616344709cdf6120faa7bdfb9973ce8e2100aa3905f16bfb`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:04:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:04:35 GMT
ENV HOME=/home/user
# Tue, 13 Jun 2023 07:04:36 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 13 Jun 2023 07:04:36 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 07:04:36 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 13 Jun 2023 07:05:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 13 Jun 2023 07:05:25 GMT
WORKDIR /home/user
# Tue, 13 Jun 2023 07:05:25 GMT
USER user
# Tue, 13 Jun 2023 07:05:25 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fa339e2e18ca8ee7894660c0b14e3f7ca734b3aeee8e2304b3e8c2563845ce`  
		Last Modified: Tue, 13 Jun 2023 07:05:49 GMT  
		Size: 15.5 MB (15457449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d616343ca0282e2d024ff05930f8eede4a1b1def9f5c9d7c706e5589fcfe44`  
		Last Modified: Tue, 13 Jun 2023 07:05:46 GMT  
		Size: 4.2 KB (4202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24ca3bf390591ce5506aa13625a97a7e80eb5fa1f34b25e33a9bdbfef4a1589`  
		Last Modified: Tue, 13 Jun 2023 07:05:47 GMT  
		Size: 4.5 MB (4474751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm variant v5

```console
$ docker pull irssi@sha256:ec8e8fb46b70710ad03ffd0b0437286a0ec119c785edb791566d4534b21abf23
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70391870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb94ca655a3ecc2baf5113690a7bfa622f05cc2c362c9383c0a9bcfd736acf7d`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:48:31 GMT
ADD file:54a716f17b23e4fa49d1d5c0a7f63becc295873c116d19bb4753d34f1ca6affb in / 
# Mon, 12 Jun 2023 23:48:31 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 00:48:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 00:48:44 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:48:44 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:48:45 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:48:45 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:49:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 00:49:43 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:49:43 GMT
USER user
# Thu, 22 Jun 2023 00:49:43 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:70c60174b18d99741c33011138b5abf2f4d8eca0384521ccb43db3612078e36f`  
		Last Modified: Mon, 12 Jun 2023 23:51:26 GMT  
		Size: 27.0 MB (26982142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2fce51156cf8962c69bb6b4557b25c7c07264ce1ae06bcea0709030ed202ab`  
		Last Modified: Thu, 22 Jun 2023 00:50:07 GMT  
		Size: 17.1 MB (17083367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78197c8422a93eb658c23dff5d622f2d4f7524f184ddec1d7eda45e518c4354f`  
		Last Modified: Thu, 22 Jun 2023 00:50:03 GMT  
		Size: 3.4 KB (3370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4257c989a7f7bddb1161416c0d8ad56a66c61b37802ca313fea85633c9511567`  
		Last Modified: Thu, 22 Jun 2023 00:50:08 GMT  
		Size: 26.3 MB (26322991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm variant v7

```console
$ docker pull irssi@sha256:6b07201205f1936d606641ab462c40bcb52da3a8867b54d3c275685eeeb90ecb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45156187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0bc29edfecb98551b42621135d0e6a9a8df4e4eaf154137cf368ede533f1ceb`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:47 GMT
ADD file:319a24b7e30fc548f9dcf48ad6cee469e8bf7e89c67901cf3851e41e75693489 in / 
# Mon, 12 Jun 2023 23:58:47 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 17:16:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 17:16:56 GMT
ENV HOME=/home/user
# Tue, 13 Jun 2023 17:16:57 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 13 Jun 2023 17:16:57 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 17:16:57 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 13 Jun 2023 17:17:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 13 Jun 2023 17:17:44 GMT
WORKDIR /home/user
# Tue, 13 Jun 2023 17:17:45 GMT
USER user
# Tue, 13 Jun 2023 17:17:45 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b7c295cb849275e211d18b720d2349cc84c0038be1a362aca4765ceb3342043c`  
		Last Modified: Tue, 13 Jun 2023 00:04:24 GMT  
		Size: 26.6 MB (26578690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849490fbc07826e4ba5d7341723cfc86674072f6dea1fef7ee6c95a2d47f94ea`  
		Last Modified: Tue, 13 Jun 2023 17:18:12 GMT  
		Size: 14.4 MB (14385956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2ac9297b563c1cb4c92586f2e565024907221ef118e14789c48461ec982ce1`  
		Last Modified: Tue, 13 Jun 2023 17:18:08 GMT  
		Size: 4.2 KB (4190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0386945f81bf6c09429e43066eab30120446fd066a8e3d3450bf756774b9bad2`  
		Last Modified: Tue, 13 Jun 2023 17:18:09 GMT  
		Size: 4.2 MB (4187351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:266e75793b01d3790ac03073281aa85091694092f5da2a74804a57096c65e8cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74817663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2788ad4db80732ee28509ee691fff308c9dbf05d0f10c8264187cf487aea3e8`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:13 GMT
ADD file:f75c3fe22fec548b35a86a9a5802fdc97497f5d253cf630d65f13282169d3f3f in / 
# Mon, 12 Jun 2023 23:40:14 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 00:59:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 00:59:33 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:59:34 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:59:34 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:59:34 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:00:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 01:00:22 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:00:22 GMT
USER user
# Thu, 22 Jun 2023 01:00:23 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:95039a22a7cc3ae41d71f075e6e09e91e8da850fb5f80aba2f4a09f254520539`  
		Last Modified: Mon, 12 Jun 2023 23:44:08 GMT  
		Size: 29.2 MB (29152534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07791bb7d3b8da337cb7da387519554fbdb05d5d18a9015f7fd00751b524b4c6`  
		Last Modified: Thu, 22 Jun 2023 01:01:08 GMT  
		Size: 18.0 MB (18024086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b6d1cc205388e8478b3e53f9a0bd93b14aeac4315990aac3ad7b6d885c9ebe`  
		Last Modified: Thu, 22 Jun 2023 01:01:05 GMT  
		Size: 3.4 KB (3371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93207a63a416b94a1d0f7cf4c0794018f105ecd47ec4d24bc1ccf38d3269c5e`  
		Last Modified: Thu, 22 Jun 2023 01:01:09 GMT  
		Size: 27.6 MB (27637672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; 386

```console
$ docker pull irssi@sha256:0189dd47eeb861dff6aae81b129a397bf423c30f9d10edafdfe0f60eabbacecf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76490983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4845371b0a05c37bd8b6d4f60b11c9829ab2a362e65e8f85033cd78c89200eb8`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:20 GMT
ADD file:c7ecc5e2bed99e2cbca26f9f4247cd9bc399749556f4084e9357a9b00bb80530 in / 
# Mon, 12 Jun 2023 23:39:20 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 00:52:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 00:52:29 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:52:29 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:52:29 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:52:30 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:53:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 00:53:34 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:53:34 GMT
USER user
# Thu, 22 Jun 2023 00:53:34 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:82a41d17956dd7c8ebb39c9ce936fd26841bdbec98d0a185e3db8154b352edff`  
		Last Modified: Mon, 12 Jun 2023 23:46:21 GMT  
		Size: 30.1 MB (30140741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb531271cfa6ef221334ee9305eae83f672ba29341a2024e4520dbf81b6aa8f`  
		Last Modified: Thu, 22 Jun 2023 00:54:50 GMT  
		Size: 17.8 MB (17783961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9dc41e70935097ed849f2b07b7ad815928f38688133be530d26cacf20f94040`  
		Last Modified: Thu, 22 Jun 2023 00:54:44 GMT  
		Size: 3.4 KB (3367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6bf06950cb921c0ef76ebc588fa3c5a0b713fdfa45199468d58e625ada6e6a9`  
		Last Modified: Thu, 22 Jun 2023 00:54:51 GMT  
		Size: 28.6 MB (28562914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; mips64le

```console
$ docker pull irssi@sha256:fcad96467ecda441065d8062d7deffe2231cf5473de7f214932098cb7469b642
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.4 MB (48376311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:385baa614e97ceda4073810d1f47b470ba54a00c18ced3b057f8f8a21f9688cd`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Jun 2023 00:10:34 GMT
ADD file:4d5c7737e954f157e3d7ea47cc1814c46ec5c753a3d5d828ad9614969b572253 in / 
# Tue, 13 Jun 2023 00:10:38 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 14:58:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 14:58:45 GMT
ENV HOME=/home/user
# Tue, 13 Jun 2023 14:58:52 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 13 Jun 2023 14:58:55 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 14:58:58 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 13 Jun 2023 15:02:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 13 Jun 2023 15:02:56 GMT
WORKDIR /home/user
# Tue, 13 Jun 2023 15:02:59 GMT
USER user
# Tue, 13 Jun 2023 15:03:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:61bd6562a93acd0a3b327321e5465408e1d921b3ce1fb4fe353633330c3ede91`  
		Last Modified: Tue, 13 Jun 2023 00:23:53 GMT  
		Size: 29.6 MB (29634422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cd3adcf928d62813a219ad0c5c5c8015b780b4a6b4bb1ded47ae7f4e77036b`  
		Last Modified: Tue, 13 Jun 2023 15:03:43 GMT  
		Size: 14.4 MB (14421797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b360405355f5536c6ebb3ed5466c97a155165087081278fd8326b9c6a618e41c`  
		Last Modified: Tue, 13 Jun 2023 15:03:30 GMT  
		Size: 4.1 KB (4066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cf810f1b3cb9d35488e456c3cd9a56a60af589307368bb89a24c740fc94727`  
		Last Modified: Tue, 13 Jun 2023 15:03:33 GMT  
		Size: 4.3 MB (4316026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; ppc64le

```console
$ docker pull irssi@sha256:2c84f21d14766ef5faf43cbde7d5d21da7fbb7380ad823f06c9ffe0e6af8246f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55734024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39a07dc4dd7e0a6d1e413452909230f2fef5affd9aa6aad211c12e99096995bf`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:18:20 GMT
ADD file:b17eabe509462fa1a2e4c5421e877e3e4149085e3da07a421a66c7b06566c457 in / 
# Mon, 12 Jun 2023 23:18:22 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 08:47:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 08:47:07 GMT
ENV HOME=/home/user
# Tue, 13 Jun 2023 08:47:08 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 13 Jun 2023 08:47:08 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 08:47:08 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 13 Jun 2023 08:48:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 13 Jun 2023 08:48:26 GMT
WORKDIR /home/user
# Tue, 13 Jun 2023 08:48:26 GMT
USER user
# Tue, 13 Jun 2023 08:48:26 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2973ac0be4a80a6cecbb73370e92810a6f67a98e12e61b3044aa63a322dab03a`  
		Last Modified: Mon, 12 Jun 2023 23:25:03 GMT  
		Size: 35.3 MB (35290790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc5bd67d599f4e07b6f68f09a02d378eac43824b1a4cda56b24bc1c51d7c5ee`  
		Last Modified: Tue, 13 Jun 2023 08:48:45 GMT  
		Size: 15.8 MB (15756316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382a2c88702295eea22c668bccd54ea16eae65ffa15581e3bc67235a3c431e1b`  
		Last Modified: Tue, 13 Jun 2023 08:48:40 GMT  
		Size: 4.2 KB (4204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0199a0ffe4039f498bae34b531ebd5b5c6cdfa729e2233e3f5ca444d92962e`  
		Last Modified: Tue, 13 Jun 2023 08:48:41 GMT  
		Size: 4.7 MB (4682714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; s390x

```console
$ docker pull irssi@sha256:e400a68cd9ed507fdcb70211f4e758d4ab1abe4cbee7d36f701992e245230b72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50165469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20e837351a85c5d1ad2a54b291f29efa67fb03ba9dc35ea6662bdfc54510e130`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Jun 2023 04:30:13 GMT
ADD file:558e8c34e969d458ce6bf4207d9c0fe05d2e67d3457c1d5689666749e82ef2ab in / 
# Tue, 13 Jun 2023 04:30:14 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 20:32:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 20:32:02 GMT
ENV HOME=/home/user
# Tue, 13 Jun 2023 20:32:03 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 13 Jun 2023 20:32:03 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 20:32:03 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 13 Jun 2023 20:32:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 13 Jun 2023 20:32:36 GMT
WORKDIR /home/user
# Tue, 13 Jun 2023 20:32:36 GMT
USER user
# Tue, 13 Jun 2023 20:32:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6a752e2308c741009b6f5a88a8ea6764b96ebe7f544197912d8ef9a3ec8c8763`  
		Last Modified: Tue, 13 Jun 2023 04:34:49 GMT  
		Size: 29.7 MB (29652514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8801b0ffac290f142720ddaa925d39bcd3618f1c130f5a0497634f2efa2d16d7`  
		Last Modified: Tue, 13 Jun 2023 20:33:03 GMT  
		Size: 15.8 MB (15757517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11c128c370af2f7eac6f07cfb2de9128c708f7328806131725ec7b950c46718`  
		Last Modified: Tue, 13 Jun 2023 20:33:00 GMT  
		Size: 4.2 KB (4206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a967901fa87998ad3b8800f8eb690db5ce84ded9e821210ddeda55901e488136`  
		Last Modified: Tue, 13 Jun 2023 20:33:01 GMT  
		Size: 4.8 MB (4751232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
