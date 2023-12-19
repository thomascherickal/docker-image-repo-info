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
-	[`irssi:1.4.5`](#irssi145)
-	[`irssi:1.4.5-alpine`](#irssi145-alpine)
-	[`irssi:1.4.5-alpine3.18`](#irssi145-alpine318)
-	[`irssi:1.4.5-bookworm`](#irssi145-bookworm)
-	[`irssi:alpine`](#irssialpine)
-	[`irssi:alpine3.18`](#irssialpine318)
-	[`irssi:bookworm`](#irssibookworm)
-	[`irssi:latest`](#irssilatest)

## `irssi:1`

```console
$ docker pull irssi@sha256:9bbaebbdef964fd13f87622f887af48afe01d1ef67ec7152da0e993626f8c347
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
$ docker pull irssi@sha256:75930e1081143e5ac73cc553fd47dd75a236c5587dad0b13ed4f593d5efec999
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76071375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e784ee8f60cc445019f7f2a00f02a16d18715a384904180fa30548888ea9a9e2`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:27 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Tue, 19 Dec 2023 01:20:28 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:11:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:11:41 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 08:11:42 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 08:11:42 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 08:11:42 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 08:12:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 08:12:22 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 08:12:22 GMT
USER user
# Tue, 19 Dec 2023 08:12:22 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f576257a7efd8fa2eab590d15da13ff3e351ddd5f66e1f18853950d0a847940`  
		Last Modified: Tue, 19 Dec 2023 08:12:41 GMT  
		Size: 18.3 MB (18263304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8709b16d66af9e29995cd9f313628ac25626d9a3b9f14337a489a0b53dede1`  
		Last Modified: Tue, 19 Dec 2023 08:12:37 GMT  
		Size: 3.4 KB (3376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4721ae122aaf701fec4c0ab60bcd8186c440f5439303bb23fc19aaa3cc886e`  
		Last Modified: Tue, 19 Dec 2023 08:12:42 GMT  
		Size: 28.7 MB (28678732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm variant v5

```console
$ docker pull irssi@sha256:54f4b6e9ea13a0ad57b6507d166cc7d60f705a1f0fb2c8b1a21ccf71be8b4817
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70247719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f71b3c5dc081e54b3f8c57c1d3be303a0147a4ac5656f26d0698b3673bce8f5`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:55:22 GMT
ADD file:9503ab966c9dd707eeccc7c2f633bccc94c199f8714ec4ff2c8b54dde3dbabf9 in / 
# Tue, 19 Dec 2023 01:55:22 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 05:37:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 05:37:07 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 05:37:08 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 05:37:08 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 05:37:08 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 05:37:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 05:37:54 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 05:37:54 GMT
USER user
# Tue, 19 Dec 2023 05:37:54 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1ae9a2844c8c70942d2220553689b62e841cc706d77284fbfedbd770080fd699`  
		Last Modified: Tue, 19 Dec 2023 01:58:33 GMT  
		Size: 26.9 MB (26885440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8c63a38cdf609e2fc7e6adb6d2a2ddee5ee1e185ced4c5667fa93153ddaca4`  
		Last Modified: Tue, 19 Dec 2023 05:38:20 GMT  
		Size: 17.0 MB (17034518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5baba07d2ad153cdc8a55cf44e4e53c2d24eccd878b7c013029ad93e53dad92b`  
		Last Modified: Tue, 19 Dec 2023 05:38:15 GMT  
		Size: 3.4 KB (3382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b675c572666d53e7aaee086d9f3a892e01803b6b84ab820ee1100726092e714`  
		Last Modified: Tue, 19 Dec 2023 05:38:21 GMT  
		Size: 26.3 MB (26324379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm variant v7

```console
$ docker pull irssi@sha256:b58087a750d2ecb0db246fa2b83fce92398c136af518ddc7bcae63e75637be1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66568253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0abed9b964bf4864c88c0c97e43a26973a28db129f9679f226eba9307dd515ec`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 02:07:50 GMT
ADD file:aef112919e7924ad6da32181b1df5099cd692680c104118da3a24cd4dfe55a1d in / 
# Tue, 19 Dec 2023 02:07:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:25:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:25:13 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 08:25:13 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 08:25:14 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 08:25:14 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 08:25:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 08:25:50 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 08:25:50 GMT
USER user
# Tue, 19 Dec 2023 08:25:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:65ab19615c01a3b542f77fadb3bd27872b6a20cba3e9269fb951de36d8fa6805`  
		Last Modified: Tue, 19 Dec 2023 02:11:52 GMT  
		Size: 24.7 MB (24718157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34312fc906c50709273b2bfc296cbc5e618081aab636bea0270e632aa1250a58`  
		Last Modified: Tue, 19 Dec 2023 08:26:13 GMT  
		Size: 16.6 MB (16626329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ae59c8630536591ee4c9f224e24066f5ea55d87cd4d710f4758493e40f4d90`  
		Last Modified: Tue, 19 Dec 2023 08:26:07 GMT  
		Size: 3.4 KB (3375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653d387ba5d23d5a1d3207409abeb6f1857445f450f723a518d7f30d8305a612`  
		Last Modified: Tue, 19 Dec 2023 08:26:13 GMT  
		Size: 25.2 MB (25220392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:ca5674fca34098dff53db48ae2b739f5bf5deef41b342fe154e13d37c4ca22d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74826194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e84ec8b67ce32fad14adb38e81b191c731737445551e607aadf4cb648de22d25`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:11 GMT
ADD file:262fd7bf0bc26e5d2a229fba52626e22b8a93beac29733acfc60e716c26e689d in / 
# Tue, 19 Dec 2023 01:41:11 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:35:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 07:35:16 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 07:35:17 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 07:35:17 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 07:35:17 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 07:35:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 07:35:50 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 07:35:50 GMT
USER user
# Tue, 19 Dec 2023 07:35:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:24e221e92a36ab5b0075dd156b4f2ff095532a9b0927946cf6070bb1bea208b8`  
		Last Modified: Tue, 19 Dec 2023 01:44:38 GMT  
		Size: 29.2 MB (29157269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3b65976afca6b69a78f82bba0cfd53e915de68b3497418795c0fe90dde04d6`  
		Last Modified: Tue, 19 Dec 2023 07:36:07 GMT  
		Size: 18.0 MB (18025714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1487d5e5dd099dea8c8f5cfa983386ef698d0b7ba74af27991d128c2eb77509a`  
		Last Modified: Tue, 19 Dec 2023 07:36:04 GMT  
		Size: 3.4 KB (3375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027137ab6d543546e67a802c5b15757aae71ceb8e7be44d4ab7e3701b466102e`  
		Last Modified: Tue, 19 Dec 2023 07:36:07 GMT  
		Size: 27.6 MB (27639836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; 386

```console
$ docker pull irssi@sha256:f4a77a97b8bd86a99d34d5fb0a8786e1a8f95758005b4ba99deb96a2b24d589a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76522898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e29421276ec13208c270be47f6eb04f62363c92fbf673bd983a1aa520e2fedc`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Nov 2023 04:39:53 GMT
ADD file:930e1b9d85b6927c4d3046f7c75de2f3bfc6ec29100c314d0ab2b780ea30e962 in / 
# Tue, 21 Nov 2023 04:39:53 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:18:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:18:00 GMT
ENV HOME=/home/user
# Tue, 21 Nov 2023 09:18:01 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Nov 2023 09:18:01 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 09:18:01 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 21 Nov 2023 09:18:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Nov 2023 09:18:58 GMT
WORKDIR /home/user
# Tue, 21 Nov 2023 09:18:58 GMT
USER user
# Tue, 21 Nov 2023 09:18:58 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c0734eabce8885d8904dbd11b77aa97c2d2b04bc8e2af9e89d47c4bda590dd8e`  
		Last Modified: Tue, 21 Nov 2023 04:44:34 GMT  
		Size: 30.2 MB (30164109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd0a88ad6c1f45a640f6b1e3509a00f0489ea5e7317905ff14b60fca6f24086`  
		Last Modified: Tue, 21 Nov 2023 09:19:21 GMT  
		Size: 17.8 MB (17789102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e785a0b684a75cef890d58447965564ea0ab287ad9b7fa38d00a4e9cfe5de7`  
		Last Modified: Tue, 21 Nov 2023 09:19:15 GMT  
		Size: 3.4 KB (3372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397cc87253be0de402ae3c1da69d2224514616b57b478236526d9f020d3b6ad6`  
		Last Modified: Tue, 21 Nov 2023 09:19:23 GMT  
		Size: 28.6 MB (28566315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; mips64le

```console
$ docker pull irssi@sha256:9c4985936b28f111411e9b54fe41acdb3b06222c5e22b4783ac53322ddf57794
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73894339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:370cd0afda43f756d5b75c9726905baa31206388d01ef49a763d8e033950a631`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 16:36:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 16:36:50 GMT
ENV HOME=/home/user
# Tue, 21 Nov 2023 16:36:56 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Nov 2023 16:37:00 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 16:37:03 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 21 Nov 2023 16:40:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Nov 2023 16:40:50 GMT
WORKDIR /home/user
# Tue, 21 Nov 2023 16:40:54 GMT
USER user
# Tue, 21 Nov 2023 16:40:58 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a2caa6a91dd837ff86958b77bc3534a4003f0cc9611e0b48c76361698bc605`  
		Last Modified: Tue, 21 Nov 2023 16:41:28 GMT  
		Size: 16.7 MB (16741807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6247f0644042c0a753bfe2ff1b7c28d43caaf3330ed88b170167a6fe8a0d35`  
		Last Modified: Tue, 21 Nov 2023 16:41:12 GMT  
		Size: 3.3 KB (3296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb6fda2e80956777959da56923ad2794e7af2f4a510933d7b85d0bf680feb2b`  
		Last Modified: Tue, 21 Nov 2023 16:41:33 GMT  
		Size: 28.0 MB (28007252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; ppc64le

```console
$ docker pull irssi@sha256:3f4f99d9914f9e72defad07d78d6e7c12b79184ab4aba83db835de09bc8f75bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82095380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60c6389f9028a4f1e86f03b0bf0bfed6a3d3f45126cdde79535e1136d045b8ff`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 08:14:12 GMT
ENV HOME=/home/user
# Tue, 21 Nov 2023 08:14:13 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Nov 2023 08:14:14 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 08:14:14 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 21 Nov 2023 08:15:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Nov 2023 08:15:10 GMT
WORKDIR /home/user
# Tue, 21 Nov 2023 08:15:10 GMT
USER user
# Tue, 21 Nov 2023 08:15:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990142f84c0c74390b332399beb412942fc74379d8c617ede6f2b0f701fd5f63`  
		Last Modified: Tue, 21 Nov 2023 08:15:42 GMT  
		Size: 18.8 MB (18764965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145cb9bddb869ec0a23e4a981ffb5078fc4852784403e1f0cb05eb86e52276cf`  
		Last Modified: Tue, 21 Nov 2023 08:15:38 GMT  
		Size: 3.4 KB (3371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c79418540c78592e0ce7f96f5df8dd9db310edd58c6f158ba3389cd2290920`  
		Last Modified: Tue, 21 Nov 2023 08:15:43 GMT  
		Size: 30.2 MB (30185437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; s390x

```console
$ docker pull irssi@sha256:19d5614ead4badb612e08ba2483418078e52144432cb38d8393c825b31ebe63f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72933796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2a7878077011d582ad7647ec003c06a9ed22ba2e0b5280c344ed18a0f1b8c40`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:42:37 GMT
ADD file:f06f12fa5a93afc3a79ac4371d24b0a471a5a1818cf34c1d90004c8f410914b9 in / 
# Tue, 19 Dec 2023 01:42:39 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:29:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:29:37 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 08:29:37 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 08:29:37 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 08:29:38 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 08:30:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 08:30:17 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 08:30:17 GMT
USER user
# Tue, 19 Dec 2023 08:30:17 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:bc6b1888979d3ceb063da848b2034e980e2c2613642159c1e856550b79aa620c`  
		Last Modified: Tue, 19 Dec 2023 01:47:38 GMT  
		Size: 27.5 MB (27491874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d93a78aafed26613c2aa62cc6ab76d24cde8ba422049c8c4aff454d7e8b6f0`  
		Last Modified: Tue, 19 Dec 2023 08:30:47 GMT  
		Size: 18.2 MB (18210518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506c18d3ee4758db831ecc9a8b1ea9f2562b6972d70a1fb2cd98603a28811f5f`  
		Last Modified: Tue, 19 Dec 2023 08:30:44 GMT  
		Size: 3.4 KB (3376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64e09b7ab558543c54810d6e85b3a3fab5eb5ae4fec9423bfdc282f16c15bcc`  
		Last Modified: Tue, 19 Dec 2023 08:30:48 GMT  
		Size: 27.2 MB (27228028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1-alpine`

```console
$ docker pull irssi@sha256:b404269638b505c913a02979a9f253a8e9e904e585c6bb3011b7afbc06908340
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
$ docker pull irssi@sha256:bac3d5c9afaa50fa166d54e4f8a6b82f8519d5f41f60e154925a961f498c67cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18451924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b18b85f03e9dae76ebfd3a15dd2180db03fc5728ce1980f8ae072a7fbbdc15f3`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:28:32 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 05:28:32 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 05:28:33 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 05:28:33 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 05:28:33 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 05:28:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 05:28:52 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 05:28:52 GMT
USER user
# Fri, 01 Dec 2023 05:28:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2253ad6954238459aeb69a5812221ad8d0a9cf6473cb145f43ec969741e3f7c`  
		Last Modified: Fri, 01 Dec 2023 05:29:12 GMT  
		Size: 9.6 MB (9645529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027edf83d9867e80bd5e7041a3da7cbbd50027d7f1e9018f1174b20ca77aea09`  
		Last Modified: Fri, 01 Dec 2023 05:29:10 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf95bf3609411e5c119950c792cabbb3c647eb384dafacbce7a70a601533c44`  
		Last Modified: Fri, 01 Dec 2023 05:29:11 GMT  
		Size: 5.4 MB (5402689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:51601527f7062d912289288c810b48a9d00b3922cef2a58b04787672ff913d07
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17271200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3301b14e65fec26ab44af0807bbcd5ac7cfb9230618a31edcde72367a83b21da`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 01:09:50 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 01:09:50 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 01:09:51 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 01:09:51 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 01:09:51 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 01:10:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 01:10:08 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 01:10:08 GMT
USER user
# Fri, 01 Dec 2023 01:10:08 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0389ed6f59ff0e95c3c6c4566157405d8b3bb4b5a827a5a1fd24edf934393c`  
		Last Modified: Fri, 01 Dec 2023 01:10:22 GMT  
		Size: 8.9 MB (8880077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4039f2bf7cbc0fa8f9a5e8a20f20a5035b388d7a42a95d9d6f0a3a58446eed`  
		Last Modified: Fri, 01 Dec 2023 01:10:19 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184e5e97ecd8a9cf4081a03b9f6a83022561e425f3294a0d09c345420c858123`  
		Last Modified: Fri, 01 Dec 2023 01:10:21 GMT  
		Size: 5.2 MB (5242968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:6ff758c9743e67bc2781d127b56339f483bfbb1251763d398a335d3a95ae9744
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16630768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ba268037301e762641733ac31d7ab82c0538e3658cc00205b6ca74c23bb5332`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:41:57 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 08:41:57 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 08:41:57 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 08:41:57 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 08:41:57 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 08:42:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 08:42:12 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 08:42:12 GMT
USER user
# Fri, 01 Dec 2023 08:42:12 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505553baa092b1ac5dc9c2a961456e9728d5bfe4d15f5a93644f58c1a0c75d14`  
		Last Modified: Fri, 01 Dec 2023 08:42:31 GMT  
		Size: 8.7 MB (8721323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc7d412e24534e4f0eebe098495c5878f5184667c4180f22eb8b50bff5d78cf`  
		Last Modified: Fri, 01 Dec 2023 08:42:29 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d25439b4dd4f4d92fd4be67af55606656fd511d66a1f63715b0dd6d2eeab5b`  
		Last Modified: Fri, 01 Dec 2023 08:42:30 GMT  
		Size: 5.0 MB (5007154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:444032f59c771f9f8ecc9f1374f55b4f94016696d5e58a0931e61ae604748369
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18316372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a03091ab8bcbd9db84ead2d162e748af025192b4ebc302c6a42bd11b034e026b`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:37:23 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 09:37:23 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 09:37:24 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 09:37:24 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 09:37:24 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 09:37:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 09:37:36 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 09:37:36 GMT
USER user
# Fri, 01 Dec 2023 09:37:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408050d673681e97a81fefc3f0d62dc535741ab369d0f890dfd492fea579fc73`  
		Last Modified: Fri, 01 Dec 2023 09:37:55 GMT  
		Size: 9.7 MB (9672911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b351c7a82544307a7a55c5daa20a529cd389facb270805cea95b2040f8b864`  
		Last Modified: Fri, 01 Dec 2023 09:37:53 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad688b9a5733e1a4e2feaddf0a4ae2395f72b5d718efc48685befed72ad2d440`  
		Last Modified: Fri, 01 Dec 2023 09:37:54 GMT  
		Size: 5.3 MB (5309143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; 386

```console
$ docker pull irssi@sha256:cb5e5eb3ce2e5c8a080af15a2414c7078412473c44bfe7c15196f957fdd3931b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17557886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e422f2a321a825ce4ac90dad135af83afa3ee86cd59d10d667a313c1b2ec35a7`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 01 Dec 2023 02:03:44 GMT
ADD file:92902088cd15ed8f5dca2f7fc6570fb4e4824fac8b09e091c88e96bbd0ca814b in / 
# Fri, 01 Dec 2023 02:03:44 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:02:03 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 09:02:03 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 09:02:03 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 09:02:04 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 09:02:04 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 09:02:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 09:02:38 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 09:02:38 GMT
USER user
# Fri, 01 Dec 2023 09:02:38 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4966a8bd129b0a6adf93dc295a8fbe8f665d3194a684a5ce199c1c3596dbf3d9`  
		Last Modified: Fri, 01 Dec 2023 02:04:18 GMT  
		Size: 3.2 MB (3238831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194fdb04cb3e17be198ec377fafeb3f5716927ef33b40df425a942b4f3f7e50`  
		Last Modified: Fri, 01 Dec 2023 09:03:00 GMT  
		Size: 8.9 MB (8904478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc41f0a0151cdbeed763c916854e38b017669921f3a79d0554e77543dcb09acb`  
		Last Modified: Fri, 01 Dec 2023 09:02:57 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5a928454e9d9ee194c2842f26954fc39b31e235b0de4f542f9acc45af1737f`  
		Last Modified: Fri, 01 Dec 2023 09:02:58 GMT  
		Size: 5.4 MB (5413293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:e3eba53096e51def6997bdc72c51cf88f0019645321ee59bdd20b49b4236a617
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18717510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:890fc74fc94817011bde8d06e7b449e6407828cbbff17d07e69de027ad3d77f4`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:04:09 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 05:04:12 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 05:04:20 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 05:04:21 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 05:04:21 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 05:04:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 05:04:59 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 05:05:00 GMT
USER user
# Fri, 01 Dec 2023 05:05:02 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5afc2e0a7e24376eade504bc1d0aee8fa44d1b246f3121de324296a57c0ff25d`  
		Last Modified: Fri, 01 Dec 2023 05:05:36 GMT  
		Size: 9.7 MB (9736497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04ef92e3c12ead968e636f09604f92720ce8750a3a7f114277c2ef6764219b6`  
		Last Modified: Fri, 01 Dec 2023 05:05:34 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce0f8ba67064d14f75d9e13652d96ba1e13e489eff4d5617c0e503e25106009`  
		Last Modified: Fri, 01 Dec 2023 05:05:35 GMT  
		Size: 5.6 MB (5631406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:2f5751ebf70dce38c6c48dc4a4e7f72bdae9824a0da9b3b95c277c755139592c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18708403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30063d82b1a526f916c2be961b95561fad91acd4ecfa2942d616740be6105a20`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:13:12 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 08:13:13 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 08:13:13 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 08:13:14 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 08:13:14 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 08:13:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 08:13:35 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 08:13:35 GMT
USER user
# Fri, 01 Dec 2023 08:13:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c64be9d9a3f22087e689a8436399a73b9fb1f76114c8c4b5740080a6d178c9b`  
		Last Modified: Fri, 01 Dec 2023 08:14:02 GMT  
		Size: 10.1 MB (10083001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403430efaca857233fd4cc970775e8fb9b2bfa68899058f8046852bf2a25be16`  
		Last Modified: Fri, 01 Dec 2023 08:13:59 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9630989fe7d8e6fcb8d2886d67968d8118d654dbaa9787a1e4050fe5d293e589`  
		Last Modified: Fri, 01 Dec 2023 08:14:00 GMT  
		Size: 5.4 MB (5406662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1-alpine3.18`

```console
$ docker pull irssi@sha256:b404269638b505c913a02979a9f253a8e9e904e585c6bb3011b7afbc06908340
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

### `irssi:1-alpine3.18` - linux; amd64

```console
$ docker pull irssi@sha256:bac3d5c9afaa50fa166d54e4f8a6b82f8519d5f41f60e154925a961f498c67cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18451924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b18b85f03e9dae76ebfd3a15dd2180db03fc5728ce1980f8ae072a7fbbdc15f3`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:28:32 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 05:28:32 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 05:28:33 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 05:28:33 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 05:28:33 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 05:28:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 05:28:52 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 05:28:52 GMT
USER user
# Fri, 01 Dec 2023 05:28:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2253ad6954238459aeb69a5812221ad8d0a9cf6473cb145f43ec969741e3f7c`  
		Last Modified: Fri, 01 Dec 2023 05:29:12 GMT  
		Size: 9.6 MB (9645529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027edf83d9867e80bd5e7041a3da7cbbd50027d7f1e9018f1174b20ca77aea09`  
		Last Modified: Fri, 01 Dec 2023 05:29:10 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf95bf3609411e5c119950c792cabbb3c647eb384dafacbce7a70a601533c44`  
		Last Modified: Fri, 01 Dec 2023 05:29:11 GMT  
		Size: 5.4 MB (5402689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine3.18` - linux; arm variant v6

```console
$ docker pull irssi@sha256:51601527f7062d912289288c810b48a9d00b3922cef2a58b04787672ff913d07
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17271200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3301b14e65fec26ab44af0807bbcd5ac7cfb9230618a31edcde72367a83b21da`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 01:09:50 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 01:09:50 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 01:09:51 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 01:09:51 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 01:09:51 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 01:10:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 01:10:08 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 01:10:08 GMT
USER user
# Fri, 01 Dec 2023 01:10:08 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0389ed6f59ff0e95c3c6c4566157405d8b3bb4b5a827a5a1fd24edf934393c`  
		Last Modified: Fri, 01 Dec 2023 01:10:22 GMT  
		Size: 8.9 MB (8880077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4039f2bf7cbc0fa8f9a5e8a20f20a5035b388d7a42a95d9d6f0a3a58446eed`  
		Last Modified: Fri, 01 Dec 2023 01:10:19 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184e5e97ecd8a9cf4081a03b9f6a83022561e425f3294a0d09c345420c858123`  
		Last Modified: Fri, 01 Dec 2023 01:10:21 GMT  
		Size: 5.2 MB (5242968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine3.18` - linux; arm variant v7

```console
$ docker pull irssi@sha256:6ff758c9743e67bc2781d127b56339f483bfbb1251763d398a335d3a95ae9744
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16630768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ba268037301e762641733ac31d7ab82c0538e3658cc00205b6ca74c23bb5332`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:41:57 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 08:41:57 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 08:41:57 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 08:41:57 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 08:41:57 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 08:42:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 08:42:12 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 08:42:12 GMT
USER user
# Fri, 01 Dec 2023 08:42:12 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505553baa092b1ac5dc9c2a961456e9728d5bfe4d15f5a93644f58c1a0c75d14`  
		Last Modified: Fri, 01 Dec 2023 08:42:31 GMT  
		Size: 8.7 MB (8721323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc7d412e24534e4f0eebe098495c5878f5184667c4180f22eb8b50bff5d78cf`  
		Last Modified: Fri, 01 Dec 2023 08:42:29 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d25439b4dd4f4d92fd4be67af55606656fd511d66a1f63715b0dd6d2eeab5b`  
		Last Modified: Fri, 01 Dec 2023 08:42:30 GMT  
		Size: 5.0 MB (5007154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:444032f59c771f9f8ecc9f1374f55b4f94016696d5e58a0931e61ae604748369
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18316372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a03091ab8bcbd9db84ead2d162e748af025192b4ebc302c6a42bd11b034e026b`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:37:23 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 09:37:23 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 09:37:24 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 09:37:24 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 09:37:24 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 09:37:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 09:37:36 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 09:37:36 GMT
USER user
# Fri, 01 Dec 2023 09:37:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408050d673681e97a81fefc3f0d62dc535741ab369d0f890dfd492fea579fc73`  
		Last Modified: Fri, 01 Dec 2023 09:37:55 GMT  
		Size: 9.7 MB (9672911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b351c7a82544307a7a55c5daa20a529cd389facb270805cea95b2040f8b864`  
		Last Modified: Fri, 01 Dec 2023 09:37:53 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad688b9a5733e1a4e2feaddf0a4ae2395f72b5d718efc48685befed72ad2d440`  
		Last Modified: Fri, 01 Dec 2023 09:37:54 GMT  
		Size: 5.3 MB (5309143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine3.18` - linux; 386

```console
$ docker pull irssi@sha256:cb5e5eb3ce2e5c8a080af15a2414c7078412473c44bfe7c15196f957fdd3931b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17557886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e422f2a321a825ce4ac90dad135af83afa3ee86cd59d10d667a313c1b2ec35a7`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 01 Dec 2023 02:03:44 GMT
ADD file:92902088cd15ed8f5dca2f7fc6570fb4e4824fac8b09e091c88e96bbd0ca814b in / 
# Fri, 01 Dec 2023 02:03:44 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:02:03 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 09:02:03 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 09:02:03 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 09:02:04 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 09:02:04 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 09:02:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 09:02:38 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 09:02:38 GMT
USER user
# Fri, 01 Dec 2023 09:02:38 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4966a8bd129b0a6adf93dc295a8fbe8f665d3194a684a5ce199c1c3596dbf3d9`  
		Last Modified: Fri, 01 Dec 2023 02:04:18 GMT  
		Size: 3.2 MB (3238831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194fdb04cb3e17be198ec377fafeb3f5716927ef33b40df425a942b4f3f7e50`  
		Last Modified: Fri, 01 Dec 2023 09:03:00 GMT  
		Size: 8.9 MB (8904478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc41f0a0151cdbeed763c916854e38b017669921f3a79d0554e77543dcb09acb`  
		Last Modified: Fri, 01 Dec 2023 09:02:57 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5a928454e9d9ee194c2842f26954fc39b31e235b0de4f542f9acc45af1737f`  
		Last Modified: Fri, 01 Dec 2023 09:02:58 GMT  
		Size: 5.4 MB (5413293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine3.18` - linux; ppc64le

```console
$ docker pull irssi@sha256:e3eba53096e51def6997bdc72c51cf88f0019645321ee59bdd20b49b4236a617
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18717510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:890fc74fc94817011bde8d06e7b449e6407828cbbff17d07e69de027ad3d77f4`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:04:09 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 05:04:12 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 05:04:20 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 05:04:21 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 05:04:21 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 05:04:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 05:04:59 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 05:05:00 GMT
USER user
# Fri, 01 Dec 2023 05:05:02 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5afc2e0a7e24376eade504bc1d0aee8fa44d1b246f3121de324296a57c0ff25d`  
		Last Modified: Fri, 01 Dec 2023 05:05:36 GMT  
		Size: 9.7 MB (9736497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04ef92e3c12ead968e636f09604f92720ce8750a3a7f114277c2ef6764219b6`  
		Last Modified: Fri, 01 Dec 2023 05:05:34 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce0f8ba67064d14f75d9e13652d96ba1e13e489eff4d5617c0e503e25106009`  
		Last Modified: Fri, 01 Dec 2023 05:05:35 GMT  
		Size: 5.6 MB (5631406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine3.18` - linux; s390x

```console
$ docker pull irssi@sha256:2f5751ebf70dce38c6c48dc4a4e7f72bdae9824a0da9b3b95c277c755139592c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18708403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30063d82b1a526f916c2be961b95561fad91acd4ecfa2942d616740be6105a20`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:13:12 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 08:13:13 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 08:13:13 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 08:13:14 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 08:13:14 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 08:13:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 08:13:35 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 08:13:35 GMT
USER user
# Fri, 01 Dec 2023 08:13:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c64be9d9a3f22087e689a8436399a73b9fb1f76114c8c4b5740080a6d178c9b`  
		Last Modified: Fri, 01 Dec 2023 08:14:02 GMT  
		Size: 10.1 MB (10083001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403430efaca857233fd4cc970775e8fb9b2bfa68899058f8046852bf2a25be16`  
		Last Modified: Fri, 01 Dec 2023 08:13:59 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9630989fe7d8e6fcb8d2886d67968d8118d654dbaa9787a1e4050fe5d293e589`  
		Last Modified: Fri, 01 Dec 2023 08:14:00 GMT  
		Size: 5.4 MB (5406662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1-bookworm`

```console
$ docker pull irssi@sha256:9bbaebbdef964fd13f87622f887af48afe01d1ef67ec7152da0e993626f8c347
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

### `irssi:1-bookworm` - linux; amd64

```console
$ docker pull irssi@sha256:75930e1081143e5ac73cc553fd47dd75a236c5587dad0b13ed4f593d5efec999
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76071375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e784ee8f60cc445019f7f2a00f02a16d18715a384904180fa30548888ea9a9e2`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:27 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Tue, 19 Dec 2023 01:20:28 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:11:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:11:41 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 08:11:42 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 08:11:42 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 08:11:42 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 08:12:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 08:12:22 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 08:12:22 GMT
USER user
# Tue, 19 Dec 2023 08:12:22 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f576257a7efd8fa2eab590d15da13ff3e351ddd5f66e1f18853950d0a847940`  
		Last Modified: Tue, 19 Dec 2023 08:12:41 GMT  
		Size: 18.3 MB (18263304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8709b16d66af9e29995cd9f313628ac25626d9a3b9f14337a489a0b53dede1`  
		Last Modified: Tue, 19 Dec 2023 08:12:37 GMT  
		Size: 3.4 KB (3376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4721ae122aaf701fec4c0ab60bcd8186c440f5439303bb23fc19aaa3cc886e`  
		Last Modified: Tue, 19 Dec 2023 08:12:42 GMT  
		Size: 28.7 MB (28678732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-bookworm` - linux; arm variant v5

```console
$ docker pull irssi@sha256:54f4b6e9ea13a0ad57b6507d166cc7d60f705a1f0fb2c8b1a21ccf71be8b4817
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70247719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f71b3c5dc081e54b3f8c57c1d3be303a0147a4ac5656f26d0698b3673bce8f5`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:55:22 GMT
ADD file:9503ab966c9dd707eeccc7c2f633bccc94c199f8714ec4ff2c8b54dde3dbabf9 in / 
# Tue, 19 Dec 2023 01:55:22 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 05:37:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 05:37:07 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 05:37:08 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 05:37:08 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 05:37:08 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 05:37:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 05:37:54 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 05:37:54 GMT
USER user
# Tue, 19 Dec 2023 05:37:54 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1ae9a2844c8c70942d2220553689b62e841cc706d77284fbfedbd770080fd699`  
		Last Modified: Tue, 19 Dec 2023 01:58:33 GMT  
		Size: 26.9 MB (26885440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8c63a38cdf609e2fc7e6adb6d2a2ddee5ee1e185ced4c5667fa93153ddaca4`  
		Last Modified: Tue, 19 Dec 2023 05:38:20 GMT  
		Size: 17.0 MB (17034518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5baba07d2ad153cdc8a55cf44e4e53c2d24eccd878b7c013029ad93e53dad92b`  
		Last Modified: Tue, 19 Dec 2023 05:38:15 GMT  
		Size: 3.4 KB (3382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b675c572666d53e7aaee086d9f3a892e01803b6b84ab820ee1100726092e714`  
		Last Modified: Tue, 19 Dec 2023 05:38:21 GMT  
		Size: 26.3 MB (26324379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-bookworm` - linux; arm variant v7

```console
$ docker pull irssi@sha256:b58087a750d2ecb0db246fa2b83fce92398c136af518ddc7bcae63e75637be1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66568253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0abed9b964bf4864c88c0c97e43a26973a28db129f9679f226eba9307dd515ec`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 02:07:50 GMT
ADD file:aef112919e7924ad6da32181b1df5099cd692680c104118da3a24cd4dfe55a1d in / 
# Tue, 19 Dec 2023 02:07:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:25:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:25:13 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 08:25:13 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 08:25:14 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 08:25:14 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 08:25:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 08:25:50 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 08:25:50 GMT
USER user
# Tue, 19 Dec 2023 08:25:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:65ab19615c01a3b542f77fadb3bd27872b6a20cba3e9269fb951de36d8fa6805`  
		Last Modified: Tue, 19 Dec 2023 02:11:52 GMT  
		Size: 24.7 MB (24718157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34312fc906c50709273b2bfc296cbc5e618081aab636bea0270e632aa1250a58`  
		Last Modified: Tue, 19 Dec 2023 08:26:13 GMT  
		Size: 16.6 MB (16626329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ae59c8630536591ee4c9f224e24066f5ea55d87cd4d710f4758493e40f4d90`  
		Last Modified: Tue, 19 Dec 2023 08:26:07 GMT  
		Size: 3.4 KB (3375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653d387ba5d23d5a1d3207409abeb6f1857445f450f723a518d7f30d8305a612`  
		Last Modified: Tue, 19 Dec 2023 08:26:13 GMT  
		Size: 25.2 MB (25220392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-bookworm` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:ca5674fca34098dff53db48ae2b739f5bf5deef41b342fe154e13d37c4ca22d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74826194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e84ec8b67ce32fad14adb38e81b191c731737445551e607aadf4cb648de22d25`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:11 GMT
ADD file:262fd7bf0bc26e5d2a229fba52626e22b8a93beac29733acfc60e716c26e689d in / 
# Tue, 19 Dec 2023 01:41:11 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:35:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 07:35:16 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 07:35:17 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 07:35:17 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 07:35:17 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 07:35:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 07:35:50 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 07:35:50 GMT
USER user
# Tue, 19 Dec 2023 07:35:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:24e221e92a36ab5b0075dd156b4f2ff095532a9b0927946cf6070bb1bea208b8`  
		Last Modified: Tue, 19 Dec 2023 01:44:38 GMT  
		Size: 29.2 MB (29157269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3b65976afca6b69a78f82bba0cfd53e915de68b3497418795c0fe90dde04d6`  
		Last Modified: Tue, 19 Dec 2023 07:36:07 GMT  
		Size: 18.0 MB (18025714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1487d5e5dd099dea8c8f5cfa983386ef698d0b7ba74af27991d128c2eb77509a`  
		Last Modified: Tue, 19 Dec 2023 07:36:04 GMT  
		Size: 3.4 KB (3375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027137ab6d543546e67a802c5b15757aae71ceb8e7be44d4ab7e3701b466102e`  
		Last Modified: Tue, 19 Dec 2023 07:36:07 GMT  
		Size: 27.6 MB (27639836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-bookworm` - linux; 386

```console
$ docker pull irssi@sha256:f4a77a97b8bd86a99d34d5fb0a8786e1a8f95758005b4ba99deb96a2b24d589a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76522898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e29421276ec13208c270be47f6eb04f62363c92fbf673bd983a1aa520e2fedc`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Nov 2023 04:39:53 GMT
ADD file:930e1b9d85b6927c4d3046f7c75de2f3bfc6ec29100c314d0ab2b780ea30e962 in / 
# Tue, 21 Nov 2023 04:39:53 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:18:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:18:00 GMT
ENV HOME=/home/user
# Tue, 21 Nov 2023 09:18:01 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Nov 2023 09:18:01 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 09:18:01 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 21 Nov 2023 09:18:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Nov 2023 09:18:58 GMT
WORKDIR /home/user
# Tue, 21 Nov 2023 09:18:58 GMT
USER user
# Tue, 21 Nov 2023 09:18:58 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c0734eabce8885d8904dbd11b77aa97c2d2b04bc8e2af9e89d47c4bda590dd8e`  
		Last Modified: Tue, 21 Nov 2023 04:44:34 GMT  
		Size: 30.2 MB (30164109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd0a88ad6c1f45a640f6b1e3509a00f0489ea5e7317905ff14b60fca6f24086`  
		Last Modified: Tue, 21 Nov 2023 09:19:21 GMT  
		Size: 17.8 MB (17789102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e785a0b684a75cef890d58447965564ea0ab287ad9b7fa38d00a4e9cfe5de7`  
		Last Modified: Tue, 21 Nov 2023 09:19:15 GMT  
		Size: 3.4 KB (3372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397cc87253be0de402ae3c1da69d2224514616b57b478236526d9f020d3b6ad6`  
		Last Modified: Tue, 21 Nov 2023 09:19:23 GMT  
		Size: 28.6 MB (28566315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-bookworm` - linux; mips64le

```console
$ docker pull irssi@sha256:9c4985936b28f111411e9b54fe41acdb3b06222c5e22b4783ac53322ddf57794
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73894339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:370cd0afda43f756d5b75c9726905baa31206388d01ef49a763d8e033950a631`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 16:36:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 16:36:50 GMT
ENV HOME=/home/user
# Tue, 21 Nov 2023 16:36:56 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Nov 2023 16:37:00 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 16:37:03 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 21 Nov 2023 16:40:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Nov 2023 16:40:50 GMT
WORKDIR /home/user
# Tue, 21 Nov 2023 16:40:54 GMT
USER user
# Tue, 21 Nov 2023 16:40:58 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a2caa6a91dd837ff86958b77bc3534a4003f0cc9611e0b48c76361698bc605`  
		Last Modified: Tue, 21 Nov 2023 16:41:28 GMT  
		Size: 16.7 MB (16741807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6247f0644042c0a753bfe2ff1b7c28d43caaf3330ed88b170167a6fe8a0d35`  
		Last Modified: Tue, 21 Nov 2023 16:41:12 GMT  
		Size: 3.3 KB (3296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb6fda2e80956777959da56923ad2794e7af2f4a510933d7b85d0bf680feb2b`  
		Last Modified: Tue, 21 Nov 2023 16:41:33 GMT  
		Size: 28.0 MB (28007252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-bookworm` - linux; ppc64le

```console
$ docker pull irssi@sha256:3f4f99d9914f9e72defad07d78d6e7c12b79184ab4aba83db835de09bc8f75bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82095380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60c6389f9028a4f1e86f03b0bf0bfed6a3d3f45126cdde79535e1136d045b8ff`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 08:14:12 GMT
ENV HOME=/home/user
# Tue, 21 Nov 2023 08:14:13 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Nov 2023 08:14:14 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 08:14:14 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 21 Nov 2023 08:15:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Nov 2023 08:15:10 GMT
WORKDIR /home/user
# Tue, 21 Nov 2023 08:15:10 GMT
USER user
# Tue, 21 Nov 2023 08:15:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990142f84c0c74390b332399beb412942fc74379d8c617ede6f2b0f701fd5f63`  
		Last Modified: Tue, 21 Nov 2023 08:15:42 GMT  
		Size: 18.8 MB (18764965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145cb9bddb869ec0a23e4a981ffb5078fc4852784403e1f0cb05eb86e52276cf`  
		Last Modified: Tue, 21 Nov 2023 08:15:38 GMT  
		Size: 3.4 KB (3371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c79418540c78592e0ce7f96f5df8dd9db310edd58c6f158ba3389cd2290920`  
		Last Modified: Tue, 21 Nov 2023 08:15:43 GMT  
		Size: 30.2 MB (30185437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-bookworm` - linux; s390x

```console
$ docker pull irssi@sha256:19d5614ead4badb612e08ba2483418078e52144432cb38d8393c825b31ebe63f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72933796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2a7878077011d582ad7647ec003c06a9ed22ba2e0b5280c344ed18a0f1b8c40`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:42:37 GMT
ADD file:f06f12fa5a93afc3a79ac4371d24b0a471a5a1818cf34c1d90004c8f410914b9 in / 
# Tue, 19 Dec 2023 01:42:39 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:29:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:29:37 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 08:29:37 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 08:29:37 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 08:29:38 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 08:30:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 08:30:17 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 08:30:17 GMT
USER user
# Tue, 19 Dec 2023 08:30:17 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:bc6b1888979d3ceb063da848b2034e980e2c2613642159c1e856550b79aa620c`  
		Last Modified: Tue, 19 Dec 2023 01:47:38 GMT  
		Size: 27.5 MB (27491874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d93a78aafed26613c2aa62cc6ab76d24cde8ba422049c8c4aff454d7e8b6f0`  
		Last Modified: Tue, 19 Dec 2023 08:30:47 GMT  
		Size: 18.2 MB (18210518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506c18d3ee4758db831ecc9a8b1ea9f2562b6972d70a1fb2cd98603a28811f5f`  
		Last Modified: Tue, 19 Dec 2023 08:30:44 GMT  
		Size: 3.4 KB (3376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64e09b7ab558543c54810d6e85b3a3fab5eb5ae4fec9423bfdc282f16c15bcc`  
		Last Modified: Tue, 19 Dec 2023 08:30:48 GMT  
		Size: 27.2 MB (27228028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4`

```console
$ docker pull irssi@sha256:9bbaebbdef964fd13f87622f887af48afe01d1ef67ec7152da0e993626f8c347
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
$ docker pull irssi@sha256:75930e1081143e5ac73cc553fd47dd75a236c5587dad0b13ed4f593d5efec999
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76071375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e784ee8f60cc445019f7f2a00f02a16d18715a384904180fa30548888ea9a9e2`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:27 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Tue, 19 Dec 2023 01:20:28 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:11:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:11:41 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 08:11:42 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 08:11:42 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 08:11:42 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 08:12:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 08:12:22 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 08:12:22 GMT
USER user
# Tue, 19 Dec 2023 08:12:22 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f576257a7efd8fa2eab590d15da13ff3e351ddd5f66e1f18853950d0a847940`  
		Last Modified: Tue, 19 Dec 2023 08:12:41 GMT  
		Size: 18.3 MB (18263304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8709b16d66af9e29995cd9f313628ac25626d9a3b9f14337a489a0b53dede1`  
		Last Modified: Tue, 19 Dec 2023 08:12:37 GMT  
		Size: 3.4 KB (3376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4721ae122aaf701fec4c0ab60bcd8186c440f5439303bb23fc19aaa3cc886e`  
		Last Modified: Tue, 19 Dec 2023 08:12:42 GMT  
		Size: 28.7 MB (28678732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; arm variant v5

```console
$ docker pull irssi@sha256:54f4b6e9ea13a0ad57b6507d166cc7d60f705a1f0fb2c8b1a21ccf71be8b4817
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70247719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f71b3c5dc081e54b3f8c57c1d3be303a0147a4ac5656f26d0698b3673bce8f5`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:55:22 GMT
ADD file:9503ab966c9dd707eeccc7c2f633bccc94c199f8714ec4ff2c8b54dde3dbabf9 in / 
# Tue, 19 Dec 2023 01:55:22 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 05:37:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 05:37:07 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 05:37:08 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 05:37:08 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 05:37:08 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 05:37:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 05:37:54 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 05:37:54 GMT
USER user
# Tue, 19 Dec 2023 05:37:54 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1ae9a2844c8c70942d2220553689b62e841cc706d77284fbfedbd770080fd699`  
		Last Modified: Tue, 19 Dec 2023 01:58:33 GMT  
		Size: 26.9 MB (26885440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8c63a38cdf609e2fc7e6adb6d2a2ddee5ee1e185ced4c5667fa93153ddaca4`  
		Last Modified: Tue, 19 Dec 2023 05:38:20 GMT  
		Size: 17.0 MB (17034518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5baba07d2ad153cdc8a55cf44e4e53c2d24eccd878b7c013029ad93e53dad92b`  
		Last Modified: Tue, 19 Dec 2023 05:38:15 GMT  
		Size: 3.4 KB (3382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b675c572666d53e7aaee086d9f3a892e01803b6b84ab820ee1100726092e714`  
		Last Modified: Tue, 19 Dec 2023 05:38:21 GMT  
		Size: 26.3 MB (26324379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; arm variant v7

```console
$ docker pull irssi@sha256:b58087a750d2ecb0db246fa2b83fce92398c136af518ddc7bcae63e75637be1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66568253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0abed9b964bf4864c88c0c97e43a26973a28db129f9679f226eba9307dd515ec`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 02:07:50 GMT
ADD file:aef112919e7924ad6da32181b1df5099cd692680c104118da3a24cd4dfe55a1d in / 
# Tue, 19 Dec 2023 02:07:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:25:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:25:13 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 08:25:13 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 08:25:14 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 08:25:14 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 08:25:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 08:25:50 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 08:25:50 GMT
USER user
# Tue, 19 Dec 2023 08:25:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:65ab19615c01a3b542f77fadb3bd27872b6a20cba3e9269fb951de36d8fa6805`  
		Last Modified: Tue, 19 Dec 2023 02:11:52 GMT  
		Size: 24.7 MB (24718157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34312fc906c50709273b2bfc296cbc5e618081aab636bea0270e632aa1250a58`  
		Last Modified: Tue, 19 Dec 2023 08:26:13 GMT  
		Size: 16.6 MB (16626329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ae59c8630536591ee4c9f224e24066f5ea55d87cd4d710f4758493e40f4d90`  
		Last Modified: Tue, 19 Dec 2023 08:26:07 GMT  
		Size: 3.4 KB (3375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653d387ba5d23d5a1d3207409abeb6f1857445f450f723a518d7f30d8305a612`  
		Last Modified: Tue, 19 Dec 2023 08:26:13 GMT  
		Size: 25.2 MB (25220392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:ca5674fca34098dff53db48ae2b739f5bf5deef41b342fe154e13d37c4ca22d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74826194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e84ec8b67ce32fad14adb38e81b191c731737445551e607aadf4cb648de22d25`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:11 GMT
ADD file:262fd7bf0bc26e5d2a229fba52626e22b8a93beac29733acfc60e716c26e689d in / 
# Tue, 19 Dec 2023 01:41:11 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:35:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 07:35:16 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 07:35:17 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 07:35:17 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 07:35:17 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 07:35:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 07:35:50 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 07:35:50 GMT
USER user
# Tue, 19 Dec 2023 07:35:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:24e221e92a36ab5b0075dd156b4f2ff095532a9b0927946cf6070bb1bea208b8`  
		Last Modified: Tue, 19 Dec 2023 01:44:38 GMT  
		Size: 29.2 MB (29157269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3b65976afca6b69a78f82bba0cfd53e915de68b3497418795c0fe90dde04d6`  
		Last Modified: Tue, 19 Dec 2023 07:36:07 GMT  
		Size: 18.0 MB (18025714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1487d5e5dd099dea8c8f5cfa983386ef698d0b7ba74af27991d128c2eb77509a`  
		Last Modified: Tue, 19 Dec 2023 07:36:04 GMT  
		Size: 3.4 KB (3375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027137ab6d543546e67a802c5b15757aae71ceb8e7be44d4ab7e3701b466102e`  
		Last Modified: Tue, 19 Dec 2023 07:36:07 GMT  
		Size: 27.6 MB (27639836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; 386

```console
$ docker pull irssi@sha256:f4a77a97b8bd86a99d34d5fb0a8786e1a8f95758005b4ba99deb96a2b24d589a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76522898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e29421276ec13208c270be47f6eb04f62363c92fbf673bd983a1aa520e2fedc`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Nov 2023 04:39:53 GMT
ADD file:930e1b9d85b6927c4d3046f7c75de2f3bfc6ec29100c314d0ab2b780ea30e962 in / 
# Tue, 21 Nov 2023 04:39:53 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:18:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:18:00 GMT
ENV HOME=/home/user
# Tue, 21 Nov 2023 09:18:01 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Nov 2023 09:18:01 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 09:18:01 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 21 Nov 2023 09:18:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Nov 2023 09:18:58 GMT
WORKDIR /home/user
# Tue, 21 Nov 2023 09:18:58 GMT
USER user
# Tue, 21 Nov 2023 09:18:58 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c0734eabce8885d8904dbd11b77aa97c2d2b04bc8e2af9e89d47c4bda590dd8e`  
		Last Modified: Tue, 21 Nov 2023 04:44:34 GMT  
		Size: 30.2 MB (30164109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd0a88ad6c1f45a640f6b1e3509a00f0489ea5e7317905ff14b60fca6f24086`  
		Last Modified: Tue, 21 Nov 2023 09:19:21 GMT  
		Size: 17.8 MB (17789102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e785a0b684a75cef890d58447965564ea0ab287ad9b7fa38d00a4e9cfe5de7`  
		Last Modified: Tue, 21 Nov 2023 09:19:15 GMT  
		Size: 3.4 KB (3372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397cc87253be0de402ae3c1da69d2224514616b57b478236526d9f020d3b6ad6`  
		Last Modified: Tue, 21 Nov 2023 09:19:23 GMT  
		Size: 28.6 MB (28566315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; mips64le

```console
$ docker pull irssi@sha256:9c4985936b28f111411e9b54fe41acdb3b06222c5e22b4783ac53322ddf57794
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73894339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:370cd0afda43f756d5b75c9726905baa31206388d01ef49a763d8e033950a631`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 16:36:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 16:36:50 GMT
ENV HOME=/home/user
# Tue, 21 Nov 2023 16:36:56 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Nov 2023 16:37:00 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 16:37:03 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 21 Nov 2023 16:40:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Nov 2023 16:40:50 GMT
WORKDIR /home/user
# Tue, 21 Nov 2023 16:40:54 GMT
USER user
# Tue, 21 Nov 2023 16:40:58 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a2caa6a91dd837ff86958b77bc3534a4003f0cc9611e0b48c76361698bc605`  
		Last Modified: Tue, 21 Nov 2023 16:41:28 GMT  
		Size: 16.7 MB (16741807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6247f0644042c0a753bfe2ff1b7c28d43caaf3330ed88b170167a6fe8a0d35`  
		Last Modified: Tue, 21 Nov 2023 16:41:12 GMT  
		Size: 3.3 KB (3296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb6fda2e80956777959da56923ad2794e7af2f4a510933d7b85d0bf680feb2b`  
		Last Modified: Tue, 21 Nov 2023 16:41:33 GMT  
		Size: 28.0 MB (28007252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; ppc64le

```console
$ docker pull irssi@sha256:3f4f99d9914f9e72defad07d78d6e7c12b79184ab4aba83db835de09bc8f75bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82095380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60c6389f9028a4f1e86f03b0bf0bfed6a3d3f45126cdde79535e1136d045b8ff`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 08:14:12 GMT
ENV HOME=/home/user
# Tue, 21 Nov 2023 08:14:13 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Nov 2023 08:14:14 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 08:14:14 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 21 Nov 2023 08:15:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Nov 2023 08:15:10 GMT
WORKDIR /home/user
# Tue, 21 Nov 2023 08:15:10 GMT
USER user
# Tue, 21 Nov 2023 08:15:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990142f84c0c74390b332399beb412942fc74379d8c617ede6f2b0f701fd5f63`  
		Last Modified: Tue, 21 Nov 2023 08:15:42 GMT  
		Size: 18.8 MB (18764965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145cb9bddb869ec0a23e4a981ffb5078fc4852784403e1f0cb05eb86e52276cf`  
		Last Modified: Tue, 21 Nov 2023 08:15:38 GMT  
		Size: 3.4 KB (3371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c79418540c78592e0ce7f96f5df8dd9db310edd58c6f158ba3389cd2290920`  
		Last Modified: Tue, 21 Nov 2023 08:15:43 GMT  
		Size: 30.2 MB (30185437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; s390x

```console
$ docker pull irssi@sha256:19d5614ead4badb612e08ba2483418078e52144432cb38d8393c825b31ebe63f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72933796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2a7878077011d582ad7647ec003c06a9ed22ba2e0b5280c344ed18a0f1b8c40`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:42:37 GMT
ADD file:f06f12fa5a93afc3a79ac4371d24b0a471a5a1818cf34c1d90004c8f410914b9 in / 
# Tue, 19 Dec 2023 01:42:39 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:29:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:29:37 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 08:29:37 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 08:29:37 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 08:29:38 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 08:30:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 08:30:17 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 08:30:17 GMT
USER user
# Tue, 19 Dec 2023 08:30:17 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:bc6b1888979d3ceb063da848b2034e980e2c2613642159c1e856550b79aa620c`  
		Last Modified: Tue, 19 Dec 2023 01:47:38 GMT  
		Size: 27.5 MB (27491874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d93a78aafed26613c2aa62cc6ab76d24cde8ba422049c8c4aff454d7e8b6f0`  
		Last Modified: Tue, 19 Dec 2023 08:30:47 GMT  
		Size: 18.2 MB (18210518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506c18d3ee4758db831ecc9a8b1ea9f2562b6972d70a1fb2cd98603a28811f5f`  
		Last Modified: Tue, 19 Dec 2023 08:30:44 GMT  
		Size: 3.4 KB (3376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64e09b7ab558543c54810d6e85b3a3fab5eb5ae4fec9423bfdc282f16c15bcc`  
		Last Modified: Tue, 19 Dec 2023 08:30:48 GMT  
		Size: 27.2 MB (27228028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4-alpine`

```console
$ docker pull irssi@sha256:b404269638b505c913a02979a9f253a8e9e904e585c6bb3011b7afbc06908340
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
$ docker pull irssi@sha256:bac3d5c9afaa50fa166d54e4f8a6b82f8519d5f41f60e154925a961f498c67cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18451924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b18b85f03e9dae76ebfd3a15dd2180db03fc5728ce1980f8ae072a7fbbdc15f3`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:28:32 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 05:28:32 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 05:28:33 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 05:28:33 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 05:28:33 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 05:28:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 05:28:52 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 05:28:52 GMT
USER user
# Fri, 01 Dec 2023 05:28:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2253ad6954238459aeb69a5812221ad8d0a9cf6473cb145f43ec969741e3f7c`  
		Last Modified: Fri, 01 Dec 2023 05:29:12 GMT  
		Size: 9.6 MB (9645529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027edf83d9867e80bd5e7041a3da7cbbd50027d7f1e9018f1174b20ca77aea09`  
		Last Modified: Fri, 01 Dec 2023 05:29:10 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf95bf3609411e5c119950c792cabbb3c647eb384dafacbce7a70a601533c44`  
		Last Modified: Fri, 01 Dec 2023 05:29:11 GMT  
		Size: 5.4 MB (5402689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:51601527f7062d912289288c810b48a9d00b3922cef2a58b04787672ff913d07
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17271200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3301b14e65fec26ab44af0807bbcd5ac7cfb9230618a31edcde72367a83b21da`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 01:09:50 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 01:09:50 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 01:09:51 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 01:09:51 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 01:09:51 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 01:10:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 01:10:08 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 01:10:08 GMT
USER user
# Fri, 01 Dec 2023 01:10:08 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0389ed6f59ff0e95c3c6c4566157405d8b3bb4b5a827a5a1fd24edf934393c`  
		Last Modified: Fri, 01 Dec 2023 01:10:22 GMT  
		Size: 8.9 MB (8880077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4039f2bf7cbc0fa8f9a5e8a20f20a5035b388d7a42a95d9d6f0a3a58446eed`  
		Last Modified: Fri, 01 Dec 2023 01:10:19 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184e5e97ecd8a9cf4081a03b9f6a83022561e425f3294a0d09c345420c858123`  
		Last Modified: Fri, 01 Dec 2023 01:10:21 GMT  
		Size: 5.2 MB (5242968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:6ff758c9743e67bc2781d127b56339f483bfbb1251763d398a335d3a95ae9744
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16630768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ba268037301e762641733ac31d7ab82c0538e3658cc00205b6ca74c23bb5332`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:41:57 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 08:41:57 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 08:41:57 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 08:41:57 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 08:41:57 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 08:42:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 08:42:12 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 08:42:12 GMT
USER user
# Fri, 01 Dec 2023 08:42:12 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505553baa092b1ac5dc9c2a961456e9728d5bfe4d15f5a93644f58c1a0c75d14`  
		Last Modified: Fri, 01 Dec 2023 08:42:31 GMT  
		Size: 8.7 MB (8721323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc7d412e24534e4f0eebe098495c5878f5184667c4180f22eb8b50bff5d78cf`  
		Last Modified: Fri, 01 Dec 2023 08:42:29 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d25439b4dd4f4d92fd4be67af55606656fd511d66a1f63715b0dd6d2eeab5b`  
		Last Modified: Fri, 01 Dec 2023 08:42:30 GMT  
		Size: 5.0 MB (5007154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:444032f59c771f9f8ecc9f1374f55b4f94016696d5e58a0931e61ae604748369
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18316372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a03091ab8bcbd9db84ead2d162e748af025192b4ebc302c6a42bd11b034e026b`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:37:23 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 09:37:23 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 09:37:24 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 09:37:24 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 09:37:24 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 09:37:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 09:37:36 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 09:37:36 GMT
USER user
# Fri, 01 Dec 2023 09:37:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408050d673681e97a81fefc3f0d62dc535741ab369d0f890dfd492fea579fc73`  
		Last Modified: Fri, 01 Dec 2023 09:37:55 GMT  
		Size: 9.7 MB (9672911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b351c7a82544307a7a55c5daa20a529cd389facb270805cea95b2040f8b864`  
		Last Modified: Fri, 01 Dec 2023 09:37:53 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad688b9a5733e1a4e2feaddf0a4ae2395f72b5d718efc48685befed72ad2d440`  
		Last Modified: Fri, 01 Dec 2023 09:37:54 GMT  
		Size: 5.3 MB (5309143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine` - linux; 386

```console
$ docker pull irssi@sha256:cb5e5eb3ce2e5c8a080af15a2414c7078412473c44bfe7c15196f957fdd3931b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17557886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e422f2a321a825ce4ac90dad135af83afa3ee86cd59d10d667a313c1b2ec35a7`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 01 Dec 2023 02:03:44 GMT
ADD file:92902088cd15ed8f5dca2f7fc6570fb4e4824fac8b09e091c88e96bbd0ca814b in / 
# Fri, 01 Dec 2023 02:03:44 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:02:03 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 09:02:03 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 09:02:03 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 09:02:04 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 09:02:04 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 09:02:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 09:02:38 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 09:02:38 GMT
USER user
# Fri, 01 Dec 2023 09:02:38 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4966a8bd129b0a6adf93dc295a8fbe8f665d3194a684a5ce199c1c3596dbf3d9`  
		Last Modified: Fri, 01 Dec 2023 02:04:18 GMT  
		Size: 3.2 MB (3238831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194fdb04cb3e17be198ec377fafeb3f5716927ef33b40df425a942b4f3f7e50`  
		Last Modified: Fri, 01 Dec 2023 09:03:00 GMT  
		Size: 8.9 MB (8904478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc41f0a0151cdbeed763c916854e38b017669921f3a79d0554e77543dcb09acb`  
		Last Modified: Fri, 01 Dec 2023 09:02:57 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5a928454e9d9ee194c2842f26954fc39b31e235b0de4f542f9acc45af1737f`  
		Last Modified: Fri, 01 Dec 2023 09:02:58 GMT  
		Size: 5.4 MB (5413293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:e3eba53096e51def6997bdc72c51cf88f0019645321ee59bdd20b49b4236a617
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18717510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:890fc74fc94817011bde8d06e7b449e6407828cbbff17d07e69de027ad3d77f4`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:04:09 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 05:04:12 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 05:04:20 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 05:04:21 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 05:04:21 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 05:04:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 05:04:59 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 05:05:00 GMT
USER user
# Fri, 01 Dec 2023 05:05:02 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5afc2e0a7e24376eade504bc1d0aee8fa44d1b246f3121de324296a57c0ff25d`  
		Last Modified: Fri, 01 Dec 2023 05:05:36 GMT  
		Size: 9.7 MB (9736497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04ef92e3c12ead968e636f09604f92720ce8750a3a7f114277c2ef6764219b6`  
		Last Modified: Fri, 01 Dec 2023 05:05:34 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce0f8ba67064d14f75d9e13652d96ba1e13e489eff4d5617c0e503e25106009`  
		Last Modified: Fri, 01 Dec 2023 05:05:35 GMT  
		Size: 5.6 MB (5631406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:2f5751ebf70dce38c6c48dc4a4e7f72bdae9824a0da9b3b95c277c755139592c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18708403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30063d82b1a526f916c2be961b95561fad91acd4ecfa2942d616740be6105a20`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:13:12 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 08:13:13 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 08:13:13 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 08:13:14 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 08:13:14 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 08:13:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 08:13:35 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 08:13:35 GMT
USER user
# Fri, 01 Dec 2023 08:13:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c64be9d9a3f22087e689a8436399a73b9fb1f76114c8c4b5740080a6d178c9b`  
		Last Modified: Fri, 01 Dec 2023 08:14:02 GMT  
		Size: 10.1 MB (10083001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403430efaca857233fd4cc970775e8fb9b2bfa68899058f8046852bf2a25be16`  
		Last Modified: Fri, 01 Dec 2023 08:13:59 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9630989fe7d8e6fcb8d2886d67968d8118d654dbaa9787a1e4050fe5d293e589`  
		Last Modified: Fri, 01 Dec 2023 08:14:00 GMT  
		Size: 5.4 MB (5406662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4-alpine3.18`

```console
$ docker pull irssi@sha256:b404269638b505c913a02979a9f253a8e9e904e585c6bb3011b7afbc06908340
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

### `irssi:1.4-alpine3.18` - linux; amd64

```console
$ docker pull irssi@sha256:bac3d5c9afaa50fa166d54e4f8a6b82f8519d5f41f60e154925a961f498c67cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18451924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b18b85f03e9dae76ebfd3a15dd2180db03fc5728ce1980f8ae072a7fbbdc15f3`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:28:32 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 05:28:32 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 05:28:33 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 05:28:33 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 05:28:33 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 05:28:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 05:28:52 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 05:28:52 GMT
USER user
# Fri, 01 Dec 2023 05:28:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2253ad6954238459aeb69a5812221ad8d0a9cf6473cb145f43ec969741e3f7c`  
		Last Modified: Fri, 01 Dec 2023 05:29:12 GMT  
		Size: 9.6 MB (9645529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027edf83d9867e80bd5e7041a3da7cbbd50027d7f1e9018f1174b20ca77aea09`  
		Last Modified: Fri, 01 Dec 2023 05:29:10 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf95bf3609411e5c119950c792cabbb3c647eb384dafacbce7a70a601533c44`  
		Last Modified: Fri, 01 Dec 2023 05:29:11 GMT  
		Size: 5.4 MB (5402689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine3.18` - linux; arm variant v6

```console
$ docker pull irssi@sha256:51601527f7062d912289288c810b48a9d00b3922cef2a58b04787672ff913d07
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17271200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3301b14e65fec26ab44af0807bbcd5ac7cfb9230618a31edcde72367a83b21da`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 01:09:50 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 01:09:50 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 01:09:51 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 01:09:51 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 01:09:51 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 01:10:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 01:10:08 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 01:10:08 GMT
USER user
# Fri, 01 Dec 2023 01:10:08 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0389ed6f59ff0e95c3c6c4566157405d8b3bb4b5a827a5a1fd24edf934393c`  
		Last Modified: Fri, 01 Dec 2023 01:10:22 GMT  
		Size: 8.9 MB (8880077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4039f2bf7cbc0fa8f9a5e8a20f20a5035b388d7a42a95d9d6f0a3a58446eed`  
		Last Modified: Fri, 01 Dec 2023 01:10:19 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184e5e97ecd8a9cf4081a03b9f6a83022561e425f3294a0d09c345420c858123`  
		Last Modified: Fri, 01 Dec 2023 01:10:21 GMT  
		Size: 5.2 MB (5242968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine3.18` - linux; arm variant v7

```console
$ docker pull irssi@sha256:6ff758c9743e67bc2781d127b56339f483bfbb1251763d398a335d3a95ae9744
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16630768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ba268037301e762641733ac31d7ab82c0538e3658cc00205b6ca74c23bb5332`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:41:57 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 08:41:57 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 08:41:57 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 08:41:57 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 08:41:57 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 08:42:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 08:42:12 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 08:42:12 GMT
USER user
# Fri, 01 Dec 2023 08:42:12 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505553baa092b1ac5dc9c2a961456e9728d5bfe4d15f5a93644f58c1a0c75d14`  
		Last Modified: Fri, 01 Dec 2023 08:42:31 GMT  
		Size: 8.7 MB (8721323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc7d412e24534e4f0eebe098495c5878f5184667c4180f22eb8b50bff5d78cf`  
		Last Modified: Fri, 01 Dec 2023 08:42:29 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d25439b4dd4f4d92fd4be67af55606656fd511d66a1f63715b0dd6d2eeab5b`  
		Last Modified: Fri, 01 Dec 2023 08:42:30 GMT  
		Size: 5.0 MB (5007154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:444032f59c771f9f8ecc9f1374f55b4f94016696d5e58a0931e61ae604748369
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18316372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a03091ab8bcbd9db84ead2d162e748af025192b4ebc302c6a42bd11b034e026b`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:37:23 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 09:37:23 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 09:37:24 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 09:37:24 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 09:37:24 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 09:37:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 09:37:36 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 09:37:36 GMT
USER user
# Fri, 01 Dec 2023 09:37:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408050d673681e97a81fefc3f0d62dc535741ab369d0f890dfd492fea579fc73`  
		Last Modified: Fri, 01 Dec 2023 09:37:55 GMT  
		Size: 9.7 MB (9672911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b351c7a82544307a7a55c5daa20a529cd389facb270805cea95b2040f8b864`  
		Last Modified: Fri, 01 Dec 2023 09:37:53 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad688b9a5733e1a4e2feaddf0a4ae2395f72b5d718efc48685befed72ad2d440`  
		Last Modified: Fri, 01 Dec 2023 09:37:54 GMT  
		Size: 5.3 MB (5309143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine3.18` - linux; 386

```console
$ docker pull irssi@sha256:cb5e5eb3ce2e5c8a080af15a2414c7078412473c44bfe7c15196f957fdd3931b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17557886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e422f2a321a825ce4ac90dad135af83afa3ee86cd59d10d667a313c1b2ec35a7`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 01 Dec 2023 02:03:44 GMT
ADD file:92902088cd15ed8f5dca2f7fc6570fb4e4824fac8b09e091c88e96bbd0ca814b in / 
# Fri, 01 Dec 2023 02:03:44 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:02:03 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 09:02:03 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 09:02:03 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 09:02:04 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 09:02:04 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 09:02:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 09:02:38 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 09:02:38 GMT
USER user
# Fri, 01 Dec 2023 09:02:38 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4966a8bd129b0a6adf93dc295a8fbe8f665d3194a684a5ce199c1c3596dbf3d9`  
		Last Modified: Fri, 01 Dec 2023 02:04:18 GMT  
		Size: 3.2 MB (3238831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194fdb04cb3e17be198ec377fafeb3f5716927ef33b40df425a942b4f3f7e50`  
		Last Modified: Fri, 01 Dec 2023 09:03:00 GMT  
		Size: 8.9 MB (8904478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc41f0a0151cdbeed763c916854e38b017669921f3a79d0554e77543dcb09acb`  
		Last Modified: Fri, 01 Dec 2023 09:02:57 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5a928454e9d9ee194c2842f26954fc39b31e235b0de4f542f9acc45af1737f`  
		Last Modified: Fri, 01 Dec 2023 09:02:58 GMT  
		Size: 5.4 MB (5413293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine3.18` - linux; ppc64le

```console
$ docker pull irssi@sha256:e3eba53096e51def6997bdc72c51cf88f0019645321ee59bdd20b49b4236a617
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18717510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:890fc74fc94817011bde8d06e7b449e6407828cbbff17d07e69de027ad3d77f4`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:04:09 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 05:04:12 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 05:04:20 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 05:04:21 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 05:04:21 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 05:04:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 05:04:59 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 05:05:00 GMT
USER user
# Fri, 01 Dec 2023 05:05:02 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5afc2e0a7e24376eade504bc1d0aee8fa44d1b246f3121de324296a57c0ff25d`  
		Last Modified: Fri, 01 Dec 2023 05:05:36 GMT  
		Size: 9.7 MB (9736497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04ef92e3c12ead968e636f09604f92720ce8750a3a7f114277c2ef6764219b6`  
		Last Modified: Fri, 01 Dec 2023 05:05:34 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce0f8ba67064d14f75d9e13652d96ba1e13e489eff4d5617c0e503e25106009`  
		Last Modified: Fri, 01 Dec 2023 05:05:35 GMT  
		Size: 5.6 MB (5631406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine3.18` - linux; s390x

```console
$ docker pull irssi@sha256:2f5751ebf70dce38c6c48dc4a4e7f72bdae9824a0da9b3b95c277c755139592c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18708403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30063d82b1a526f916c2be961b95561fad91acd4ecfa2942d616740be6105a20`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:13:12 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 08:13:13 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 08:13:13 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 08:13:14 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 08:13:14 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 08:13:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 08:13:35 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 08:13:35 GMT
USER user
# Fri, 01 Dec 2023 08:13:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c64be9d9a3f22087e689a8436399a73b9fb1f76114c8c4b5740080a6d178c9b`  
		Last Modified: Fri, 01 Dec 2023 08:14:02 GMT  
		Size: 10.1 MB (10083001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403430efaca857233fd4cc970775e8fb9b2bfa68899058f8046852bf2a25be16`  
		Last Modified: Fri, 01 Dec 2023 08:13:59 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9630989fe7d8e6fcb8d2886d67968d8118d654dbaa9787a1e4050fe5d293e589`  
		Last Modified: Fri, 01 Dec 2023 08:14:00 GMT  
		Size: 5.4 MB (5406662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4-bookworm`

```console
$ docker pull irssi@sha256:9bbaebbdef964fd13f87622f887af48afe01d1ef67ec7152da0e993626f8c347
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

### `irssi:1.4-bookworm` - linux; amd64

```console
$ docker pull irssi@sha256:75930e1081143e5ac73cc553fd47dd75a236c5587dad0b13ed4f593d5efec999
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76071375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e784ee8f60cc445019f7f2a00f02a16d18715a384904180fa30548888ea9a9e2`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:27 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Tue, 19 Dec 2023 01:20:28 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:11:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:11:41 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 08:11:42 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 08:11:42 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 08:11:42 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 08:12:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 08:12:22 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 08:12:22 GMT
USER user
# Tue, 19 Dec 2023 08:12:22 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f576257a7efd8fa2eab590d15da13ff3e351ddd5f66e1f18853950d0a847940`  
		Last Modified: Tue, 19 Dec 2023 08:12:41 GMT  
		Size: 18.3 MB (18263304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8709b16d66af9e29995cd9f313628ac25626d9a3b9f14337a489a0b53dede1`  
		Last Modified: Tue, 19 Dec 2023 08:12:37 GMT  
		Size: 3.4 KB (3376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4721ae122aaf701fec4c0ab60bcd8186c440f5439303bb23fc19aaa3cc886e`  
		Last Modified: Tue, 19 Dec 2023 08:12:42 GMT  
		Size: 28.7 MB (28678732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-bookworm` - linux; arm variant v5

```console
$ docker pull irssi@sha256:54f4b6e9ea13a0ad57b6507d166cc7d60f705a1f0fb2c8b1a21ccf71be8b4817
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70247719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f71b3c5dc081e54b3f8c57c1d3be303a0147a4ac5656f26d0698b3673bce8f5`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:55:22 GMT
ADD file:9503ab966c9dd707eeccc7c2f633bccc94c199f8714ec4ff2c8b54dde3dbabf9 in / 
# Tue, 19 Dec 2023 01:55:22 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 05:37:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 05:37:07 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 05:37:08 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 05:37:08 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 05:37:08 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 05:37:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 05:37:54 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 05:37:54 GMT
USER user
# Tue, 19 Dec 2023 05:37:54 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1ae9a2844c8c70942d2220553689b62e841cc706d77284fbfedbd770080fd699`  
		Last Modified: Tue, 19 Dec 2023 01:58:33 GMT  
		Size: 26.9 MB (26885440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8c63a38cdf609e2fc7e6adb6d2a2ddee5ee1e185ced4c5667fa93153ddaca4`  
		Last Modified: Tue, 19 Dec 2023 05:38:20 GMT  
		Size: 17.0 MB (17034518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5baba07d2ad153cdc8a55cf44e4e53c2d24eccd878b7c013029ad93e53dad92b`  
		Last Modified: Tue, 19 Dec 2023 05:38:15 GMT  
		Size: 3.4 KB (3382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b675c572666d53e7aaee086d9f3a892e01803b6b84ab820ee1100726092e714`  
		Last Modified: Tue, 19 Dec 2023 05:38:21 GMT  
		Size: 26.3 MB (26324379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-bookworm` - linux; arm variant v7

```console
$ docker pull irssi@sha256:b58087a750d2ecb0db246fa2b83fce92398c136af518ddc7bcae63e75637be1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66568253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0abed9b964bf4864c88c0c97e43a26973a28db129f9679f226eba9307dd515ec`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 02:07:50 GMT
ADD file:aef112919e7924ad6da32181b1df5099cd692680c104118da3a24cd4dfe55a1d in / 
# Tue, 19 Dec 2023 02:07:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:25:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:25:13 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 08:25:13 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 08:25:14 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 08:25:14 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 08:25:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 08:25:50 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 08:25:50 GMT
USER user
# Tue, 19 Dec 2023 08:25:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:65ab19615c01a3b542f77fadb3bd27872b6a20cba3e9269fb951de36d8fa6805`  
		Last Modified: Tue, 19 Dec 2023 02:11:52 GMT  
		Size: 24.7 MB (24718157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34312fc906c50709273b2bfc296cbc5e618081aab636bea0270e632aa1250a58`  
		Last Modified: Tue, 19 Dec 2023 08:26:13 GMT  
		Size: 16.6 MB (16626329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ae59c8630536591ee4c9f224e24066f5ea55d87cd4d710f4758493e40f4d90`  
		Last Modified: Tue, 19 Dec 2023 08:26:07 GMT  
		Size: 3.4 KB (3375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653d387ba5d23d5a1d3207409abeb6f1857445f450f723a518d7f30d8305a612`  
		Last Modified: Tue, 19 Dec 2023 08:26:13 GMT  
		Size: 25.2 MB (25220392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-bookworm` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:ca5674fca34098dff53db48ae2b739f5bf5deef41b342fe154e13d37c4ca22d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74826194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e84ec8b67ce32fad14adb38e81b191c731737445551e607aadf4cb648de22d25`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:11 GMT
ADD file:262fd7bf0bc26e5d2a229fba52626e22b8a93beac29733acfc60e716c26e689d in / 
# Tue, 19 Dec 2023 01:41:11 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:35:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 07:35:16 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 07:35:17 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 07:35:17 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 07:35:17 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 07:35:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 07:35:50 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 07:35:50 GMT
USER user
# Tue, 19 Dec 2023 07:35:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:24e221e92a36ab5b0075dd156b4f2ff095532a9b0927946cf6070bb1bea208b8`  
		Last Modified: Tue, 19 Dec 2023 01:44:38 GMT  
		Size: 29.2 MB (29157269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3b65976afca6b69a78f82bba0cfd53e915de68b3497418795c0fe90dde04d6`  
		Last Modified: Tue, 19 Dec 2023 07:36:07 GMT  
		Size: 18.0 MB (18025714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1487d5e5dd099dea8c8f5cfa983386ef698d0b7ba74af27991d128c2eb77509a`  
		Last Modified: Tue, 19 Dec 2023 07:36:04 GMT  
		Size: 3.4 KB (3375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027137ab6d543546e67a802c5b15757aae71ceb8e7be44d4ab7e3701b466102e`  
		Last Modified: Tue, 19 Dec 2023 07:36:07 GMT  
		Size: 27.6 MB (27639836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-bookworm` - linux; 386

```console
$ docker pull irssi@sha256:f4a77a97b8bd86a99d34d5fb0a8786e1a8f95758005b4ba99deb96a2b24d589a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76522898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e29421276ec13208c270be47f6eb04f62363c92fbf673bd983a1aa520e2fedc`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Nov 2023 04:39:53 GMT
ADD file:930e1b9d85b6927c4d3046f7c75de2f3bfc6ec29100c314d0ab2b780ea30e962 in / 
# Tue, 21 Nov 2023 04:39:53 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:18:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:18:00 GMT
ENV HOME=/home/user
# Tue, 21 Nov 2023 09:18:01 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Nov 2023 09:18:01 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 09:18:01 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 21 Nov 2023 09:18:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Nov 2023 09:18:58 GMT
WORKDIR /home/user
# Tue, 21 Nov 2023 09:18:58 GMT
USER user
# Tue, 21 Nov 2023 09:18:58 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c0734eabce8885d8904dbd11b77aa97c2d2b04bc8e2af9e89d47c4bda590dd8e`  
		Last Modified: Tue, 21 Nov 2023 04:44:34 GMT  
		Size: 30.2 MB (30164109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd0a88ad6c1f45a640f6b1e3509a00f0489ea5e7317905ff14b60fca6f24086`  
		Last Modified: Tue, 21 Nov 2023 09:19:21 GMT  
		Size: 17.8 MB (17789102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e785a0b684a75cef890d58447965564ea0ab287ad9b7fa38d00a4e9cfe5de7`  
		Last Modified: Tue, 21 Nov 2023 09:19:15 GMT  
		Size: 3.4 KB (3372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397cc87253be0de402ae3c1da69d2224514616b57b478236526d9f020d3b6ad6`  
		Last Modified: Tue, 21 Nov 2023 09:19:23 GMT  
		Size: 28.6 MB (28566315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-bookworm` - linux; mips64le

```console
$ docker pull irssi@sha256:9c4985936b28f111411e9b54fe41acdb3b06222c5e22b4783ac53322ddf57794
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73894339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:370cd0afda43f756d5b75c9726905baa31206388d01ef49a763d8e033950a631`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 16:36:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 16:36:50 GMT
ENV HOME=/home/user
# Tue, 21 Nov 2023 16:36:56 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Nov 2023 16:37:00 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 16:37:03 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 21 Nov 2023 16:40:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Nov 2023 16:40:50 GMT
WORKDIR /home/user
# Tue, 21 Nov 2023 16:40:54 GMT
USER user
# Tue, 21 Nov 2023 16:40:58 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a2caa6a91dd837ff86958b77bc3534a4003f0cc9611e0b48c76361698bc605`  
		Last Modified: Tue, 21 Nov 2023 16:41:28 GMT  
		Size: 16.7 MB (16741807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6247f0644042c0a753bfe2ff1b7c28d43caaf3330ed88b170167a6fe8a0d35`  
		Last Modified: Tue, 21 Nov 2023 16:41:12 GMT  
		Size: 3.3 KB (3296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb6fda2e80956777959da56923ad2794e7af2f4a510933d7b85d0bf680feb2b`  
		Last Modified: Tue, 21 Nov 2023 16:41:33 GMT  
		Size: 28.0 MB (28007252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-bookworm` - linux; ppc64le

```console
$ docker pull irssi@sha256:3f4f99d9914f9e72defad07d78d6e7c12b79184ab4aba83db835de09bc8f75bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82095380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60c6389f9028a4f1e86f03b0bf0bfed6a3d3f45126cdde79535e1136d045b8ff`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 08:14:12 GMT
ENV HOME=/home/user
# Tue, 21 Nov 2023 08:14:13 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Nov 2023 08:14:14 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 08:14:14 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 21 Nov 2023 08:15:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Nov 2023 08:15:10 GMT
WORKDIR /home/user
# Tue, 21 Nov 2023 08:15:10 GMT
USER user
# Tue, 21 Nov 2023 08:15:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990142f84c0c74390b332399beb412942fc74379d8c617ede6f2b0f701fd5f63`  
		Last Modified: Tue, 21 Nov 2023 08:15:42 GMT  
		Size: 18.8 MB (18764965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145cb9bddb869ec0a23e4a981ffb5078fc4852784403e1f0cb05eb86e52276cf`  
		Last Modified: Tue, 21 Nov 2023 08:15:38 GMT  
		Size: 3.4 KB (3371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c79418540c78592e0ce7f96f5df8dd9db310edd58c6f158ba3389cd2290920`  
		Last Modified: Tue, 21 Nov 2023 08:15:43 GMT  
		Size: 30.2 MB (30185437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-bookworm` - linux; s390x

```console
$ docker pull irssi@sha256:19d5614ead4badb612e08ba2483418078e52144432cb38d8393c825b31ebe63f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72933796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2a7878077011d582ad7647ec003c06a9ed22ba2e0b5280c344ed18a0f1b8c40`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:42:37 GMT
ADD file:f06f12fa5a93afc3a79ac4371d24b0a471a5a1818cf34c1d90004c8f410914b9 in / 
# Tue, 19 Dec 2023 01:42:39 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:29:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:29:37 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 08:29:37 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 08:29:37 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 08:29:38 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 08:30:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 08:30:17 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 08:30:17 GMT
USER user
# Tue, 19 Dec 2023 08:30:17 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:bc6b1888979d3ceb063da848b2034e980e2c2613642159c1e856550b79aa620c`  
		Last Modified: Tue, 19 Dec 2023 01:47:38 GMT  
		Size: 27.5 MB (27491874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d93a78aafed26613c2aa62cc6ab76d24cde8ba422049c8c4aff454d7e8b6f0`  
		Last Modified: Tue, 19 Dec 2023 08:30:47 GMT  
		Size: 18.2 MB (18210518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506c18d3ee4758db831ecc9a8b1ea9f2562b6972d70a1fb2cd98603a28811f5f`  
		Last Modified: Tue, 19 Dec 2023 08:30:44 GMT  
		Size: 3.4 KB (3376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64e09b7ab558543c54810d6e85b3a3fab5eb5ae4fec9423bfdc282f16c15bcc`  
		Last Modified: Tue, 19 Dec 2023 08:30:48 GMT  
		Size: 27.2 MB (27228028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4.5`

```console
$ docker pull irssi@sha256:9bbaebbdef964fd13f87622f887af48afe01d1ef67ec7152da0e993626f8c347
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

### `irssi:1.4.5` - linux; amd64

```console
$ docker pull irssi@sha256:75930e1081143e5ac73cc553fd47dd75a236c5587dad0b13ed4f593d5efec999
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76071375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e784ee8f60cc445019f7f2a00f02a16d18715a384904180fa30548888ea9a9e2`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:27 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Tue, 19 Dec 2023 01:20:28 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:11:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:11:41 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 08:11:42 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 08:11:42 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 08:11:42 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 08:12:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 08:12:22 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 08:12:22 GMT
USER user
# Tue, 19 Dec 2023 08:12:22 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f576257a7efd8fa2eab590d15da13ff3e351ddd5f66e1f18853950d0a847940`  
		Last Modified: Tue, 19 Dec 2023 08:12:41 GMT  
		Size: 18.3 MB (18263304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8709b16d66af9e29995cd9f313628ac25626d9a3b9f14337a489a0b53dede1`  
		Last Modified: Tue, 19 Dec 2023 08:12:37 GMT  
		Size: 3.4 KB (3376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4721ae122aaf701fec4c0ab60bcd8186c440f5439303bb23fc19aaa3cc886e`  
		Last Modified: Tue, 19 Dec 2023 08:12:42 GMT  
		Size: 28.7 MB (28678732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5` - linux; arm variant v5

```console
$ docker pull irssi@sha256:54f4b6e9ea13a0ad57b6507d166cc7d60f705a1f0fb2c8b1a21ccf71be8b4817
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70247719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f71b3c5dc081e54b3f8c57c1d3be303a0147a4ac5656f26d0698b3673bce8f5`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:55:22 GMT
ADD file:9503ab966c9dd707eeccc7c2f633bccc94c199f8714ec4ff2c8b54dde3dbabf9 in / 
# Tue, 19 Dec 2023 01:55:22 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 05:37:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 05:37:07 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 05:37:08 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 05:37:08 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 05:37:08 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 05:37:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 05:37:54 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 05:37:54 GMT
USER user
# Tue, 19 Dec 2023 05:37:54 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1ae9a2844c8c70942d2220553689b62e841cc706d77284fbfedbd770080fd699`  
		Last Modified: Tue, 19 Dec 2023 01:58:33 GMT  
		Size: 26.9 MB (26885440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8c63a38cdf609e2fc7e6adb6d2a2ddee5ee1e185ced4c5667fa93153ddaca4`  
		Last Modified: Tue, 19 Dec 2023 05:38:20 GMT  
		Size: 17.0 MB (17034518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5baba07d2ad153cdc8a55cf44e4e53c2d24eccd878b7c013029ad93e53dad92b`  
		Last Modified: Tue, 19 Dec 2023 05:38:15 GMT  
		Size: 3.4 KB (3382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b675c572666d53e7aaee086d9f3a892e01803b6b84ab820ee1100726092e714`  
		Last Modified: Tue, 19 Dec 2023 05:38:21 GMT  
		Size: 26.3 MB (26324379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5` - linux; arm variant v7

```console
$ docker pull irssi@sha256:b58087a750d2ecb0db246fa2b83fce92398c136af518ddc7bcae63e75637be1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66568253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0abed9b964bf4864c88c0c97e43a26973a28db129f9679f226eba9307dd515ec`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 02:07:50 GMT
ADD file:aef112919e7924ad6da32181b1df5099cd692680c104118da3a24cd4dfe55a1d in / 
# Tue, 19 Dec 2023 02:07:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:25:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:25:13 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 08:25:13 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 08:25:14 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 08:25:14 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 08:25:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 08:25:50 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 08:25:50 GMT
USER user
# Tue, 19 Dec 2023 08:25:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:65ab19615c01a3b542f77fadb3bd27872b6a20cba3e9269fb951de36d8fa6805`  
		Last Modified: Tue, 19 Dec 2023 02:11:52 GMT  
		Size: 24.7 MB (24718157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34312fc906c50709273b2bfc296cbc5e618081aab636bea0270e632aa1250a58`  
		Last Modified: Tue, 19 Dec 2023 08:26:13 GMT  
		Size: 16.6 MB (16626329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ae59c8630536591ee4c9f224e24066f5ea55d87cd4d710f4758493e40f4d90`  
		Last Modified: Tue, 19 Dec 2023 08:26:07 GMT  
		Size: 3.4 KB (3375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653d387ba5d23d5a1d3207409abeb6f1857445f450f723a518d7f30d8305a612`  
		Last Modified: Tue, 19 Dec 2023 08:26:13 GMT  
		Size: 25.2 MB (25220392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:ca5674fca34098dff53db48ae2b739f5bf5deef41b342fe154e13d37c4ca22d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74826194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e84ec8b67ce32fad14adb38e81b191c731737445551e607aadf4cb648de22d25`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:11 GMT
ADD file:262fd7bf0bc26e5d2a229fba52626e22b8a93beac29733acfc60e716c26e689d in / 
# Tue, 19 Dec 2023 01:41:11 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:35:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 07:35:16 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 07:35:17 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 07:35:17 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 07:35:17 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 07:35:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 07:35:50 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 07:35:50 GMT
USER user
# Tue, 19 Dec 2023 07:35:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:24e221e92a36ab5b0075dd156b4f2ff095532a9b0927946cf6070bb1bea208b8`  
		Last Modified: Tue, 19 Dec 2023 01:44:38 GMT  
		Size: 29.2 MB (29157269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3b65976afca6b69a78f82bba0cfd53e915de68b3497418795c0fe90dde04d6`  
		Last Modified: Tue, 19 Dec 2023 07:36:07 GMT  
		Size: 18.0 MB (18025714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1487d5e5dd099dea8c8f5cfa983386ef698d0b7ba74af27991d128c2eb77509a`  
		Last Modified: Tue, 19 Dec 2023 07:36:04 GMT  
		Size: 3.4 KB (3375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027137ab6d543546e67a802c5b15757aae71ceb8e7be44d4ab7e3701b466102e`  
		Last Modified: Tue, 19 Dec 2023 07:36:07 GMT  
		Size: 27.6 MB (27639836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5` - linux; 386

```console
$ docker pull irssi@sha256:f4a77a97b8bd86a99d34d5fb0a8786e1a8f95758005b4ba99deb96a2b24d589a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76522898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e29421276ec13208c270be47f6eb04f62363c92fbf673bd983a1aa520e2fedc`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Nov 2023 04:39:53 GMT
ADD file:930e1b9d85b6927c4d3046f7c75de2f3bfc6ec29100c314d0ab2b780ea30e962 in / 
# Tue, 21 Nov 2023 04:39:53 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:18:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:18:00 GMT
ENV HOME=/home/user
# Tue, 21 Nov 2023 09:18:01 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Nov 2023 09:18:01 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 09:18:01 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 21 Nov 2023 09:18:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Nov 2023 09:18:58 GMT
WORKDIR /home/user
# Tue, 21 Nov 2023 09:18:58 GMT
USER user
# Tue, 21 Nov 2023 09:18:58 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c0734eabce8885d8904dbd11b77aa97c2d2b04bc8e2af9e89d47c4bda590dd8e`  
		Last Modified: Tue, 21 Nov 2023 04:44:34 GMT  
		Size: 30.2 MB (30164109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd0a88ad6c1f45a640f6b1e3509a00f0489ea5e7317905ff14b60fca6f24086`  
		Last Modified: Tue, 21 Nov 2023 09:19:21 GMT  
		Size: 17.8 MB (17789102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e785a0b684a75cef890d58447965564ea0ab287ad9b7fa38d00a4e9cfe5de7`  
		Last Modified: Tue, 21 Nov 2023 09:19:15 GMT  
		Size: 3.4 KB (3372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397cc87253be0de402ae3c1da69d2224514616b57b478236526d9f020d3b6ad6`  
		Last Modified: Tue, 21 Nov 2023 09:19:23 GMT  
		Size: 28.6 MB (28566315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5` - linux; mips64le

```console
$ docker pull irssi@sha256:9c4985936b28f111411e9b54fe41acdb3b06222c5e22b4783ac53322ddf57794
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73894339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:370cd0afda43f756d5b75c9726905baa31206388d01ef49a763d8e033950a631`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 16:36:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 16:36:50 GMT
ENV HOME=/home/user
# Tue, 21 Nov 2023 16:36:56 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Nov 2023 16:37:00 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 16:37:03 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 21 Nov 2023 16:40:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Nov 2023 16:40:50 GMT
WORKDIR /home/user
# Tue, 21 Nov 2023 16:40:54 GMT
USER user
# Tue, 21 Nov 2023 16:40:58 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a2caa6a91dd837ff86958b77bc3534a4003f0cc9611e0b48c76361698bc605`  
		Last Modified: Tue, 21 Nov 2023 16:41:28 GMT  
		Size: 16.7 MB (16741807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6247f0644042c0a753bfe2ff1b7c28d43caaf3330ed88b170167a6fe8a0d35`  
		Last Modified: Tue, 21 Nov 2023 16:41:12 GMT  
		Size: 3.3 KB (3296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb6fda2e80956777959da56923ad2794e7af2f4a510933d7b85d0bf680feb2b`  
		Last Modified: Tue, 21 Nov 2023 16:41:33 GMT  
		Size: 28.0 MB (28007252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5` - linux; ppc64le

```console
$ docker pull irssi@sha256:3f4f99d9914f9e72defad07d78d6e7c12b79184ab4aba83db835de09bc8f75bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82095380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60c6389f9028a4f1e86f03b0bf0bfed6a3d3f45126cdde79535e1136d045b8ff`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 08:14:12 GMT
ENV HOME=/home/user
# Tue, 21 Nov 2023 08:14:13 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Nov 2023 08:14:14 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 08:14:14 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 21 Nov 2023 08:15:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Nov 2023 08:15:10 GMT
WORKDIR /home/user
# Tue, 21 Nov 2023 08:15:10 GMT
USER user
# Tue, 21 Nov 2023 08:15:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990142f84c0c74390b332399beb412942fc74379d8c617ede6f2b0f701fd5f63`  
		Last Modified: Tue, 21 Nov 2023 08:15:42 GMT  
		Size: 18.8 MB (18764965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145cb9bddb869ec0a23e4a981ffb5078fc4852784403e1f0cb05eb86e52276cf`  
		Last Modified: Tue, 21 Nov 2023 08:15:38 GMT  
		Size: 3.4 KB (3371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c79418540c78592e0ce7f96f5df8dd9db310edd58c6f158ba3389cd2290920`  
		Last Modified: Tue, 21 Nov 2023 08:15:43 GMT  
		Size: 30.2 MB (30185437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5` - linux; s390x

```console
$ docker pull irssi@sha256:19d5614ead4badb612e08ba2483418078e52144432cb38d8393c825b31ebe63f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72933796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2a7878077011d582ad7647ec003c06a9ed22ba2e0b5280c344ed18a0f1b8c40`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:42:37 GMT
ADD file:f06f12fa5a93afc3a79ac4371d24b0a471a5a1818cf34c1d90004c8f410914b9 in / 
# Tue, 19 Dec 2023 01:42:39 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:29:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:29:37 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 08:29:37 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 08:29:37 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 08:29:38 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 08:30:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 08:30:17 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 08:30:17 GMT
USER user
# Tue, 19 Dec 2023 08:30:17 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:bc6b1888979d3ceb063da848b2034e980e2c2613642159c1e856550b79aa620c`  
		Last Modified: Tue, 19 Dec 2023 01:47:38 GMT  
		Size: 27.5 MB (27491874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d93a78aafed26613c2aa62cc6ab76d24cde8ba422049c8c4aff454d7e8b6f0`  
		Last Modified: Tue, 19 Dec 2023 08:30:47 GMT  
		Size: 18.2 MB (18210518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506c18d3ee4758db831ecc9a8b1ea9f2562b6972d70a1fb2cd98603a28811f5f`  
		Last Modified: Tue, 19 Dec 2023 08:30:44 GMT  
		Size: 3.4 KB (3376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64e09b7ab558543c54810d6e85b3a3fab5eb5ae4fec9423bfdc282f16c15bcc`  
		Last Modified: Tue, 19 Dec 2023 08:30:48 GMT  
		Size: 27.2 MB (27228028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4.5-alpine`

```console
$ docker pull irssi@sha256:b404269638b505c913a02979a9f253a8e9e904e585c6bb3011b7afbc06908340
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

### `irssi:1.4.5-alpine` - linux; amd64

```console
$ docker pull irssi@sha256:bac3d5c9afaa50fa166d54e4f8a6b82f8519d5f41f60e154925a961f498c67cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18451924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b18b85f03e9dae76ebfd3a15dd2180db03fc5728ce1980f8ae072a7fbbdc15f3`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:28:32 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 05:28:32 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 05:28:33 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 05:28:33 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 05:28:33 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 05:28:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 05:28:52 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 05:28:52 GMT
USER user
# Fri, 01 Dec 2023 05:28:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2253ad6954238459aeb69a5812221ad8d0a9cf6473cb145f43ec969741e3f7c`  
		Last Modified: Fri, 01 Dec 2023 05:29:12 GMT  
		Size: 9.6 MB (9645529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027edf83d9867e80bd5e7041a3da7cbbd50027d7f1e9018f1174b20ca77aea09`  
		Last Modified: Fri, 01 Dec 2023 05:29:10 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf95bf3609411e5c119950c792cabbb3c647eb384dafacbce7a70a601533c44`  
		Last Modified: Fri, 01 Dec 2023 05:29:11 GMT  
		Size: 5.4 MB (5402689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:51601527f7062d912289288c810b48a9d00b3922cef2a58b04787672ff913d07
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17271200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3301b14e65fec26ab44af0807bbcd5ac7cfb9230618a31edcde72367a83b21da`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 01:09:50 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 01:09:50 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 01:09:51 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 01:09:51 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 01:09:51 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 01:10:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 01:10:08 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 01:10:08 GMT
USER user
# Fri, 01 Dec 2023 01:10:08 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0389ed6f59ff0e95c3c6c4566157405d8b3bb4b5a827a5a1fd24edf934393c`  
		Last Modified: Fri, 01 Dec 2023 01:10:22 GMT  
		Size: 8.9 MB (8880077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4039f2bf7cbc0fa8f9a5e8a20f20a5035b388d7a42a95d9d6f0a3a58446eed`  
		Last Modified: Fri, 01 Dec 2023 01:10:19 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184e5e97ecd8a9cf4081a03b9f6a83022561e425f3294a0d09c345420c858123`  
		Last Modified: Fri, 01 Dec 2023 01:10:21 GMT  
		Size: 5.2 MB (5242968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:6ff758c9743e67bc2781d127b56339f483bfbb1251763d398a335d3a95ae9744
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16630768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ba268037301e762641733ac31d7ab82c0538e3658cc00205b6ca74c23bb5332`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:41:57 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 08:41:57 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 08:41:57 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 08:41:57 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 08:41:57 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 08:42:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 08:42:12 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 08:42:12 GMT
USER user
# Fri, 01 Dec 2023 08:42:12 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505553baa092b1ac5dc9c2a961456e9728d5bfe4d15f5a93644f58c1a0c75d14`  
		Last Modified: Fri, 01 Dec 2023 08:42:31 GMT  
		Size: 8.7 MB (8721323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc7d412e24534e4f0eebe098495c5878f5184667c4180f22eb8b50bff5d78cf`  
		Last Modified: Fri, 01 Dec 2023 08:42:29 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d25439b4dd4f4d92fd4be67af55606656fd511d66a1f63715b0dd6d2eeab5b`  
		Last Modified: Fri, 01 Dec 2023 08:42:30 GMT  
		Size: 5.0 MB (5007154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:444032f59c771f9f8ecc9f1374f55b4f94016696d5e58a0931e61ae604748369
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18316372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a03091ab8bcbd9db84ead2d162e748af025192b4ebc302c6a42bd11b034e026b`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:37:23 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 09:37:23 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 09:37:24 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 09:37:24 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 09:37:24 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 09:37:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 09:37:36 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 09:37:36 GMT
USER user
# Fri, 01 Dec 2023 09:37:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408050d673681e97a81fefc3f0d62dc535741ab369d0f890dfd492fea579fc73`  
		Last Modified: Fri, 01 Dec 2023 09:37:55 GMT  
		Size: 9.7 MB (9672911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b351c7a82544307a7a55c5daa20a529cd389facb270805cea95b2040f8b864`  
		Last Modified: Fri, 01 Dec 2023 09:37:53 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad688b9a5733e1a4e2feaddf0a4ae2395f72b5d718efc48685befed72ad2d440`  
		Last Modified: Fri, 01 Dec 2023 09:37:54 GMT  
		Size: 5.3 MB (5309143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-alpine` - linux; 386

```console
$ docker pull irssi@sha256:cb5e5eb3ce2e5c8a080af15a2414c7078412473c44bfe7c15196f957fdd3931b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17557886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e422f2a321a825ce4ac90dad135af83afa3ee86cd59d10d667a313c1b2ec35a7`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 01 Dec 2023 02:03:44 GMT
ADD file:92902088cd15ed8f5dca2f7fc6570fb4e4824fac8b09e091c88e96bbd0ca814b in / 
# Fri, 01 Dec 2023 02:03:44 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:02:03 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 09:02:03 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 09:02:03 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 09:02:04 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 09:02:04 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 09:02:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 09:02:38 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 09:02:38 GMT
USER user
# Fri, 01 Dec 2023 09:02:38 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4966a8bd129b0a6adf93dc295a8fbe8f665d3194a684a5ce199c1c3596dbf3d9`  
		Last Modified: Fri, 01 Dec 2023 02:04:18 GMT  
		Size: 3.2 MB (3238831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194fdb04cb3e17be198ec377fafeb3f5716927ef33b40df425a942b4f3f7e50`  
		Last Modified: Fri, 01 Dec 2023 09:03:00 GMT  
		Size: 8.9 MB (8904478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc41f0a0151cdbeed763c916854e38b017669921f3a79d0554e77543dcb09acb`  
		Last Modified: Fri, 01 Dec 2023 09:02:57 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5a928454e9d9ee194c2842f26954fc39b31e235b0de4f542f9acc45af1737f`  
		Last Modified: Fri, 01 Dec 2023 09:02:58 GMT  
		Size: 5.4 MB (5413293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:e3eba53096e51def6997bdc72c51cf88f0019645321ee59bdd20b49b4236a617
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18717510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:890fc74fc94817011bde8d06e7b449e6407828cbbff17d07e69de027ad3d77f4`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:04:09 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 05:04:12 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 05:04:20 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 05:04:21 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 05:04:21 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 05:04:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 05:04:59 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 05:05:00 GMT
USER user
# Fri, 01 Dec 2023 05:05:02 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5afc2e0a7e24376eade504bc1d0aee8fa44d1b246f3121de324296a57c0ff25d`  
		Last Modified: Fri, 01 Dec 2023 05:05:36 GMT  
		Size: 9.7 MB (9736497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04ef92e3c12ead968e636f09604f92720ce8750a3a7f114277c2ef6764219b6`  
		Last Modified: Fri, 01 Dec 2023 05:05:34 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce0f8ba67064d14f75d9e13652d96ba1e13e489eff4d5617c0e503e25106009`  
		Last Modified: Fri, 01 Dec 2023 05:05:35 GMT  
		Size: 5.6 MB (5631406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:2f5751ebf70dce38c6c48dc4a4e7f72bdae9824a0da9b3b95c277c755139592c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18708403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30063d82b1a526f916c2be961b95561fad91acd4ecfa2942d616740be6105a20`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:13:12 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 08:13:13 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 08:13:13 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 08:13:14 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 08:13:14 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 08:13:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 08:13:35 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 08:13:35 GMT
USER user
# Fri, 01 Dec 2023 08:13:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c64be9d9a3f22087e689a8436399a73b9fb1f76114c8c4b5740080a6d178c9b`  
		Last Modified: Fri, 01 Dec 2023 08:14:02 GMT  
		Size: 10.1 MB (10083001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403430efaca857233fd4cc970775e8fb9b2bfa68899058f8046852bf2a25be16`  
		Last Modified: Fri, 01 Dec 2023 08:13:59 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9630989fe7d8e6fcb8d2886d67968d8118d654dbaa9787a1e4050fe5d293e589`  
		Last Modified: Fri, 01 Dec 2023 08:14:00 GMT  
		Size: 5.4 MB (5406662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4.5-alpine3.18`

```console
$ docker pull irssi@sha256:b404269638b505c913a02979a9f253a8e9e904e585c6bb3011b7afbc06908340
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

### `irssi:1.4.5-alpine3.18` - linux; amd64

```console
$ docker pull irssi@sha256:bac3d5c9afaa50fa166d54e4f8a6b82f8519d5f41f60e154925a961f498c67cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18451924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b18b85f03e9dae76ebfd3a15dd2180db03fc5728ce1980f8ae072a7fbbdc15f3`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:28:32 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 05:28:32 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 05:28:33 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 05:28:33 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 05:28:33 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 05:28:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 05:28:52 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 05:28:52 GMT
USER user
# Fri, 01 Dec 2023 05:28:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2253ad6954238459aeb69a5812221ad8d0a9cf6473cb145f43ec969741e3f7c`  
		Last Modified: Fri, 01 Dec 2023 05:29:12 GMT  
		Size: 9.6 MB (9645529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027edf83d9867e80bd5e7041a3da7cbbd50027d7f1e9018f1174b20ca77aea09`  
		Last Modified: Fri, 01 Dec 2023 05:29:10 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf95bf3609411e5c119950c792cabbb3c647eb384dafacbce7a70a601533c44`  
		Last Modified: Fri, 01 Dec 2023 05:29:11 GMT  
		Size: 5.4 MB (5402689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-alpine3.18` - linux; arm variant v6

```console
$ docker pull irssi@sha256:51601527f7062d912289288c810b48a9d00b3922cef2a58b04787672ff913d07
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17271200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3301b14e65fec26ab44af0807bbcd5ac7cfb9230618a31edcde72367a83b21da`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 01:09:50 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 01:09:50 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 01:09:51 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 01:09:51 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 01:09:51 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 01:10:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 01:10:08 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 01:10:08 GMT
USER user
# Fri, 01 Dec 2023 01:10:08 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0389ed6f59ff0e95c3c6c4566157405d8b3bb4b5a827a5a1fd24edf934393c`  
		Last Modified: Fri, 01 Dec 2023 01:10:22 GMT  
		Size: 8.9 MB (8880077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4039f2bf7cbc0fa8f9a5e8a20f20a5035b388d7a42a95d9d6f0a3a58446eed`  
		Last Modified: Fri, 01 Dec 2023 01:10:19 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184e5e97ecd8a9cf4081a03b9f6a83022561e425f3294a0d09c345420c858123`  
		Last Modified: Fri, 01 Dec 2023 01:10:21 GMT  
		Size: 5.2 MB (5242968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-alpine3.18` - linux; arm variant v7

```console
$ docker pull irssi@sha256:6ff758c9743e67bc2781d127b56339f483bfbb1251763d398a335d3a95ae9744
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16630768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ba268037301e762641733ac31d7ab82c0538e3658cc00205b6ca74c23bb5332`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:41:57 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 08:41:57 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 08:41:57 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 08:41:57 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 08:41:57 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 08:42:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 08:42:12 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 08:42:12 GMT
USER user
# Fri, 01 Dec 2023 08:42:12 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505553baa092b1ac5dc9c2a961456e9728d5bfe4d15f5a93644f58c1a0c75d14`  
		Last Modified: Fri, 01 Dec 2023 08:42:31 GMT  
		Size: 8.7 MB (8721323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc7d412e24534e4f0eebe098495c5878f5184667c4180f22eb8b50bff5d78cf`  
		Last Modified: Fri, 01 Dec 2023 08:42:29 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d25439b4dd4f4d92fd4be67af55606656fd511d66a1f63715b0dd6d2eeab5b`  
		Last Modified: Fri, 01 Dec 2023 08:42:30 GMT  
		Size: 5.0 MB (5007154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:444032f59c771f9f8ecc9f1374f55b4f94016696d5e58a0931e61ae604748369
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18316372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a03091ab8bcbd9db84ead2d162e748af025192b4ebc302c6a42bd11b034e026b`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:37:23 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 09:37:23 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 09:37:24 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 09:37:24 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 09:37:24 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 09:37:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 09:37:36 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 09:37:36 GMT
USER user
# Fri, 01 Dec 2023 09:37:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408050d673681e97a81fefc3f0d62dc535741ab369d0f890dfd492fea579fc73`  
		Last Modified: Fri, 01 Dec 2023 09:37:55 GMT  
		Size: 9.7 MB (9672911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b351c7a82544307a7a55c5daa20a529cd389facb270805cea95b2040f8b864`  
		Last Modified: Fri, 01 Dec 2023 09:37:53 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad688b9a5733e1a4e2feaddf0a4ae2395f72b5d718efc48685befed72ad2d440`  
		Last Modified: Fri, 01 Dec 2023 09:37:54 GMT  
		Size: 5.3 MB (5309143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-alpine3.18` - linux; 386

```console
$ docker pull irssi@sha256:cb5e5eb3ce2e5c8a080af15a2414c7078412473c44bfe7c15196f957fdd3931b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17557886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e422f2a321a825ce4ac90dad135af83afa3ee86cd59d10d667a313c1b2ec35a7`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 01 Dec 2023 02:03:44 GMT
ADD file:92902088cd15ed8f5dca2f7fc6570fb4e4824fac8b09e091c88e96bbd0ca814b in / 
# Fri, 01 Dec 2023 02:03:44 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:02:03 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 09:02:03 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 09:02:03 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 09:02:04 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 09:02:04 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 09:02:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 09:02:38 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 09:02:38 GMT
USER user
# Fri, 01 Dec 2023 09:02:38 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4966a8bd129b0a6adf93dc295a8fbe8f665d3194a684a5ce199c1c3596dbf3d9`  
		Last Modified: Fri, 01 Dec 2023 02:04:18 GMT  
		Size: 3.2 MB (3238831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194fdb04cb3e17be198ec377fafeb3f5716927ef33b40df425a942b4f3f7e50`  
		Last Modified: Fri, 01 Dec 2023 09:03:00 GMT  
		Size: 8.9 MB (8904478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc41f0a0151cdbeed763c916854e38b017669921f3a79d0554e77543dcb09acb`  
		Last Modified: Fri, 01 Dec 2023 09:02:57 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5a928454e9d9ee194c2842f26954fc39b31e235b0de4f542f9acc45af1737f`  
		Last Modified: Fri, 01 Dec 2023 09:02:58 GMT  
		Size: 5.4 MB (5413293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-alpine3.18` - linux; ppc64le

```console
$ docker pull irssi@sha256:e3eba53096e51def6997bdc72c51cf88f0019645321ee59bdd20b49b4236a617
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18717510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:890fc74fc94817011bde8d06e7b449e6407828cbbff17d07e69de027ad3d77f4`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:04:09 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 05:04:12 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 05:04:20 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 05:04:21 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 05:04:21 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 05:04:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 05:04:59 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 05:05:00 GMT
USER user
# Fri, 01 Dec 2023 05:05:02 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5afc2e0a7e24376eade504bc1d0aee8fa44d1b246f3121de324296a57c0ff25d`  
		Last Modified: Fri, 01 Dec 2023 05:05:36 GMT  
		Size: 9.7 MB (9736497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04ef92e3c12ead968e636f09604f92720ce8750a3a7f114277c2ef6764219b6`  
		Last Modified: Fri, 01 Dec 2023 05:05:34 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce0f8ba67064d14f75d9e13652d96ba1e13e489eff4d5617c0e503e25106009`  
		Last Modified: Fri, 01 Dec 2023 05:05:35 GMT  
		Size: 5.6 MB (5631406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-alpine3.18` - linux; s390x

```console
$ docker pull irssi@sha256:2f5751ebf70dce38c6c48dc4a4e7f72bdae9824a0da9b3b95c277c755139592c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18708403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30063d82b1a526f916c2be961b95561fad91acd4ecfa2942d616740be6105a20`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:13:12 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 08:13:13 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 08:13:13 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 08:13:14 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 08:13:14 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 08:13:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 08:13:35 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 08:13:35 GMT
USER user
# Fri, 01 Dec 2023 08:13:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c64be9d9a3f22087e689a8436399a73b9fb1f76114c8c4b5740080a6d178c9b`  
		Last Modified: Fri, 01 Dec 2023 08:14:02 GMT  
		Size: 10.1 MB (10083001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403430efaca857233fd4cc970775e8fb9b2bfa68899058f8046852bf2a25be16`  
		Last Modified: Fri, 01 Dec 2023 08:13:59 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9630989fe7d8e6fcb8d2886d67968d8118d654dbaa9787a1e4050fe5d293e589`  
		Last Modified: Fri, 01 Dec 2023 08:14:00 GMT  
		Size: 5.4 MB (5406662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4.5-bookworm`

```console
$ docker pull irssi@sha256:9bbaebbdef964fd13f87622f887af48afe01d1ef67ec7152da0e993626f8c347
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

### `irssi:1.4.5-bookworm` - linux; amd64

```console
$ docker pull irssi@sha256:75930e1081143e5ac73cc553fd47dd75a236c5587dad0b13ed4f593d5efec999
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76071375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e784ee8f60cc445019f7f2a00f02a16d18715a384904180fa30548888ea9a9e2`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:27 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Tue, 19 Dec 2023 01:20:28 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:11:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:11:41 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 08:11:42 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 08:11:42 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 08:11:42 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 08:12:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 08:12:22 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 08:12:22 GMT
USER user
# Tue, 19 Dec 2023 08:12:22 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f576257a7efd8fa2eab590d15da13ff3e351ddd5f66e1f18853950d0a847940`  
		Last Modified: Tue, 19 Dec 2023 08:12:41 GMT  
		Size: 18.3 MB (18263304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8709b16d66af9e29995cd9f313628ac25626d9a3b9f14337a489a0b53dede1`  
		Last Modified: Tue, 19 Dec 2023 08:12:37 GMT  
		Size: 3.4 KB (3376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4721ae122aaf701fec4c0ab60bcd8186c440f5439303bb23fc19aaa3cc886e`  
		Last Modified: Tue, 19 Dec 2023 08:12:42 GMT  
		Size: 28.7 MB (28678732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-bookworm` - linux; arm variant v5

```console
$ docker pull irssi@sha256:54f4b6e9ea13a0ad57b6507d166cc7d60f705a1f0fb2c8b1a21ccf71be8b4817
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70247719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f71b3c5dc081e54b3f8c57c1d3be303a0147a4ac5656f26d0698b3673bce8f5`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:55:22 GMT
ADD file:9503ab966c9dd707eeccc7c2f633bccc94c199f8714ec4ff2c8b54dde3dbabf9 in / 
# Tue, 19 Dec 2023 01:55:22 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 05:37:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 05:37:07 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 05:37:08 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 05:37:08 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 05:37:08 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 05:37:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 05:37:54 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 05:37:54 GMT
USER user
# Tue, 19 Dec 2023 05:37:54 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1ae9a2844c8c70942d2220553689b62e841cc706d77284fbfedbd770080fd699`  
		Last Modified: Tue, 19 Dec 2023 01:58:33 GMT  
		Size: 26.9 MB (26885440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8c63a38cdf609e2fc7e6adb6d2a2ddee5ee1e185ced4c5667fa93153ddaca4`  
		Last Modified: Tue, 19 Dec 2023 05:38:20 GMT  
		Size: 17.0 MB (17034518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5baba07d2ad153cdc8a55cf44e4e53c2d24eccd878b7c013029ad93e53dad92b`  
		Last Modified: Tue, 19 Dec 2023 05:38:15 GMT  
		Size: 3.4 KB (3382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b675c572666d53e7aaee086d9f3a892e01803b6b84ab820ee1100726092e714`  
		Last Modified: Tue, 19 Dec 2023 05:38:21 GMT  
		Size: 26.3 MB (26324379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-bookworm` - linux; arm variant v7

```console
$ docker pull irssi@sha256:b58087a750d2ecb0db246fa2b83fce92398c136af518ddc7bcae63e75637be1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66568253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0abed9b964bf4864c88c0c97e43a26973a28db129f9679f226eba9307dd515ec`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 02:07:50 GMT
ADD file:aef112919e7924ad6da32181b1df5099cd692680c104118da3a24cd4dfe55a1d in / 
# Tue, 19 Dec 2023 02:07:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:25:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:25:13 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 08:25:13 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 08:25:14 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 08:25:14 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 08:25:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 08:25:50 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 08:25:50 GMT
USER user
# Tue, 19 Dec 2023 08:25:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:65ab19615c01a3b542f77fadb3bd27872b6a20cba3e9269fb951de36d8fa6805`  
		Last Modified: Tue, 19 Dec 2023 02:11:52 GMT  
		Size: 24.7 MB (24718157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34312fc906c50709273b2bfc296cbc5e618081aab636bea0270e632aa1250a58`  
		Last Modified: Tue, 19 Dec 2023 08:26:13 GMT  
		Size: 16.6 MB (16626329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ae59c8630536591ee4c9f224e24066f5ea55d87cd4d710f4758493e40f4d90`  
		Last Modified: Tue, 19 Dec 2023 08:26:07 GMT  
		Size: 3.4 KB (3375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653d387ba5d23d5a1d3207409abeb6f1857445f450f723a518d7f30d8305a612`  
		Last Modified: Tue, 19 Dec 2023 08:26:13 GMT  
		Size: 25.2 MB (25220392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-bookworm` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:ca5674fca34098dff53db48ae2b739f5bf5deef41b342fe154e13d37c4ca22d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74826194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e84ec8b67ce32fad14adb38e81b191c731737445551e607aadf4cb648de22d25`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:11 GMT
ADD file:262fd7bf0bc26e5d2a229fba52626e22b8a93beac29733acfc60e716c26e689d in / 
# Tue, 19 Dec 2023 01:41:11 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:35:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 07:35:16 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 07:35:17 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 07:35:17 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 07:35:17 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 07:35:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 07:35:50 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 07:35:50 GMT
USER user
# Tue, 19 Dec 2023 07:35:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:24e221e92a36ab5b0075dd156b4f2ff095532a9b0927946cf6070bb1bea208b8`  
		Last Modified: Tue, 19 Dec 2023 01:44:38 GMT  
		Size: 29.2 MB (29157269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3b65976afca6b69a78f82bba0cfd53e915de68b3497418795c0fe90dde04d6`  
		Last Modified: Tue, 19 Dec 2023 07:36:07 GMT  
		Size: 18.0 MB (18025714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1487d5e5dd099dea8c8f5cfa983386ef698d0b7ba74af27991d128c2eb77509a`  
		Last Modified: Tue, 19 Dec 2023 07:36:04 GMT  
		Size: 3.4 KB (3375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027137ab6d543546e67a802c5b15757aae71ceb8e7be44d4ab7e3701b466102e`  
		Last Modified: Tue, 19 Dec 2023 07:36:07 GMT  
		Size: 27.6 MB (27639836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-bookworm` - linux; 386

```console
$ docker pull irssi@sha256:f4a77a97b8bd86a99d34d5fb0a8786e1a8f95758005b4ba99deb96a2b24d589a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76522898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e29421276ec13208c270be47f6eb04f62363c92fbf673bd983a1aa520e2fedc`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Nov 2023 04:39:53 GMT
ADD file:930e1b9d85b6927c4d3046f7c75de2f3bfc6ec29100c314d0ab2b780ea30e962 in / 
# Tue, 21 Nov 2023 04:39:53 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:18:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:18:00 GMT
ENV HOME=/home/user
# Tue, 21 Nov 2023 09:18:01 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Nov 2023 09:18:01 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 09:18:01 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 21 Nov 2023 09:18:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Nov 2023 09:18:58 GMT
WORKDIR /home/user
# Tue, 21 Nov 2023 09:18:58 GMT
USER user
# Tue, 21 Nov 2023 09:18:58 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c0734eabce8885d8904dbd11b77aa97c2d2b04bc8e2af9e89d47c4bda590dd8e`  
		Last Modified: Tue, 21 Nov 2023 04:44:34 GMT  
		Size: 30.2 MB (30164109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd0a88ad6c1f45a640f6b1e3509a00f0489ea5e7317905ff14b60fca6f24086`  
		Last Modified: Tue, 21 Nov 2023 09:19:21 GMT  
		Size: 17.8 MB (17789102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e785a0b684a75cef890d58447965564ea0ab287ad9b7fa38d00a4e9cfe5de7`  
		Last Modified: Tue, 21 Nov 2023 09:19:15 GMT  
		Size: 3.4 KB (3372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397cc87253be0de402ae3c1da69d2224514616b57b478236526d9f020d3b6ad6`  
		Last Modified: Tue, 21 Nov 2023 09:19:23 GMT  
		Size: 28.6 MB (28566315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-bookworm` - linux; mips64le

```console
$ docker pull irssi@sha256:9c4985936b28f111411e9b54fe41acdb3b06222c5e22b4783ac53322ddf57794
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73894339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:370cd0afda43f756d5b75c9726905baa31206388d01ef49a763d8e033950a631`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 16:36:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 16:36:50 GMT
ENV HOME=/home/user
# Tue, 21 Nov 2023 16:36:56 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Nov 2023 16:37:00 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 16:37:03 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 21 Nov 2023 16:40:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Nov 2023 16:40:50 GMT
WORKDIR /home/user
# Tue, 21 Nov 2023 16:40:54 GMT
USER user
# Tue, 21 Nov 2023 16:40:58 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a2caa6a91dd837ff86958b77bc3534a4003f0cc9611e0b48c76361698bc605`  
		Last Modified: Tue, 21 Nov 2023 16:41:28 GMT  
		Size: 16.7 MB (16741807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6247f0644042c0a753bfe2ff1b7c28d43caaf3330ed88b170167a6fe8a0d35`  
		Last Modified: Tue, 21 Nov 2023 16:41:12 GMT  
		Size: 3.3 KB (3296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb6fda2e80956777959da56923ad2794e7af2f4a510933d7b85d0bf680feb2b`  
		Last Modified: Tue, 21 Nov 2023 16:41:33 GMT  
		Size: 28.0 MB (28007252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-bookworm` - linux; ppc64le

```console
$ docker pull irssi@sha256:3f4f99d9914f9e72defad07d78d6e7c12b79184ab4aba83db835de09bc8f75bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82095380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60c6389f9028a4f1e86f03b0bf0bfed6a3d3f45126cdde79535e1136d045b8ff`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 08:14:12 GMT
ENV HOME=/home/user
# Tue, 21 Nov 2023 08:14:13 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Nov 2023 08:14:14 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 08:14:14 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 21 Nov 2023 08:15:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Nov 2023 08:15:10 GMT
WORKDIR /home/user
# Tue, 21 Nov 2023 08:15:10 GMT
USER user
# Tue, 21 Nov 2023 08:15:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990142f84c0c74390b332399beb412942fc74379d8c617ede6f2b0f701fd5f63`  
		Last Modified: Tue, 21 Nov 2023 08:15:42 GMT  
		Size: 18.8 MB (18764965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145cb9bddb869ec0a23e4a981ffb5078fc4852784403e1f0cb05eb86e52276cf`  
		Last Modified: Tue, 21 Nov 2023 08:15:38 GMT  
		Size: 3.4 KB (3371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c79418540c78592e0ce7f96f5df8dd9db310edd58c6f158ba3389cd2290920`  
		Last Modified: Tue, 21 Nov 2023 08:15:43 GMT  
		Size: 30.2 MB (30185437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-bookworm` - linux; s390x

```console
$ docker pull irssi@sha256:19d5614ead4badb612e08ba2483418078e52144432cb38d8393c825b31ebe63f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72933796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2a7878077011d582ad7647ec003c06a9ed22ba2e0b5280c344ed18a0f1b8c40`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:42:37 GMT
ADD file:f06f12fa5a93afc3a79ac4371d24b0a471a5a1818cf34c1d90004c8f410914b9 in / 
# Tue, 19 Dec 2023 01:42:39 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:29:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:29:37 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 08:29:37 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 08:29:37 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 08:29:38 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 08:30:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 08:30:17 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 08:30:17 GMT
USER user
# Tue, 19 Dec 2023 08:30:17 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:bc6b1888979d3ceb063da848b2034e980e2c2613642159c1e856550b79aa620c`  
		Last Modified: Tue, 19 Dec 2023 01:47:38 GMT  
		Size: 27.5 MB (27491874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d93a78aafed26613c2aa62cc6ab76d24cde8ba422049c8c4aff454d7e8b6f0`  
		Last Modified: Tue, 19 Dec 2023 08:30:47 GMT  
		Size: 18.2 MB (18210518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506c18d3ee4758db831ecc9a8b1ea9f2562b6972d70a1fb2cd98603a28811f5f`  
		Last Modified: Tue, 19 Dec 2023 08:30:44 GMT  
		Size: 3.4 KB (3376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64e09b7ab558543c54810d6e85b3a3fab5eb5ae4fec9423bfdc282f16c15bcc`  
		Last Modified: Tue, 19 Dec 2023 08:30:48 GMT  
		Size: 27.2 MB (27228028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:alpine`

```console
$ docker pull irssi@sha256:b404269638b505c913a02979a9f253a8e9e904e585c6bb3011b7afbc06908340
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
$ docker pull irssi@sha256:bac3d5c9afaa50fa166d54e4f8a6b82f8519d5f41f60e154925a961f498c67cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18451924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b18b85f03e9dae76ebfd3a15dd2180db03fc5728ce1980f8ae072a7fbbdc15f3`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:28:32 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 05:28:32 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 05:28:33 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 05:28:33 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 05:28:33 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 05:28:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 05:28:52 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 05:28:52 GMT
USER user
# Fri, 01 Dec 2023 05:28:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2253ad6954238459aeb69a5812221ad8d0a9cf6473cb145f43ec969741e3f7c`  
		Last Modified: Fri, 01 Dec 2023 05:29:12 GMT  
		Size: 9.6 MB (9645529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027edf83d9867e80bd5e7041a3da7cbbd50027d7f1e9018f1174b20ca77aea09`  
		Last Modified: Fri, 01 Dec 2023 05:29:10 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf95bf3609411e5c119950c792cabbb3c647eb384dafacbce7a70a601533c44`  
		Last Modified: Fri, 01 Dec 2023 05:29:11 GMT  
		Size: 5.4 MB (5402689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:51601527f7062d912289288c810b48a9d00b3922cef2a58b04787672ff913d07
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17271200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3301b14e65fec26ab44af0807bbcd5ac7cfb9230618a31edcde72367a83b21da`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 01:09:50 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 01:09:50 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 01:09:51 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 01:09:51 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 01:09:51 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 01:10:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 01:10:08 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 01:10:08 GMT
USER user
# Fri, 01 Dec 2023 01:10:08 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0389ed6f59ff0e95c3c6c4566157405d8b3bb4b5a827a5a1fd24edf934393c`  
		Last Modified: Fri, 01 Dec 2023 01:10:22 GMT  
		Size: 8.9 MB (8880077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4039f2bf7cbc0fa8f9a5e8a20f20a5035b388d7a42a95d9d6f0a3a58446eed`  
		Last Modified: Fri, 01 Dec 2023 01:10:19 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184e5e97ecd8a9cf4081a03b9f6a83022561e425f3294a0d09c345420c858123`  
		Last Modified: Fri, 01 Dec 2023 01:10:21 GMT  
		Size: 5.2 MB (5242968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:6ff758c9743e67bc2781d127b56339f483bfbb1251763d398a335d3a95ae9744
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16630768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ba268037301e762641733ac31d7ab82c0538e3658cc00205b6ca74c23bb5332`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:41:57 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 08:41:57 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 08:41:57 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 08:41:57 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 08:41:57 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 08:42:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 08:42:12 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 08:42:12 GMT
USER user
# Fri, 01 Dec 2023 08:42:12 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505553baa092b1ac5dc9c2a961456e9728d5bfe4d15f5a93644f58c1a0c75d14`  
		Last Modified: Fri, 01 Dec 2023 08:42:31 GMT  
		Size: 8.7 MB (8721323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc7d412e24534e4f0eebe098495c5878f5184667c4180f22eb8b50bff5d78cf`  
		Last Modified: Fri, 01 Dec 2023 08:42:29 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d25439b4dd4f4d92fd4be67af55606656fd511d66a1f63715b0dd6d2eeab5b`  
		Last Modified: Fri, 01 Dec 2023 08:42:30 GMT  
		Size: 5.0 MB (5007154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:444032f59c771f9f8ecc9f1374f55b4f94016696d5e58a0931e61ae604748369
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18316372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a03091ab8bcbd9db84ead2d162e748af025192b4ebc302c6a42bd11b034e026b`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:37:23 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 09:37:23 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 09:37:24 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 09:37:24 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 09:37:24 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 09:37:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 09:37:36 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 09:37:36 GMT
USER user
# Fri, 01 Dec 2023 09:37:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408050d673681e97a81fefc3f0d62dc535741ab369d0f890dfd492fea579fc73`  
		Last Modified: Fri, 01 Dec 2023 09:37:55 GMT  
		Size: 9.7 MB (9672911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b351c7a82544307a7a55c5daa20a529cd389facb270805cea95b2040f8b864`  
		Last Modified: Fri, 01 Dec 2023 09:37:53 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad688b9a5733e1a4e2feaddf0a4ae2395f72b5d718efc48685befed72ad2d440`  
		Last Modified: Fri, 01 Dec 2023 09:37:54 GMT  
		Size: 5.3 MB (5309143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; 386

```console
$ docker pull irssi@sha256:cb5e5eb3ce2e5c8a080af15a2414c7078412473c44bfe7c15196f957fdd3931b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17557886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e422f2a321a825ce4ac90dad135af83afa3ee86cd59d10d667a313c1b2ec35a7`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 01 Dec 2023 02:03:44 GMT
ADD file:92902088cd15ed8f5dca2f7fc6570fb4e4824fac8b09e091c88e96bbd0ca814b in / 
# Fri, 01 Dec 2023 02:03:44 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:02:03 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 09:02:03 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 09:02:03 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 09:02:04 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 09:02:04 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 09:02:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 09:02:38 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 09:02:38 GMT
USER user
# Fri, 01 Dec 2023 09:02:38 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4966a8bd129b0a6adf93dc295a8fbe8f665d3194a684a5ce199c1c3596dbf3d9`  
		Last Modified: Fri, 01 Dec 2023 02:04:18 GMT  
		Size: 3.2 MB (3238831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194fdb04cb3e17be198ec377fafeb3f5716927ef33b40df425a942b4f3f7e50`  
		Last Modified: Fri, 01 Dec 2023 09:03:00 GMT  
		Size: 8.9 MB (8904478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc41f0a0151cdbeed763c916854e38b017669921f3a79d0554e77543dcb09acb`  
		Last Modified: Fri, 01 Dec 2023 09:02:57 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5a928454e9d9ee194c2842f26954fc39b31e235b0de4f542f9acc45af1737f`  
		Last Modified: Fri, 01 Dec 2023 09:02:58 GMT  
		Size: 5.4 MB (5413293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:e3eba53096e51def6997bdc72c51cf88f0019645321ee59bdd20b49b4236a617
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18717510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:890fc74fc94817011bde8d06e7b449e6407828cbbff17d07e69de027ad3d77f4`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:04:09 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 05:04:12 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 05:04:20 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 05:04:21 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 05:04:21 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 05:04:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 05:04:59 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 05:05:00 GMT
USER user
# Fri, 01 Dec 2023 05:05:02 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5afc2e0a7e24376eade504bc1d0aee8fa44d1b246f3121de324296a57c0ff25d`  
		Last Modified: Fri, 01 Dec 2023 05:05:36 GMT  
		Size: 9.7 MB (9736497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04ef92e3c12ead968e636f09604f92720ce8750a3a7f114277c2ef6764219b6`  
		Last Modified: Fri, 01 Dec 2023 05:05:34 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce0f8ba67064d14f75d9e13652d96ba1e13e489eff4d5617c0e503e25106009`  
		Last Modified: Fri, 01 Dec 2023 05:05:35 GMT  
		Size: 5.6 MB (5631406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; s390x

```console
$ docker pull irssi@sha256:2f5751ebf70dce38c6c48dc4a4e7f72bdae9824a0da9b3b95c277c755139592c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18708403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30063d82b1a526f916c2be961b95561fad91acd4ecfa2942d616740be6105a20`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:13:12 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 08:13:13 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 08:13:13 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 08:13:14 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 08:13:14 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 08:13:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 08:13:35 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 08:13:35 GMT
USER user
# Fri, 01 Dec 2023 08:13:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c64be9d9a3f22087e689a8436399a73b9fb1f76114c8c4b5740080a6d178c9b`  
		Last Modified: Fri, 01 Dec 2023 08:14:02 GMT  
		Size: 10.1 MB (10083001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403430efaca857233fd4cc970775e8fb9b2bfa68899058f8046852bf2a25be16`  
		Last Modified: Fri, 01 Dec 2023 08:13:59 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9630989fe7d8e6fcb8d2886d67968d8118d654dbaa9787a1e4050fe5d293e589`  
		Last Modified: Fri, 01 Dec 2023 08:14:00 GMT  
		Size: 5.4 MB (5406662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:alpine3.18`

```console
$ docker pull irssi@sha256:b404269638b505c913a02979a9f253a8e9e904e585c6bb3011b7afbc06908340
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

### `irssi:alpine3.18` - linux; amd64

```console
$ docker pull irssi@sha256:bac3d5c9afaa50fa166d54e4f8a6b82f8519d5f41f60e154925a961f498c67cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18451924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b18b85f03e9dae76ebfd3a15dd2180db03fc5728ce1980f8ae072a7fbbdc15f3`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:28:32 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 05:28:32 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 05:28:33 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 05:28:33 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 05:28:33 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 05:28:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 05:28:52 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 05:28:52 GMT
USER user
# Fri, 01 Dec 2023 05:28:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2253ad6954238459aeb69a5812221ad8d0a9cf6473cb145f43ec969741e3f7c`  
		Last Modified: Fri, 01 Dec 2023 05:29:12 GMT  
		Size: 9.6 MB (9645529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027edf83d9867e80bd5e7041a3da7cbbd50027d7f1e9018f1174b20ca77aea09`  
		Last Modified: Fri, 01 Dec 2023 05:29:10 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf95bf3609411e5c119950c792cabbb3c647eb384dafacbce7a70a601533c44`  
		Last Modified: Fri, 01 Dec 2023 05:29:11 GMT  
		Size: 5.4 MB (5402689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine3.18` - linux; arm variant v6

```console
$ docker pull irssi@sha256:51601527f7062d912289288c810b48a9d00b3922cef2a58b04787672ff913d07
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17271200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3301b14e65fec26ab44af0807bbcd5ac7cfb9230618a31edcde72367a83b21da`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 01:09:50 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 01:09:50 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 01:09:51 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 01:09:51 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 01:09:51 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 01:10:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 01:10:08 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 01:10:08 GMT
USER user
# Fri, 01 Dec 2023 01:10:08 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0389ed6f59ff0e95c3c6c4566157405d8b3bb4b5a827a5a1fd24edf934393c`  
		Last Modified: Fri, 01 Dec 2023 01:10:22 GMT  
		Size: 8.9 MB (8880077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4039f2bf7cbc0fa8f9a5e8a20f20a5035b388d7a42a95d9d6f0a3a58446eed`  
		Last Modified: Fri, 01 Dec 2023 01:10:19 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184e5e97ecd8a9cf4081a03b9f6a83022561e425f3294a0d09c345420c858123`  
		Last Modified: Fri, 01 Dec 2023 01:10:21 GMT  
		Size: 5.2 MB (5242968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine3.18` - linux; arm variant v7

```console
$ docker pull irssi@sha256:6ff758c9743e67bc2781d127b56339f483bfbb1251763d398a335d3a95ae9744
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16630768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ba268037301e762641733ac31d7ab82c0538e3658cc00205b6ca74c23bb5332`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:41:57 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 08:41:57 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 08:41:57 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 08:41:57 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 08:41:57 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 08:42:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 08:42:12 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 08:42:12 GMT
USER user
# Fri, 01 Dec 2023 08:42:12 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505553baa092b1ac5dc9c2a961456e9728d5bfe4d15f5a93644f58c1a0c75d14`  
		Last Modified: Fri, 01 Dec 2023 08:42:31 GMT  
		Size: 8.7 MB (8721323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc7d412e24534e4f0eebe098495c5878f5184667c4180f22eb8b50bff5d78cf`  
		Last Modified: Fri, 01 Dec 2023 08:42:29 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d25439b4dd4f4d92fd4be67af55606656fd511d66a1f63715b0dd6d2eeab5b`  
		Last Modified: Fri, 01 Dec 2023 08:42:30 GMT  
		Size: 5.0 MB (5007154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine3.18` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:444032f59c771f9f8ecc9f1374f55b4f94016696d5e58a0931e61ae604748369
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18316372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a03091ab8bcbd9db84ead2d162e748af025192b4ebc302c6a42bd11b034e026b`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:37:23 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 09:37:23 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 09:37:24 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 09:37:24 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 09:37:24 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 09:37:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 09:37:36 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 09:37:36 GMT
USER user
# Fri, 01 Dec 2023 09:37:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408050d673681e97a81fefc3f0d62dc535741ab369d0f890dfd492fea579fc73`  
		Last Modified: Fri, 01 Dec 2023 09:37:55 GMT  
		Size: 9.7 MB (9672911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b351c7a82544307a7a55c5daa20a529cd389facb270805cea95b2040f8b864`  
		Last Modified: Fri, 01 Dec 2023 09:37:53 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad688b9a5733e1a4e2feaddf0a4ae2395f72b5d718efc48685befed72ad2d440`  
		Last Modified: Fri, 01 Dec 2023 09:37:54 GMT  
		Size: 5.3 MB (5309143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine3.18` - linux; 386

```console
$ docker pull irssi@sha256:cb5e5eb3ce2e5c8a080af15a2414c7078412473c44bfe7c15196f957fdd3931b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17557886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e422f2a321a825ce4ac90dad135af83afa3ee86cd59d10d667a313c1b2ec35a7`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 01 Dec 2023 02:03:44 GMT
ADD file:92902088cd15ed8f5dca2f7fc6570fb4e4824fac8b09e091c88e96bbd0ca814b in / 
# Fri, 01 Dec 2023 02:03:44 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:02:03 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 09:02:03 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 09:02:03 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 09:02:04 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 09:02:04 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 09:02:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 09:02:38 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 09:02:38 GMT
USER user
# Fri, 01 Dec 2023 09:02:38 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4966a8bd129b0a6adf93dc295a8fbe8f665d3194a684a5ce199c1c3596dbf3d9`  
		Last Modified: Fri, 01 Dec 2023 02:04:18 GMT  
		Size: 3.2 MB (3238831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194fdb04cb3e17be198ec377fafeb3f5716927ef33b40df425a942b4f3f7e50`  
		Last Modified: Fri, 01 Dec 2023 09:03:00 GMT  
		Size: 8.9 MB (8904478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc41f0a0151cdbeed763c916854e38b017669921f3a79d0554e77543dcb09acb`  
		Last Modified: Fri, 01 Dec 2023 09:02:57 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5a928454e9d9ee194c2842f26954fc39b31e235b0de4f542f9acc45af1737f`  
		Last Modified: Fri, 01 Dec 2023 09:02:58 GMT  
		Size: 5.4 MB (5413293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine3.18` - linux; ppc64le

```console
$ docker pull irssi@sha256:e3eba53096e51def6997bdc72c51cf88f0019645321ee59bdd20b49b4236a617
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18717510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:890fc74fc94817011bde8d06e7b449e6407828cbbff17d07e69de027ad3d77f4`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:04:09 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 05:04:12 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 05:04:20 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 05:04:21 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 05:04:21 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 05:04:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 05:04:59 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 05:05:00 GMT
USER user
# Fri, 01 Dec 2023 05:05:02 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5afc2e0a7e24376eade504bc1d0aee8fa44d1b246f3121de324296a57c0ff25d`  
		Last Modified: Fri, 01 Dec 2023 05:05:36 GMT  
		Size: 9.7 MB (9736497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04ef92e3c12ead968e636f09604f92720ce8750a3a7f114277c2ef6764219b6`  
		Last Modified: Fri, 01 Dec 2023 05:05:34 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce0f8ba67064d14f75d9e13652d96ba1e13e489eff4d5617c0e503e25106009`  
		Last Modified: Fri, 01 Dec 2023 05:05:35 GMT  
		Size: 5.6 MB (5631406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine3.18` - linux; s390x

```console
$ docker pull irssi@sha256:2f5751ebf70dce38c6c48dc4a4e7f72bdae9824a0da9b3b95c277c755139592c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18708403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30063d82b1a526f916c2be961b95561fad91acd4ecfa2942d616740be6105a20`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:13:12 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 01 Dec 2023 08:13:13 GMT
ENV HOME=/home/user
# Fri, 01 Dec 2023 08:13:13 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 01 Dec 2023 08:13:14 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 08:13:14 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 01 Dec 2023 08:13:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 01 Dec 2023 08:13:35 GMT
WORKDIR /home/user
# Fri, 01 Dec 2023 08:13:35 GMT
USER user
# Fri, 01 Dec 2023 08:13:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c64be9d9a3f22087e689a8436399a73b9fb1f76114c8c4b5740080a6d178c9b`  
		Last Modified: Fri, 01 Dec 2023 08:14:02 GMT  
		Size: 10.1 MB (10083001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403430efaca857233fd4cc970775e8fb9b2bfa68899058f8046852bf2a25be16`  
		Last Modified: Fri, 01 Dec 2023 08:13:59 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9630989fe7d8e6fcb8d2886d67968d8118d654dbaa9787a1e4050fe5d293e589`  
		Last Modified: Fri, 01 Dec 2023 08:14:00 GMT  
		Size: 5.4 MB (5406662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:bookworm`

```console
$ docker pull irssi@sha256:9bbaebbdef964fd13f87622f887af48afe01d1ef67ec7152da0e993626f8c347
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

### `irssi:bookworm` - linux; amd64

```console
$ docker pull irssi@sha256:75930e1081143e5ac73cc553fd47dd75a236c5587dad0b13ed4f593d5efec999
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76071375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e784ee8f60cc445019f7f2a00f02a16d18715a384904180fa30548888ea9a9e2`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:27 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Tue, 19 Dec 2023 01:20:28 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:11:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:11:41 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 08:11:42 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 08:11:42 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 08:11:42 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 08:12:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 08:12:22 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 08:12:22 GMT
USER user
# Tue, 19 Dec 2023 08:12:22 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f576257a7efd8fa2eab590d15da13ff3e351ddd5f66e1f18853950d0a847940`  
		Last Modified: Tue, 19 Dec 2023 08:12:41 GMT  
		Size: 18.3 MB (18263304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8709b16d66af9e29995cd9f313628ac25626d9a3b9f14337a489a0b53dede1`  
		Last Modified: Tue, 19 Dec 2023 08:12:37 GMT  
		Size: 3.4 KB (3376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4721ae122aaf701fec4c0ab60bcd8186c440f5439303bb23fc19aaa3cc886e`  
		Last Modified: Tue, 19 Dec 2023 08:12:42 GMT  
		Size: 28.7 MB (28678732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:bookworm` - linux; arm variant v5

```console
$ docker pull irssi@sha256:54f4b6e9ea13a0ad57b6507d166cc7d60f705a1f0fb2c8b1a21ccf71be8b4817
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70247719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f71b3c5dc081e54b3f8c57c1d3be303a0147a4ac5656f26d0698b3673bce8f5`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:55:22 GMT
ADD file:9503ab966c9dd707eeccc7c2f633bccc94c199f8714ec4ff2c8b54dde3dbabf9 in / 
# Tue, 19 Dec 2023 01:55:22 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 05:37:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 05:37:07 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 05:37:08 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 05:37:08 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 05:37:08 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 05:37:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 05:37:54 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 05:37:54 GMT
USER user
# Tue, 19 Dec 2023 05:37:54 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1ae9a2844c8c70942d2220553689b62e841cc706d77284fbfedbd770080fd699`  
		Last Modified: Tue, 19 Dec 2023 01:58:33 GMT  
		Size: 26.9 MB (26885440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8c63a38cdf609e2fc7e6adb6d2a2ddee5ee1e185ced4c5667fa93153ddaca4`  
		Last Modified: Tue, 19 Dec 2023 05:38:20 GMT  
		Size: 17.0 MB (17034518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5baba07d2ad153cdc8a55cf44e4e53c2d24eccd878b7c013029ad93e53dad92b`  
		Last Modified: Tue, 19 Dec 2023 05:38:15 GMT  
		Size: 3.4 KB (3382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b675c572666d53e7aaee086d9f3a892e01803b6b84ab820ee1100726092e714`  
		Last Modified: Tue, 19 Dec 2023 05:38:21 GMT  
		Size: 26.3 MB (26324379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:bookworm` - linux; arm variant v7

```console
$ docker pull irssi@sha256:b58087a750d2ecb0db246fa2b83fce92398c136af518ddc7bcae63e75637be1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66568253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0abed9b964bf4864c88c0c97e43a26973a28db129f9679f226eba9307dd515ec`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 02:07:50 GMT
ADD file:aef112919e7924ad6da32181b1df5099cd692680c104118da3a24cd4dfe55a1d in / 
# Tue, 19 Dec 2023 02:07:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:25:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:25:13 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 08:25:13 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 08:25:14 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 08:25:14 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 08:25:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 08:25:50 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 08:25:50 GMT
USER user
# Tue, 19 Dec 2023 08:25:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:65ab19615c01a3b542f77fadb3bd27872b6a20cba3e9269fb951de36d8fa6805`  
		Last Modified: Tue, 19 Dec 2023 02:11:52 GMT  
		Size: 24.7 MB (24718157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34312fc906c50709273b2bfc296cbc5e618081aab636bea0270e632aa1250a58`  
		Last Modified: Tue, 19 Dec 2023 08:26:13 GMT  
		Size: 16.6 MB (16626329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ae59c8630536591ee4c9f224e24066f5ea55d87cd4d710f4758493e40f4d90`  
		Last Modified: Tue, 19 Dec 2023 08:26:07 GMT  
		Size: 3.4 KB (3375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653d387ba5d23d5a1d3207409abeb6f1857445f450f723a518d7f30d8305a612`  
		Last Modified: Tue, 19 Dec 2023 08:26:13 GMT  
		Size: 25.2 MB (25220392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:bookworm` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:ca5674fca34098dff53db48ae2b739f5bf5deef41b342fe154e13d37c4ca22d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74826194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e84ec8b67ce32fad14adb38e81b191c731737445551e607aadf4cb648de22d25`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:11 GMT
ADD file:262fd7bf0bc26e5d2a229fba52626e22b8a93beac29733acfc60e716c26e689d in / 
# Tue, 19 Dec 2023 01:41:11 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:35:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 07:35:16 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 07:35:17 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 07:35:17 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 07:35:17 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 07:35:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 07:35:50 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 07:35:50 GMT
USER user
# Tue, 19 Dec 2023 07:35:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:24e221e92a36ab5b0075dd156b4f2ff095532a9b0927946cf6070bb1bea208b8`  
		Last Modified: Tue, 19 Dec 2023 01:44:38 GMT  
		Size: 29.2 MB (29157269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3b65976afca6b69a78f82bba0cfd53e915de68b3497418795c0fe90dde04d6`  
		Last Modified: Tue, 19 Dec 2023 07:36:07 GMT  
		Size: 18.0 MB (18025714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1487d5e5dd099dea8c8f5cfa983386ef698d0b7ba74af27991d128c2eb77509a`  
		Last Modified: Tue, 19 Dec 2023 07:36:04 GMT  
		Size: 3.4 KB (3375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027137ab6d543546e67a802c5b15757aae71ceb8e7be44d4ab7e3701b466102e`  
		Last Modified: Tue, 19 Dec 2023 07:36:07 GMT  
		Size: 27.6 MB (27639836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:bookworm` - linux; 386

```console
$ docker pull irssi@sha256:f4a77a97b8bd86a99d34d5fb0a8786e1a8f95758005b4ba99deb96a2b24d589a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76522898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e29421276ec13208c270be47f6eb04f62363c92fbf673bd983a1aa520e2fedc`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Nov 2023 04:39:53 GMT
ADD file:930e1b9d85b6927c4d3046f7c75de2f3bfc6ec29100c314d0ab2b780ea30e962 in / 
# Tue, 21 Nov 2023 04:39:53 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:18:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:18:00 GMT
ENV HOME=/home/user
# Tue, 21 Nov 2023 09:18:01 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Nov 2023 09:18:01 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 09:18:01 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 21 Nov 2023 09:18:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Nov 2023 09:18:58 GMT
WORKDIR /home/user
# Tue, 21 Nov 2023 09:18:58 GMT
USER user
# Tue, 21 Nov 2023 09:18:58 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c0734eabce8885d8904dbd11b77aa97c2d2b04bc8e2af9e89d47c4bda590dd8e`  
		Last Modified: Tue, 21 Nov 2023 04:44:34 GMT  
		Size: 30.2 MB (30164109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd0a88ad6c1f45a640f6b1e3509a00f0489ea5e7317905ff14b60fca6f24086`  
		Last Modified: Tue, 21 Nov 2023 09:19:21 GMT  
		Size: 17.8 MB (17789102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e785a0b684a75cef890d58447965564ea0ab287ad9b7fa38d00a4e9cfe5de7`  
		Last Modified: Tue, 21 Nov 2023 09:19:15 GMT  
		Size: 3.4 KB (3372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397cc87253be0de402ae3c1da69d2224514616b57b478236526d9f020d3b6ad6`  
		Last Modified: Tue, 21 Nov 2023 09:19:23 GMT  
		Size: 28.6 MB (28566315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:bookworm` - linux; mips64le

```console
$ docker pull irssi@sha256:9c4985936b28f111411e9b54fe41acdb3b06222c5e22b4783ac53322ddf57794
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73894339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:370cd0afda43f756d5b75c9726905baa31206388d01ef49a763d8e033950a631`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 16:36:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 16:36:50 GMT
ENV HOME=/home/user
# Tue, 21 Nov 2023 16:36:56 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Nov 2023 16:37:00 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 16:37:03 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 21 Nov 2023 16:40:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Nov 2023 16:40:50 GMT
WORKDIR /home/user
# Tue, 21 Nov 2023 16:40:54 GMT
USER user
# Tue, 21 Nov 2023 16:40:58 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a2caa6a91dd837ff86958b77bc3534a4003f0cc9611e0b48c76361698bc605`  
		Last Modified: Tue, 21 Nov 2023 16:41:28 GMT  
		Size: 16.7 MB (16741807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6247f0644042c0a753bfe2ff1b7c28d43caaf3330ed88b170167a6fe8a0d35`  
		Last Modified: Tue, 21 Nov 2023 16:41:12 GMT  
		Size: 3.3 KB (3296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb6fda2e80956777959da56923ad2794e7af2f4a510933d7b85d0bf680feb2b`  
		Last Modified: Tue, 21 Nov 2023 16:41:33 GMT  
		Size: 28.0 MB (28007252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:bookworm` - linux; ppc64le

```console
$ docker pull irssi@sha256:3f4f99d9914f9e72defad07d78d6e7c12b79184ab4aba83db835de09bc8f75bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82095380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60c6389f9028a4f1e86f03b0bf0bfed6a3d3f45126cdde79535e1136d045b8ff`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 08:14:12 GMT
ENV HOME=/home/user
# Tue, 21 Nov 2023 08:14:13 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Nov 2023 08:14:14 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 08:14:14 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 21 Nov 2023 08:15:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Nov 2023 08:15:10 GMT
WORKDIR /home/user
# Tue, 21 Nov 2023 08:15:10 GMT
USER user
# Tue, 21 Nov 2023 08:15:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990142f84c0c74390b332399beb412942fc74379d8c617ede6f2b0f701fd5f63`  
		Last Modified: Tue, 21 Nov 2023 08:15:42 GMT  
		Size: 18.8 MB (18764965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145cb9bddb869ec0a23e4a981ffb5078fc4852784403e1f0cb05eb86e52276cf`  
		Last Modified: Tue, 21 Nov 2023 08:15:38 GMT  
		Size: 3.4 KB (3371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c79418540c78592e0ce7f96f5df8dd9db310edd58c6f158ba3389cd2290920`  
		Last Modified: Tue, 21 Nov 2023 08:15:43 GMT  
		Size: 30.2 MB (30185437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:bookworm` - linux; s390x

```console
$ docker pull irssi@sha256:19d5614ead4badb612e08ba2483418078e52144432cb38d8393c825b31ebe63f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72933796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2a7878077011d582ad7647ec003c06a9ed22ba2e0b5280c344ed18a0f1b8c40`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:42:37 GMT
ADD file:f06f12fa5a93afc3a79ac4371d24b0a471a5a1818cf34c1d90004c8f410914b9 in / 
# Tue, 19 Dec 2023 01:42:39 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:29:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:29:37 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 08:29:37 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 08:29:37 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 08:29:38 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 08:30:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 08:30:17 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 08:30:17 GMT
USER user
# Tue, 19 Dec 2023 08:30:17 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:bc6b1888979d3ceb063da848b2034e980e2c2613642159c1e856550b79aa620c`  
		Last Modified: Tue, 19 Dec 2023 01:47:38 GMT  
		Size: 27.5 MB (27491874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d93a78aafed26613c2aa62cc6ab76d24cde8ba422049c8c4aff454d7e8b6f0`  
		Last Modified: Tue, 19 Dec 2023 08:30:47 GMT  
		Size: 18.2 MB (18210518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506c18d3ee4758db831ecc9a8b1ea9f2562b6972d70a1fb2cd98603a28811f5f`  
		Last Modified: Tue, 19 Dec 2023 08:30:44 GMT  
		Size: 3.4 KB (3376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64e09b7ab558543c54810d6e85b3a3fab5eb5ae4fec9423bfdc282f16c15bcc`  
		Last Modified: Tue, 19 Dec 2023 08:30:48 GMT  
		Size: 27.2 MB (27228028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:latest`

```console
$ docker pull irssi@sha256:9bbaebbdef964fd13f87622f887af48afe01d1ef67ec7152da0e993626f8c347
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
$ docker pull irssi@sha256:75930e1081143e5ac73cc553fd47dd75a236c5587dad0b13ed4f593d5efec999
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76071375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e784ee8f60cc445019f7f2a00f02a16d18715a384904180fa30548888ea9a9e2`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:27 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Tue, 19 Dec 2023 01:20:28 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:11:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:11:41 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 08:11:42 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 08:11:42 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 08:11:42 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 08:12:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 08:12:22 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 08:12:22 GMT
USER user
# Tue, 19 Dec 2023 08:12:22 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f576257a7efd8fa2eab590d15da13ff3e351ddd5f66e1f18853950d0a847940`  
		Last Modified: Tue, 19 Dec 2023 08:12:41 GMT  
		Size: 18.3 MB (18263304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8709b16d66af9e29995cd9f313628ac25626d9a3b9f14337a489a0b53dede1`  
		Last Modified: Tue, 19 Dec 2023 08:12:37 GMT  
		Size: 3.4 KB (3376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4721ae122aaf701fec4c0ab60bcd8186c440f5439303bb23fc19aaa3cc886e`  
		Last Modified: Tue, 19 Dec 2023 08:12:42 GMT  
		Size: 28.7 MB (28678732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm variant v5

```console
$ docker pull irssi@sha256:54f4b6e9ea13a0ad57b6507d166cc7d60f705a1f0fb2c8b1a21ccf71be8b4817
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70247719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f71b3c5dc081e54b3f8c57c1d3be303a0147a4ac5656f26d0698b3673bce8f5`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:55:22 GMT
ADD file:9503ab966c9dd707eeccc7c2f633bccc94c199f8714ec4ff2c8b54dde3dbabf9 in / 
# Tue, 19 Dec 2023 01:55:22 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 05:37:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 05:37:07 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 05:37:08 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 05:37:08 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 05:37:08 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 05:37:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 05:37:54 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 05:37:54 GMT
USER user
# Tue, 19 Dec 2023 05:37:54 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1ae9a2844c8c70942d2220553689b62e841cc706d77284fbfedbd770080fd699`  
		Last Modified: Tue, 19 Dec 2023 01:58:33 GMT  
		Size: 26.9 MB (26885440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8c63a38cdf609e2fc7e6adb6d2a2ddee5ee1e185ced4c5667fa93153ddaca4`  
		Last Modified: Tue, 19 Dec 2023 05:38:20 GMT  
		Size: 17.0 MB (17034518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5baba07d2ad153cdc8a55cf44e4e53c2d24eccd878b7c013029ad93e53dad92b`  
		Last Modified: Tue, 19 Dec 2023 05:38:15 GMT  
		Size: 3.4 KB (3382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b675c572666d53e7aaee086d9f3a892e01803b6b84ab820ee1100726092e714`  
		Last Modified: Tue, 19 Dec 2023 05:38:21 GMT  
		Size: 26.3 MB (26324379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm variant v7

```console
$ docker pull irssi@sha256:b58087a750d2ecb0db246fa2b83fce92398c136af518ddc7bcae63e75637be1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66568253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0abed9b964bf4864c88c0c97e43a26973a28db129f9679f226eba9307dd515ec`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 02:07:50 GMT
ADD file:aef112919e7924ad6da32181b1df5099cd692680c104118da3a24cd4dfe55a1d in / 
# Tue, 19 Dec 2023 02:07:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:25:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:25:13 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 08:25:13 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 08:25:14 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 08:25:14 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 08:25:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 08:25:50 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 08:25:50 GMT
USER user
# Tue, 19 Dec 2023 08:25:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:65ab19615c01a3b542f77fadb3bd27872b6a20cba3e9269fb951de36d8fa6805`  
		Last Modified: Tue, 19 Dec 2023 02:11:52 GMT  
		Size: 24.7 MB (24718157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34312fc906c50709273b2bfc296cbc5e618081aab636bea0270e632aa1250a58`  
		Last Modified: Tue, 19 Dec 2023 08:26:13 GMT  
		Size: 16.6 MB (16626329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ae59c8630536591ee4c9f224e24066f5ea55d87cd4d710f4758493e40f4d90`  
		Last Modified: Tue, 19 Dec 2023 08:26:07 GMT  
		Size: 3.4 KB (3375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653d387ba5d23d5a1d3207409abeb6f1857445f450f723a518d7f30d8305a612`  
		Last Modified: Tue, 19 Dec 2023 08:26:13 GMT  
		Size: 25.2 MB (25220392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:ca5674fca34098dff53db48ae2b739f5bf5deef41b342fe154e13d37c4ca22d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74826194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e84ec8b67ce32fad14adb38e81b191c731737445551e607aadf4cb648de22d25`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:11 GMT
ADD file:262fd7bf0bc26e5d2a229fba52626e22b8a93beac29733acfc60e716c26e689d in / 
# Tue, 19 Dec 2023 01:41:11 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:35:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 07:35:16 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 07:35:17 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 07:35:17 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 07:35:17 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 07:35:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 07:35:50 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 07:35:50 GMT
USER user
# Tue, 19 Dec 2023 07:35:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:24e221e92a36ab5b0075dd156b4f2ff095532a9b0927946cf6070bb1bea208b8`  
		Last Modified: Tue, 19 Dec 2023 01:44:38 GMT  
		Size: 29.2 MB (29157269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3b65976afca6b69a78f82bba0cfd53e915de68b3497418795c0fe90dde04d6`  
		Last Modified: Tue, 19 Dec 2023 07:36:07 GMT  
		Size: 18.0 MB (18025714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1487d5e5dd099dea8c8f5cfa983386ef698d0b7ba74af27991d128c2eb77509a`  
		Last Modified: Tue, 19 Dec 2023 07:36:04 GMT  
		Size: 3.4 KB (3375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027137ab6d543546e67a802c5b15757aae71ceb8e7be44d4ab7e3701b466102e`  
		Last Modified: Tue, 19 Dec 2023 07:36:07 GMT  
		Size: 27.6 MB (27639836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; 386

```console
$ docker pull irssi@sha256:f4a77a97b8bd86a99d34d5fb0a8786e1a8f95758005b4ba99deb96a2b24d589a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76522898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e29421276ec13208c270be47f6eb04f62363c92fbf673bd983a1aa520e2fedc`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Nov 2023 04:39:53 GMT
ADD file:930e1b9d85b6927c4d3046f7c75de2f3bfc6ec29100c314d0ab2b780ea30e962 in / 
# Tue, 21 Nov 2023 04:39:53 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:18:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:18:00 GMT
ENV HOME=/home/user
# Tue, 21 Nov 2023 09:18:01 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Nov 2023 09:18:01 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 09:18:01 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 21 Nov 2023 09:18:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Nov 2023 09:18:58 GMT
WORKDIR /home/user
# Tue, 21 Nov 2023 09:18:58 GMT
USER user
# Tue, 21 Nov 2023 09:18:58 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c0734eabce8885d8904dbd11b77aa97c2d2b04bc8e2af9e89d47c4bda590dd8e`  
		Last Modified: Tue, 21 Nov 2023 04:44:34 GMT  
		Size: 30.2 MB (30164109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd0a88ad6c1f45a640f6b1e3509a00f0489ea5e7317905ff14b60fca6f24086`  
		Last Modified: Tue, 21 Nov 2023 09:19:21 GMT  
		Size: 17.8 MB (17789102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e785a0b684a75cef890d58447965564ea0ab287ad9b7fa38d00a4e9cfe5de7`  
		Last Modified: Tue, 21 Nov 2023 09:19:15 GMT  
		Size: 3.4 KB (3372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397cc87253be0de402ae3c1da69d2224514616b57b478236526d9f020d3b6ad6`  
		Last Modified: Tue, 21 Nov 2023 09:19:23 GMT  
		Size: 28.6 MB (28566315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; mips64le

```console
$ docker pull irssi@sha256:9c4985936b28f111411e9b54fe41acdb3b06222c5e22b4783ac53322ddf57794
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73894339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:370cd0afda43f756d5b75c9726905baa31206388d01ef49a763d8e033950a631`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 16:36:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 16:36:50 GMT
ENV HOME=/home/user
# Tue, 21 Nov 2023 16:36:56 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Nov 2023 16:37:00 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 16:37:03 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 21 Nov 2023 16:40:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Nov 2023 16:40:50 GMT
WORKDIR /home/user
# Tue, 21 Nov 2023 16:40:54 GMT
USER user
# Tue, 21 Nov 2023 16:40:58 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a2caa6a91dd837ff86958b77bc3534a4003f0cc9611e0b48c76361698bc605`  
		Last Modified: Tue, 21 Nov 2023 16:41:28 GMT  
		Size: 16.7 MB (16741807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6247f0644042c0a753bfe2ff1b7c28d43caaf3330ed88b170167a6fe8a0d35`  
		Last Modified: Tue, 21 Nov 2023 16:41:12 GMT  
		Size: 3.3 KB (3296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb6fda2e80956777959da56923ad2794e7af2f4a510933d7b85d0bf680feb2b`  
		Last Modified: Tue, 21 Nov 2023 16:41:33 GMT  
		Size: 28.0 MB (28007252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; ppc64le

```console
$ docker pull irssi@sha256:3f4f99d9914f9e72defad07d78d6e7c12b79184ab4aba83db835de09bc8f75bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82095380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60c6389f9028a4f1e86f03b0bf0bfed6a3d3f45126cdde79535e1136d045b8ff`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 08:14:12 GMT
ENV HOME=/home/user
# Tue, 21 Nov 2023 08:14:13 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Nov 2023 08:14:14 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 08:14:14 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 21 Nov 2023 08:15:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Nov 2023 08:15:10 GMT
WORKDIR /home/user
# Tue, 21 Nov 2023 08:15:10 GMT
USER user
# Tue, 21 Nov 2023 08:15:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990142f84c0c74390b332399beb412942fc74379d8c617ede6f2b0f701fd5f63`  
		Last Modified: Tue, 21 Nov 2023 08:15:42 GMT  
		Size: 18.8 MB (18764965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145cb9bddb869ec0a23e4a981ffb5078fc4852784403e1f0cb05eb86e52276cf`  
		Last Modified: Tue, 21 Nov 2023 08:15:38 GMT  
		Size: 3.4 KB (3371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c79418540c78592e0ce7f96f5df8dd9db310edd58c6f158ba3389cd2290920`  
		Last Modified: Tue, 21 Nov 2023 08:15:43 GMT  
		Size: 30.2 MB (30185437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; s390x

```console
$ docker pull irssi@sha256:19d5614ead4badb612e08ba2483418078e52144432cb38d8393c825b31ebe63f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72933796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2a7878077011d582ad7647ec003c06a9ed22ba2e0b5280c344ed18a0f1b8c40`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 01:42:37 GMT
ADD file:f06f12fa5a93afc3a79ac4371d24b0a471a5a1818cf34c1d90004c8f410914b9 in / 
# Tue, 19 Dec 2023 01:42:39 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:29:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:29:37 GMT
ENV HOME=/home/user
# Tue, 19 Dec 2023 08:29:37 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 19 Dec 2023 08:29:37 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 08:29:38 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 19 Dec 2023 08:30:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 19 Dec 2023 08:30:17 GMT
WORKDIR /home/user
# Tue, 19 Dec 2023 08:30:17 GMT
USER user
# Tue, 19 Dec 2023 08:30:17 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:bc6b1888979d3ceb063da848b2034e980e2c2613642159c1e856550b79aa620c`  
		Last Modified: Tue, 19 Dec 2023 01:47:38 GMT  
		Size: 27.5 MB (27491874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d93a78aafed26613c2aa62cc6ab76d24cde8ba422049c8c4aff454d7e8b6f0`  
		Last Modified: Tue, 19 Dec 2023 08:30:47 GMT  
		Size: 18.2 MB (18210518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506c18d3ee4758db831ecc9a8b1ea9f2562b6972d70a1fb2cd98603a28811f5f`  
		Last Modified: Tue, 19 Dec 2023 08:30:44 GMT  
		Size: 3.4 KB (3376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64e09b7ab558543c54810d6e85b3a3fab5eb5ae4fec9423bfdc282f16c15bcc`  
		Last Modified: Tue, 19 Dec 2023 08:30:48 GMT  
		Size: 27.2 MB (27228028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
