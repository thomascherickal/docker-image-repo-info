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
$ docker pull irssi@sha256:69927d1ad99aec69bddc2a42727ee72f0bd0d005a9aba5c0667166b045d2dc34
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
$ docker pull irssi@sha256:58fc1c672bf293069b7789a309a03bcb34c93951017f2488c4037de7c2c68269
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (76048658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2e78b1ae299bcd0f8deef087b5454642320d910c779322916fad90990fbc810`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:42 GMT
ADD file:ba1250b6ecd5dd09d4914189d72741c2817988994e7da514bf62be439a34bdb5 in / 
# Mon, 12 Jun 2023 23:20:42 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 01:27:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 01:27:04 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:27:04 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:27:04 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:27:04 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:27:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 01:27:52 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:27:52 GMT
USER user
# Thu, 22 Jun 2023 01:27:53 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:5b5fe70539cd6989aa19f25826309f9715a9489cf1c057982d6a84c1ad8975c7`  
		Last Modified: Mon, 12 Jun 2023 23:25:49 GMT  
		Size: 29.1 MB (29124744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4909e07c2d187606b474bffed67e6b8f97ee741deba3ee1a6cc6e03a57e06d25`  
		Last Modified: Thu, 22 Jun 2023 01:28:49 GMT  
		Size: 18.2 MB (18242756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed55928edc7533b8545259265ffa0db2e9687da3460557c3885e41a0b49cbe0`  
		Last Modified: Thu, 22 Jun 2023 01:28:45 GMT  
		Size: 3.4 KB (3372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6731e4fa8db1fd048929e347b2b35f7b30b5a7d41015d14037ee7149376b11af`  
		Last Modified: Thu, 22 Jun 2023 01:28:50 GMT  
		Size: 28.7 MB (28677786 bytes)  
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
$ docker pull irssi@sha256:04fe9086e0677c27e634b48247d835bd76d770fb2d93a37e98e0f5d10ad930d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66699462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:347dde6d1977d7559b809d379aeb2d49c7dc1edb227ac50753bb5b436492f450`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Jul 2023 00:57:54 GMT
ADD file:d168d1710cbca4edb322c26348dafaf2b3a64980f52b8b790f334cdbd6a7047e in / 
# Tue, 04 Jul 2023 00:57:55 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:02:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:02:14 GMT
ENV HOME=/home/user
# Tue, 04 Jul 2023 05:02:15 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 04 Jul 2023 05:02:15 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 05:02:15 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 04 Jul 2023 05:02:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 04 Jul 2023 05:02:53 GMT
WORKDIR /home/user
# Tue, 04 Jul 2023 05:02:53 GMT
USER user
# Tue, 04 Jul 2023 05:02:53 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:340ace0baa422f18db718d7634c1c88a9650f4871dda2630ef15577120aa6816`  
		Last Modified: Tue, 04 Jul 2023 01:02:50 GMT  
		Size: 24.8 MB (24801264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26335a3dcbbb3fe7c73c15fa804eb199dc3d2c6f72d4b272290495ddc7d5d52`  
		Last Modified: Tue, 04 Jul 2023 05:03:15 GMT  
		Size: 16.7 MB (16675209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d7691ca1849da70e59df47ce1ae57125e975051c107f00f45a7c3cf16dba8d`  
		Last Modified: Tue, 04 Jul 2023 05:03:10 GMT  
		Size: 3.4 KB (3368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6467c4b92ddee02bde53da36ae6e65510038840b918475ce6e8b1923576edebc`  
		Last Modified: Tue, 04 Jul 2023 05:03:15 GMT  
		Size: 25.2 MB (25219621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:c7c88dad0daea3ad57151de33054217941d7becf80f2dc11592f3a5dccc31cd9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74817355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63655ff173ab77b3325bf30ffb4193bc7ac59ae13e21dfb4f90bf03ae3939077`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:51:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:51:17 GMT
ENV HOME=/home/user
# Tue, 04 Jul 2023 03:51:17 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 04 Jul 2023 03:51:18 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 03:51:18 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 04 Jul 2023 03:51:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 04 Jul 2023 03:51:56 GMT
WORKDIR /home/user
# Tue, 04 Jul 2023 03:51:56 GMT
USER user
# Tue, 04 Jul 2023 03:51:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14ecf60c320eb05ae2ba16ad2774d3066ce556d0aacc4cfda7f3de6cf9aa09d`  
		Last Modified: Tue, 04 Jul 2023 03:52:21 GMT  
		Size: 18.0 MB (18023969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8369f911d29dedde0b1e053fb13ffe68ef5bc4ee1bf9929783256c66bb74805`  
		Last Modified: Tue, 04 Jul 2023 03:52:18 GMT  
		Size: 3.4 KB (3370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0551107dfe1234434d37c2834437f715c93fdc6d340114d753b92612ab6d41cd`  
		Last Modified: Tue, 04 Jul 2023 03:52:22 GMT  
		Size: 27.6 MB (27637558 bytes)  
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
$ docker pull irssi@sha256:acbfc7fb13e89e47dad3c9137ef7fa896c5b75ac6533c06b67ade3057c9e2f97
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74052670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b08a4afb9566f8f4288fec8c2b1904505266fadc1a760928b037691c498c116`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:02 GMT
ADD file:f91bd2a174259cb69646fc34ba2fc6b8941ad8e171d2d7952a4d8ac3d95e2ad7 in / 
# Tue, 13 Jun 2023 00:09:06 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 02:26:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 02:26:40 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 02:26:47 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 02:26:50 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 02:26:53 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 02:30:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 02:30:54 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 02:30:57 GMT
USER user
# Thu, 22 Jun 2023 02:31:01 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:3fc28260a4d871ef9781cad2bb064ad7212a5063de3a1d35dba938ce82115e5b`  
		Last Modified: Tue, 13 Jun 2023 00:22:29 GMT  
		Size: 29.1 MB (29118129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b823be8377fd7186d28f794a5ec6493660f4e2208ded12e67636ec8750257d5`  
		Last Modified: Thu, 22 Jun 2023 02:31:36 GMT  
		Size: 16.9 MB (16925138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b18026dd902a0919c3a20766c7d6592948e9284efb4931907978339a21d327c`  
		Last Modified: Thu, 22 Jun 2023 02:31:17 GMT  
		Size: 3.3 KB (3298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a7f08c49e09c90d3e8b01aa906a42cfb03f4a598b544ec9a61c25259e54c77`  
		Last Modified: Thu, 22 Jun 2023 02:31:39 GMT  
		Size: 28.0 MB (28006105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; ppc64le

```console
$ docker pull irssi@sha256:808102c091e0f450e9fd0ff09dd607c235a6972c0982e8a909041d95ecdc9bb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82057404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6db42123514bb5bb81836bd52afbea22d1c59d575a9cf77f3cf7c9ada892240`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:51 GMT
ADD file:51887002f5002ccc662adbc6ecf1129e3db375a7a77b93da43cc9a8326b3c4b9 in / 
# Tue, 04 Jul 2023 01:17:53 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:36:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:36:17 GMT
ENV HOME=/home/user
# Tue, 04 Jul 2023 06:36:19 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 04 Jul 2023 06:36:19 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 06:36:20 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 04 Jul 2023 06:38:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 04 Jul 2023 06:38:43 GMT
WORKDIR /home/user
# Tue, 04 Jul 2023 06:38:43 GMT
USER user
# Tue, 04 Jul 2023 06:38:44 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ba99a1aa5a92d949d988e66df7723a542fd81bc30eef9d4269e8a899820d4bb2`  
		Last Modified: Tue, 04 Jul 2023 01:24:36 GMT  
		Size: 33.1 MB (33116716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a472629dc3d35e78fd046fa9c53281082c6b5a3cbf7f446fdcd3c04302e339`  
		Last Modified: Tue, 04 Jul 2023 06:39:27 GMT  
		Size: 18.8 MB (18754069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd7eaa97c83385d341b2e6b1823b9021baeb70ce87fcc47e593bff57983efce`  
		Last Modified: Tue, 04 Jul 2023 06:39:20 GMT  
		Size: 3.4 KB (3370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bc505f4c9f16e57c14adb02d3910e21d2031362fc3775c1f499928e77048f2`  
		Last Modified: Tue, 04 Jul 2023 06:39:29 GMT  
		Size: 30.2 MB (30183249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; s390x

```console
$ docker pull irssi@sha256:baa1df37d716889924e03405a3a5a2258c9e4520c6ad647a93d27caa6aba256f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72925568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:251b812805e137b9e051579adf3a25dd277d29aeacde9c29977afa4e7e513e0a`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Jun 2023 04:29:41 GMT
ADD file:739f4c23557ec0af5f4ba492c847b5d2f09dd81211c675d0e9eabe865d794e81 in / 
# Tue, 13 Jun 2023 04:29:43 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 08:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 08:51:21 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 08:51:21 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 08:51:21 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 08:51:22 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 08:51:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 08:52:00 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 08:52:00 GMT
USER user
# Thu, 22 Jun 2023 08:52:00 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6571b3abd058e377c7bd231c9029aff6eb25486bffb50229076d2e6a356a517f`  
		Last Modified: Tue, 13 Jun 2023 04:34:21 GMT  
		Size: 27.5 MB (27487928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0716cb6af8f5fcdc92d2d74f09de86858ee69ef8a2db7db71d6d60048930182`  
		Last Modified: Thu, 22 Jun 2023 08:53:07 GMT  
		Size: 18.2 MB (18206342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72ba9f202ec95947aa092a1c8f9fbac3cb975b47cf804734a0804722f737334`  
		Last Modified: Thu, 22 Jun 2023 08:53:04 GMT  
		Size: 3.4 KB (3368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e63e7ec95d8ded21367b4197e518b0bbc792b85525d9ca92b313e772bd4ec5`  
		Last Modified: Thu, 22 Jun 2023 08:53:08 GMT  
		Size: 27.2 MB (27227930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1-alpine`

```console
$ docker pull irssi@sha256:46a65610bad93dc8966f7e0a385bad0c9047a4d05c2f6ffedb5b2d3d0226138a
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
$ docker pull irssi@sha256:a768693cbea894b7b6135922520f7d532a6245dff8a3863024244a8ef9ffb14e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18439974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6be6e0e30722062f7d0e647c925e5239badb1739c57c83238d83b8a422b169fe`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:28:06 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:28:06 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:28:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:28:07 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:28:07 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:28:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:28:26 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:28:26 GMT
USER user
# Thu, 22 Jun 2023 01:28:26 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdb311d04d5ef03d3a3d6136863478ca52e56c787391712823006f36d8d5b9e`  
		Last Modified: Thu, 22 Jun 2023 01:29:12 GMT  
		Size: 9.6 MB (9637888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c8f7b98870f87f73429e0fb3e302a979d79d0c313dc49f64bd4b6d52763c08`  
		Last Modified: Thu, 22 Jun 2023 01:29:10 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3e36b711d362f59b8801dbb9ce1a3ec3bcaa5edd5b2366634e350cf308faee`  
		Last Modified: Thu, 22 Jun 2023 01:29:11 GMT  
		Size: 5.4 MB (5402922 bytes)  
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
$ docker pull irssi@sha256:6e7b11efe55cad75bda8ed33f8f0cd39a6c1e9978fc0c6e5272a2034b7ad35b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16621926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20abb587081f9ea7c13c022008f41792c8deeaca15a52406320be5f7e2aefd62`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:15 GMT
ADD file:082f034323c559f3cb9feb6422c88b1ec8017f436d6109e238a5c5384a32a90a in / 
# Wed, 14 Jun 2023 22:36:15 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:44:06 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:44:06 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:44:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:44:07 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:44:07 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:44:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:44:21 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:44:21 GMT
USER user
# Thu, 22 Jun 2023 01:44:21 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:633ba29fd335042456b6e2c073636f6fa30de56f1331c442914739b92a479974`  
		Last Modified: Wed, 14 Jun 2023 22:36:49 GMT  
		Size: 2.9 MB (2898508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e832bd75bc8892fffbcd2098ea32615beca89d5932e7bd6eae1c7973395a4a3c`  
		Last Modified: Thu, 22 Jun 2023 01:45:04 GMT  
		Size: 8.7 MB (8713654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9047f01d89a8f17a367c34c160949fb95db656ce766205320464b4f6a764b845`  
		Last Modified: Thu, 22 Jun 2023 01:45:01 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01ed6e5b2633e51a886c41895b2477ea69e8db678ddac23148e963ee8532ac0`  
		Last Modified: Thu, 22 Jun 2023 01:45:03 GMT  
		Size: 5.0 MB (5008480 bytes)  
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
$ docker pull irssi@sha256:95e45ba9fe7403d47a90aa5cbebc48878a954aa9248132df17d0b1964b5735f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18704414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c077a39e383a52f1690468a909209454afb356ca12011e784cc206bb0eabb553`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:49 GMT
ADD file:694c636c0dd19fd01accbc189e4c1dc4d063952692c6e7eb26dce02a7adba833 in / 
# Thu, 15 Jun 2023 00:39:49 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:46:07 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:46:08 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:46:09 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:46:09 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:46:10 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:46:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:46:37 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:46:38 GMT
USER user
# Thu, 22 Jun 2023 01:46:38 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ffa4a466dbb8eebd7e7f25590a9df12390de9016abf82279c29c9a64aa76491a`  
		Last Modified: Thu, 15 Jun 2023 00:40:26 GMT  
		Size: 3.3 MB (3344781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f791e21598b0753fdaac6f0554ec6cece5879b619efdbbb4c1b4449a37503445`  
		Last Modified: Thu, 22 Jun 2023 01:47:27 GMT  
		Size: 9.7 MB (9727162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05af372d8f57623b63ce194292c9d6e8cadad5b62006778fb3386de60bcded93`  
		Last Modified: Thu, 22 Jun 2023 01:47:24 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d0975696ee4b7f29a8e63ef0198dd4294f329a0a3db44dbe09d39d6194767f`  
		Last Modified: Thu, 22 Jun 2023 01:47:26 GMT  
		Size: 5.6 MB (5631188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:4f9ea0549297b400ee4e290a3e5d2548d5f935d01d81d209a4260dd9d9499e89
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18700399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31793e9f59a88f5efa8fcc186bd96e790b7d579acb15af792bf14f89c96d95f5`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 08:52:18 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 08:52:19 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 08:52:19 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 08:52:20 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 08:52:20 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 08:52:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 08:52:44 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 08:52:44 GMT
USER user
# Thu, 22 Jun 2023 08:52:44 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27869a2a741a6e4efe8b45710576e604e3fc468cef7d0feaa97e003f76aeb10`  
		Last Modified: Thu, 22 Jun 2023 08:53:34 GMT  
		Size: 10.1 MB (10078671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b47042a99d33af0f2ed5b3830ae99f7b13bb137fb93f1ace7e2d4922994df8d`  
		Last Modified: Thu, 22 Jun 2023 08:53:32 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24432dec00488946bcee10e0f328cc956d09781dd4d8165e1228aeecc1c4d390`  
		Last Modified: Thu, 22 Jun 2023 08:53:33 GMT  
		Size: 5.4 MB (5406948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1-alpine3.18`

```console
$ docker pull irssi@sha256:46a65610bad93dc8966f7e0a385bad0c9047a4d05c2f6ffedb5b2d3d0226138a
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
$ docker pull irssi@sha256:a768693cbea894b7b6135922520f7d532a6245dff8a3863024244a8ef9ffb14e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18439974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6be6e0e30722062f7d0e647c925e5239badb1739c57c83238d83b8a422b169fe`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:28:06 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:28:06 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:28:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:28:07 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:28:07 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:28:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:28:26 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:28:26 GMT
USER user
# Thu, 22 Jun 2023 01:28:26 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdb311d04d5ef03d3a3d6136863478ca52e56c787391712823006f36d8d5b9e`  
		Last Modified: Thu, 22 Jun 2023 01:29:12 GMT  
		Size: 9.6 MB (9637888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c8f7b98870f87f73429e0fb3e302a979d79d0c313dc49f64bd4b6d52763c08`  
		Last Modified: Thu, 22 Jun 2023 01:29:10 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3e36b711d362f59b8801dbb9ce1a3ec3bcaa5edd5b2366634e350cf308faee`  
		Last Modified: Thu, 22 Jun 2023 01:29:11 GMT  
		Size: 5.4 MB (5402922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

### `irssi:1-alpine3.18` - linux; arm variant v7

```console
$ docker pull irssi@sha256:6e7b11efe55cad75bda8ed33f8f0cd39a6c1e9978fc0c6e5272a2034b7ad35b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16621926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20abb587081f9ea7c13c022008f41792c8deeaca15a52406320be5f7e2aefd62`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:15 GMT
ADD file:082f034323c559f3cb9feb6422c88b1ec8017f436d6109e238a5c5384a32a90a in / 
# Wed, 14 Jun 2023 22:36:15 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:44:06 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:44:06 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:44:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:44:07 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:44:07 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:44:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:44:21 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:44:21 GMT
USER user
# Thu, 22 Jun 2023 01:44:21 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:633ba29fd335042456b6e2c073636f6fa30de56f1331c442914739b92a479974`  
		Last Modified: Wed, 14 Jun 2023 22:36:49 GMT  
		Size: 2.9 MB (2898508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e832bd75bc8892fffbcd2098ea32615beca89d5932e7bd6eae1c7973395a4a3c`  
		Last Modified: Thu, 22 Jun 2023 01:45:04 GMT  
		Size: 8.7 MB (8713654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9047f01d89a8f17a367c34c160949fb95db656ce766205320464b4f6a764b845`  
		Last Modified: Thu, 22 Jun 2023 01:45:01 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01ed6e5b2633e51a886c41895b2477ea69e8db678ddac23148e963ee8532ac0`  
		Last Modified: Thu, 22 Jun 2023 01:45:03 GMT  
		Size: 5.0 MB (5008480 bytes)  
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

### `irssi:1-alpine3.18` - linux; ppc64le

```console
$ docker pull irssi@sha256:95e45ba9fe7403d47a90aa5cbebc48878a954aa9248132df17d0b1964b5735f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18704414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c077a39e383a52f1690468a909209454afb356ca12011e784cc206bb0eabb553`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:49 GMT
ADD file:694c636c0dd19fd01accbc189e4c1dc4d063952692c6e7eb26dce02a7adba833 in / 
# Thu, 15 Jun 2023 00:39:49 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:46:07 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:46:08 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:46:09 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:46:09 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:46:10 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:46:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:46:37 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:46:38 GMT
USER user
# Thu, 22 Jun 2023 01:46:38 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ffa4a466dbb8eebd7e7f25590a9df12390de9016abf82279c29c9a64aa76491a`  
		Last Modified: Thu, 15 Jun 2023 00:40:26 GMT  
		Size: 3.3 MB (3344781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f791e21598b0753fdaac6f0554ec6cece5879b619efdbbb4c1b4449a37503445`  
		Last Modified: Thu, 22 Jun 2023 01:47:27 GMT  
		Size: 9.7 MB (9727162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05af372d8f57623b63ce194292c9d6e8cadad5b62006778fb3386de60bcded93`  
		Last Modified: Thu, 22 Jun 2023 01:47:24 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d0975696ee4b7f29a8e63ef0198dd4294f329a0a3db44dbe09d39d6194767f`  
		Last Modified: Thu, 22 Jun 2023 01:47:26 GMT  
		Size: 5.6 MB (5631188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine3.18` - linux; s390x

```console
$ docker pull irssi@sha256:4f9ea0549297b400ee4e290a3e5d2548d5f935d01d81d209a4260dd9d9499e89
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18700399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31793e9f59a88f5efa8fcc186bd96e790b7d579acb15af792bf14f89c96d95f5`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 08:52:18 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 08:52:19 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 08:52:19 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 08:52:20 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 08:52:20 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 08:52:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 08:52:44 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 08:52:44 GMT
USER user
# Thu, 22 Jun 2023 08:52:44 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27869a2a741a6e4efe8b45710576e604e3fc468cef7d0feaa97e003f76aeb10`  
		Last Modified: Thu, 22 Jun 2023 08:53:34 GMT  
		Size: 10.1 MB (10078671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b47042a99d33af0f2ed5b3830ae99f7b13bb137fb93f1ace7e2d4922994df8d`  
		Last Modified: Thu, 22 Jun 2023 08:53:32 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24432dec00488946bcee10e0f328cc956d09781dd4d8165e1228aeecc1c4d390`  
		Last Modified: Thu, 22 Jun 2023 08:53:33 GMT  
		Size: 5.4 MB (5406948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1-bookworm`

```console
$ docker pull irssi@sha256:69927d1ad99aec69bddc2a42727ee72f0bd0d005a9aba5c0667166b045d2dc34
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
$ docker pull irssi@sha256:58fc1c672bf293069b7789a309a03bcb34c93951017f2488c4037de7c2c68269
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (76048658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2e78b1ae299bcd0f8deef087b5454642320d910c779322916fad90990fbc810`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:42 GMT
ADD file:ba1250b6ecd5dd09d4914189d72741c2817988994e7da514bf62be439a34bdb5 in / 
# Mon, 12 Jun 2023 23:20:42 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 01:27:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 01:27:04 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:27:04 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:27:04 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:27:04 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:27:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 01:27:52 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:27:52 GMT
USER user
# Thu, 22 Jun 2023 01:27:53 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:5b5fe70539cd6989aa19f25826309f9715a9489cf1c057982d6a84c1ad8975c7`  
		Last Modified: Mon, 12 Jun 2023 23:25:49 GMT  
		Size: 29.1 MB (29124744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4909e07c2d187606b474bffed67e6b8f97ee741deba3ee1a6cc6e03a57e06d25`  
		Last Modified: Thu, 22 Jun 2023 01:28:49 GMT  
		Size: 18.2 MB (18242756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed55928edc7533b8545259265ffa0db2e9687da3460557c3885e41a0b49cbe0`  
		Last Modified: Thu, 22 Jun 2023 01:28:45 GMT  
		Size: 3.4 KB (3372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6731e4fa8db1fd048929e347b2b35f7b30b5a7d41015d14037ee7149376b11af`  
		Last Modified: Thu, 22 Jun 2023 01:28:50 GMT  
		Size: 28.7 MB (28677786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

### `irssi:1-bookworm` - linux; arm variant v7

```console
$ docker pull irssi@sha256:04fe9086e0677c27e634b48247d835bd76d770fb2d93a37e98e0f5d10ad930d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66699462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:347dde6d1977d7559b809d379aeb2d49c7dc1edb227ac50753bb5b436492f450`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Jul 2023 00:57:54 GMT
ADD file:d168d1710cbca4edb322c26348dafaf2b3a64980f52b8b790f334cdbd6a7047e in / 
# Tue, 04 Jul 2023 00:57:55 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:02:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:02:14 GMT
ENV HOME=/home/user
# Tue, 04 Jul 2023 05:02:15 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 04 Jul 2023 05:02:15 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 05:02:15 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 04 Jul 2023 05:02:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 04 Jul 2023 05:02:53 GMT
WORKDIR /home/user
# Tue, 04 Jul 2023 05:02:53 GMT
USER user
# Tue, 04 Jul 2023 05:02:53 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:340ace0baa422f18db718d7634c1c88a9650f4871dda2630ef15577120aa6816`  
		Last Modified: Tue, 04 Jul 2023 01:02:50 GMT  
		Size: 24.8 MB (24801264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26335a3dcbbb3fe7c73c15fa804eb199dc3d2c6f72d4b272290495ddc7d5d52`  
		Last Modified: Tue, 04 Jul 2023 05:03:15 GMT  
		Size: 16.7 MB (16675209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d7691ca1849da70e59df47ce1ae57125e975051c107f00f45a7c3cf16dba8d`  
		Last Modified: Tue, 04 Jul 2023 05:03:10 GMT  
		Size: 3.4 KB (3368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6467c4b92ddee02bde53da36ae6e65510038840b918475ce6e8b1923576edebc`  
		Last Modified: Tue, 04 Jul 2023 05:03:15 GMT  
		Size: 25.2 MB (25219621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-bookworm` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:c7c88dad0daea3ad57151de33054217941d7becf80f2dc11592f3a5dccc31cd9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74817355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63655ff173ab77b3325bf30ffb4193bc7ac59ae13e21dfb4f90bf03ae3939077`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:51:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:51:17 GMT
ENV HOME=/home/user
# Tue, 04 Jul 2023 03:51:17 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 04 Jul 2023 03:51:18 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 03:51:18 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 04 Jul 2023 03:51:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 04 Jul 2023 03:51:56 GMT
WORKDIR /home/user
# Tue, 04 Jul 2023 03:51:56 GMT
USER user
# Tue, 04 Jul 2023 03:51:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14ecf60c320eb05ae2ba16ad2774d3066ce556d0aacc4cfda7f3de6cf9aa09d`  
		Last Modified: Tue, 04 Jul 2023 03:52:21 GMT  
		Size: 18.0 MB (18023969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8369f911d29dedde0b1e053fb13ffe68ef5bc4ee1bf9929783256c66bb74805`  
		Last Modified: Tue, 04 Jul 2023 03:52:18 GMT  
		Size: 3.4 KB (3370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0551107dfe1234434d37c2834437f715c93fdc6d340114d753b92612ab6d41cd`  
		Last Modified: Tue, 04 Jul 2023 03:52:22 GMT  
		Size: 27.6 MB (27637558 bytes)  
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

### `irssi:1-bookworm` - linux; mips64le

```console
$ docker pull irssi@sha256:acbfc7fb13e89e47dad3c9137ef7fa896c5b75ac6533c06b67ade3057c9e2f97
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74052670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b08a4afb9566f8f4288fec8c2b1904505266fadc1a760928b037691c498c116`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:02 GMT
ADD file:f91bd2a174259cb69646fc34ba2fc6b8941ad8e171d2d7952a4d8ac3d95e2ad7 in / 
# Tue, 13 Jun 2023 00:09:06 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 02:26:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 02:26:40 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 02:26:47 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 02:26:50 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 02:26:53 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 02:30:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 02:30:54 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 02:30:57 GMT
USER user
# Thu, 22 Jun 2023 02:31:01 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:3fc28260a4d871ef9781cad2bb064ad7212a5063de3a1d35dba938ce82115e5b`  
		Last Modified: Tue, 13 Jun 2023 00:22:29 GMT  
		Size: 29.1 MB (29118129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b823be8377fd7186d28f794a5ec6493660f4e2208ded12e67636ec8750257d5`  
		Last Modified: Thu, 22 Jun 2023 02:31:36 GMT  
		Size: 16.9 MB (16925138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b18026dd902a0919c3a20766c7d6592948e9284efb4931907978339a21d327c`  
		Last Modified: Thu, 22 Jun 2023 02:31:17 GMT  
		Size: 3.3 KB (3298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a7f08c49e09c90d3e8b01aa906a42cfb03f4a598b544ec9a61c25259e54c77`  
		Last Modified: Thu, 22 Jun 2023 02:31:39 GMT  
		Size: 28.0 MB (28006105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-bookworm` - linux; ppc64le

```console
$ docker pull irssi@sha256:808102c091e0f450e9fd0ff09dd607c235a6972c0982e8a909041d95ecdc9bb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82057404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6db42123514bb5bb81836bd52afbea22d1c59d575a9cf77f3cf7c9ada892240`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:51 GMT
ADD file:51887002f5002ccc662adbc6ecf1129e3db375a7a77b93da43cc9a8326b3c4b9 in / 
# Tue, 04 Jul 2023 01:17:53 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:36:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:36:17 GMT
ENV HOME=/home/user
# Tue, 04 Jul 2023 06:36:19 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 04 Jul 2023 06:36:19 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 06:36:20 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 04 Jul 2023 06:38:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 04 Jul 2023 06:38:43 GMT
WORKDIR /home/user
# Tue, 04 Jul 2023 06:38:43 GMT
USER user
# Tue, 04 Jul 2023 06:38:44 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ba99a1aa5a92d949d988e66df7723a542fd81bc30eef9d4269e8a899820d4bb2`  
		Last Modified: Tue, 04 Jul 2023 01:24:36 GMT  
		Size: 33.1 MB (33116716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a472629dc3d35e78fd046fa9c53281082c6b5a3cbf7f446fdcd3c04302e339`  
		Last Modified: Tue, 04 Jul 2023 06:39:27 GMT  
		Size: 18.8 MB (18754069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd7eaa97c83385d341b2e6b1823b9021baeb70ce87fcc47e593bff57983efce`  
		Last Modified: Tue, 04 Jul 2023 06:39:20 GMT  
		Size: 3.4 KB (3370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bc505f4c9f16e57c14adb02d3910e21d2031362fc3775c1f499928e77048f2`  
		Last Modified: Tue, 04 Jul 2023 06:39:29 GMT  
		Size: 30.2 MB (30183249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-bookworm` - linux; s390x

```console
$ docker pull irssi@sha256:baa1df37d716889924e03405a3a5a2258c9e4520c6ad647a93d27caa6aba256f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72925568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:251b812805e137b9e051579adf3a25dd277d29aeacde9c29977afa4e7e513e0a`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Jun 2023 04:29:41 GMT
ADD file:739f4c23557ec0af5f4ba492c847b5d2f09dd81211c675d0e9eabe865d794e81 in / 
# Tue, 13 Jun 2023 04:29:43 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 08:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 08:51:21 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 08:51:21 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 08:51:21 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 08:51:22 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 08:51:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 08:52:00 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 08:52:00 GMT
USER user
# Thu, 22 Jun 2023 08:52:00 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6571b3abd058e377c7bd231c9029aff6eb25486bffb50229076d2e6a356a517f`  
		Last Modified: Tue, 13 Jun 2023 04:34:21 GMT  
		Size: 27.5 MB (27487928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0716cb6af8f5fcdc92d2d74f09de86858ee69ef8a2db7db71d6d60048930182`  
		Last Modified: Thu, 22 Jun 2023 08:53:07 GMT  
		Size: 18.2 MB (18206342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72ba9f202ec95947aa092a1c8f9fbac3cb975b47cf804734a0804722f737334`  
		Last Modified: Thu, 22 Jun 2023 08:53:04 GMT  
		Size: 3.4 KB (3368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e63e7ec95d8ded21367b4197e518b0bbc792b85525d9ca92b313e772bd4ec5`  
		Last Modified: Thu, 22 Jun 2023 08:53:08 GMT  
		Size: 27.2 MB (27227930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4`

```console
$ docker pull irssi@sha256:69927d1ad99aec69bddc2a42727ee72f0bd0d005a9aba5c0667166b045d2dc34
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
$ docker pull irssi@sha256:58fc1c672bf293069b7789a309a03bcb34c93951017f2488c4037de7c2c68269
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (76048658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2e78b1ae299bcd0f8deef087b5454642320d910c779322916fad90990fbc810`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:42 GMT
ADD file:ba1250b6ecd5dd09d4914189d72741c2817988994e7da514bf62be439a34bdb5 in / 
# Mon, 12 Jun 2023 23:20:42 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 01:27:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 01:27:04 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:27:04 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:27:04 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:27:04 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:27:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 01:27:52 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:27:52 GMT
USER user
# Thu, 22 Jun 2023 01:27:53 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:5b5fe70539cd6989aa19f25826309f9715a9489cf1c057982d6a84c1ad8975c7`  
		Last Modified: Mon, 12 Jun 2023 23:25:49 GMT  
		Size: 29.1 MB (29124744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4909e07c2d187606b474bffed67e6b8f97ee741deba3ee1a6cc6e03a57e06d25`  
		Last Modified: Thu, 22 Jun 2023 01:28:49 GMT  
		Size: 18.2 MB (18242756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed55928edc7533b8545259265ffa0db2e9687da3460557c3885e41a0b49cbe0`  
		Last Modified: Thu, 22 Jun 2023 01:28:45 GMT  
		Size: 3.4 KB (3372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6731e4fa8db1fd048929e347b2b35f7b30b5a7d41015d14037ee7149376b11af`  
		Last Modified: Thu, 22 Jun 2023 01:28:50 GMT  
		Size: 28.7 MB (28677786 bytes)  
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
$ docker pull irssi@sha256:04fe9086e0677c27e634b48247d835bd76d770fb2d93a37e98e0f5d10ad930d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66699462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:347dde6d1977d7559b809d379aeb2d49c7dc1edb227ac50753bb5b436492f450`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Jul 2023 00:57:54 GMT
ADD file:d168d1710cbca4edb322c26348dafaf2b3a64980f52b8b790f334cdbd6a7047e in / 
# Tue, 04 Jul 2023 00:57:55 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:02:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:02:14 GMT
ENV HOME=/home/user
# Tue, 04 Jul 2023 05:02:15 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 04 Jul 2023 05:02:15 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 05:02:15 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 04 Jul 2023 05:02:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 04 Jul 2023 05:02:53 GMT
WORKDIR /home/user
# Tue, 04 Jul 2023 05:02:53 GMT
USER user
# Tue, 04 Jul 2023 05:02:53 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:340ace0baa422f18db718d7634c1c88a9650f4871dda2630ef15577120aa6816`  
		Last Modified: Tue, 04 Jul 2023 01:02:50 GMT  
		Size: 24.8 MB (24801264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26335a3dcbbb3fe7c73c15fa804eb199dc3d2c6f72d4b272290495ddc7d5d52`  
		Last Modified: Tue, 04 Jul 2023 05:03:15 GMT  
		Size: 16.7 MB (16675209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d7691ca1849da70e59df47ce1ae57125e975051c107f00f45a7c3cf16dba8d`  
		Last Modified: Tue, 04 Jul 2023 05:03:10 GMT  
		Size: 3.4 KB (3368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6467c4b92ddee02bde53da36ae6e65510038840b918475ce6e8b1923576edebc`  
		Last Modified: Tue, 04 Jul 2023 05:03:15 GMT  
		Size: 25.2 MB (25219621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:c7c88dad0daea3ad57151de33054217941d7becf80f2dc11592f3a5dccc31cd9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74817355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63655ff173ab77b3325bf30ffb4193bc7ac59ae13e21dfb4f90bf03ae3939077`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:51:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:51:17 GMT
ENV HOME=/home/user
# Tue, 04 Jul 2023 03:51:17 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 04 Jul 2023 03:51:18 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 03:51:18 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 04 Jul 2023 03:51:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 04 Jul 2023 03:51:56 GMT
WORKDIR /home/user
# Tue, 04 Jul 2023 03:51:56 GMT
USER user
# Tue, 04 Jul 2023 03:51:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14ecf60c320eb05ae2ba16ad2774d3066ce556d0aacc4cfda7f3de6cf9aa09d`  
		Last Modified: Tue, 04 Jul 2023 03:52:21 GMT  
		Size: 18.0 MB (18023969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8369f911d29dedde0b1e053fb13ffe68ef5bc4ee1bf9929783256c66bb74805`  
		Last Modified: Tue, 04 Jul 2023 03:52:18 GMT  
		Size: 3.4 KB (3370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0551107dfe1234434d37c2834437f715c93fdc6d340114d753b92612ab6d41cd`  
		Last Modified: Tue, 04 Jul 2023 03:52:22 GMT  
		Size: 27.6 MB (27637558 bytes)  
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
$ docker pull irssi@sha256:acbfc7fb13e89e47dad3c9137ef7fa896c5b75ac6533c06b67ade3057c9e2f97
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74052670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b08a4afb9566f8f4288fec8c2b1904505266fadc1a760928b037691c498c116`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:02 GMT
ADD file:f91bd2a174259cb69646fc34ba2fc6b8941ad8e171d2d7952a4d8ac3d95e2ad7 in / 
# Tue, 13 Jun 2023 00:09:06 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 02:26:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 02:26:40 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 02:26:47 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 02:26:50 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 02:26:53 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 02:30:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 02:30:54 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 02:30:57 GMT
USER user
# Thu, 22 Jun 2023 02:31:01 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:3fc28260a4d871ef9781cad2bb064ad7212a5063de3a1d35dba938ce82115e5b`  
		Last Modified: Tue, 13 Jun 2023 00:22:29 GMT  
		Size: 29.1 MB (29118129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b823be8377fd7186d28f794a5ec6493660f4e2208ded12e67636ec8750257d5`  
		Last Modified: Thu, 22 Jun 2023 02:31:36 GMT  
		Size: 16.9 MB (16925138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b18026dd902a0919c3a20766c7d6592948e9284efb4931907978339a21d327c`  
		Last Modified: Thu, 22 Jun 2023 02:31:17 GMT  
		Size: 3.3 KB (3298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a7f08c49e09c90d3e8b01aa906a42cfb03f4a598b544ec9a61c25259e54c77`  
		Last Modified: Thu, 22 Jun 2023 02:31:39 GMT  
		Size: 28.0 MB (28006105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; ppc64le

```console
$ docker pull irssi@sha256:808102c091e0f450e9fd0ff09dd607c235a6972c0982e8a909041d95ecdc9bb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82057404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6db42123514bb5bb81836bd52afbea22d1c59d575a9cf77f3cf7c9ada892240`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:51 GMT
ADD file:51887002f5002ccc662adbc6ecf1129e3db375a7a77b93da43cc9a8326b3c4b9 in / 
# Tue, 04 Jul 2023 01:17:53 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:36:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:36:17 GMT
ENV HOME=/home/user
# Tue, 04 Jul 2023 06:36:19 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 04 Jul 2023 06:36:19 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 06:36:20 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 04 Jul 2023 06:38:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 04 Jul 2023 06:38:43 GMT
WORKDIR /home/user
# Tue, 04 Jul 2023 06:38:43 GMT
USER user
# Tue, 04 Jul 2023 06:38:44 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ba99a1aa5a92d949d988e66df7723a542fd81bc30eef9d4269e8a899820d4bb2`  
		Last Modified: Tue, 04 Jul 2023 01:24:36 GMT  
		Size: 33.1 MB (33116716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a472629dc3d35e78fd046fa9c53281082c6b5a3cbf7f446fdcd3c04302e339`  
		Last Modified: Tue, 04 Jul 2023 06:39:27 GMT  
		Size: 18.8 MB (18754069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd7eaa97c83385d341b2e6b1823b9021baeb70ce87fcc47e593bff57983efce`  
		Last Modified: Tue, 04 Jul 2023 06:39:20 GMT  
		Size: 3.4 KB (3370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bc505f4c9f16e57c14adb02d3910e21d2031362fc3775c1f499928e77048f2`  
		Last Modified: Tue, 04 Jul 2023 06:39:29 GMT  
		Size: 30.2 MB (30183249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; s390x

```console
$ docker pull irssi@sha256:baa1df37d716889924e03405a3a5a2258c9e4520c6ad647a93d27caa6aba256f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72925568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:251b812805e137b9e051579adf3a25dd277d29aeacde9c29977afa4e7e513e0a`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Jun 2023 04:29:41 GMT
ADD file:739f4c23557ec0af5f4ba492c847b5d2f09dd81211c675d0e9eabe865d794e81 in / 
# Tue, 13 Jun 2023 04:29:43 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 08:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 08:51:21 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 08:51:21 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 08:51:21 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 08:51:22 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 08:51:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 08:52:00 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 08:52:00 GMT
USER user
# Thu, 22 Jun 2023 08:52:00 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6571b3abd058e377c7bd231c9029aff6eb25486bffb50229076d2e6a356a517f`  
		Last Modified: Tue, 13 Jun 2023 04:34:21 GMT  
		Size: 27.5 MB (27487928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0716cb6af8f5fcdc92d2d74f09de86858ee69ef8a2db7db71d6d60048930182`  
		Last Modified: Thu, 22 Jun 2023 08:53:07 GMT  
		Size: 18.2 MB (18206342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72ba9f202ec95947aa092a1c8f9fbac3cb975b47cf804734a0804722f737334`  
		Last Modified: Thu, 22 Jun 2023 08:53:04 GMT  
		Size: 3.4 KB (3368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e63e7ec95d8ded21367b4197e518b0bbc792b85525d9ca92b313e772bd4ec5`  
		Last Modified: Thu, 22 Jun 2023 08:53:08 GMT  
		Size: 27.2 MB (27227930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4-alpine`

```console
$ docker pull irssi@sha256:46a65610bad93dc8966f7e0a385bad0c9047a4d05c2f6ffedb5b2d3d0226138a
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
$ docker pull irssi@sha256:a768693cbea894b7b6135922520f7d532a6245dff8a3863024244a8ef9ffb14e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18439974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6be6e0e30722062f7d0e647c925e5239badb1739c57c83238d83b8a422b169fe`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:28:06 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:28:06 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:28:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:28:07 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:28:07 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:28:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:28:26 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:28:26 GMT
USER user
# Thu, 22 Jun 2023 01:28:26 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdb311d04d5ef03d3a3d6136863478ca52e56c787391712823006f36d8d5b9e`  
		Last Modified: Thu, 22 Jun 2023 01:29:12 GMT  
		Size: 9.6 MB (9637888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c8f7b98870f87f73429e0fb3e302a979d79d0c313dc49f64bd4b6d52763c08`  
		Last Modified: Thu, 22 Jun 2023 01:29:10 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3e36b711d362f59b8801dbb9ce1a3ec3bcaa5edd5b2366634e350cf308faee`  
		Last Modified: Thu, 22 Jun 2023 01:29:11 GMT  
		Size: 5.4 MB (5402922 bytes)  
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
$ docker pull irssi@sha256:6e7b11efe55cad75bda8ed33f8f0cd39a6c1e9978fc0c6e5272a2034b7ad35b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16621926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20abb587081f9ea7c13c022008f41792c8deeaca15a52406320be5f7e2aefd62`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:15 GMT
ADD file:082f034323c559f3cb9feb6422c88b1ec8017f436d6109e238a5c5384a32a90a in / 
# Wed, 14 Jun 2023 22:36:15 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:44:06 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:44:06 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:44:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:44:07 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:44:07 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:44:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:44:21 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:44:21 GMT
USER user
# Thu, 22 Jun 2023 01:44:21 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:633ba29fd335042456b6e2c073636f6fa30de56f1331c442914739b92a479974`  
		Last Modified: Wed, 14 Jun 2023 22:36:49 GMT  
		Size: 2.9 MB (2898508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e832bd75bc8892fffbcd2098ea32615beca89d5932e7bd6eae1c7973395a4a3c`  
		Last Modified: Thu, 22 Jun 2023 01:45:04 GMT  
		Size: 8.7 MB (8713654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9047f01d89a8f17a367c34c160949fb95db656ce766205320464b4f6a764b845`  
		Last Modified: Thu, 22 Jun 2023 01:45:01 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01ed6e5b2633e51a886c41895b2477ea69e8db678ddac23148e963ee8532ac0`  
		Last Modified: Thu, 22 Jun 2023 01:45:03 GMT  
		Size: 5.0 MB (5008480 bytes)  
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
$ docker pull irssi@sha256:95e45ba9fe7403d47a90aa5cbebc48878a954aa9248132df17d0b1964b5735f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18704414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c077a39e383a52f1690468a909209454afb356ca12011e784cc206bb0eabb553`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:49 GMT
ADD file:694c636c0dd19fd01accbc189e4c1dc4d063952692c6e7eb26dce02a7adba833 in / 
# Thu, 15 Jun 2023 00:39:49 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:46:07 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:46:08 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:46:09 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:46:09 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:46:10 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:46:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:46:37 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:46:38 GMT
USER user
# Thu, 22 Jun 2023 01:46:38 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ffa4a466dbb8eebd7e7f25590a9df12390de9016abf82279c29c9a64aa76491a`  
		Last Modified: Thu, 15 Jun 2023 00:40:26 GMT  
		Size: 3.3 MB (3344781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f791e21598b0753fdaac6f0554ec6cece5879b619efdbbb4c1b4449a37503445`  
		Last Modified: Thu, 22 Jun 2023 01:47:27 GMT  
		Size: 9.7 MB (9727162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05af372d8f57623b63ce194292c9d6e8cadad5b62006778fb3386de60bcded93`  
		Last Modified: Thu, 22 Jun 2023 01:47:24 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d0975696ee4b7f29a8e63ef0198dd4294f329a0a3db44dbe09d39d6194767f`  
		Last Modified: Thu, 22 Jun 2023 01:47:26 GMT  
		Size: 5.6 MB (5631188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:4f9ea0549297b400ee4e290a3e5d2548d5f935d01d81d209a4260dd9d9499e89
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18700399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31793e9f59a88f5efa8fcc186bd96e790b7d579acb15af792bf14f89c96d95f5`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 08:52:18 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 08:52:19 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 08:52:19 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 08:52:20 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 08:52:20 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 08:52:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 08:52:44 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 08:52:44 GMT
USER user
# Thu, 22 Jun 2023 08:52:44 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27869a2a741a6e4efe8b45710576e604e3fc468cef7d0feaa97e003f76aeb10`  
		Last Modified: Thu, 22 Jun 2023 08:53:34 GMT  
		Size: 10.1 MB (10078671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b47042a99d33af0f2ed5b3830ae99f7b13bb137fb93f1ace7e2d4922994df8d`  
		Last Modified: Thu, 22 Jun 2023 08:53:32 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24432dec00488946bcee10e0f328cc956d09781dd4d8165e1228aeecc1c4d390`  
		Last Modified: Thu, 22 Jun 2023 08:53:33 GMT  
		Size: 5.4 MB (5406948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4-alpine3.18`

```console
$ docker pull irssi@sha256:46a65610bad93dc8966f7e0a385bad0c9047a4d05c2f6ffedb5b2d3d0226138a
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
$ docker pull irssi@sha256:a768693cbea894b7b6135922520f7d532a6245dff8a3863024244a8ef9ffb14e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18439974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6be6e0e30722062f7d0e647c925e5239badb1739c57c83238d83b8a422b169fe`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:28:06 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:28:06 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:28:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:28:07 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:28:07 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:28:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:28:26 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:28:26 GMT
USER user
# Thu, 22 Jun 2023 01:28:26 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdb311d04d5ef03d3a3d6136863478ca52e56c787391712823006f36d8d5b9e`  
		Last Modified: Thu, 22 Jun 2023 01:29:12 GMT  
		Size: 9.6 MB (9637888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c8f7b98870f87f73429e0fb3e302a979d79d0c313dc49f64bd4b6d52763c08`  
		Last Modified: Thu, 22 Jun 2023 01:29:10 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3e36b711d362f59b8801dbb9ce1a3ec3bcaa5edd5b2366634e350cf308faee`  
		Last Modified: Thu, 22 Jun 2023 01:29:11 GMT  
		Size: 5.4 MB (5402922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

### `irssi:1.4-alpine3.18` - linux; arm variant v7

```console
$ docker pull irssi@sha256:6e7b11efe55cad75bda8ed33f8f0cd39a6c1e9978fc0c6e5272a2034b7ad35b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16621926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20abb587081f9ea7c13c022008f41792c8deeaca15a52406320be5f7e2aefd62`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:15 GMT
ADD file:082f034323c559f3cb9feb6422c88b1ec8017f436d6109e238a5c5384a32a90a in / 
# Wed, 14 Jun 2023 22:36:15 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:44:06 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:44:06 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:44:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:44:07 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:44:07 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:44:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:44:21 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:44:21 GMT
USER user
# Thu, 22 Jun 2023 01:44:21 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:633ba29fd335042456b6e2c073636f6fa30de56f1331c442914739b92a479974`  
		Last Modified: Wed, 14 Jun 2023 22:36:49 GMT  
		Size: 2.9 MB (2898508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e832bd75bc8892fffbcd2098ea32615beca89d5932e7bd6eae1c7973395a4a3c`  
		Last Modified: Thu, 22 Jun 2023 01:45:04 GMT  
		Size: 8.7 MB (8713654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9047f01d89a8f17a367c34c160949fb95db656ce766205320464b4f6a764b845`  
		Last Modified: Thu, 22 Jun 2023 01:45:01 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01ed6e5b2633e51a886c41895b2477ea69e8db678ddac23148e963ee8532ac0`  
		Last Modified: Thu, 22 Jun 2023 01:45:03 GMT  
		Size: 5.0 MB (5008480 bytes)  
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

### `irssi:1.4-alpine3.18` - linux; ppc64le

```console
$ docker pull irssi@sha256:95e45ba9fe7403d47a90aa5cbebc48878a954aa9248132df17d0b1964b5735f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18704414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c077a39e383a52f1690468a909209454afb356ca12011e784cc206bb0eabb553`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:49 GMT
ADD file:694c636c0dd19fd01accbc189e4c1dc4d063952692c6e7eb26dce02a7adba833 in / 
# Thu, 15 Jun 2023 00:39:49 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:46:07 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:46:08 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:46:09 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:46:09 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:46:10 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:46:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:46:37 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:46:38 GMT
USER user
# Thu, 22 Jun 2023 01:46:38 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ffa4a466dbb8eebd7e7f25590a9df12390de9016abf82279c29c9a64aa76491a`  
		Last Modified: Thu, 15 Jun 2023 00:40:26 GMT  
		Size: 3.3 MB (3344781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f791e21598b0753fdaac6f0554ec6cece5879b619efdbbb4c1b4449a37503445`  
		Last Modified: Thu, 22 Jun 2023 01:47:27 GMT  
		Size: 9.7 MB (9727162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05af372d8f57623b63ce194292c9d6e8cadad5b62006778fb3386de60bcded93`  
		Last Modified: Thu, 22 Jun 2023 01:47:24 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d0975696ee4b7f29a8e63ef0198dd4294f329a0a3db44dbe09d39d6194767f`  
		Last Modified: Thu, 22 Jun 2023 01:47:26 GMT  
		Size: 5.6 MB (5631188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine3.18` - linux; s390x

```console
$ docker pull irssi@sha256:4f9ea0549297b400ee4e290a3e5d2548d5f935d01d81d209a4260dd9d9499e89
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18700399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31793e9f59a88f5efa8fcc186bd96e790b7d579acb15af792bf14f89c96d95f5`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 08:52:18 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 08:52:19 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 08:52:19 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 08:52:20 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 08:52:20 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 08:52:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 08:52:44 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 08:52:44 GMT
USER user
# Thu, 22 Jun 2023 08:52:44 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27869a2a741a6e4efe8b45710576e604e3fc468cef7d0feaa97e003f76aeb10`  
		Last Modified: Thu, 22 Jun 2023 08:53:34 GMT  
		Size: 10.1 MB (10078671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b47042a99d33af0f2ed5b3830ae99f7b13bb137fb93f1ace7e2d4922994df8d`  
		Last Modified: Thu, 22 Jun 2023 08:53:32 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24432dec00488946bcee10e0f328cc956d09781dd4d8165e1228aeecc1c4d390`  
		Last Modified: Thu, 22 Jun 2023 08:53:33 GMT  
		Size: 5.4 MB (5406948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4-bookworm`

```console
$ docker pull irssi@sha256:69927d1ad99aec69bddc2a42727ee72f0bd0d005a9aba5c0667166b045d2dc34
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
$ docker pull irssi@sha256:58fc1c672bf293069b7789a309a03bcb34c93951017f2488c4037de7c2c68269
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (76048658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2e78b1ae299bcd0f8deef087b5454642320d910c779322916fad90990fbc810`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:42 GMT
ADD file:ba1250b6ecd5dd09d4914189d72741c2817988994e7da514bf62be439a34bdb5 in / 
# Mon, 12 Jun 2023 23:20:42 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 01:27:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 01:27:04 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:27:04 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:27:04 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:27:04 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:27:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 01:27:52 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:27:52 GMT
USER user
# Thu, 22 Jun 2023 01:27:53 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:5b5fe70539cd6989aa19f25826309f9715a9489cf1c057982d6a84c1ad8975c7`  
		Last Modified: Mon, 12 Jun 2023 23:25:49 GMT  
		Size: 29.1 MB (29124744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4909e07c2d187606b474bffed67e6b8f97ee741deba3ee1a6cc6e03a57e06d25`  
		Last Modified: Thu, 22 Jun 2023 01:28:49 GMT  
		Size: 18.2 MB (18242756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed55928edc7533b8545259265ffa0db2e9687da3460557c3885e41a0b49cbe0`  
		Last Modified: Thu, 22 Jun 2023 01:28:45 GMT  
		Size: 3.4 KB (3372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6731e4fa8db1fd048929e347b2b35f7b30b5a7d41015d14037ee7149376b11af`  
		Last Modified: Thu, 22 Jun 2023 01:28:50 GMT  
		Size: 28.7 MB (28677786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

### `irssi:1.4-bookworm` - linux; arm variant v7

```console
$ docker pull irssi@sha256:04fe9086e0677c27e634b48247d835bd76d770fb2d93a37e98e0f5d10ad930d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66699462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:347dde6d1977d7559b809d379aeb2d49c7dc1edb227ac50753bb5b436492f450`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Jul 2023 00:57:54 GMT
ADD file:d168d1710cbca4edb322c26348dafaf2b3a64980f52b8b790f334cdbd6a7047e in / 
# Tue, 04 Jul 2023 00:57:55 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:02:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:02:14 GMT
ENV HOME=/home/user
# Tue, 04 Jul 2023 05:02:15 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 04 Jul 2023 05:02:15 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 05:02:15 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 04 Jul 2023 05:02:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 04 Jul 2023 05:02:53 GMT
WORKDIR /home/user
# Tue, 04 Jul 2023 05:02:53 GMT
USER user
# Tue, 04 Jul 2023 05:02:53 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:340ace0baa422f18db718d7634c1c88a9650f4871dda2630ef15577120aa6816`  
		Last Modified: Tue, 04 Jul 2023 01:02:50 GMT  
		Size: 24.8 MB (24801264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26335a3dcbbb3fe7c73c15fa804eb199dc3d2c6f72d4b272290495ddc7d5d52`  
		Last Modified: Tue, 04 Jul 2023 05:03:15 GMT  
		Size: 16.7 MB (16675209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d7691ca1849da70e59df47ce1ae57125e975051c107f00f45a7c3cf16dba8d`  
		Last Modified: Tue, 04 Jul 2023 05:03:10 GMT  
		Size: 3.4 KB (3368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6467c4b92ddee02bde53da36ae6e65510038840b918475ce6e8b1923576edebc`  
		Last Modified: Tue, 04 Jul 2023 05:03:15 GMT  
		Size: 25.2 MB (25219621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-bookworm` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:c7c88dad0daea3ad57151de33054217941d7becf80f2dc11592f3a5dccc31cd9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74817355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63655ff173ab77b3325bf30ffb4193bc7ac59ae13e21dfb4f90bf03ae3939077`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:51:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:51:17 GMT
ENV HOME=/home/user
# Tue, 04 Jul 2023 03:51:17 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 04 Jul 2023 03:51:18 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 03:51:18 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 04 Jul 2023 03:51:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 04 Jul 2023 03:51:56 GMT
WORKDIR /home/user
# Tue, 04 Jul 2023 03:51:56 GMT
USER user
# Tue, 04 Jul 2023 03:51:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14ecf60c320eb05ae2ba16ad2774d3066ce556d0aacc4cfda7f3de6cf9aa09d`  
		Last Modified: Tue, 04 Jul 2023 03:52:21 GMT  
		Size: 18.0 MB (18023969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8369f911d29dedde0b1e053fb13ffe68ef5bc4ee1bf9929783256c66bb74805`  
		Last Modified: Tue, 04 Jul 2023 03:52:18 GMT  
		Size: 3.4 KB (3370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0551107dfe1234434d37c2834437f715c93fdc6d340114d753b92612ab6d41cd`  
		Last Modified: Tue, 04 Jul 2023 03:52:22 GMT  
		Size: 27.6 MB (27637558 bytes)  
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

### `irssi:1.4-bookworm` - linux; mips64le

```console
$ docker pull irssi@sha256:acbfc7fb13e89e47dad3c9137ef7fa896c5b75ac6533c06b67ade3057c9e2f97
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74052670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b08a4afb9566f8f4288fec8c2b1904505266fadc1a760928b037691c498c116`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:02 GMT
ADD file:f91bd2a174259cb69646fc34ba2fc6b8941ad8e171d2d7952a4d8ac3d95e2ad7 in / 
# Tue, 13 Jun 2023 00:09:06 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 02:26:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 02:26:40 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 02:26:47 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 02:26:50 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 02:26:53 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 02:30:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 02:30:54 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 02:30:57 GMT
USER user
# Thu, 22 Jun 2023 02:31:01 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:3fc28260a4d871ef9781cad2bb064ad7212a5063de3a1d35dba938ce82115e5b`  
		Last Modified: Tue, 13 Jun 2023 00:22:29 GMT  
		Size: 29.1 MB (29118129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b823be8377fd7186d28f794a5ec6493660f4e2208ded12e67636ec8750257d5`  
		Last Modified: Thu, 22 Jun 2023 02:31:36 GMT  
		Size: 16.9 MB (16925138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b18026dd902a0919c3a20766c7d6592948e9284efb4931907978339a21d327c`  
		Last Modified: Thu, 22 Jun 2023 02:31:17 GMT  
		Size: 3.3 KB (3298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a7f08c49e09c90d3e8b01aa906a42cfb03f4a598b544ec9a61c25259e54c77`  
		Last Modified: Thu, 22 Jun 2023 02:31:39 GMT  
		Size: 28.0 MB (28006105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-bookworm` - linux; ppc64le

```console
$ docker pull irssi@sha256:808102c091e0f450e9fd0ff09dd607c235a6972c0982e8a909041d95ecdc9bb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82057404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6db42123514bb5bb81836bd52afbea22d1c59d575a9cf77f3cf7c9ada892240`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:51 GMT
ADD file:51887002f5002ccc662adbc6ecf1129e3db375a7a77b93da43cc9a8326b3c4b9 in / 
# Tue, 04 Jul 2023 01:17:53 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:36:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:36:17 GMT
ENV HOME=/home/user
# Tue, 04 Jul 2023 06:36:19 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 04 Jul 2023 06:36:19 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 06:36:20 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 04 Jul 2023 06:38:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 04 Jul 2023 06:38:43 GMT
WORKDIR /home/user
# Tue, 04 Jul 2023 06:38:43 GMT
USER user
# Tue, 04 Jul 2023 06:38:44 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ba99a1aa5a92d949d988e66df7723a542fd81bc30eef9d4269e8a899820d4bb2`  
		Last Modified: Tue, 04 Jul 2023 01:24:36 GMT  
		Size: 33.1 MB (33116716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a472629dc3d35e78fd046fa9c53281082c6b5a3cbf7f446fdcd3c04302e339`  
		Last Modified: Tue, 04 Jul 2023 06:39:27 GMT  
		Size: 18.8 MB (18754069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd7eaa97c83385d341b2e6b1823b9021baeb70ce87fcc47e593bff57983efce`  
		Last Modified: Tue, 04 Jul 2023 06:39:20 GMT  
		Size: 3.4 KB (3370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bc505f4c9f16e57c14adb02d3910e21d2031362fc3775c1f499928e77048f2`  
		Last Modified: Tue, 04 Jul 2023 06:39:29 GMT  
		Size: 30.2 MB (30183249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-bookworm` - linux; s390x

```console
$ docker pull irssi@sha256:baa1df37d716889924e03405a3a5a2258c9e4520c6ad647a93d27caa6aba256f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72925568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:251b812805e137b9e051579adf3a25dd277d29aeacde9c29977afa4e7e513e0a`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Jun 2023 04:29:41 GMT
ADD file:739f4c23557ec0af5f4ba492c847b5d2f09dd81211c675d0e9eabe865d794e81 in / 
# Tue, 13 Jun 2023 04:29:43 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 08:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 08:51:21 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 08:51:21 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 08:51:21 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 08:51:22 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 08:51:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 08:52:00 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 08:52:00 GMT
USER user
# Thu, 22 Jun 2023 08:52:00 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6571b3abd058e377c7bd231c9029aff6eb25486bffb50229076d2e6a356a517f`  
		Last Modified: Tue, 13 Jun 2023 04:34:21 GMT  
		Size: 27.5 MB (27487928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0716cb6af8f5fcdc92d2d74f09de86858ee69ef8a2db7db71d6d60048930182`  
		Last Modified: Thu, 22 Jun 2023 08:53:07 GMT  
		Size: 18.2 MB (18206342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72ba9f202ec95947aa092a1c8f9fbac3cb975b47cf804734a0804722f737334`  
		Last Modified: Thu, 22 Jun 2023 08:53:04 GMT  
		Size: 3.4 KB (3368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e63e7ec95d8ded21367b4197e518b0bbc792b85525d9ca92b313e772bd4ec5`  
		Last Modified: Thu, 22 Jun 2023 08:53:08 GMT  
		Size: 27.2 MB (27227930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4.4`

```console
$ docker pull irssi@sha256:69927d1ad99aec69bddc2a42727ee72f0bd0d005a9aba5c0667166b045d2dc34
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
$ docker pull irssi@sha256:58fc1c672bf293069b7789a309a03bcb34c93951017f2488c4037de7c2c68269
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (76048658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2e78b1ae299bcd0f8deef087b5454642320d910c779322916fad90990fbc810`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:42 GMT
ADD file:ba1250b6ecd5dd09d4914189d72741c2817988994e7da514bf62be439a34bdb5 in / 
# Mon, 12 Jun 2023 23:20:42 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 01:27:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 01:27:04 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:27:04 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:27:04 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:27:04 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:27:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 01:27:52 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:27:52 GMT
USER user
# Thu, 22 Jun 2023 01:27:53 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:5b5fe70539cd6989aa19f25826309f9715a9489cf1c057982d6a84c1ad8975c7`  
		Last Modified: Mon, 12 Jun 2023 23:25:49 GMT  
		Size: 29.1 MB (29124744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4909e07c2d187606b474bffed67e6b8f97ee741deba3ee1a6cc6e03a57e06d25`  
		Last Modified: Thu, 22 Jun 2023 01:28:49 GMT  
		Size: 18.2 MB (18242756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed55928edc7533b8545259265ffa0db2e9687da3460557c3885e41a0b49cbe0`  
		Last Modified: Thu, 22 Jun 2023 01:28:45 GMT  
		Size: 3.4 KB (3372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6731e4fa8db1fd048929e347b2b35f7b30b5a7d41015d14037ee7149376b11af`  
		Last Modified: Thu, 22 Jun 2023 01:28:50 GMT  
		Size: 28.7 MB (28677786 bytes)  
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
$ docker pull irssi@sha256:04fe9086e0677c27e634b48247d835bd76d770fb2d93a37e98e0f5d10ad930d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66699462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:347dde6d1977d7559b809d379aeb2d49c7dc1edb227ac50753bb5b436492f450`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Jul 2023 00:57:54 GMT
ADD file:d168d1710cbca4edb322c26348dafaf2b3a64980f52b8b790f334cdbd6a7047e in / 
# Tue, 04 Jul 2023 00:57:55 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:02:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:02:14 GMT
ENV HOME=/home/user
# Tue, 04 Jul 2023 05:02:15 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 04 Jul 2023 05:02:15 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 05:02:15 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 04 Jul 2023 05:02:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 04 Jul 2023 05:02:53 GMT
WORKDIR /home/user
# Tue, 04 Jul 2023 05:02:53 GMT
USER user
# Tue, 04 Jul 2023 05:02:53 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:340ace0baa422f18db718d7634c1c88a9650f4871dda2630ef15577120aa6816`  
		Last Modified: Tue, 04 Jul 2023 01:02:50 GMT  
		Size: 24.8 MB (24801264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26335a3dcbbb3fe7c73c15fa804eb199dc3d2c6f72d4b272290495ddc7d5d52`  
		Last Modified: Tue, 04 Jul 2023 05:03:15 GMT  
		Size: 16.7 MB (16675209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d7691ca1849da70e59df47ce1ae57125e975051c107f00f45a7c3cf16dba8d`  
		Last Modified: Tue, 04 Jul 2023 05:03:10 GMT  
		Size: 3.4 KB (3368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6467c4b92ddee02bde53da36ae6e65510038840b918475ce6e8b1923576edebc`  
		Last Modified: Tue, 04 Jul 2023 05:03:15 GMT  
		Size: 25.2 MB (25219621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.4` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:c7c88dad0daea3ad57151de33054217941d7becf80f2dc11592f3a5dccc31cd9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74817355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63655ff173ab77b3325bf30ffb4193bc7ac59ae13e21dfb4f90bf03ae3939077`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:51:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:51:17 GMT
ENV HOME=/home/user
# Tue, 04 Jul 2023 03:51:17 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 04 Jul 2023 03:51:18 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 03:51:18 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 04 Jul 2023 03:51:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 04 Jul 2023 03:51:56 GMT
WORKDIR /home/user
# Tue, 04 Jul 2023 03:51:56 GMT
USER user
# Tue, 04 Jul 2023 03:51:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14ecf60c320eb05ae2ba16ad2774d3066ce556d0aacc4cfda7f3de6cf9aa09d`  
		Last Modified: Tue, 04 Jul 2023 03:52:21 GMT  
		Size: 18.0 MB (18023969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8369f911d29dedde0b1e053fb13ffe68ef5bc4ee1bf9929783256c66bb74805`  
		Last Modified: Tue, 04 Jul 2023 03:52:18 GMT  
		Size: 3.4 KB (3370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0551107dfe1234434d37c2834437f715c93fdc6d340114d753b92612ab6d41cd`  
		Last Modified: Tue, 04 Jul 2023 03:52:22 GMT  
		Size: 27.6 MB (27637558 bytes)  
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
$ docker pull irssi@sha256:acbfc7fb13e89e47dad3c9137ef7fa896c5b75ac6533c06b67ade3057c9e2f97
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74052670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b08a4afb9566f8f4288fec8c2b1904505266fadc1a760928b037691c498c116`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:02 GMT
ADD file:f91bd2a174259cb69646fc34ba2fc6b8941ad8e171d2d7952a4d8ac3d95e2ad7 in / 
# Tue, 13 Jun 2023 00:09:06 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 02:26:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 02:26:40 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 02:26:47 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 02:26:50 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 02:26:53 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 02:30:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 02:30:54 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 02:30:57 GMT
USER user
# Thu, 22 Jun 2023 02:31:01 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:3fc28260a4d871ef9781cad2bb064ad7212a5063de3a1d35dba938ce82115e5b`  
		Last Modified: Tue, 13 Jun 2023 00:22:29 GMT  
		Size: 29.1 MB (29118129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b823be8377fd7186d28f794a5ec6493660f4e2208ded12e67636ec8750257d5`  
		Last Modified: Thu, 22 Jun 2023 02:31:36 GMT  
		Size: 16.9 MB (16925138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b18026dd902a0919c3a20766c7d6592948e9284efb4931907978339a21d327c`  
		Last Modified: Thu, 22 Jun 2023 02:31:17 GMT  
		Size: 3.3 KB (3298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a7f08c49e09c90d3e8b01aa906a42cfb03f4a598b544ec9a61c25259e54c77`  
		Last Modified: Thu, 22 Jun 2023 02:31:39 GMT  
		Size: 28.0 MB (28006105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.4` - linux; ppc64le

```console
$ docker pull irssi@sha256:808102c091e0f450e9fd0ff09dd607c235a6972c0982e8a909041d95ecdc9bb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82057404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6db42123514bb5bb81836bd52afbea22d1c59d575a9cf77f3cf7c9ada892240`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:51 GMT
ADD file:51887002f5002ccc662adbc6ecf1129e3db375a7a77b93da43cc9a8326b3c4b9 in / 
# Tue, 04 Jul 2023 01:17:53 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:36:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:36:17 GMT
ENV HOME=/home/user
# Tue, 04 Jul 2023 06:36:19 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 04 Jul 2023 06:36:19 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 06:36:20 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 04 Jul 2023 06:38:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 04 Jul 2023 06:38:43 GMT
WORKDIR /home/user
# Tue, 04 Jul 2023 06:38:43 GMT
USER user
# Tue, 04 Jul 2023 06:38:44 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ba99a1aa5a92d949d988e66df7723a542fd81bc30eef9d4269e8a899820d4bb2`  
		Last Modified: Tue, 04 Jul 2023 01:24:36 GMT  
		Size: 33.1 MB (33116716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a472629dc3d35e78fd046fa9c53281082c6b5a3cbf7f446fdcd3c04302e339`  
		Last Modified: Tue, 04 Jul 2023 06:39:27 GMT  
		Size: 18.8 MB (18754069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd7eaa97c83385d341b2e6b1823b9021baeb70ce87fcc47e593bff57983efce`  
		Last Modified: Tue, 04 Jul 2023 06:39:20 GMT  
		Size: 3.4 KB (3370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bc505f4c9f16e57c14adb02d3910e21d2031362fc3775c1f499928e77048f2`  
		Last Modified: Tue, 04 Jul 2023 06:39:29 GMT  
		Size: 30.2 MB (30183249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.4` - linux; s390x

```console
$ docker pull irssi@sha256:baa1df37d716889924e03405a3a5a2258c9e4520c6ad647a93d27caa6aba256f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72925568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:251b812805e137b9e051579adf3a25dd277d29aeacde9c29977afa4e7e513e0a`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Jun 2023 04:29:41 GMT
ADD file:739f4c23557ec0af5f4ba492c847b5d2f09dd81211c675d0e9eabe865d794e81 in / 
# Tue, 13 Jun 2023 04:29:43 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 08:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 08:51:21 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 08:51:21 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 08:51:21 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 08:51:22 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 08:51:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 08:52:00 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 08:52:00 GMT
USER user
# Thu, 22 Jun 2023 08:52:00 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6571b3abd058e377c7bd231c9029aff6eb25486bffb50229076d2e6a356a517f`  
		Last Modified: Tue, 13 Jun 2023 04:34:21 GMT  
		Size: 27.5 MB (27487928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0716cb6af8f5fcdc92d2d74f09de86858ee69ef8a2db7db71d6d60048930182`  
		Last Modified: Thu, 22 Jun 2023 08:53:07 GMT  
		Size: 18.2 MB (18206342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72ba9f202ec95947aa092a1c8f9fbac3cb975b47cf804734a0804722f737334`  
		Last Modified: Thu, 22 Jun 2023 08:53:04 GMT  
		Size: 3.4 KB (3368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e63e7ec95d8ded21367b4197e518b0bbc792b85525d9ca92b313e772bd4ec5`  
		Last Modified: Thu, 22 Jun 2023 08:53:08 GMT  
		Size: 27.2 MB (27227930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4.4-alpine`

```console
$ docker pull irssi@sha256:46a65610bad93dc8966f7e0a385bad0c9047a4d05c2f6ffedb5b2d3d0226138a
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
$ docker pull irssi@sha256:a768693cbea894b7b6135922520f7d532a6245dff8a3863024244a8ef9ffb14e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18439974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6be6e0e30722062f7d0e647c925e5239badb1739c57c83238d83b8a422b169fe`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:28:06 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:28:06 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:28:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:28:07 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:28:07 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:28:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:28:26 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:28:26 GMT
USER user
# Thu, 22 Jun 2023 01:28:26 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdb311d04d5ef03d3a3d6136863478ca52e56c787391712823006f36d8d5b9e`  
		Last Modified: Thu, 22 Jun 2023 01:29:12 GMT  
		Size: 9.6 MB (9637888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c8f7b98870f87f73429e0fb3e302a979d79d0c313dc49f64bd4b6d52763c08`  
		Last Modified: Thu, 22 Jun 2023 01:29:10 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3e36b711d362f59b8801dbb9ce1a3ec3bcaa5edd5b2366634e350cf308faee`  
		Last Modified: Thu, 22 Jun 2023 01:29:11 GMT  
		Size: 5.4 MB (5402922 bytes)  
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
$ docker pull irssi@sha256:6e7b11efe55cad75bda8ed33f8f0cd39a6c1e9978fc0c6e5272a2034b7ad35b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16621926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20abb587081f9ea7c13c022008f41792c8deeaca15a52406320be5f7e2aefd62`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:15 GMT
ADD file:082f034323c559f3cb9feb6422c88b1ec8017f436d6109e238a5c5384a32a90a in / 
# Wed, 14 Jun 2023 22:36:15 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:44:06 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:44:06 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:44:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:44:07 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:44:07 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:44:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:44:21 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:44:21 GMT
USER user
# Thu, 22 Jun 2023 01:44:21 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:633ba29fd335042456b6e2c073636f6fa30de56f1331c442914739b92a479974`  
		Last Modified: Wed, 14 Jun 2023 22:36:49 GMT  
		Size: 2.9 MB (2898508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e832bd75bc8892fffbcd2098ea32615beca89d5932e7bd6eae1c7973395a4a3c`  
		Last Modified: Thu, 22 Jun 2023 01:45:04 GMT  
		Size: 8.7 MB (8713654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9047f01d89a8f17a367c34c160949fb95db656ce766205320464b4f6a764b845`  
		Last Modified: Thu, 22 Jun 2023 01:45:01 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01ed6e5b2633e51a886c41895b2477ea69e8db678ddac23148e963ee8532ac0`  
		Last Modified: Thu, 22 Jun 2023 01:45:03 GMT  
		Size: 5.0 MB (5008480 bytes)  
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
$ docker pull irssi@sha256:95e45ba9fe7403d47a90aa5cbebc48878a954aa9248132df17d0b1964b5735f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18704414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c077a39e383a52f1690468a909209454afb356ca12011e784cc206bb0eabb553`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:49 GMT
ADD file:694c636c0dd19fd01accbc189e4c1dc4d063952692c6e7eb26dce02a7adba833 in / 
# Thu, 15 Jun 2023 00:39:49 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:46:07 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:46:08 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:46:09 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:46:09 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:46:10 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:46:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:46:37 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:46:38 GMT
USER user
# Thu, 22 Jun 2023 01:46:38 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ffa4a466dbb8eebd7e7f25590a9df12390de9016abf82279c29c9a64aa76491a`  
		Last Modified: Thu, 15 Jun 2023 00:40:26 GMT  
		Size: 3.3 MB (3344781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f791e21598b0753fdaac6f0554ec6cece5879b619efdbbb4c1b4449a37503445`  
		Last Modified: Thu, 22 Jun 2023 01:47:27 GMT  
		Size: 9.7 MB (9727162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05af372d8f57623b63ce194292c9d6e8cadad5b62006778fb3386de60bcded93`  
		Last Modified: Thu, 22 Jun 2023 01:47:24 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d0975696ee4b7f29a8e63ef0198dd4294f329a0a3db44dbe09d39d6194767f`  
		Last Modified: Thu, 22 Jun 2023 01:47:26 GMT  
		Size: 5.6 MB (5631188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.4-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:4f9ea0549297b400ee4e290a3e5d2548d5f935d01d81d209a4260dd9d9499e89
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18700399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31793e9f59a88f5efa8fcc186bd96e790b7d579acb15af792bf14f89c96d95f5`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 08:52:18 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 08:52:19 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 08:52:19 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 08:52:20 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 08:52:20 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 08:52:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 08:52:44 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 08:52:44 GMT
USER user
# Thu, 22 Jun 2023 08:52:44 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27869a2a741a6e4efe8b45710576e604e3fc468cef7d0feaa97e003f76aeb10`  
		Last Modified: Thu, 22 Jun 2023 08:53:34 GMT  
		Size: 10.1 MB (10078671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b47042a99d33af0f2ed5b3830ae99f7b13bb137fb93f1ace7e2d4922994df8d`  
		Last Modified: Thu, 22 Jun 2023 08:53:32 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24432dec00488946bcee10e0f328cc956d09781dd4d8165e1228aeecc1c4d390`  
		Last Modified: Thu, 22 Jun 2023 08:53:33 GMT  
		Size: 5.4 MB (5406948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4.4-alpine3.18`

```console
$ docker pull irssi@sha256:46a65610bad93dc8966f7e0a385bad0c9047a4d05c2f6ffedb5b2d3d0226138a
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

### `irssi:1.4.4-alpine3.18` - linux; amd64

```console
$ docker pull irssi@sha256:a768693cbea894b7b6135922520f7d532a6245dff8a3863024244a8ef9ffb14e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18439974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6be6e0e30722062f7d0e647c925e5239badb1739c57c83238d83b8a422b169fe`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:28:06 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:28:06 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:28:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:28:07 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:28:07 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:28:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:28:26 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:28:26 GMT
USER user
# Thu, 22 Jun 2023 01:28:26 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdb311d04d5ef03d3a3d6136863478ca52e56c787391712823006f36d8d5b9e`  
		Last Modified: Thu, 22 Jun 2023 01:29:12 GMT  
		Size: 9.6 MB (9637888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c8f7b98870f87f73429e0fb3e302a979d79d0c313dc49f64bd4b6d52763c08`  
		Last Modified: Thu, 22 Jun 2023 01:29:10 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3e36b711d362f59b8801dbb9ce1a3ec3bcaa5edd5b2366634e350cf308faee`  
		Last Modified: Thu, 22 Jun 2023 01:29:11 GMT  
		Size: 5.4 MB (5402922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

### `irssi:1.4.4-alpine3.18` - linux; arm variant v7

```console
$ docker pull irssi@sha256:6e7b11efe55cad75bda8ed33f8f0cd39a6c1e9978fc0c6e5272a2034b7ad35b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16621926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20abb587081f9ea7c13c022008f41792c8deeaca15a52406320be5f7e2aefd62`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:15 GMT
ADD file:082f034323c559f3cb9feb6422c88b1ec8017f436d6109e238a5c5384a32a90a in / 
# Wed, 14 Jun 2023 22:36:15 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:44:06 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:44:06 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:44:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:44:07 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:44:07 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:44:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:44:21 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:44:21 GMT
USER user
# Thu, 22 Jun 2023 01:44:21 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:633ba29fd335042456b6e2c073636f6fa30de56f1331c442914739b92a479974`  
		Last Modified: Wed, 14 Jun 2023 22:36:49 GMT  
		Size: 2.9 MB (2898508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e832bd75bc8892fffbcd2098ea32615beca89d5932e7bd6eae1c7973395a4a3c`  
		Last Modified: Thu, 22 Jun 2023 01:45:04 GMT  
		Size: 8.7 MB (8713654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9047f01d89a8f17a367c34c160949fb95db656ce766205320464b4f6a764b845`  
		Last Modified: Thu, 22 Jun 2023 01:45:01 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01ed6e5b2633e51a886c41895b2477ea69e8db678ddac23148e963ee8532ac0`  
		Last Modified: Thu, 22 Jun 2023 01:45:03 GMT  
		Size: 5.0 MB (5008480 bytes)  
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

### `irssi:1.4.4-alpine3.18` - linux; ppc64le

```console
$ docker pull irssi@sha256:95e45ba9fe7403d47a90aa5cbebc48878a954aa9248132df17d0b1964b5735f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18704414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c077a39e383a52f1690468a909209454afb356ca12011e784cc206bb0eabb553`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:49 GMT
ADD file:694c636c0dd19fd01accbc189e4c1dc4d063952692c6e7eb26dce02a7adba833 in / 
# Thu, 15 Jun 2023 00:39:49 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:46:07 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:46:08 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:46:09 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:46:09 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:46:10 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:46:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:46:37 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:46:38 GMT
USER user
# Thu, 22 Jun 2023 01:46:38 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ffa4a466dbb8eebd7e7f25590a9df12390de9016abf82279c29c9a64aa76491a`  
		Last Modified: Thu, 15 Jun 2023 00:40:26 GMT  
		Size: 3.3 MB (3344781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f791e21598b0753fdaac6f0554ec6cece5879b619efdbbb4c1b4449a37503445`  
		Last Modified: Thu, 22 Jun 2023 01:47:27 GMT  
		Size: 9.7 MB (9727162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05af372d8f57623b63ce194292c9d6e8cadad5b62006778fb3386de60bcded93`  
		Last Modified: Thu, 22 Jun 2023 01:47:24 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d0975696ee4b7f29a8e63ef0198dd4294f329a0a3db44dbe09d39d6194767f`  
		Last Modified: Thu, 22 Jun 2023 01:47:26 GMT  
		Size: 5.6 MB (5631188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.4-alpine3.18` - linux; s390x

```console
$ docker pull irssi@sha256:4f9ea0549297b400ee4e290a3e5d2548d5f935d01d81d209a4260dd9d9499e89
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18700399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31793e9f59a88f5efa8fcc186bd96e790b7d579acb15af792bf14f89c96d95f5`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 08:52:18 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 08:52:19 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 08:52:19 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 08:52:20 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 08:52:20 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 08:52:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 08:52:44 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 08:52:44 GMT
USER user
# Thu, 22 Jun 2023 08:52:44 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27869a2a741a6e4efe8b45710576e604e3fc468cef7d0feaa97e003f76aeb10`  
		Last Modified: Thu, 22 Jun 2023 08:53:34 GMT  
		Size: 10.1 MB (10078671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b47042a99d33af0f2ed5b3830ae99f7b13bb137fb93f1ace7e2d4922994df8d`  
		Last Modified: Thu, 22 Jun 2023 08:53:32 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24432dec00488946bcee10e0f328cc956d09781dd4d8165e1228aeecc1c4d390`  
		Last Modified: Thu, 22 Jun 2023 08:53:33 GMT  
		Size: 5.4 MB (5406948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4.4-bookworm`

```console
$ docker pull irssi@sha256:69927d1ad99aec69bddc2a42727ee72f0bd0d005a9aba5c0667166b045d2dc34
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

### `irssi:1.4.4-bookworm` - linux; amd64

```console
$ docker pull irssi@sha256:58fc1c672bf293069b7789a309a03bcb34c93951017f2488c4037de7c2c68269
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (76048658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2e78b1ae299bcd0f8deef087b5454642320d910c779322916fad90990fbc810`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:42 GMT
ADD file:ba1250b6ecd5dd09d4914189d72741c2817988994e7da514bf62be439a34bdb5 in / 
# Mon, 12 Jun 2023 23:20:42 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 01:27:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 01:27:04 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:27:04 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:27:04 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:27:04 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:27:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 01:27:52 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:27:52 GMT
USER user
# Thu, 22 Jun 2023 01:27:53 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:5b5fe70539cd6989aa19f25826309f9715a9489cf1c057982d6a84c1ad8975c7`  
		Last Modified: Mon, 12 Jun 2023 23:25:49 GMT  
		Size: 29.1 MB (29124744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4909e07c2d187606b474bffed67e6b8f97ee741deba3ee1a6cc6e03a57e06d25`  
		Last Modified: Thu, 22 Jun 2023 01:28:49 GMT  
		Size: 18.2 MB (18242756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed55928edc7533b8545259265ffa0db2e9687da3460557c3885e41a0b49cbe0`  
		Last Modified: Thu, 22 Jun 2023 01:28:45 GMT  
		Size: 3.4 KB (3372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6731e4fa8db1fd048929e347b2b35f7b30b5a7d41015d14037ee7149376b11af`  
		Last Modified: Thu, 22 Jun 2023 01:28:50 GMT  
		Size: 28.7 MB (28677786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

### `irssi:1.4.4-bookworm` - linux; arm variant v7

```console
$ docker pull irssi@sha256:04fe9086e0677c27e634b48247d835bd76d770fb2d93a37e98e0f5d10ad930d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66699462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:347dde6d1977d7559b809d379aeb2d49c7dc1edb227ac50753bb5b436492f450`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Jul 2023 00:57:54 GMT
ADD file:d168d1710cbca4edb322c26348dafaf2b3a64980f52b8b790f334cdbd6a7047e in / 
# Tue, 04 Jul 2023 00:57:55 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:02:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:02:14 GMT
ENV HOME=/home/user
# Tue, 04 Jul 2023 05:02:15 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 04 Jul 2023 05:02:15 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 05:02:15 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 04 Jul 2023 05:02:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 04 Jul 2023 05:02:53 GMT
WORKDIR /home/user
# Tue, 04 Jul 2023 05:02:53 GMT
USER user
# Tue, 04 Jul 2023 05:02:53 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:340ace0baa422f18db718d7634c1c88a9650f4871dda2630ef15577120aa6816`  
		Last Modified: Tue, 04 Jul 2023 01:02:50 GMT  
		Size: 24.8 MB (24801264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26335a3dcbbb3fe7c73c15fa804eb199dc3d2c6f72d4b272290495ddc7d5d52`  
		Last Modified: Tue, 04 Jul 2023 05:03:15 GMT  
		Size: 16.7 MB (16675209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d7691ca1849da70e59df47ce1ae57125e975051c107f00f45a7c3cf16dba8d`  
		Last Modified: Tue, 04 Jul 2023 05:03:10 GMT  
		Size: 3.4 KB (3368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6467c4b92ddee02bde53da36ae6e65510038840b918475ce6e8b1923576edebc`  
		Last Modified: Tue, 04 Jul 2023 05:03:15 GMT  
		Size: 25.2 MB (25219621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.4-bookworm` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:c7c88dad0daea3ad57151de33054217941d7becf80f2dc11592f3a5dccc31cd9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74817355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63655ff173ab77b3325bf30ffb4193bc7ac59ae13e21dfb4f90bf03ae3939077`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:51:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:51:17 GMT
ENV HOME=/home/user
# Tue, 04 Jul 2023 03:51:17 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 04 Jul 2023 03:51:18 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 03:51:18 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 04 Jul 2023 03:51:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 04 Jul 2023 03:51:56 GMT
WORKDIR /home/user
# Tue, 04 Jul 2023 03:51:56 GMT
USER user
# Tue, 04 Jul 2023 03:51:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14ecf60c320eb05ae2ba16ad2774d3066ce556d0aacc4cfda7f3de6cf9aa09d`  
		Last Modified: Tue, 04 Jul 2023 03:52:21 GMT  
		Size: 18.0 MB (18023969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8369f911d29dedde0b1e053fb13ffe68ef5bc4ee1bf9929783256c66bb74805`  
		Last Modified: Tue, 04 Jul 2023 03:52:18 GMT  
		Size: 3.4 KB (3370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0551107dfe1234434d37c2834437f715c93fdc6d340114d753b92612ab6d41cd`  
		Last Modified: Tue, 04 Jul 2023 03:52:22 GMT  
		Size: 27.6 MB (27637558 bytes)  
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

### `irssi:1.4.4-bookworm` - linux; mips64le

```console
$ docker pull irssi@sha256:acbfc7fb13e89e47dad3c9137ef7fa896c5b75ac6533c06b67ade3057c9e2f97
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74052670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b08a4afb9566f8f4288fec8c2b1904505266fadc1a760928b037691c498c116`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:02 GMT
ADD file:f91bd2a174259cb69646fc34ba2fc6b8941ad8e171d2d7952a4d8ac3d95e2ad7 in / 
# Tue, 13 Jun 2023 00:09:06 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 02:26:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 02:26:40 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 02:26:47 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 02:26:50 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 02:26:53 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 02:30:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 02:30:54 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 02:30:57 GMT
USER user
# Thu, 22 Jun 2023 02:31:01 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:3fc28260a4d871ef9781cad2bb064ad7212a5063de3a1d35dba938ce82115e5b`  
		Last Modified: Tue, 13 Jun 2023 00:22:29 GMT  
		Size: 29.1 MB (29118129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b823be8377fd7186d28f794a5ec6493660f4e2208ded12e67636ec8750257d5`  
		Last Modified: Thu, 22 Jun 2023 02:31:36 GMT  
		Size: 16.9 MB (16925138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b18026dd902a0919c3a20766c7d6592948e9284efb4931907978339a21d327c`  
		Last Modified: Thu, 22 Jun 2023 02:31:17 GMT  
		Size: 3.3 KB (3298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a7f08c49e09c90d3e8b01aa906a42cfb03f4a598b544ec9a61c25259e54c77`  
		Last Modified: Thu, 22 Jun 2023 02:31:39 GMT  
		Size: 28.0 MB (28006105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.4-bookworm` - linux; ppc64le

```console
$ docker pull irssi@sha256:808102c091e0f450e9fd0ff09dd607c235a6972c0982e8a909041d95ecdc9bb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82057404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6db42123514bb5bb81836bd52afbea22d1c59d575a9cf77f3cf7c9ada892240`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:51 GMT
ADD file:51887002f5002ccc662adbc6ecf1129e3db375a7a77b93da43cc9a8326b3c4b9 in / 
# Tue, 04 Jul 2023 01:17:53 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:36:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:36:17 GMT
ENV HOME=/home/user
# Tue, 04 Jul 2023 06:36:19 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 04 Jul 2023 06:36:19 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 06:36:20 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 04 Jul 2023 06:38:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 04 Jul 2023 06:38:43 GMT
WORKDIR /home/user
# Tue, 04 Jul 2023 06:38:43 GMT
USER user
# Tue, 04 Jul 2023 06:38:44 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ba99a1aa5a92d949d988e66df7723a542fd81bc30eef9d4269e8a899820d4bb2`  
		Last Modified: Tue, 04 Jul 2023 01:24:36 GMT  
		Size: 33.1 MB (33116716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a472629dc3d35e78fd046fa9c53281082c6b5a3cbf7f446fdcd3c04302e339`  
		Last Modified: Tue, 04 Jul 2023 06:39:27 GMT  
		Size: 18.8 MB (18754069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd7eaa97c83385d341b2e6b1823b9021baeb70ce87fcc47e593bff57983efce`  
		Last Modified: Tue, 04 Jul 2023 06:39:20 GMT  
		Size: 3.4 KB (3370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bc505f4c9f16e57c14adb02d3910e21d2031362fc3775c1f499928e77048f2`  
		Last Modified: Tue, 04 Jul 2023 06:39:29 GMT  
		Size: 30.2 MB (30183249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.4-bookworm` - linux; s390x

```console
$ docker pull irssi@sha256:baa1df37d716889924e03405a3a5a2258c9e4520c6ad647a93d27caa6aba256f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72925568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:251b812805e137b9e051579adf3a25dd277d29aeacde9c29977afa4e7e513e0a`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Jun 2023 04:29:41 GMT
ADD file:739f4c23557ec0af5f4ba492c847b5d2f09dd81211c675d0e9eabe865d794e81 in / 
# Tue, 13 Jun 2023 04:29:43 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 08:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 08:51:21 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 08:51:21 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 08:51:21 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 08:51:22 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 08:51:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 08:52:00 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 08:52:00 GMT
USER user
# Thu, 22 Jun 2023 08:52:00 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6571b3abd058e377c7bd231c9029aff6eb25486bffb50229076d2e6a356a517f`  
		Last Modified: Tue, 13 Jun 2023 04:34:21 GMT  
		Size: 27.5 MB (27487928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0716cb6af8f5fcdc92d2d74f09de86858ee69ef8a2db7db71d6d60048930182`  
		Last Modified: Thu, 22 Jun 2023 08:53:07 GMT  
		Size: 18.2 MB (18206342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72ba9f202ec95947aa092a1c8f9fbac3cb975b47cf804734a0804722f737334`  
		Last Modified: Thu, 22 Jun 2023 08:53:04 GMT  
		Size: 3.4 KB (3368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e63e7ec95d8ded21367b4197e518b0bbc792b85525d9ca92b313e772bd4ec5`  
		Last Modified: Thu, 22 Jun 2023 08:53:08 GMT  
		Size: 27.2 MB (27227930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:alpine`

```console
$ docker pull irssi@sha256:46a65610bad93dc8966f7e0a385bad0c9047a4d05c2f6ffedb5b2d3d0226138a
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
$ docker pull irssi@sha256:a768693cbea894b7b6135922520f7d532a6245dff8a3863024244a8ef9ffb14e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18439974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6be6e0e30722062f7d0e647c925e5239badb1739c57c83238d83b8a422b169fe`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:28:06 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:28:06 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:28:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:28:07 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:28:07 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:28:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:28:26 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:28:26 GMT
USER user
# Thu, 22 Jun 2023 01:28:26 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdb311d04d5ef03d3a3d6136863478ca52e56c787391712823006f36d8d5b9e`  
		Last Modified: Thu, 22 Jun 2023 01:29:12 GMT  
		Size: 9.6 MB (9637888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c8f7b98870f87f73429e0fb3e302a979d79d0c313dc49f64bd4b6d52763c08`  
		Last Modified: Thu, 22 Jun 2023 01:29:10 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3e36b711d362f59b8801dbb9ce1a3ec3bcaa5edd5b2366634e350cf308faee`  
		Last Modified: Thu, 22 Jun 2023 01:29:11 GMT  
		Size: 5.4 MB (5402922 bytes)  
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
$ docker pull irssi@sha256:6e7b11efe55cad75bda8ed33f8f0cd39a6c1e9978fc0c6e5272a2034b7ad35b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16621926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20abb587081f9ea7c13c022008f41792c8deeaca15a52406320be5f7e2aefd62`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:15 GMT
ADD file:082f034323c559f3cb9feb6422c88b1ec8017f436d6109e238a5c5384a32a90a in / 
# Wed, 14 Jun 2023 22:36:15 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:44:06 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:44:06 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:44:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:44:07 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:44:07 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:44:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:44:21 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:44:21 GMT
USER user
# Thu, 22 Jun 2023 01:44:21 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:633ba29fd335042456b6e2c073636f6fa30de56f1331c442914739b92a479974`  
		Last Modified: Wed, 14 Jun 2023 22:36:49 GMT  
		Size: 2.9 MB (2898508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e832bd75bc8892fffbcd2098ea32615beca89d5932e7bd6eae1c7973395a4a3c`  
		Last Modified: Thu, 22 Jun 2023 01:45:04 GMT  
		Size: 8.7 MB (8713654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9047f01d89a8f17a367c34c160949fb95db656ce766205320464b4f6a764b845`  
		Last Modified: Thu, 22 Jun 2023 01:45:01 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01ed6e5b2633e51a886c41895b2477ea69e8db678ddac23148e963ee8532ac0`  
		Last Modified: Thu, 22 Jun 2023 01:45:03 GMT  
		Size: 5.0 MB (5008480 bytes)  
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
$ docker pull irssi@sha256:95e45ba9fe7403d47a90aa5cbebc48878a954aa9248132df17d0b1964b5735f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18704414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c077a39e383a52f1690468a909209454afb356ca12011e784cc206bb0eabb553`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:49 GMT
ADD file:694c636c0dd19fd01accbc189e4c1dc4d063952692c6e7eb26dce02a7adba833 in / 
# Thu, 15 Jun 2023 00:39:49 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:46:07 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:46:08 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:46:09 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:46:09 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:46:10 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:46:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:46:37 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:46:38 GMT
USER user
# Thu, 22 Jun 2023 01:46:38 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ffa4a466dbb8eebd7e7f25590a9df12390de9016abf82279c29c9a64aa76491a`  
		Last Modified: Thu, 15 Jun 2023 00:40:26 GMT  
		Size: 3.3 MB (3344781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f791e21598b0753fdaac6f0554ec6cece5879b619efdbbb4c1b4449a37503445`  
		Last Modified: Thu, 22 Jun 2023 01:47:27 GMT  
		Size: 9.7 MB (9727162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05af372d8f57623b63ce194292c9d6e8cadad5b62006778fb3386de60bcded93`  
		Last Modified: Thu, 22 Jun 2023 01:47:24 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d0975696ee4b7f29a8e63ef0198dd4294f329a0a3db44dbe09d39d6194767f`  
		Last Modified: Thu, 22 Jun 2023 01:47:26 GMT  
		Size: 5.6 MB (5631188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; s390x

```console
$ docker pull irssi@sha256:4f9ea0549297b400ee4e290a3e5d2548d5f935d01d81d209a4260dd9d9499e89
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18700399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31793e9f59a88f5efa8fcc186bd96e790b7d579acb15af792bf14f89c96d95f5`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 08:52:18 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 08:52:19 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 08:52:19 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 08:52:20 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 08:52:20 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 08:52:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 08:52:44 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 08:52:44 GMT
USER user
# Thu, 22 Jun 2023 08:52:44 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27869a2a741a6e4efe8b45710576e604e3fc468cef7d0feaa97e003f76aeb10`  
		Last Modified: Thu, 22 Jun 2023 08:53:34 GMT  
		Size: 10.1 MB (10078671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b47042a99d33af0f2ed5b3830ae99f7b13bb137fb93f1ace7e2d4922994df8d`  
		Last Modified: Thu, 22 Jun 2023 08:53:32 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24432dec00488946bcee10e0f328cc956d09781dd4d8165e1228aeecc1c4d390`  
		Last Modified: Thu, 22 Jun 2023 08:53:33 GMT  
		Size: 5.4 MB (5406948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:alpine3.18`

```console
$ docker pull irssi@sha256:46a65610bad93dc8966f7e0a385bad0c9047a4d05c2f6ffedb5b2d3d0226138a
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
$ docker pull irssi@sha256:a768693cbea894b7b6135922520f7d532a6245dff8a3863024244a8ef9ffb14e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18439974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6be6e0e30722062f7d0e647c925e5239badb1739c57c83238d83b8a422b169fe`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:28:06 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:28:06 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:28:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:28:07 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:28:07 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:28:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:28:26 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:28:26 GMT
USER user
# Thu, 22 Jun 2023 01:28:26 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdb311d04d5ef03d3a3d6136863478ca52e56c787391712823006f36d8d5b9e`  
		Last Modified: Thu, 22 Jun 2023 01:29:12 GMT  
		Size: 9.6 MB (9637888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c8f7b98870f87f73429e0fb3e302a979d79d0c313dc49f64bd4b6d52763c08`  
		Last Modified: Thu, 22 Jun 2023 01:29:10 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3e36b711d362f59b8801dbb9ce1a3ec3bcaa5edd5b2366634e350cf308faee`  
		Last Modified: Thu, 22 Jun 2023 01:29:11 GMT  
		Size: 5.4 MB (5402922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

### `irssi:alpine3.18` - linux; arm variant v7

```console
$ docker pull irssi@sha256:6e7b11efe55cad75bda8ed33f8f0cd39a6c1e9978fc0c6e5272a2034b7ad35b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16621926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20abb587081f9ea7c13c022008f41792c8deeaca15a52406320be5f7e2aefd62`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:15 GMT
ADD file:082f034323c559f3cb9feb6422c88b1ec8017f436d6109e238a5c5384a32a90a in / 
# Wed, 14 Jun 2023 22:36:15 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:44:06 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:44:06 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:44:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:44:07 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:44:07 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:44:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:44:21 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:44:21 GMT
USER user
# Thu, 22 Jun 2023 01:44:21 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:633ba29fd335042456b6e2c073636f6fa30de56f1331c442914739b92a479974`  
		Last Modified: Wed, 14 Jun 2023 22:36:49 GMT  
		Size: 2.9 MB (2898508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e832bd75bc8892fffbcd2098ea32615beca89d5932e7bd6eae1c7973395a4a3c`  
		Last Modified: Thu, 22 Jun 2023 01:45:04 GMT  
		Size: 8.7 MB (8713654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9047f01d89a8f17a367c34c160949fb95db656ce766205320464b4f6a764b845`  
		Last Modified: Thu, 22 Jun 2023 01:45:01 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01ed6e5b2633e51a886c41895b2477ea69e8db678ddac23148e963ee8532ac0`  
		Last Modified: Thu, 22 Jun 2023 01:45:03 GMT  
		Size: 5.0 MB (5008480 bytes)  
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

### `irssi:alpine3.18` - linux; ppc64le

```console
$ docker pull irssi@sha256:95e45ba9fe7403d47a90aa5cbebc48878a954aa9248132df17d0b1964b5735f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18704414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c077a39e383a52f1690468a909209454afb356ca12011e784cc206bb0eabb553`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:49 GMT
ADD file:694c636c0dd19fd01accbc189e4c1dc4d063952692c6e7eb26dce02a7adba833 in / 
# Thu, 15 Jun 2023 00:39:49 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:46:07 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:46:08 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:46:09 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:46:09 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:46:10 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:46:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:46:37 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:46:38 GMT
USER user
# Thu, 22 Jun 2023 01:46:38 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ffa4a466dbb8eebd7e7f25590a9df12390de9016abf82279c29c9a64aa76491a`  
		Last Modified: Thu, 15 Jun 2023 00:40:26 GMT  
		Size: 3.3 MB (3344781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f791e21598b0753fdaac6f0554ec6cece5879b619efdbbb4c1b4449a37503445`  
		Last Modified: Thu, 22 Jun 2023 01:47:27 GMT  
		Size: 9.7 MB (9727162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05af372d8f57623b63ce194292c9d6e8cadad5b62006778fb3386de60bcded93`  
		Last Modified: Thu, 22 Jun 2023 01:47:24 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d0975696ee4b7f29a8e63ef0198dd4294f329a0a3db44dbe09d39d6194767f`  
		Last Modified: Thu, 22 Jun 2023 01:47:26 GMT  
		Size: 5.6 MB (5631188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine3.18` - linux; s390x

```console
$ docker pull irssi@sha256:4f9ea0549297b400ee4e290a3e5d2548d5f935d01d81d209a4260dd9d9499e89
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18700399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31793e9f59a88f5efa8fcc186bd96e790b7d579acb15af792bf14f89c96d95f5`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 08:52:18 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 08:52:19 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 08:52:19 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 08:52:20 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 08:52:20 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 08:52:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 08:52:44 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 08:52:44 GMT
USER user
# Thu, 22 Jun 2023 08:52:44 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27869a2a741a6e4efe8b45710576e604e3fc468cef7d0feaa97e003f76aeb10`  
		Last Modified: Thu, 22 Jun 2023 08:53:34 GMT  
		Size: 10.1 MB (10078671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b47042a99d33af0f2ed5b3830ae99f7b13bb137fb93f1ace7e2d4922994df8d`  
		Last Modified: Thu, 22 Jun 2023 08:53:32 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24432dec00488946bcee10e0f328cc956d09781dd4d8165e1228aeecc1c4d390`  
		Last Modified: Thu, 22 Jun 2023 08:53:33 GMT  
		Size: 5.4 MB (5406948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:bookworm`

```console
$ docker pull irssi@sha256:69927d1ad99aec69bddc2a42727ee72f0bd0d005a9aba5c0667166b045d2dc34
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
$ docker pull irssi@sha256:58fc1c672bf293069b7789a309a03bcb34c93951017f2488c4037de7c2c68269
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (76048658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2e78b1ae299bcd0f8deef087b5454642320d910c779322916fad90990fbc810`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:42 GMT
ADD file:ba1250b6ecd5dd09d4914189d72741c2817988994e7da514bf62be439a34bdb5 in / 
# Mon, 12 Jun 2023 23:20:42 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 01:27:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 01:27:04 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:27:04 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:27:04 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:27:04 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:27:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 01:27:52 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:27:52 GMT
USER user
# Thu, 22 Jun 2023 01:27:53 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:5b5fe70539cd6989aa19f25826309f9715a9489cf1c057982d6a84c1ad8975c7`  
		Last Modified: Mon, 12 Jun 2023 23:25:49 GMT  
		Size: 29.1 MB (29124744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4909e07c2d187606b474bffed67e6b8f97ee741deba3ee1a6cc6e03a57e06d25`  
		Last Modified: Thu, 22 Jun 2023 01:28:49 GMT  
		Size: 18.2 MB (18242756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed55928edc7533b8545259265ffa0db2e9687da3460557c3885e41a0b49cbe0`  
		Last Modified: Thu, 22 Jun 2023 01:28:45 GMT  
		Size: 3.4 KB (3372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6731e4fa8db1fd048929e347b2b35f7b30b5a7d41015d14037ee7149376b11af`  
		Last Modified: Thu, 22 Jun 2023 01:28:50 GMT  
		Size: 28.7 MB (28677786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

### `irssi:bookworm` - linux; arm variant v7

```console
$ docker pull irssi@sha256:04fe9086e0677c27e634b48247d835bd76d770fb2d93a37e98e0f5d10ad930d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66699462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:347dde6d1977d7559b809d379aeb2d49c7dc1edb227ac50753bb5b436492f450`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Jul 2023 00:57:54 GMT
ADD file:d168d1710cbca4edb322c26348dafaf2b3a64980f52b8b790f334cdbd6a7047e in / 
# Tue, 04 Jul 2023 00:57:55 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:02:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:02:14 GMT
ENV HOME=/home/user
# Tue, 04 Jul 2023 05:02:15 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 04 Jul 2023 05:02:15 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 05:02:15 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 04 Jul 2023 05:02:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 04 Jul 2023 05:02:53 GMT
WORKDIR /home/user
# Tue, 04 Jul 2023 05:02:53 GMT
USER user
# Tue, 04 Jul 2023 05:02:53 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:340ace0baa422f18db718d7634c1c88a9650f4871dda2630ef15577120aa6816`  
		Last Modified: Tue, 04 Jul 2023 01:02:50 GMT  
		Size: 24.8 MB (24801264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26335a3dcbbb3fe7c73c15fa804eb199dc3d2c6f72d4b272290495ddc7d5d52`  
		Last Modified: Tue, 04 Jul 2023 05:03:15 GMT  
		Size: 16.7 MB (16675209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d7691ca1849da70e59df47ce1ae57125e975051c107f00f45a7c3cf16dba8d`  
		Last Modified: Tue, 04 Jul 2023 05:03:10 GMT  
		Size: 3.4 KB (3368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6467c4b92ddee02bde53da36ae6e65510038840b918475ce6e8b1923576edebc`  
		Last Modified: Tue, 04 Jul 2023 05:03:15 GMT  
		Size: 25.2 MB (25219621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:bookworm` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:c7c88dad0daea3ad57151de33054217941d7becf80f2dc11592f3a5dccc31cd9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74817355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63655ff173ab77b3325bf30ffb4193bc7ac59ae13e21dfb4f90bf03ae3939077`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:51:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:51:17 GMT
ENV HOME=/home/user
# Tue, 04 Jul 2023 03:51:17 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 04 Jul 2023 03:51:18 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 03:51:18 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 04 Jul 2023 03:51:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 04 Jul 2023 03:51:56 GMT
WORKDIR /home/user
# Tue, 04 Jul 2023 03:51:56 GMT
USER user
# Tue, 04 Jul 2023 03:51:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14ecf60c320eb05ae2ba16ad2774d3066ce556d0aacc4cfda7f3de6cf9aa09d`  
		Last Modified: Tue, 04 Jul 2023 03:52:21 GMT  
		Size: 18.0 MB (18023969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8369f911d29dedde0b1e053fb13ffe68ef5bc4ee1bf9929783256c66bb74805`  
		Last Modified: Tue, 04 Jul 2023 03:52:18 GMT  
		Size: 3.4 KB (3370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0551107dfe1234434d37c2834437f715c93fdc6d340114d753b92612ab6d41cd`  
		Last Modified: Tue, 04 Jul 2023 03:52:22 GMT  
		Size: 27.6 MB (27637558 bytes)  
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

### `irssi:bookworm` - linux; mips64le

```console
$ docker pull irssi@sha256:acbfc7fb13e89e47dad3c9137ef7fa896c5b75ac6533c06b67ade3057c9e2f97
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74052670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b08a4afb9566f8f4288fec8c2b1904505266fadc1a760928b037691c498c116`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:02 GMT
ADD file:f91bd2a174259cb69646fc34ba2fc6b8941ad8e171d2d7952a4d8ac3d95e2ad7 in / 
# Tue, 13 Jun 2023 00:09:06 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 02:26:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 02:26:40 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 02:26:47 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 02:26:50 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 02:26:53 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 02:30:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 02:30:54 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 02:30:57 GMT
USER user
# Thu, 22 Jun 2023 02:31:01 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:3fc28260a4d871ef9781cad2bb064ad7212a5063de3a1d35dba938ce82115e5b`  
		Last Modified: Tue, 13 Jun 2023 00:22:29 GMT  
		Size: 29.1 MB (29118129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b823be8377fd7186d28f794a5ec6493660f4e2208ded12e67636ec8750257d5`  
		Last Modified: Thu, 22 Jun 2023 02:31:36 GMT  
		Size: 16.9 MB (16925138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b18026dd902a0919c3a20766c7d6592948e9284efb4931907978339a21d327c`  
		Last Modified: Thu, 22 Jun 2023 02:31:17 GMT  
		Size: 3.3 KB (3298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a7f08c49e09c90d3e8b01aa906a42cfb03f4a598b544ec9a61c25259e54c77`  
		Last Modified: Thu, 22 Jun 2023 02:31:39 GMT  
		Size: 28.0 MB (28006105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:bookworm` - linux; ppc64le

```console
$ docker pull irssi@sha256:808102c091e0f450e9fd0ff09dd607c235a6972c0982e8a909041d95ecdc9bb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82057404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6db42123514bb5bb81836bd52afbea22d1c59d575a9cf77f3cf7c9ada892240`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:51 GMT
ADD file:51887002f5002ccc662adbc6ecf1129e3db375a7a77b93da43cc9a8326b3c4b9 in / 
# Tue, 04 Jul 2023 01:17:53 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:36:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:36:17 GMT
ENV HOME=/home/user
# Tue, 04 Jul 2023 06:36:19 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 04 Jul 2023 06:36:19 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 06:36:20 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 04 Jul 2023 06:38:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 04 Jul 2023 06:38:43 GMT
WORKDIR /home/user
# Tue, 04 Jul 2023 06:38:43 GMT
USER user
# Tue, 04 Jul 2023 06:38:44 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ba99a1aa5a92d949d988e66df7723a542fd81bc30eef9d4269e8a899820d4bb2`  
		Last Modified: Tue, 04 Jul 2023 01:24:36 GMT  
		Size: 33.1 MB (33116716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a472629dc3d35e78fd046fa9c53281082c6b5a3cbf7f446fdcd3c04302e339`  
		Last Modified: Tue, 04 Jul 2023 06:39:27 GMT  
		Size: 18.8 MB (18754069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd7eaa97c83385d341b2e6b1823b9021baeb70ce87fcc47e593bff57983efce`  
		Last Modified: Tue, 04 Jul 2023 06:39:20 GMT  
		Size: 3.4 KB (3370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bc505f4c9f16e57c14adb02d3910e21d2031362fc3775c1f499928e77048f2`  
		Last Modified: Tue, 04 Jul 2023 06:39:29 GMT  
		Size: 30.2 MB (30183249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:bookworm` - linux; s390x

```console
$ docker pull irssi@sha256:baa1df37d716889924e03405a3a5a2258c9e4520c6ad647a93d27caa6aba256f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72925568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:251b812805e137b9e051579adf3a25dd277d29aeacde9c29977afa4e7e513e0a`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Jun 2023 04:29:41 GMT
ADD file:739f4c23557ec0af5f4ba492c847b5d2f09dd81211c675d0e9eabe865d794e81 in / 
# Tue, 13 Jun 2023 04:29:43 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 08:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 08:51:21 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 08:51:21 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 08:51:21 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 08:51:22 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 08:51:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 08:52:00 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 08:52:00 GMT
USER user
# Thu, 22 Jun 2023 08:52:00 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6571b3abd058e377c7bd231c9029aff6eb25486bffb50229076d2e6a356a517f`  
		Last Modified: Tue, 13 Jun 2023 04:34:21 GMT  
		Size: 27.5 MB (27487928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0716cb6af8f5fcdc92d2d74f09de86858ee69ef8a2db7db71d6d60048930182`  
		Last Modified: Thu, 22 Jun 2023 08:53:07 GMT  
		Size: 18.2 MB (18206342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72ba9f202ec95947aa092a1c8f9fbac3cb975b47cf804734a0804722f737334`  
		Last Modified: Thu, 22 Jun 2023 08:53:04 GMT  
		Size: 3.4 KB (3368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e63e7ec95d8ded21367b4197e518b0bbc792b85525d9ca92b313e772bd4ec5`  
		Last Modified: Thu, 22 Jun 2023 08:53:08 GMT  
		Size: 27.2 MB (27227930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:latest`

```console
$ docker pull irssi@sha256:69927d1ad99aec69bddc2a42727ee72f0bd0d005a9aba5c0667166b045d2dc34
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
$ docker pull irssi@sha256:58fc1c672bf293069b7789a309a03bcb34c93951017f2488c4037de7c2c68269
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.0 MB (76048658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2e78b1ae299bcd0f8deef087b5454642320d910c779322916fad90990fbc810`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:42 GMT
ADD file:ba1250b6ecd5dd09d4914189d72741c2817988994e7da514bf62be439a34bdb5 in / 
# Mon, 12 Jun 2023 23:20:42 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 01:27:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 01:27:04 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:27:04 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:27:04 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:27:04 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:27:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 01:27:52 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:27:52 GMT
USER user
# Thu, 22 Jun 2023 01:27:53 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:5b5fe70539cd6989aa19f25826309f9715a9489cf1c057982d6a84c1ad8975c7`  
		Last Modified: Mon, 12 Jun 2023 23:25:49 GMT  
		Size: 29.1 MB (29124744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4909e07c2d187606b474bffed67e6b8f97ee741deba3ee1a6cc6e03a57e06d25`  
		Last Modified: Thu, 22 Jun 2023 01:28:49 GMT  
		Size: 18.2 MB (18242756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed55928edc7533b8545259265ffa0db2e9687da3460557c3885e41a0b49cbe0`  
		Last Modified: Thu, 22 Jun 2023 01:28:45 GMT  
		Size: 3.4 KB (3372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6731e4fa8db1fd048929e347b2b35f7b30b5a7d41015d14037ee7149376b11af`  
		Last Modified: Thu, 22 Jun 2023 01:28:50 GMT  
		Size: 28.7 MB (28677786 bytes)  
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
$ docker pull irssi@sha256:04fe9086e0677c27e634b48247d835bd76d770fb2d93a37e98e0f5d10ad930d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66699462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:347dde6d1977d7559b809d379aeb2d49c7dc1edb227ac50753bb5b436492f450`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Jul 2023 00:57:54 GMT
ADD file:d168d1710cbca4edb322c26348dafaf2b3a64980f52b8b790f334cdbd6a7047e in / 
# Tue, 04 Jul 2023 00:57:55 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:02:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:02:14 GMT
ENV HOME=/home/user
# Tue, 04 Jul 2023 05:02:15 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 04 Jul 2023 05:02:15 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 05:02:15 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 04 Jul 2023 05:02:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 04 Jul 2023 05:02:53 GMT
WORKDIR /home/user
# Tue, 04 Jul 2023 05:02:53 GMT
USER user
# Tue, 04 Jul 2023 05:02:53 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:340ace0baa422f18db718d7634c1c88a9650f4871dda2630ef15577120aa6816`  
		Last Modified: Tue, 04 Jul 2023 01:02:50 GMT  
		Size: 24.8 MB (24801264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26335a3dcbbb3fe7c73c15fa804eb199dc3d2c6f72d4b272290495ddc7d5d52`  
		Last Modified: Tue, 04 Jul 2023 05:03:15 GMT  
		Size: 16.7 MB (16675209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d7691ca1849da70e59df47ce1ae57125e975051c107f00f45a7c3cf16dba8d`  
		Last Modified: Tue, 04 Jul 2023 05:03:10 GMT  
		Size: 3.4 KB (3368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6467c4b92ddee02bde53da36ae6e65510038840b918475ce6e8b1923576edebc`  
		Last Modified: Tue, 04 Jul 2023 05:03:15 GMT  
		Size: 25.2 MB (25219621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:c7c88dad0daea3ad57151de33054217941d7becf80f2dc11592f3a5dccc31cd9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74817355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63655ff173ab77b3325bf30ffb4193bc7ac59ae13e21dfb4f90bf03ae3939077`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:51:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:51:17 GMT
ENV HOME=/home/user
# Tue, 04 Jul 2023 03:51:17 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 04 Jul 2023 03:51:18 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 03:51:18 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 04 Jul 2023 03:51:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 04 Jul 2023 03:51:56 GMT
WORKDIR /home/user
# Tue, 04 Jul 2023 03:51:56 GMT
USER user
# Tue, 04 Jul 2023 03:51:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14ecf60c320eb05ae2ba16ad2774d3066ce556d0aacc4cfda7f3de6cf9aa09d`  
		Last Modified: Tue, 04 Jul 2023 03:52:21 GMT  
		Size: 18.0 MB (18023969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8369f911d29dedde0b1e053fb13ffe68ef5bc4ee1bf9929783256c66bb74805`  
		Last Modified: Tue, 04 Jul 2023 03:52:18 GMT  
		Size: 3.4 KB (3370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0551107dfe1234434d37c2834437f715c93fdc6d340114d753b92612ab6d41cd`  
		Last Modified: Tue, 04 Jul 2023 03:52:22 GMT  
		Size: 27.6 MB (27637558 bytes)  
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
$ docker pull irssi@sha256:acbfc7fb13e89e47dad3c9137ef7fa896c5b75ac6533c06b67ade3057c9e2f97
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74052670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b08a4afb9566f8f4288fec8c2b1904505266fadc1a760928b037691c498c116`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:02 GMT
ADD file:f91bd2a174259cb69646fc34ba2fc6b8941ad8e171d2d7952a4d8ac3d95e2ad7 in / 
# Tue, 13 Jun 2023 00:09:06 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 02:26:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 02:26:40 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 02:26:47 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 02:26:50 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 02:26:53 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 02:30:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 02:30:54 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 02:30:57 GMT
USER user
# Thu, 22 Jun 2023 02:31:01 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:3fc28260a4d871ef9781cad2bb064ad7212a5063de3a1d35dba938ce82115e5b`  
		Last Modified: Tue, 13 Jun 2023 00:22:29 GMT  
		Size: 29.1 MB (29118129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b823be8377fd7186d28f794a5ec6493660f4e2208ded12e67636ec8750257d5`  
		Last Modified: Thu, 22 Jun 2023 02:31:36 GMT  
		Size: 16.9 MB (16925138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b18026dd902a0919c3a20766c7d6592948e9284efb4931907978339a21d327c`  
		Last Modified: Thu, 22 Jun 2023 02:31:17 GMT  
		Size: 3.3 KB (3298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a7f08c49e09c90d3e8b01aa906a42cfb03f4a598b544ec9a61c25259e54c77`  
		Last Modified: Thu, 22 Jun 2023 02:31:39 GMT  
		Size: 28.0 MB (28006105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; ppc64le

```console
$ docker pull irssi@sha256:808102c091e0f450e9fd0ff09dd607c235a6972c0982e8a909041d95ecdc9bb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82057404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6db42123514bb5bb81836bd52afbea22d1c59d575a9cf77f3cf7c9ada892240`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:51 GMT
ADD file:51887002f5002ccc662adbc6ecf1129e3db375a7a77b93da43cc9a8326b3c4b9 in / 
# Tue, 04 Jul 2023 01:17:53 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:36:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:36:17 GMT
ENV HOME=/home/user
# Tue, 04 Jul 2023 06:36:19 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 04 Jul 2023 06:36:19 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 06:36:20 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 04 Jul 2023 06:38:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 04 Jul 2023 06:38:43 GMT
WORKDIR /home/user
# Tue, 04 Jul 2023 06:38:43 GMT
USER user
# Tue, 04 Jul 2023 06:38:44 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ba99a1aa5a92d949d988e66df7723a542fd81bc30eef9d4269e8a899820d4bb2`  
		Last Modified: Tue, 04 Jul 2023 01:24:36 GMT  
		Size: 33.1 MB (33116716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a472629dc3d35e78fd046fa9c53281082c6b5a3cbf7f446fdcd3c04302e339`  
		Last Modified: Tue, 04 Jul 2023 06:39:27 GMT  
		Size: 18.8 MB (18754069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd7eaa97c83385d341b2e6b1823b9021baeb70ce87fcc47e593bff57983efce`  
		Last Modified: Tue, 04 Jul 2023 06:39:20 GMT  
		Size: 3.4 KB (3370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bc505f4c9f16e57c14adb02d3910e21d2031362fc3775c1f499928e77048f2`  
		Last Modified: Tue, 04 Jul 2023 06:39:29 GMT  
		Size: 30.2 MB (30183249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; s390x

```console
$ docker pull irssi@sha256:baa1df37d716889924e03405a3a5a2258c9e4520c6ad647a93d27caa6aba256f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72925568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:251b812805e137b9e051579adf3a25dd277d29aeacde9c29977afa4e7e513e0a`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Jun 2023 04:29:41 GMT
ADD file:739f4c23557ec0af5f4ba492c847b5d2f09dd81211c675d0e9eabe865d794e81 in / 
# Tue, 13 Jun 2023 04:29:43 GMT
CMD ["bash"]
# Thu, 22 Jun 2023 08:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jun 2023 08:51:21 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 08:51:21 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 08:51:21 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 08:51:22 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 08:51:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 22 Jun 2023 08:52:00 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 08:52:00 GMT
USER user
# Thu, 22 Jun 2023 08:52:00 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6571b3abd058e377c7bd231c9029aff6eb25486bffb50229076d2e6a356a517f`  
		Last Modified: Tue, 13 Jun 2023 04:34:21 GMT  
		Size: 27.5 MB (27487928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0716cb6af8f5fcdc92d2d74f09de86858ee69ef8a2db7db71d6d60048930182`  
		Last Modified: Thu, 22 Jun 2023 08:53:07 GMT  
		Size: 18.2 MB (18206342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72ba9f202ec95947aa092a1c8f9fbac3cb975b47cf804734a0804722f737334`  
		Last Modified: Thu, 22 Jun 2023 08:53:04 GMT  
		Size: 3.4 KB (3368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e63e7ec95d8ded21367b4197e518b0bbc792b85525d9ca92b313e772bd4ec5`  
		Last Modified: Thu, 22 Jun 2023 08:53:08 GMT  
		Size: 27.2 MB (27227930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
