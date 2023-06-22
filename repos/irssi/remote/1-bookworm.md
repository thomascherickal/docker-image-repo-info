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
