<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `irssi`

-	[`irssi:1`](#irssi1)
-	[`irssi:1.2`](#irssi12)
-	[`irssi:1.2.2`](#irssi122)
-	[`irssi:1.2.2-alpine`](#irssi122-alpine)
-	[`irssi:1.2-alpine`](#irssi12-alpine)
-	[`irssi:1-alpine`](#irssi1-alpine)
-	[`irssi:alpine`](#irssialpine)
-	[`irssi:latest`](#irssilatest)

## `irssi:1`

```console
$ docker pull irssi@sha256:522eb796ea2bd9501803f99d612ca113a6a28deaefb89506517574dd268c2aed
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

### `irssi:1` - linux; amd64

```console
$ docker pull irssi@sha256:af02b4b7fd40efc410580773ef0c4ff3a14877b2ea4598edb12d4485310c9d96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50541239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87fea6963c9b2b4d42b3e2d8cf658c714fe03da2a2b0804ddf3c61463626c3a4`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:38:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:38:44 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 09:38:46 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 09:38:46 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 09:38:46 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 09:39:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 09:39:55 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 09:39:55 GMT
USER user
# Tue, 12 Jan 2021 09:39:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db80d14f483469e745ac0212bdf1e73f6158b62e49fff6c240aaee12bcdb7e5`  
		Last Modified: Tue, 12 Jan 2021 09:40:28 GMT  
		Size: 17.0 MB (16999919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2969bb11828af3b3ece9cee2d04141672d87b04890d6dee06b3619d9040a88`  
		Last Modified: Tue, 12 Jan 2021 09:40:24 GMT  
		Size: 4.2 KB (4180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511f4c020a955d0bea6de98441803a9eac6cc037996ffe42c834faa70865002f`  
		Last Modified: Tue, 12 Jan 2021 09:40:24 GMT  
		Size: 6.4 MB (6429071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm variant v5

```console
$ docker pull irssi@sha256:8cab443d7c6e0757d9ce2e72494462ddc8a086259ae61939a21de094e1a5fa51
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46825932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b5a984afad6b9f1273f5d3a3fdf77eef2de72dd911d5ad6668efb725b341631`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:34 GMT
ADD file:57136a762436a5d41e60c61db0d89baea17a289845ea55565e45cc79a9e81e23 in / 
# Tue, 12 Jan 2021 00:51:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:22:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:22:31 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 02:22:34 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 02:22:35 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 02:22:36 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 02:24:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 02:24:15 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 02:24:16 GMT
USER user
# Tue, 12 Jan 2021 02:24:17 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2e2535e18472e7491a1d935b1f44ac842e4cc5c4d3de40cecb77b56b44515910`  
		Last Modified: Tue, 12 Jan 2021 01:00:19 GMT  
		Size: 24.9 MB (24851909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8e230c8f512600659fd9bc5c4209a057c8be3d630b5888c34eea16d7610d2b`  
		Last Modified: Tue, 12 Jan 2021 02:24:44 GMT  
		Size: 15.9 MB (15907342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc34cc4cc032ca0d1cd996d051d2ac727da40f24f63f04a8c581962c7be9714c`  
		Last Modified: Tue, 12 Jan 2021 02:24:36 GMT  
		Size: 4.2 KB (4196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ec18b89f11758e0608a36f62371cf2ae5c4e59a9b0dddd2be9e65a6a497ae6`  
		Last Modified: Tue, 12 Jan 2021 02:24:38 GMT  
		Size: 6.1 MB (6062485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm variant v7

```console
$ docker pull irssi@sha256:a2f1914a650a4be6d11af87e5ed84c1d4204c483f1207f1b22104ca9349f6853
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44217380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deac85e27be886cc14446c41ebef26c4591b3fcc10e4510a417fbd5f8bc29f59`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:01:09 GMT
ADD file:1db27e410cc7caf4a97a7313c57260fd01aa134b84306914ef0948dcca27372d in / 
# Tue, 12 Jan 2021 00:01:12 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:48:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:48:04 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 03:48:06 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 03:48:06 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 03:48:07 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 03:49:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 03:49:33 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 03:49:34 GMT
USER user
# Tue, 12 Jan 2021 03:49:35 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:be493c6a598447fe5f46a390f3bee10f2d2ba2215d39829fe84eb40a7add18fc`  
		Last Modified: Tue, 12 Jan 2021 00:11:14 GMT  
		Size: 22.7 MB (22715905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce11a682b5a576d870bc1134f3a1482a65e9a1a819efd9c2ba568ebb74bcb3d`  
		Last Modified: Tue, 12 Jan 2021 03:50:14 GMT  
		Size: 15.6 MB (15566916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9dc5728e6ac838fbdf40b834aa7a033f738e7fcc3d4aef6a9a7fbac68e847a`  
		Last Modified: Tue, 12 Jan 2021 03:50:06 GMT  
		Size: 4.2 KB (4191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3566dad55b7fe7f28faa8cc4d3c3976a2592b6ca38e01d8b737f182493c0d5`  
		Last Modified: Tue, 12 Jan 2021 03:50:08 GMT  
		Size: 5.9 MB (5930368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:3abc760da20db96c1e183fe88265b47682cd5abbfc323a6dd55a023de85afd57
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49034646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9178faeae913664578ce317ea4499f0033456a24a0ddfc2efd43cdd2127f1840`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 04:53:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 04:53:02 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 04:53:05 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 04:53:06 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 04:53:06 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 04:56:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 04:56:39 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 04:56:40 GMT
USER user
# Tue, 12 Jan 2021 04:56:40 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e408b8961089722d96b5bd880822657cac883e9b44768370093db02d6200dfe3`  
		Last Modified: Tue, 12 Jan 2021 04:57:15 GMT  
		Size: 16.8 MB (16778122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afdadf12a13a42383ba5740842cd7b61dbba6da3fa80bec8d250855733181f48`  
		Last Modified: Tue, 12 Jan 2021 04:57:09 GMT  
		Size: 4.2 KB (4212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a44d48fea5067528d59d38b1cd576db46e2cd4281da1fa1a4c0fc94d27f181e7`  
		Last Modified: Tue, 12 Jan 2021 04:57:10 GMT  
		Size: 6.4 MB (6387820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; 386

```console
$ docker pull irssi@sha256:bec995a740efa7f49fdd192fd4ca0d3d3b3a38f046aaa370e5310282c9c4970c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50398828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60ba27bbd1583680fd2f22bffab1a7e0888e91c87bfee095e0e32e0b924ab347`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:42:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:42:03 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 03:42:04 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 03:42:04 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 03:42:05 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 03:43:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 03:43:11 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 03:43:12 GMT
USER user
# Tue, 12 Jan 2021 03:43:12 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b2bfe52460501b552bf3e631c00eeeb8631995af9376813640417a3c000f94`  
		Last Modified: Tue, 12 Jan 2021 03:43:49 GMT  
		Size: 16.5 MB (16525249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cd9259438a5b49a8c24083be2c9392e846bd3967fa7053c1f61cf8df091fc6`  
		Last Modified: Tue, 12 Jan 2021 03:43:35 GMT  
		Size: 4.2 KB (4167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520edb3023f4d0e01d7b8688a80d79a8ad58b9863037245eb8c5039d54c87965`  
		Last Modified: Tue, 12 Jan 2021 03:43:35 GMT  
		Size: 6.1 MB (6101421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; mips64le

```console
$ docker pull irssi@sha256:411d5291afdf74c5ade425b1117d505dbad5aae79b36c1bef0b2d4db2f02b8c4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47760566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d840df00faf9203081c843e4d607519333ad6c0167fd5190bebe8ea2247c49a`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 01:16:21 GMT
ADD file:e75a4429a4b3b0f7a646f85af88d412a98006cdf44ea6744b90fea7419840831 in / 
# Tue, 12 Jan 2021 01:16:22 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 05:52:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 05:52:21 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 05:52:22 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 05:52:23 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 05:52:23 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 05:54:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 05:54:55 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 05:54:55 GMT
USER user
# Tue, 12 Jan 2021 05:54:55 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c8d46df0b1a64c5ee6879aa09ea5818b36bcae5d39b941d7262bcff617be9873`  
		Last Modified: Tue, 12 Jan 2021 01:23:17 GMT  
		Size: 25.8 MB (25778695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5793705193bafef88f2e73d14ffad74a82df82eb504610af9e4317e2503abab`  
		Last Modified: Tue, 12 Jan 2021 05:55:38 GMT  
		Size: 15.7 MB (15687581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a046b9b47a317fbef9325c9df6ce038cf8e3b45de45ac125ef10922b340f951`  
		Last Modified: Tue, 12 Jan 2021 05:55:22 GMT  
		Size: 4.2 KB (4180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29b4995081445e06aaea12c5a1676c5fbfec79be31fd4ef6995273093a726f4`  
		Last Modified: Tue, 12 Jan 2021 05:55:27 GMT  
		Size: 6.3 MB (6290110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; ppc64le

```console
$ docker pull irssi@sha256:6842568cae6c8c6d79b417ba7b42fc08c09e9b8a5f44451f02e162cbb031af3e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.7 MB (54721702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32f18ae696de1cd0c23aadcb2ef012b92e8a46605f9d81908264954f5c2abcc6`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:44:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:44:42 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 02:44:55 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 02:45:06 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 02:45:15 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 02:53:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 02:53:59 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 02:54:02 GMT
USER user
# Tue, 12 Jan 2021 02:54:04 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d49326825512307a99b49b2bc483f9841c4196b0f020811e9ad66498bbe53f9`  
		Last Modified: Tue, 12 Jan 2021 02:54:45 GMT  
		Size: 17.4 MB (17403860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cddccfe8b27784a6c3bcc136f813e67d85217d590538a6b0f24b392a147c7c95`  
		Last Modified: Tue, 12 Jan 2021 02:54:38 GMT  
		Size: 4.2 KB (4224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fb7721e869a0a3572123da5a5a9d5b7795cf9332fa06b604b378c8faeb362a`  
		Last Modified: Tue, 12 Jan 2021 02:54:38 GMT  
		Size: 6.8 MB (6780781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; s390x

```console
$ docker pull irssi@sha256:ee350953d01f28ad635e1194152c20c0473f6e7bec4e6f4845c77cdd382238d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48997191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0365621040654b09bb5f1eea8657cdcca5cc5bcff9eecc979b39778390d29ee3`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:42:22 GMT
ADD file:c01d899d503187f788db0a7d658bf3f2b6541026a4c654707d3272f6d3ffaf58 in / 
# Tue, 12 Jan 2021 00:42:24 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:03:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:03:40 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 03:03:42 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 03:03:43 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 03:03:43 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 03:04:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 03:04:59 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 03:04:59 GMT
USER user
# Tue, 12 Jan 2021 03:04:59 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a0e3e06c0bd0347fefe8bde60780e7e551c0cdf1cbcf40be3d052e823d5ec118`  
		Last Modified: Tue, 12 Jan 2021 00:52:32 GMT  
		Size: 25.7 MB (25723406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b9fea8e4ca0ebc541e54ebc984bc5b2264637e7f0e8154e889fbf10a8774fe`  
		Last Modified: Tue, 12 Jan 2021 03:06:05 GMT  
		Size: 16.9 MB (16886327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d589abf4465e5265aca738df455a2f19f87b34932c190bbab36796c9633fe04`  
		Last Modified: Tue, 12 Jan 2021 03:06:05 GMT  
		Size: 4.2 KB (4219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:972f06fed78cf1528b81dc5167b378256a0153188898adfc443a2390f52c89ab`  
		Last Modified: Tue, 12 Jan 2021 03:06:06 GMT  
		Size: 6.4 MB (6383239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2`

```console
$ docker pull irssi@sha256:522eb796ea2bd9501803f99d612ca113a6a28deaefb89506517574dd268c2aed
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

### `irssi:1.2` - linux; amd64

```console
$ docker pull irssi@sha256:af02b4b7fd40efc410580773ef0c4ff3a14877b2ea4598edb12d4485310c9d96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50541239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87fea6963c9b2b4d42b3e2d8cf658c714fe03da2a2b0804ddf3c61463626c3a4`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:38:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:38:44 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 09:38:46 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 09:38:46 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 09:38:46 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 09:39:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 09:39:55 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 09:39:55 GMT
USER user
# Tue, 12 Jan 2021 09:39:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db80d14f483469e745ac0212bdf1e73f6158b62e49fff6c240aaee12bcdb7e5`  
		Last Modified: Tue, 12 Jan 2021 09:40:28 GMT  
		Size: 17.0 MB (16999919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2969bb11828af3b3ece9cee2d04141672d87b04890d6dee06b3619d9040a88`  
		Last Modified: Tue, 12 Jan 2021 09:40:24 GMT  
		Size: 4.2 KB (4180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511f4c020a955d0bea6de98441803a9eac6cc037996ffe42c834faa70865002f`  
		Last Modified: Tue, 12 Jan 2021 09:40:24 GMT  
		Size: 6.4 MB (6429071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; arm variant v5

```console
$ docker pull irssi@sha256:8cab443d7c6e0757d9ce2e72494462ddc8a086259ae61939a21de094e1a5fa51
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46825932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b5a984afad6b9f1273f5d3a3fdf77eef2de72dd911d5ad6668efb725b341631`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:34 GMT
ADD file:57136a762436a5d41e60c61db0d89baea17a289845ea55565e45cc79a9e81e23 in / 
# Tue, 12 Jan 2021 00:51:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:22:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:22:31 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 02:22:34 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 02:22:35 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 02:22:36 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 02:24:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 02:24:15 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 02:24:16 GMT
USER user
# Tue, 12 Jan 2021 02:24:17 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2e2535e18472e7491a1d935b1f44ac842e4cc5c4d3de40cecb77b56b44515910`  
		Last Modified: Tue, 12 Jan 2021 01:00:19 GMT  
		Size: 24.9 MB (24851909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8e230c8f512600659fd9bc5c4209a057c8be3d630b5888c34eea16d7610d2b`  
		Last Modified: Tue, 12 Jan 2021 02:24:44 GMT  
		Size: 15.9 MB (15907342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc34cc4cc032ca0d1cd996d051d2ac727da40f24f63f04a8c581962c7be9714c`  
		Last Modified: Tue, 12 Jan 2021 02:24:36 GMT  
		Size: 4.2 KB (4196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ec18b89f11758e0608a36f62371cf2ae5c4e59a9b0dddd2be9e65a6a497ae6`  
		Last Modified: Tue, 12 Jan 2021 02:24:38 GMT  
		Size: 6.1 MB (6062485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; arm variant v7

```console
$ docker pull irssi@sha256:a2f1914a650a4be6d11af87e5ed84c1d4204c483f1207f1b22104ca9349f6853
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44217380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deac85e27be886cc14446c41ebef26c4591b3fcc10e4510a417fbd5f8bc29f59`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:01:09 GMT
ADD file:1db27e410cc7caf4a97a7313c57260fd01aa134b84306914ef0948dcca27372d in / 
# Tue, 12 Jan 2021 00:01:12 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:48:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:48:04 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 03:48:06 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 03:48:06 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 03:48:07 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 03:49:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 03:49:33 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 03:49:34 GMT
USER user
# Tue, 12 Jan 2021 03:49:35 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:be493c6a598447fe5f46a390f3bee10f2d2ba2215d39829fe84eb40a7add18fc`  
		Last Modified: Tue, 12 Jan 2021 00:11:14 GMT  
		Size: 22.7 MB (22715905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce11a682b5a576d870bc1134f3a1482a65e9a1a819efd9c2ba568ebb74bcb3d`  
		Last Modified: Tue, 12 Jan 2021 03:50:14 GMT  
		Size: 15.6 MB (15566916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9dc5728e6ac838fbdf40b834aa7a033f738e7fcc3d4aef6a9a7fbac68e847a`  
		Last Modified: Tue, 12 Jan 2021 03:50:06 GMT  
		Size: 4.2 KB (4191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3566dad55b7fe7f28faa8cc4d3c3976a2592b6ca38e01d8b737f182493c0d5`  
		Last Modified: Tue, 12 Jan 2021 03:50:08 GMT  
		Size: 5.9 MB (5930368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:3abc760da20db96c1e183fe88265b47682cd5abbfc323a6dd55a023de85afd57
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49034646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9178faeae913664578ce317ea4499f0033456a24a0ddfc2efd43cdd2127f1840`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 04:53:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 04:53:02 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 04:53:05 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 04:53:06 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 04:53:06 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 04:56:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 04:56:39 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 04:56:40 GMT
USER user
# Tue, 12 Jan 2021 04:56:40 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e408b8961089722d96b5bd880822657cac883e9b44768370093db02d6200dfe3`  
		Last Modified: Tue, 12 Jan 2021 04:57:15 GMT  
		Size: 16.8 MB (16778122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afdadf12a13a42383ba5740842cd7b61dbba6da3fa80bec8d250855733181f48`  
		Last Modified: Tue, 12 Jan 2021 04:57:09 GMT  
		Size: 4.2 KB (4212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a44d48fea5067528d59d38b1cd576db46e2cd4281da1fa1a4c0fc94d27f181e7`  
		Last Modified: Tue, 12 Jan 2021 04:57:10 GMT  
		Size: 6.4 MB (6387820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; 386

```console
$ docker pull irssi@sha256:bec995a740efa7f49fdd192fd4ca0d3d3b3a38f046aaa370e5310282c9c4970c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50398828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60ba27bbd1583680fd2f22bffab1a7e0888e91c87bfee095e0e32e0b924ab347`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:42:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:42:03 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 03:42:04 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 03:42:04 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 03:42:05 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 03:43:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 03:43:11 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 03:43:12 GMT
USER user
# Tue, 12 Jan 2021 03:43:12 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b2bfe52460501b552bf3e631c00eeeb8631995af9376813640417a3c000f94`  
		Last Modified: Tue, 12 Jan 2021 03:43:49 GMT  
		Size: 16.5 MB (16525249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cd9259438a5b49a8c24083be2c9392e846bd3967fa7053c1f61cf8df091fc6`  
		Last Modified: Tue, 12 Jan 2021 03:43:35 GMT  
		Size: 4.2 KB (4167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520edb3023f4d0e01d7b8688a80d79a8ad58b9863037245eb8c5039d54c87965`  
		Last Modified: Tue, 12 Jan 2021 03:43:35 GMT  
		Size: 6.1 MB (6101421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; mips64le

```console
$ docker pull irssi@sha256:411d5291afdf74c5ade425b1117d505dbad5aae79b36c1bef0b2d4db2f02b8c4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47760566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d840df00faf9203081c843e4d607519333ad6c0167fd5190bebe8ea2247c49a`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 01:16:21 GMT
ADD file:e75a4429a4b3b0f7a646f85af88d412a98006cdf44ea6744b90fea7419840831 in / 
# Tue, 12 Jan 2021 01:16:22 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 05:52:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 05:52:21 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 05:52:22 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 05:52:23 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 05:52:23 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 05:54:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 05:54:55 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 05:54:55 GMT
USER user
# Tue, 12 Jan 2021 05:54:55 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c8d46df0b1a64c5ee6879aa09ea5818b36bcae5d39b941d7262bcff617be9873`  
		Last Modified: Tue, 12 Jan 2021 01:23:17 GMT  
		Size: 25.8 MB (25778695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5793705193bafef88f2e73d14ffad74a82df82eb504610af9e4317e2503abab`  
		Last Modified: Tue, 12 Jan 2021 05:55:38 GMT  
		Size: 15.7 MB (15687581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a046b9b47a317fbef9325c9df6ce038cf8e3b45de45ac125ef10922b340f951`  
		Last Modified: Tue, 12 Jan 2021 05:55:22 GMT  
		Size: 4.2 KB (4180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29b4995081445e06aaea12c5a1676c5fbfec79be31fd4ef6995273093a726f4`  
		Last Modified: Tue, 12 Jan 2021 05:55:27 GMT  
		Size: 6.3 MB (6290110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; ppc64le

```console
$ docker pull irssi@sha256:6842568cae6c8c6d79b417ba7b42fc08c09e9b8a5f44451f02e162cbb031af3e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.7 MB (54721702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32f18ae696de1cd0c23aadcb2ef012b92e8a46605f9d81908264954f5c2abcc6`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:44:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:44:42 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 02:44:55 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 02:45:06 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 02:45:15 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 02:53:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 02:53:59 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 02:54:02 GMT
USER user
# Tue, 12 Jan 2021 02:54:04 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d49326825512307a99b49b2bc483f9841c4196b0f020811e9ad66498bbe53f9`  
		Last Modified: Tue, 12 Jan 2021 02:54:45 GMT  
		Size: 17.4 MB (17403860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cddccfe8b27784a6c3bcc136f813e67d85217d590538a6b0f24b392a147c7c95`  
		Last Modified: Tue, 12 Jan 2021 02:54:38 GMT  
		Size: 4.2 KB (4224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fb7721e869a0a3572123da5a5a9d5b7795cf9332fa06b604b378c8faeb362a`  
		Last Modified: Tue, 12 Jan 2021 02:54:38 GMT  
		Size: 6.8 MB (6780781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; s390x

```console
$ docker pull irssi@sha256:ee350953d01f28ad635e1194152c20c0473f6e7bec4e6f4845c77cdd382238d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48997191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0365621040654b09bb5f1eea8657cdcca5cc5bcff9eecc979b39778390d29ee3`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:42:22 GMT
ADD file:c01d899d503187f788db0a7d658bf3f2b6541026a4c654707d3272f6d3ffaf58 in / 
# Tue, 12 Jan 2021 00:42:24 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:03:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:03:40 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 03:03:42 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 03:03:43 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 03:03:43 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 03:04:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 03:04:59 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 03:04:59 GMT
USER user
# Tue, 12 Jan 2021 03:04:59 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a0e3e06c0bd0347fefe8bde60780e7e551c0cdf1cbcf40be3d052e823d5ec118`  
		Last Modified: Tue, 12 Jan 2021 00:52:32 GMT  
		Size: 25.7 MB (25723406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b9fea8e4ca0ebc541e54ebc984bc5b2264637e7f0e8154e889fbf10a8774fe`  
		Last Modified: Tue, 12 Jan 2021 03:06:05 GMT  
		Size: 16.9 MB (16886327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d589abf4465e5265aca738df455a2f19f87b34932c190bbab36796c9633fe04`  
		Last Modified: Tue, 12 Jan 2021 03:06:05 GMT  
		Size: 4.2 KB (4219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:972f06fed78cf1528b81dc5167b378256a0153188898adfc443a2390f52c89ab`  
		Last Modified: Tue, 12 Jan 2021 03:06:06 GMT  
		Size: 6.4 MB (6383239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2.2`

```console
$ docker pull irssi@sha256:522eb796ea2bd9501803f99d612ca113a6a28deaefb89506517574dd268c2aed
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

### `irssi:1.2.2` - linux; amd64

```console
$ docker pull irssi@sha256:af02b4b7fd40efc410580773ef0c4ff3a14877b2ea4598edb12d4485310c9d96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50541239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87fea6963c9b2b4d42b3e2d8cf658c714fe03da2a2b0804ddf3c61463626c3a4`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:38:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:38:44 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 09:38:46 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 09:38:46 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 09:38:46 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 09:39:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 09:39:55 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 09:39:55 GMT
USER user
# Tue, 12 Jan 2021 09:39:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db80d14f483469e745ac0212bdf1e73f6158b62e49fff6c240aaee12bcdb7e5`  
		Last Modified: Tue, 12 Jan 2021 09:40:28 GMT  
		Size: 17.0 MB (16999919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2969bb11828af3b3ece9cee2d04141672d87b04890d6dee06b3619d9040a88`  
		Last Modified: Tue, 12 Jan 2021 09:40:24 GMT  
		Size: 4.2 KB (4180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511f4c020a955d0bea6de98441803a9eac6cc037996ffe42c834faa70865002f`  
		Last Modified: Tue, 12 Jan 2021 09:40:24 GMT  
		Size: 6.4 MB (6429071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2` - linux; arm variant v5

```console
$ docker pull irssi@sha256:8cab443d7c6e0757d9ce2e72494462ddc8a086259ae61939a21de094e1a5fa51
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46825932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b5a984afad6b9f1273f5d3a3fdf77eef2de72dd911d5ad6668efb725b341631`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:34 GMT
ADD file:57136a762436a5d41e60c61db0d89baea17a289845ea55565e45cc79a9e81e23 in / 
# Tue, 12 Jan 2021 00:51:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:22:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:22:31 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 02:22:34 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 02:22:35 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 02:22:36 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 02:24:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 02:24:15 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 02:24:16 GMT
USER user
# Tue, 12 Jan 2021 02:24:17 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2e2535e18472e7491a1d935b1f44ac842e4cc5c4d3de40cecb77b56b44515910`  
		Last Modified: Tue, 12 Jan 2021 01:00:19 GMT  
		Size: 24.9 MB (24851909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8e230c8f512600659fd9bc5c4209a057c8be3d630b5888c34eea16d7610d2b`  
		Last Modified: Tue, 12 Jan 2021 02:24:44 GMT  
		Size: 15.9 MB (15907342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc34cc4cc032ca0d1cd996d051d2ac727da40f24f63f04a8c581962c7be9714c`  
		Last Modified: Tue, 12 Jan 2021 02:24:36 GMT  
		Size: 4.2 KB (4196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ec18b89f11758e0608a36f62371cf2ae5c4e59a9b0dddd2be9e65a6a497ae6`  
		Last Modified: Tue, 12 Jan 2021 02:24:38 GMT  
		Size: 6.1 MB (6062485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2` - linux; arm variant v7

```console
$ docker pull irssi@sha256:a2f1914a650a4be6d11af87e5ed84c1d4204c483f1207f1b22104ca9349f6853
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44217380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deac85e27be886cc14446c41ebef26c4591b3fcc10e4510a417fbd5f8bc29f59`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:01:09 GMT
ADD file:1db27e410cc7caf4a97a7313c57260fd01aa134b84306914ef0948dcca27372d in / 
# Tue, 12 Jan 2021 00:01:12 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:48:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:48:04 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 03:48:06 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 03:48:06 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 03:48:07 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 03:49:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 03:49:33 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 03:49:34 GMT
USER user
# Tue, 12 Jan 2021 03:49:35 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:be493c6a598447fe5f46a390f3bee10f2d2ba2215d39829fe84eb40a7add18fc`  
		Last Modified: Tue, 12 Jan 2021 00:11:14 GMT  
		Size: 22.7 MB (22715905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce11a682b5a576d870bc1134f3a1482a65e9a1a819efd9c2ba568ebb74bcb3d`  
		Last Modified: Tue, 12 Jan 2021 03:50:14 GMT  
		Size: 15.6 MB (15566916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9dc5728e6ac838fbdf40b834aa7a033f738e7fcc3d4aef6a9a7fbac68e847a`  
		Last Modified: Tue, 12 Jan 2021 03:50:06 GMT  
		Size: 4.2 KB (4191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3566dad55b7fe7f28faa8cc4d3c3976a2592b6ca38e01d8b737f182493c0d5`  
		Last Modified: Tue, 12 Jan 2021 03:50:08 GMT  
		Size: 5.9 MB (5930368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:3abc760da20db96c1e183fe88265b47682cd5abbfc323a6dd55a023de85afd57
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49034646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9178faeae913664578ce317ea4499f0033456a24a0ddfc2efd43cdd2127f1840`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 04:53:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 04:53:02 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 04:53:05 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 04:53:06 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 04:53:06 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 04:56:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 04:56:39 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 04:56:40 GMT
USER user
# Tue, 12 Jan 2021 04:56:40 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e408b8961089722d96b5bd880822657cac883e9b44768370093db02d6200dfe3`  
		Last Modified: Tue, 12 Jan 2021 04:57:15 GMT  
		Size: 16.8 MB (16778122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afdadf12a13a42383ba5740842cd7b61dbba6da3fa80bec8d250855733181f48`  
		Last Modified: Tue, 12 Jan 2021 04:57:09 GMT  
		Size: 4.2 KB (4212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a44d48fea5067528d59d38b1cd576db46e2cd4281da1fa1a4c0fc94d27f181e7`  
		Last Modified: Tue, 12 Jan 2021 04:57:10 GMT  
		Size: 6.4 MB (6387820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2` - linux; 386

```console
$ docker pull irssi@sha256:bec995a740efa7f49fdd192fd4ca0d3d3b3a38f046aaa370e5310282c9c4970c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50398828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60ba27bbd1583680fd2f22bffab1a7e0888e91c87bfee095e0e32e0b924ab347`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:42:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:42:03 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 03:42:04 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 03:42:04 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 03:42:05 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 03:43:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 03:43:11 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 03:43:12 GMT
USER user
# Tue, 12 Jan 2021 03:43:12 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b2bfe52460501b552bf3e631c00eeeb8631995af9376813640417a3c000f94`  
		Last Modified: Tue, 12 Jan 2021 03:43:49 GMT  
		Size: 16.5 MB (16525249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cd9259438a5b49a8c24083be2c9392e846bd3967fa7053c1f61cf8df091fc6`  
		Last Modified: Tue, 12 Jan 2021 03:43:35 GMT  
		Size: 4.2 KB (4167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520edb3023f4d0e01d7b8688a80d79a8ad58b9863037245eb8c5039d54c87965`  
		Last Modified: Tue, 12 Jan 2021 03:43:35 GMT  
		Size: 6.1 MB (6101421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2` - linux; mips64le

```console
$ docker pull irssi@sha256:411d5291afdf74c5ade425b1117d505dbad5aae79b36c1bef0b2d4db2f02b8c4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47760566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d840df00faf9203081c843e4d607519333ad6c0167fd5190bebe8ea2247c49a`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 01:16:21 GMT
ADD file:e75a4429a4b3b0f7a646f85af88d412a98006cdf44ea6744b90fea7419840831 in / 
# Tue, 12 Jan 2021 01:16:22 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 05:52:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 05:52:21 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 05:52:22 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 05:52:23 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 05:52:23 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 05:54:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 05:54:55 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 05:54:55 GMT
USER user
# Tue, 12 Jan 2021 05:54:55 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c8d46df0b1a64c5ee6879aa09ea5818b36bcae5d39b941d7262bcff617be9873`  
		Last Modified: Tue, 12 Jan 2021 01:23:17 GMT  
		Size: 25.8 MB (25778695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5793705193bafef88f2e73d14ffad74a82df82eb504610af9e4317e2503abab`  
		Last Modified: Tue, 12 Jan 2021 05:55:38 GMT  
		Size: 15.7 MB (15687581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a046b9b47a317fbef9325c9df6ce038cf8e3b45de45ac125ef10922b340f951`  
		Last Modified: Tue, 12 Jan 2021 05:55:22 GMT  
		Size: 4.2 KB (4180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29b4995081445e06aaea12c5a1676c5fbfec79be31fd4ef6995273093a726f4`  
		Last Modified: Tue, 12 Jan 2021 05:55:27 GMT  
		Size: 6.3 MB (6290110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2` - linux; ppc64le

```console
$ docker pull irssi@sha256:6842568cae6c8c6d79b417ba7b42fc08c09e9b8a5f44451f02e162cbb031af3e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.7 MB (54721702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32f18ae696de1cd0c23aadcb2ef012b92e8a46605f9d81908264954f5c2abcc6`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:44:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:44:42 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 02:44:55 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 02:45:06 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 02:45:15 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 02:53:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 02:53:59 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 02:54:02 GMT
USER user
# Tue, 12 Jan 2021 02:54:04 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d49326825512307a99b49b2bc483f9841c4196b0f020811e9ad66498bbe53f9`  
		Last Modified: Tue, 12 Jan 2021 02:54:45 GMT  
		Size: 17.4 MB (17403860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cddccfe8b27784a6c3bcc136f813e67d85217d590538a6b0f24b392a147c7c95`  
		Last Modified: Tue, 12 Jan 2021 02:54:38 GMT  
		Size: 4.2 KB (4224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fb7721e869a0a3572123da5a5a9d5b7795cf9332fa06b604b378c8faeb362a`  
		Last Modified: Tue, 12 Jan 2021 02:54:38 GMT  
		Size: 6.8 MB (6780781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2` - linux; s390x

```console
$ docker pull irssi@sha256:ee350953d01f28ad635e1194152c20c0473f6e7bec4e6f4845c77cdd382238d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48997191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0365621040654b09bb5f1eea8657cdcca5cc5bcff9eecc979b39778390d29ee3`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:42:22 GMT
ADD file:c01d899d503187f788db0a7d658bf3f2b6541026a4c654707d3272f6d3ffaf58 in / 
# Tue, 12 Jan 2021 00:42:24 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:03:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:03:40 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 03:03:42 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 03:03:43 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 03:03:43 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 03:04:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 03:04:59 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 03:04:59 GMT
USER user
# Tue, 12 Jan 2021 03:04:59 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a0e3e06c0bd0347fefe8bde60780e7e551c0cdf1cbcf40be3d052e823d5ec118`  
		Last Modified: Tue, 12 Jan 2021 00:52:32 GMT  
		Size: 25.7 MB (25723406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b9fea8e4ca0ebc541e54ebc984bc5b2264637e7f0e8154e889fbf10a8774fe`  
		Last Modified: Tue, 12 Jan 2021 03:06:05 GMT  
		Size: 16.9 MB (16886327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d589abf4465e5265aca738df455a2f19f87b34932c190bbab36796c9633fe04`  
		Last Modified: Tue, 12 Jan 2021 03:06:05 GMT  
		Size: 4.2 KB (4219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:972f06fed78cf1528b81dc5167b378256a0153188898adfc443a2390f52c89ab`  
		Last Modified: Tue, 12 Jan 2021 03:06:06 GMT  
		Size: 6.4 MB (6383239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2.2-alpine`

```console
$ docker pull irssi@sha256:c25ee7f62ca4d46118f3bf6d99d0ca677217345c4c39af3c81d4dc064d9d5273
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `irssi:1.2.2-alpine` - linux; amd64

```console
$ docker pull irssi@sha256:ed3c96e17397592cf5b995c81a438bcc7e9fe64b45b8b6e7bf4b363bffbb42b4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18831066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3bc4928d9a6257ddfbf65b6fd26f94f40c586286113b72aae141ba938c1eaee`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 11:50:31 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 11:50:31 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 11:50:32 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 11:50:33 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 11:50:33 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 11:51:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 11:51:35 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 11:51:35 GMT
USER user
# Thu, 17 Dec 2020 11:51:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544af57a7985f1cf6294d7ca87a72fb8d57d1035919e7e535416905bf1c34692`  
		Last Modified: Thu, 17 Dec 2020 11:52:08 GMT  
		Size: 9.4 MB (9426043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d538cd733b8fe263d72ebe1eb2635e2c788821400beccc433ae5349473cecc`  
		Last Modified: Thu, 17 Dec 2020 11:52:03 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d8e49930ecea4f5a3c193a935a3f6c684cffdc8cfe2de950e0a9ed604527c1`  
		Last Modified: Thu, 17 Dec 2020 11:52:05 GMT  
		Size: 6.6 MB (6588915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:d0d31f288871ddcff3eda91a7da8590aee9ef5f1fac15dea95faf2e6797657df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17581856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec62aee6fd5f61040e71fd637332a945031d7a5ab5be09bbf1e9ea610afe7883`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:42:46 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 01:42:47 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 01:42:50 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 01:42:52 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 01:42:53 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 01:43:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 01:43:37 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 01:43:37 GMT
USER user
# Thu, 17 Dec 2020 01:43:38 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:56fec67ad66eea034cf5b7d0d0ffd355c0fe87611bad132ac5a952fcaa52138b`  
		Last Modified: Wed, 16 Dec 2020 23:50:34 GMT  
		Size: 2.6 MB (2620769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b94d836e65d230b1562764e4efa431641378df3281a3c10d04b4400c1c4a0c`  
		Last Modified: Thu, 17 Dec 2020 01:43:58 GMT  
		Size: 8.7 MB (8667899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ae78c3c78f66fc22eff63e83af767658711b61331c4f1340d37e01c85148db`  
		Last Modified: Thu, 17 Dec 2020 01:43:54 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbedcbb647790af67b3c5fd5a9718fbe5ffa60962c014b389a35c30a0cbaadb3`  
		Last Modified: Thu, 17 Dec 2020 01:43:56 GMT  
		Size: 6.3 MB (6291918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:0349e6f55f49688826896f680cbbdf0faef6215e9cf8f1a7ac192f8776c427b9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17026128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:989a3c7caba88843c2d38885aed0d403ad18bc94cf3360b629dc846e96e19837`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:28 GMT
ADD file:6757438ec5b22931a1c6a274c9c1eca94f0715a405d2ba91bd8b95704ba969ca in / 
# Wed, 16 Dec 2020 23:58:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 06:41:23 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 06:41:26 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 06:41:30 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 06:41:31 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 06:41:33 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 06:42:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 06:42:14 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 06:42:15 GMT
USER user
# Thu, 17 Dec 2020 06:42:16 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:71728559ce1f58d5e0ef30be5b1d7628ff967d4038f9202818dd3d8c76feb8ab`  
		Last Modified: Wed, 16 Dec 2020 23:59:11 GMT  
		Size: 2.4 MB (2422964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85167c5ffe77cc7bdd20b2c21fcdd73fedd45a537473ca88a2656e35c33da583`  
		Last Modified: Thu, 17 Dec 2020 06:42:54 GMT  
		Size: 8.5 MB (8519311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488f6846997914a7aedd46f1cbdb5a645ad16161634d0bd3fe5cca526e539e99`  
		Last Modified: Thu, 17 Dec 2020 06:42:50 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a30b53b5c8e70e1a0b26a162d7b2e1193ec54697865e065961e4fcc81abd7de`  
		Last Modified: Thu, 17 Dec 2020 06:42:52 GMT  
		Size: 6.1 MB (6082582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:39f822ea35985436cb794fe35b19a69d7af4ac0f91d227e54df67e5845bc75be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18718334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a27c74a0aa5b37ecfe8aa50c7cfe82cfa8cad7dbf412ac2441407508468e287`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 05:43:47 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 05:43:48 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 05:43:50 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 05:43:51 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 05:43:51 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 05:44:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 05:44:40 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 05:44:41 GMT
USER user
# Thu, 17 Dec 2020 05:44:41 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10541804ed63070e711a46540c6932c1a0da18ad63fda0ad637d2b4d7f2bcfe0`  
		Last Modified: Thu, 17 Dec 2020 05:45:15 GMT  
		Size: 9.4 MB (9426509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de39d0d358356491b02870cf4003c0784c6105c729ae72eaca35d1e9b525f18`  
		Last Modified: Thu, 17 Dec 2020 05:45:12 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348ab43696fd1f1ada1d4ae1ed10e5edbdf8b32a745cf472093004cad0f90835`  
		Last Modified: Thu, 17 Dec 2020 05:45:13 GMT  
		Size: 6.6 MB (6565337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2-alpine` - linux; 386

```console
$ docker pull irssi@sha256:5bebd276e28416ee0f7e59ee6294530125689c6255ce32b8a93a262ecebc5959
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.9 MB (17923261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83462ef5f6280a1f2fe9db74f845ba72a65270dce40e0dc4060ca60a807c5b38`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:39 GMT
ADD file:c8f5b26cfa9b90dfe6ca805f2101bd199c87b93faed2af74df0cbe54ea28fa6d in / 
# Thu, 17 Dec 2020 00:38:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:38:17 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 02:38:17 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 02:38:18 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 02:38:18 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 02:38:18 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 02:39:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 02:39:09 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 02:39:09 GMT
USER user
# Thu, 17 Dec 2020 02:39:09 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:60519712d04c07db59906a2e14fa87c037b6504d612ba116ea1ef94ae08a650b`  
		Last Modified: Thu, 17 Dec 2020 00:39:32 GMT  
		Size: 2.8 MB (2810512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06c3178940033973ed318f72a5f8ff0d33bf25be75357a659043a822c6df81ba`  
		Last Modified: Thu, 17 Dec 2020 02:39:43 GMT  
		Size: 8.8 MB (8796765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79639aa5facc9bfe7f24c999a249c2a557ca5f0925373391ce3bbbd68b447f22`  
		Last Modified: Thu, 17 Dec 2020 02:39:31 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092ed5b12af773f89402cf01a27599205717f3a2fbfe1227137de64d02483a1b`  
		Last Modified: Thu, 17 Dec 2020 02:39:33 GMT  
		Size: 6.3 MB (6314739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:4fe312a7f4361a5d57b5e60186685828f48bd9d17343df23339681482e7c9ea9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.2 MB (19164089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a4c630cf61ca7ff109dc201ab890e326fd9fdbebd2eae811bdc1f56f82cdc7d`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 17 Dec 2020 00:21:03 GMT
ADD file:4a7a7b8454234532546faed6d4d392f006f235e86744822034cb829a16205d11 in / 
# Thu, 17 Dec 2020 00:21:06 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:56:31 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 02:56:42 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 02:57:03 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 02:57:08 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 02:57:12 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 02:58:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 02:58:12 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 02:58:18 GMT
USER user
# Thu, 17 Dec 2020 02:58:24 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2c090b1a59445fb94c5fb14edf51af12a8f8bc2259535b08191f26ea84a7bb05`  
		Last Modified: Thu, 17 Dec 2020 00:21:49 GMT  
		Size: 2.8 MB (2821993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b0df84c68a3d54650f320d49e1d93a459175ad8543dd54535b21145e177dbf`  
		Last Modified: Thu, 17 Dec 2020 02:59:02 GMT  
		Size: 9.5 MB (9523198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd49f242497b77f4a53bae3b2d4178f0bf1c7777c1c123b282e608c5e35fad39`  
		Last Modified: Thu, 17 Dec 2020 02:58:59 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2e7e916f728483dd87b6e03a6b4b33851600aff2b6a27fb142a06442c6d3dd`  
		Last Modified: Thu, 17 Dec 2020 02:59:01 GMT  
		Size: 6.8 MB (6817620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:a6bd86db9f1a4b22c7f44b56f5a648a6d68589d1bd99a15a326df83834baf8dc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.0 MB (18983637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d4f8b6cd831610e9a7a4a8c11d964b272d652d1d9f16f02b2cd6ebcbe87b6a6`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:44 GMT
ADD file:9e0a7f4c5f520dabbf66a5d4312ceeb614fc5073fca7a248eb070cd99f4b75ff in / 
# Wed, 16 Dec 2020 23:41:44 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:46:38 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 01:46:42 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 01:46:44 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 01:46:44 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 01:46:45 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 01:47:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 01:47:36 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 01:47:37 GMT
USER user
# Thu, 17 Dec 2020 01:47:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ae4c90d25da4580c1cd02a35a672d9113b17e063183b4148c463df4d33079192`  
		Last Modified: Wed, 16 Dec 2020 23:42:26 GMT  
		Size: 2.6 MB (2583287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79426c202e567bd2b031639f258abcf1c6efb2488fc68d99b34a1a15f708cfdc`  
		Last Modified: Thu, 17 Dec 2020 01:48:05 GMT  
		Size: 9.8 MB (9837236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856e506a1f45e3f71bb52e86d7253d3226af83bbf745c2af33176f6642f75098`  
		Last Modified: Thu, 17 Dec 2020 01:48:03 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a65d002aeeabad4d91797eef53d8dd1d87dafac9378d9f7c16a534f920159e`  
		Last Modified: Thu, 17 Dec 2020 01:48:05 GMT  
		Size: 6.6 MB (6561843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2-alpine`

```console
$ docker pull irssi@sha256:c25ee7f62ca4d46118f3bf6d99d0ca677217345c4c39af3c81d4dc064d9d5273
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `irssi:1.2-alpine` - linux; amd64

```console
$ docker pull irssi@sha256:ed3c96e17397592cf5b995c81a438bcc7e9fe64b45b8b6e7bf4b363bffbb42b4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18831066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3bc4928d9a6257ddfbf65b6fd26f94f40c586286113b72aae141ba938c1eaee`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 11:50:31 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 11:50:31 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 11:50:32 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 11:50:33 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 11:50:33 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 11:51:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 11:51:35 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 11:51:35 GMT
USER user
# Thu, 17 Dec 2020 11:51:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544af57a7985f1cf6294d7ca87a72fb8d57d1035919e7e535416905bf1c34692`  
		Last Modified: Thu, 17 Dec 2020 11:52:08 GMT  
		Size: 9.4 MB (9426043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d538cd733b8fe263d72ebe1eb2635e2c788821400beccc433ae5349473cecc`  
		Last Modified: Thu, 17 Dec 2020 11:52:03 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d8e49930ecea4f5a3c193a935a3f6c684cffdc8cfe2de950e0a9ed604527c1`  
		Last Modified: Thu, 17 Dec 2020 11:52:05 GMT  
		Size: 6.6 MB (6588915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:d0d31f288871ddcff3eda91a7da8590aee9ef5f1fac15dea95faf2e6797657df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17581856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec62aee6fd5f61040e71fd637332a945031d7a5ab5be09bbf1e9ea610afe7883`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:42:46 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 01:42:47 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 01:42:50 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 01:42:52 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 01:42:53 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 01:43:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 01:43:37 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 01:43:37 GMT
USER user
# Thu, 17 Dec 2020 01:43:38 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:56fec67ad66eea034cf5b7d0d0ffd355c0fe87611bad132ac5a952fcaa52138b`  
		Last Modified: Wed, 16 Dec 2020 23:50:34 GMT  
		Size: 2.6 MB (2620769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b94d836e65d230b1562764e4efa431641378df3281a3c10d04b4400c1c4a0c`  
		Last Modified: Thu, 17 Dec 2020 01:43:58 GMT  
		Size: 8.7 MB (8667899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ae78c3c78f66fc22eff63e83af767658711b61331c4f1340d37e01c85148db`  
		Last Modified: Thu, 17 Dec 2020 01:43:54 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbedcbb647790af67b3c5fd5a9718fbe5ffa60962c014b389a35c30a0cbaadb3`  
		Last Modified: Thu, 17 Dec 2020 01:43:56 GMT  
		Size: 6.3 MB (6291918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:0349e6f55f49688826896f680cbbdf0faef6215e9cf8f1a7ac192f8776c427b9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17026128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:989a3c7caba88843c2d38885aed0d403ad18bc94cf3360b629dc846e96e19837`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:28 GMT
ADD file:6757438ec5b22931a1c6a274c9c1eca94f0715a405d2ba91bd8b95704ba969ca in / 
# Wed, 16 Dec 2020 23:58:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 06:41:23 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 06:41:26 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 06:41:30 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 06:41:31 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 06:41:33 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 06:42:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 06:42:14 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 06:42:15 GMT
USER user
# Thu, 17 Dec 2020 06:42:16 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:71728559ce1f58d5e0ef30be5b1d7628ff967d4038f9202818dd3d8c76feb8ab`  
		Last Modified: Wed, 16 Dec 2020 23:59:11 GMT  
		Size: 2.4 MB (2422964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85167c5ffe77cc7bdd20b2c21fcdd73fedd45a537473ca88a2656e35c33da583`  
		Last Modified: Thu, 17 Dec 2020 06:42:54 GMT  
		Size: 8.5 MB (8519311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488f6846997914a7aedd46f1cbdb5a645ad16161634d0bd3fe5cca526e539e99`  
		Last Modified: Thu, 17 Dec 2020 06:42:50 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a30b53b5c8e70e1a0b26a162d7b2e1193ec54697865e065961e4fcc81abd7de`  
		Last Modified: Thu, 17 Dec 2020 06:42:52 GMT  
		Size: 6.1 MB (6082582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:39f822ea35985436cb794fe35b19a69d7af4ac0f91d227e54df67e5845bc75be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18718334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a27c74a0aa5b37ecfe8aa50c7cfe82cfa8cad7dbf412ac2441407508468e287`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 05:43:47 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 05:43:48 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 05:43:50 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 05:43:51 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 05:43:51 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 05:44:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 05:44:40 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 05:44:41 GMT
USER user
# Thu, 17 Dec 2020 05:44:41 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10541804ed63070e711a46540c6932c1a0da18ad63fda0ad637d2b4d7f2bcfe0`  
		Last Modified: Thu, 17 Dec 2020 05:45:15 GMT  
		Size: 9.4 MB (9426509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de39d0d358356491b02870cf4003c0784c6105c729ae72eaca35d1e9b525f18`  
		Last Modified: Thu, 17 Dec 2020 05:45:12 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348ab43696fd1f1ada1d4ae1ed10e5edbdf8b32a745cf472093004cad0f90835`  
		Last Modified: Thu, 17 Dec 2020 05:45:13 GMT  
		Size: 6.6 MB (6565337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; 386

```console
$ docker pull irssi@sha256:5bebd276e28416ee0f7e59ee6294530125689c6255ce32b8a93a262ecebc5959
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.9 MB (17923261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83462ef5f6280a1f2fe9db74f845ba72a65270dce40e0dc4060ca60a807c5b38`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:39 GMT
ADD file:c8f5b26cfa9b90dfe6ca805f2101bd199c87b93faed2af74df0cbe54ea28fa6d in / 
# Thu, 17 Dec 2020 00:38:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:38:17 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 02:38:17 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 02:38:18 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 02:38:18 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 02:38:18 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 02:39:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 02:39:09 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 02:39:09 GMT
USER user
# Thu, 17 Dec 2020 02:39:09 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:60519712d04c07db59906a2e14fa87c037b6504d612ba116ea1ef94ae08a650b`  
		Last Modified: Thu, 17 Dec 2020 00:39:32 GMT  
		Size: 2.8 MB (2810512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06c3178940033973ed318f72a5f8ff0d33bf25be75357a659043a822c6df81ba`  
		Last Modified: Thu, 17 Dec 2020 02:39:43 GMT  
		Size: 8.8 MB (8796765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79639aa5facc9bfe7f24c999a249c2a557ca5f0925373391ce3bbbd68b447f22`  
		Last Modified: Thu, 17 Dec 2020 02:39:31 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092ed5b12af773f89402cf01a27599205717f3a2fbfe1227137de64d02483a1b`  
		Last Modified: Thu, 17 Dec 2020 02:39:33 GMT  
		Size: 6.3 MB (6314739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:4fe312a7f4361a5d57b5e60186685828f48bd9d17343df23339681482e7c9ea9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.2 MB (19164089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a4c630cf61ca7ff109dc201ab890e326fd9fdbebd2eae811bdc1f56f82cdc7d`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 17 Dec 2020 00:21:03 GMT
ADD file:4a7a7b8454234532546faed6d4d392f006f235e86744822034cb829a16205d11 in / 
# Thu, 17 Dec 2020 00:21:06 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:56:31 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 02:56:42 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 02:57:03 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 02:57:08 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 02:57:12 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 02:58:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 02:58:12 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 02:58:18 GMT
USER user
# Thu, 17 Dec 2020 02:58:24 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2c090b1a59445fb94c5fb14edf51af12a8f8bc2259535b08191f26ea84a7bb05`  
		Last Modified: Thu, 17 Dec 2020 00:21:49 GMT  
		Size: 2.8 MB (2821993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b0df84c68a3d54650f320d49e1d93a459175ad8543dd54535b21145e177dbf`  
		Last Modified: Thu, 17 Dec 2020 02:59:02 GMT  
		Size: 9.5 MB (9523198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd49f242497b77f4a53bae3b2d4178f0bf1c7777c1c123b282e608c5e35fad39`  
		Last Modified: Thu, 17 Dec 2020 02:58:59 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2e7e916f728483dd87b6e03a6b4b33851600aff2b6a27fb142a06442c6d3dd`  
		Last Modified: Thu, 17 Dec 2020 02:59:01 GMT  
		Size: 6.8 MB (6817620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:a6bd86db9f1a4b22c7f44b56f5a648a6d68589d1bd99a15a326df83834baf8dc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.0 MB (18983637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d4f8b6cd831610e9a7a4a8c11d964b272d652d1d9f16f02b2cd6ebcbe87b6a6`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:44 GMT
ADD file:9e0a7f4c5f520dabbf66a5d4312ceeb614fc5073fca7a248eb070cd99f4b75ff in / 
# Wed, 16 Dec 2020 23:41:44 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:46:38 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 01:46:42 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 01:46:44 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 01:46:44 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 01:46:45 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 01:47:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 01:47:36 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 01:47:37 GMT
USER user
# Thu, 17 Dec 2020 01:47:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ae4c90d25da4580c1cd02a35a672d9113b17e063183b4148c463df4d33079192`  
		Last Modified: Wed, 16 Dec 2020 23:42:26 GMT  
		Size: 2.6 MB (2583287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79426c202e567bd2b031639f258abcf1c6efb2488fc68d99b34a1a15f708cfdc`  
		Last Modified: Thu, 17 Dec 2020 01:48:05 GMT  
		Size: 9.8 MB (9837236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856e506a1f45e3f71bb52e86d7253d3226af83bbf745c2af33176f6642f75098`  
		Last Modified: Thu, 17 Dec 2020 01:48:03 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a65d002aeeabad4d91797eef53d8dd1d87dafac9378d9f7c16a534f920159e`  
		Last Modified: Thu, 17 Dec 2020 01:48:05 GMT  
		Size: 6.6 MB (6561843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1-alpine`

```console
$ docker pull irssi@sha256:c25ee7f62ca4d46118f3bf6d99d0ca677217345c4c39af3c81d4dc064d9d5273
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `irssi:1-alpine` - linux; amd64

```console
$ docker pull irssi@sha256:ed3c96e17397592cf5b995c81a438bcc7e9fe64b45b8b6e7bf4b363bffbb42b4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18831066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3bc4928d9a6257ddfbf65b6fd26f94f40c586286113b72aae141ba938c1eaee`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 11:50:31 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 11:50:31 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 11:50:32 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 11:50:33 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 11:50:33 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 11:51:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 11:51:35 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 11:51:35 GMT
USER user
# Thu, 17 Dec 2020 11:51:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544af57a7985f1cf6294d7ca87a72fb8d57d1035919e7e535416905bf1c34692`  
		Last Modified: Thu, 17 Dec 2020 11:52:08 GMT  
		Size: 9.4 MB (9426043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d538cd733b8fe263d72ebe1eb2635e2c788821400beccc433ae5349473cecc`  
		Last Modified: Thu, 17 Dec 2020 11:52:03 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d8e49930ecea4f5a3c193a935a3f6c684cffdc8cfe2de950e0a9ed604527c1`  
		Last Modified: Thu, 17 Dec 2020 11:52:05 GMT  
		Size: 6.6 MB (6588915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:d0d31f288871ddcff3eda91a7da8590aee9ef5f1fac15dea95faf2e6797657df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17581856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec62aee6fd5f61040e71fd637332a945031d7a5ab5be09bbf1e9ea610afe7883`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:42:46 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 01:42:47 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 01:42:50 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 01:42:52 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 01:42:53 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 01:43:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 01:43:37 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 01:43:37 GMT
USER user
# Thu, 17 Dec 2020 01:43:38 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:56fec67ad66eea034cf5b7d0d0ffd355c0fe87611bad132ac5a952fcaa52138b`  
		Last Modified: Wed, 16 Dec 2020 23:50:34 GMT  
		Size: 2.6 MB (2620769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b94d836e65d230b1562764e4efa431641378df3281a3c10d04b4400c1c4a0c`  
		Last Modified: Thu, 17 Dec 2020 01:43:58 GMT  
		Size: 8.7 MB (8667899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ae78c3c78f66fc22eff63e83af767658711b61331c4f1340d37e01c85148db`  
		Last Modified: Thu, 17 Dec 2020 01:43:54 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbedcbb647790af67b3c5fd5a9718fbe5ffa60962c014b389a35c30a0cbaadb3`  
		Last Modified: Thu, 17 Dec 2020 01:43:56 GMT  
		Size: 6.3 MB (6291918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:0349e6f55f49688826896f680cbbdf0faef6215e9cf8f1a7ac192f8776c427b9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17026128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:989a3c7caba88843c2d38885aed0d403ad18bc94cf3360b629dc846e96e19837`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:28 GMT
ADD file:6757438ec5b22931a1c6a274c9c1eca94f0715a405d2ba91bd8b95704ba969ca in / 
# Wed, 16 Dec 2020 23:58:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 06:41:23 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 06:41:26 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 06:41:30 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 06:41:31 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 06:41:33 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 06:42:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 06:42:14 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 06:42:15 GMT
USER user
# Thu, 17 Dec 2020 06:42:16 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:71728559ce1f58d5e0ef30be5b1d7628ff967d4038f9202818dd3d8c76feb8ab`  
		Last Modified: Wed, 16 Dec 2020 23:59:11 GMT  
		Size: 2.4 MB (2422964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85167c5ffe77cc7bdd20b2c21fcdd73fedd45a537473ca88a2656e35c33da583`  
		Last Modified: Thu, 17 Dec 2020 06:42:54 GMT  
		Size: 8.5 MB (8519311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488f6846997914a7aedd46f1cbdb5a645ad16161634d0bd3fe5cca526e539e99`  
		Last Modified: Thu, 17 Dec 2020 06:42:50 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a30b53b5c8e70e1a0b26a162d7b2e1193ec54697865e065961e4fcc81abd7de`  
		Last Modified: Thu, 17 Dec 2020 06:42:52 GMT  
		Size: 6.1 MB (6082582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:39f822ea35985436cb794fe35b19a69d7af4ac0f91d227e54df67e5845bc75be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18718334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a27c74a0aa5b37ecfe8aa50c7cfe82cfa8cad7dbf412ac2441407508468e287`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 05:43:47 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 05:43:48 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 05:43:50 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 05:43:51 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 05:43:51 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 05:44:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 05:44:40 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 05:44:41 GMT
USER user
# Thu, 17 Dec 2020 05:44:41 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10541804ed63070e711a46540c6932c1a0da18ad63fda0ad637d2b4d7f2bcfe0`  
		Last Modified: Thu, 17 Dec 2020 05:45:15 GMT  
		Size: 9.4 MB (9426509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de39d0d358356491b02870cf4003c0784c6105c729ae72eaca35d1e9b525f18`  
		Last Modified: Thu, 17 Dec 2020 05:45:12 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348ab43696fd1f1ada1d4ae1ed10e5edbdf8b32a745cf472093004cad0f90835`  
		Last Modified: Thu, 17 Dec 2020 05:45:13 GMT  
		Size: 6.6 MB (6565337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; 386

```console
$ docker pull irssi@sha256:5bebd276e28416ee0f7e59ee6294530125689c6255ce32b8a93a262ecebc5959
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.9 MB (17923261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83462ef5f6280a1f2fe9db74f845ba72a65270dce40e0dc4060ca60a807c5b38`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:39 GMT
ADD file:c8f5b26cfa9b90dfe6ca805f2101bd199c87b93faed2af74df0cbe54ea28fa6d in / 
# Thu, 17 Dec 2020 00:38:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:38:17 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 02:38:17 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 02:38:18 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 02:38:18 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 02:38:18 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 02:39:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 02:39:09 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 02:39:09 GMT
USER user
# Thu, 17 Dec 2020 02:39:09 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:60519712d04c07db59906a2e14fa87c037b6504d612ba116ea1ef94ae08a650b`  
		Last Modified: Thu, 17 Dec 2020 00:39:32 GMT  
		Size: 2.8 MB (2810512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06c3178940033973ed318f72a5f8ff0d33bf25be75357a659043a822c6df81ba`  
		Last Modified: Thu, 17 Dec 2020 02:39:43 GMT  
		Size: 8.8 MB (8796765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79639aa5facc9bfe7f24c999a249c2a557ca5f0925373391ce3bbbd68b447f22`  
		Last Modified: Thu, 17 Dec 2020 02:39:31 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092ed5b12af773f89402cf01a27599205717f3a2fbfe1227137de64d02483a1b`  
		Last Modified: Thu, 17 Dec 2020 02:39:33 GMT  
		Size: 6.3 MB (6314739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:4fe312a7f4361a5d57b5e60186685828f48bd9d17343df23339681482e7c9ea9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.2 MB (19164089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a4c630cf61ca7ff109dc201ab890e326fd9fdbebd2eae811bdc1f56f82cdc7d`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 17 Dec 2020 00:21:03 GMT
ADD file:4a7a7b8454234532546faed6d4d392f006f235e86744822034cb829a16205d11 in / 
# Thu, 17 Dec 2020 00:21:06 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:56:31 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 02:56:42 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 02:57:03 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 02:57:08 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 02:57:12 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 02:58:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 02:58:12 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 02:58:18 GMT
USER user
# Thu, 17 Dec 2020 02:58:24 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2c090b1a59445fb94c5fb14edf51af12a8f8bc2259535b08191f26ea84a7bb05`  
		Last Modified: Thu, 17 Dec 2020 00:21:49 GMT  
		Size: 2.8 MB (2821993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b0df84c68a3d54650f320d49e1d93a459175ad8543dd54535b21145e177dbf`  
		Last Modified: Thu, 17 Dec 2020 02:59:02 GMT  
		Size: 9.5 MB (9523198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd49f242497b77f4a53bae3b2d4178f0bf1c7777c1c123b282e608c5e35fad39`  
		Last Modified: Thu, 17 Dec 2020 02:58:59 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2e7e916f728483dd87b6e03a6b4b33851600aff2b6a27fb142a06442c6d3dd`  
		Last Modified: Thu, 17 Dec 2020 02:59:01 GMT  
		Size: 6.8 MB (6817620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:a6bd86db9f1a4b22c7f44b56f5a648a6d68589d1bd99a15a326df83834baf8dc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.0 MB (18983637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d4f8b6cd831610e9a7a4a8c11d964b272d652d1d9f16f02b2cd6ebcbe87b6a6`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:44 GMT
ADD file:9e0a7f4c5f520dabbf66a5d4312ceeb614fc5073fca7a248eb070cd99f4b75ff in / 
# Wed, 16 Dec 2020 23:41:44 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:46:38 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 01:46:42 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 01:46:44 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 01:46:44 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 01:46:45 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 01:47:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 01:47:36 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 01:47:37 GMT
USER user
# Thu, 17 Dec 2020 01:47:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ae4c90d25da4580c1cd02a35a672d9113b17e063183b4148c463df4d33079192`  
		Last Modified: Wed, 16 Dec 2020 23:42:26 GMT  
		Size: 2.6 MB (2583287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79426c202e567bd2b031639f258abcf1c6efb2488fc68d99b34a1a15f708cfdc`  
		Last Modified: Thu, 17 Dec 2020 01:48:05 GMT  
		Size: 9.8 MB (9837236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856e506a1f45e3f71bb52e86d7253d3226af83bbf745c2af33176f6642f75098`  
		Last Modified: Thu, 17 Dec 2020 01:48:03 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a65d002aeeabad4d91797eef53d8dd1d87dafac9378d9f7c16a534f920159e`  
		Last Modified: Thu, 17 Dec 2020 01:48:05 GMT  
		Size: 6.6 MB (6561843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:alpine`

```console
$ docker pull irssi@sha256:c25ee7f62ca4d46118f3bf6d99d0ca677217345c4c39af3c81d4dc064d9d5273
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `irssi:alpine` - linux; amd64

```console
$ docker pull irssi@sha256:ed3c96e17397592cf5b995c81a438bcc7e9fe64b45b8b6e7bf4b363bffbb42b4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18831066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3bc4928d9a6257ddfbf65b6fd26f94f40c586286113b72aae141ba938c1eaee`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 11:50:31 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 11:50:31 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 11:50:32 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 11:50:33 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 11:50:33 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 11:51:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 11:51:35 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 11:51:35 GMT
USER user
# Thu, 17 Dec 2020 11:51:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544af57a7985f1cf6294d7ca87a72fb8d57d1035919e7e535416905bf1c34692`  
		Last Modified: Thu, 17 Dec 2020 11:52:08 GMT  
		Size: 9.4 MB (9426043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d538cd733b8fe263d72ebe1eb2635e2c788821400beccc433ae5349473cecc`  
		Last Modified: Thu, 17 Dec 2020 11:52:03 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d8e49930ecea4f5a3c193a935a3f6c684cffdc8cfe2de950e0a9ed604527c1`  
		Last Modified: Thu, 17 Dec 2020 11:52:05 GMT  
		Size: 6.6 MB (6588915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:d0d31f288871ddcff3eda91a7da8590aee9ef5f1fac15dea95faf2e6797657df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17581856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec62aee6fd5f61040e71fd637332a945031d7a5ab5be09bbf1e9ea610afe7883`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:42:46 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 01:42:47 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 01:42:50 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 01:42:52 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 01:42:53 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 01:43:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 01:43:37 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 01:43:37 GMT
USER user
# Thu, 17 Dec 2020 01:43:38 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:56fec67ad66eea034cf5b7d0d0ffd355c0fe87611bad132ac5a952fcaa52138b`  
		Last Modified: Wed, 16 Dec 2020 23:50:34 GMT  
		Size: 2.6 MB (2620769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b94d836e65d230b1562764e4efa431641378df3281a3c10d04b4400c1c4a0c`  
		Last Modified: Thu, 17 Dec 2020 01:43:58 GMT  
		Size: 8.7 MB (8667899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ae78c3c78f66fc22eff63e83af767658711b61331c4f1340d37e01c85148db`  
		Last Modified: Thu, 17 Dec 2020 01:43:54 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbedcbb647790af67b3c5fd5a9718fbe5ffa60962c014b389a35c30a0cbaadb3`  
		Last Modified: Thu, 17 Dec 2020 01:43:56 GMT  
		Size: 6.3 MB (6291918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:0349e6f55f49688826896f680cbbdf0faef6215e9cf8f1a7ac192f8776c427b9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17026128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:989a3c7caba88843c2d38885aed0d403ad18bc94cf3360b629dc846e96e19837`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:28 GMT
ADD file:6757438ec5b22931a1c6a274c9c1eca94f0715a405d2ba91bd8b95704ba969ca in / 
# Wed, 16 Dec 2020 23:58:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 06:41:23 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 06:41:26 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 06:41:30 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 06:41:31 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 06:41:33 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 06:42:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 06:42:14 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 06:42:15 GMT
USER user
# Thu, 17 Dec 2020 06:42:16 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:71728559ce1f58d5e0ef30be5b1d7628ff967d4038f9202818dd3d8c76feb8ab`  
		Last Modified: Wed, 16 Dec 2020 23:59:11 GMT  
		Size: 2.4 MB (2422964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85167c5ffe77cc7bdd20b2c21fcdd73fedd45a537473ca88a2656e35c33da583`  
		Last Modified: Thu, 17 Dec 2020 06:42:54 GMT  
		Size: 8.5 MB (8519311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488f6846997914a7aedd46f1cbdb5a645ad16161634d0bd3fe5cca526e539e99`  
		Last Modified: Thu, 17 Dec 2020 06:42:50 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a30b53b5c8e70e1a0b26a162d7b2e1193ec54697865e065961e4fcc81abd7de`  
		Last Modified: Thu, 17 Dec 2020 06:42:52 GMT  
		Size: 6.1 MB (6082582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:39f822ea35985436cb794fe35b19a69d7af4ac0f91d227e54df67e5845bc75be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18718334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a27c74a0aa5b37ecfe8aa50c7cfe82cfa8cad7dbf412ac2441407508468e287`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 05:43:47 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 05:43:48 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 05:43:50 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 05:43:51 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 05:43:51 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 05:44:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 05:44:40 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 05:44:41 GMT
USER user
# Thu, 17 Dec 2020 05:44:41 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10541804ed63070e711a46540c6932c1a0da18ad63fda0ad637d2b4d7f2bcfe0`  
		Last Modified: Thu, 17 Dec 2020 05:45:15 GMT  
		Size: 9.4 MB (9426509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de39d0d358356491b02870cf4003c0784c6105c729ae72eaca35d1e9b525f18`  
		Last Modified: Thu, 17 Dec 2020 05:45:12 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348ab43696fd1f1ada1d4ae1ed10e5edbdf8b32a745cf472093004cad0f90835`  
		Last Modified: Thu, 17 Dec 2020 05:45:13 GMT  
		Size: 6.6 MB (6565337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; 386

```console
$ docker pull irssi@sha256:5bebd276e28416ee0f7e59ee6294530125689c6255ce32b8a93a262ecebc5959
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.9 MB (17923261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83462ef5f6280a1f2fe9db74f845ba72a65270dce40e0dc4060ca60a807c5b38`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:39 GMT
ADD file:c8f5b26cfa9b90dfe6ca805f2101bd199c87b93faed2af74df0cbe54ea28fa6d in / 
# Thu, 17 Dec 2020 00:38:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:38:17 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 02:38:17 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 02:38:18 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 02:38:18 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 02:38:18 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 02:39:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 02:39:09 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 02:39:09 GMT
USER user
# Thu, 17 Dec 2020 02:39:09 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:60519712d04c07db59906a2e14fa87c037b6504d612ba116ea1ef94ae08a650b`  
		Last Modified: Thu, 17 Dec 2020 00:39:32 GMT  
		Size: 2.8 MB (2810512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06c3178940033973ed318f72a5f8ff0d33bf25be75357a659043a822c6df81ba`  
		Last Modified: Thu, 17 Dec 2020 02:39:43 GMT  
		Size: 8.8 MB (8796765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79639aa5facc9bfe7f24c999a249c2a557ca5f0925373391ce3bbbd68b447f22`  
		Last Modified: Thu, 17 Dec 2020 02:39:31 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092ed5b12af773f89402cf01a27599205717f3a2fbfe1227137de64d02483a1b`  
		Last Modified: Thu, 17 Dec 2020 02:39:33 GMT  
		Size: 6.3 MB (6314739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:4fe312a7f4361a5d57b5e60186685828f48bd9d17343df23339681482e7c9ea9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.2 MB (19164089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a4c630cf61ca7ff109dc201ab890e326fd9fdbebd2eae811bdc1f56f82cdc7d`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 17 Dec 2020 00:21:03 GMT
ADD file:4a7a7b8454234532546faed6d4d392f006f235e86744822034cb829a16205d11 in / 
# Thu, 17 Dec 2020 00:21:06 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:56:31 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 02:56:42 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 02:57:03 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 02:57:08 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 02:57:12 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 02:58:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 02:58:12 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 02:58:18 GMT
USER user
# Thu, 17 Dec 2020 02:58:24 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2c090b1a59445fb94c5fb14edf51af12a8f8bc2259535b08191f26ea84a7bb05`  
		Last Modified: Thu, 17 Dec 2020 00:21:49 GMT  
		Size: 2.8 MB (2821993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b0df84c68a3d54650f320d49e1d93a459175ad8543dd54535b21145e177dbf`  
		Last Modified: Thu, 17 Dec 2020 02:59:02 GMT  
		Size: 9.5 MB (9523198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd49f242497b77f4a53bae3b2d4178f0bf1c7777c1c123b282e608c5e35fad39`  
		Last Modified: Thu, 17 Dec 2020 02:58:59 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2e7e916f728483dd87b6e03a6b4b33851600aff2b6a27fb142a06442c6d3dd`  
		Last Modified: Thu, 17 Dec 2020 02:59:01 GMT  
		Size: 6.8 MB (6817620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; s390x

```console
$ docker pull irssi@sha256:a6bd86db9f1a4b22c7f44b56f5a648a6d68589d1bd99a15a326df83834baf8dc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.0 MB (18983637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d4f8b6cd831610e9a7a4a8c11d964b272d652d1d9f16f02b2cd6ebcbe87b6a6`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:44 GMT
ADD file:9e0a7f4c5f520dabbf66a5d4312ceeb614fc5073fca7a248eb070cd99f4b75ff in / 
# Wed, 16 Dec 2020 23:41:44 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:46:38 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Dec 2020 01:46:42 GMT
ENV HOME=/home/user
# Thu, 17 Dec 2020 01:46:44 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Dec 2020 01:46:44 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 01:46:45 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 17 Dec 2020 01:47:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Dec 2020 01:47:36 GMT
WORKDIR /home/user
# Thu, 17 Dec 2020 01:47:37 GMT
USER user
# Thu, 17 Dec 2020 01:47:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ae4c90d25da4580c1cd02a35a672d9113b17e063183b4148c463df4d33079192`  
		Last Modified: Wed, 16 Dec 2020 23:42:26 GMT  
		Size: 2.6 MB (2583287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79426c202e567bd2b031639f258abcf1c6efb2488fc68d99b34a1a15f708cfdc`  
		Last Modified: Thu, 17 Dec 2020 01:48:05 GMT  
		Size: 9.8 MB (9837236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856e506a1f45e3f71bb52e86d7253d3226af83bbf745c2af33176f6642f75098`  
		Last Modified: Thu, 17 Dec 2020 01:48:03 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a65d002aeeabad4d91797eef53d8dd1d87dafac9378d9f7c16a534f920159e`  
		Last Modified: Thu, 17 Dec 2020 01:48:05 GMT  
		Size: 6.6 MB (6561843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:latest`

```console
$ docker pull irssi@sha256:522eb796ea2bd9501803f99d612ca113a6a28deaefb89506517574dd268c2aed
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

### `irssi:latest` - linux; amd64

```console
$ docker pull irssi@sha256:af02b4b7fd40efc410580773ef0c4ff3a14877b2ea4598edb12d4485310c9d96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50541239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87fea6963c9b2b4d42b3e2d8cf658c714fe03da2a2b0804ddf3c61463626c3a4`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:38:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 09:38:44 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 09:38:46 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 09:38:46 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 09:38:46 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 09:39:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 09:39:55 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 09:39:55 GMT
USER user
# Tue, 12 Jan 2021 09:39:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db80d14f483469e745ac0212bdf1e73f6158b62e49fff6c240aaee12bcdb7e5`  
		Last Modified: Tue, 12 Jan 2021 09:40:28 GMT  
		Size: 17.0 MB (16999919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2969bb11828af3b3ece9cee2d04141672d87b04890d6dee06b3619d9040a88`  
		Last Modified: Tue, 12 Jan 2021 09:40:24 GMT  
		Size: 4.2 KB (4180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511f4c020a955d0bea6de98441803a9eac6cc037996ffe42c834faa70865002f`  
		Last Modified: Tue, 12 Jan 2021 09:40:24 GMT  
		Size: 6.4 MB (6429071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm variant v5

```console
$ docker pull irssi@sha256:8cab443d7c6e0757d9ce2e72494462ddc8a086259ae61939a21de094e1a5fa51
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46825932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b5a984afad6b9f1273f5d3a3fdf77eef2de72dd911d5ad6668efb725b341631`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:34 GMT
ADD file:57136a762436a5d41e60c61db0d89baea17a289845ea55565e45cc79a9e81e23 in / 
# Tue, 12 Jan 2021 00:51:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:22:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:22:31 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 02:22:34 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 02:22:35 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 02:22:36 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 02:24:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 02:24:15 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 02:24:16 GMT
USER user
# Tue, 12 Jan 2021 02:24:17 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2e2535e18472e7491a1d935b1f44ac842e4cc5c4d3de40cecb77b56b44515910`  
		Last Modified: Tue, 12 Jan 2021 01:00:19 GMT  
		Size: 24.9 MB (24851909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8e230c8f512600659fd9bc5c4209a057c8be3d630b5888c34eea16d7610d2b`  
		Last Modified: Tue, 12 Jan 2021 02:24:44 GMT  
		Size: 15.9 MB (15907342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc34cc4cc032ca0d1cd996d051d2ac727da40f24f63f04a8c581962c7be9714c`  
		Last Modified: Tue, 12 Jan 2021 02:24:36 GMT  
		Size: 4.2 KB (4196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ec18b89f11758e0608a36f62371cf2ae5c4e59a9b0dddd2be9e65a6a497ae6`  
		Last Modified: Tue, 12 Jan 2021 02:24:38 GMT  
		Size: 6.1 MB (6062485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm variant v7

```console
$ docker pull irssi@sha256:a2f1914a650a4be6d11af87e5ed84c1d4204c483f1207f1b22104ca9349f6853
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44217380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deac85e27be886cc14446c41ebef26c4591b3fcc10e4510a417fbd5f8bc29f59`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:01:09 GMT
ADD file:1db27e410cc7caf4a97a7313c57260fd01aa134b84306914ef0948dcca27372d in / 
# Tue, 12 Jan 2021 00:01:12 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:48:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:48:04 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 03:48:06 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 03:48:06 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 03:48:07 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 03:49:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 03:49:33 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 03:49:34 GMT
USER user
# Tue, 12 Jan 2021 03:49:35 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:be493c6a598447fe5f46a390f3bee10f2d2ba2215d39829fe84eb40a7add18fc`  
		Last Modified: Tue, 12 Jan 2021 00:11:14 GMT  
		Size: 22.7 MB (22715905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce11a682b5a576d870bc1134f3a1482a65e9a1a819efd9c2ba568ebb74bcb3d`  
		Last Modified: Tue, 12 Jan 2021 03:50:14 GMT  
		Size: 15.6 MB (15566916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9dc5728e6ac838fbdf40b834aa7a033f738e7fcc3d4aef6a9a7fbac68e847a`  
		Last Modified: Tue, 12 Jan 2021 03:50:06 GMT  
		Size: 4.2 KB (4191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3566dad55b7fe7f28faa8cc4d3c3976a2592b6ca38e01d8b737f182493c0d5`  
		Last Modified: Tue, 12 Jan 2021 03:50:08 GMT  
		Size: 5.9 MB (5930368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:3abc760da20db96c1e183fe88265b47682cd5abbfc323a6dd55a023de85afd57
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49034646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9178faeae913664578ce317ea4499f0033456a24a0ddfc2efd43cdd2127f1840`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 04:53:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 04:53:02 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 04:53:05 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 04:53:06 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 04:53:06 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 04:56:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 04:56:39 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 04:56:40 GMT
USER user
# Tue, 12 Jan 2021 04:56:40 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e408b8961089722d96b5bd880822657cac883e9b44768370093db02d6200dfe3`  
		Last Modified: Tue, 12 Jan 2021 04:57:15 GMT  
		Size: 16.8 MB (16778122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afdadf12a13a42383ba5740842cd7b61dbba6da3fa80bec8d250855733181f48`  
		Last Modified: Tue, 12 Jan 2021 04:57:09 GMT  
		Size: 4.2 KB (4212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a44d48fea5067528d59d38b1cd576db46e2cd4281da1fa1a4c0fc94d27f181e7`  
		Last Modified: Tue, 12 Jan 2021 04:57:10 GMT  
		Size: 6.4 MB (6387820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; 386

```console
$ docker pull irssi@sha256:bec995a740efa7f49fdd192fd4ca0d3d3b3a38f046aaa370e5310282c9c4970c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50398828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60ba27bbd1583680fd2f22bffab1a7e0888e91c87bfee095e0e32e0b924ab347`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:42:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:42:03 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 03:42:04 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 03:42:04 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 03:42:05 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 03:43:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 03:43:11 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 03:43:12 GMT
USER user
# Tue, 12 Jan 2021 03:43:12 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b2bfe52460501b552bf3e631c00eeeb8631995af9376813640417a3c000f94`  
		Last Modified: Tue, 12 Jan 2021 03:43:49 GMT  
		Size: 16.5 MB (16525249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cd9259438a5b49a8c24083be2c9392e846bd3967fa7053c1f61cf8df091fc6`  
		Last Modified: Tue, 12 Jan 2021 03:43:35 GMT  
		Size: 4.2 KB (4167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520edb3023f4d0e01d7b8688a80d79a8ad58b9863037245eb8c5039d54c87965`  
		Last Modified: Tue, 12 Jan 2021 03:43:35 GMT  
		Size: 6.1 MB (6101421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; mips64le

```console
$ docker pull irssi@sha256:411d5291afdf74c5ade425b1117d505dbad5aae79b36c1bef0b2d4db2f02b8c4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47760566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d840df00faf9203081c843e4d607519333ad6c0167fd5190bebe8ea2247c49a`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 01:16:21 GMT
ADD file:e75a4429a4b3b0f7a646f85af88d412a98006cdf44ea6744b90fea7419840831 in / 
# Tue, 12 Jan 2021 01:16:22 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 05:52:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 05:52:21 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 05:52:22 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 05:52:23 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 05:52:23 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 05:54:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 05:54:55 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 05:54:55 GMT
USER user
# Tue, 12 Jan 2021 05:54:55 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c8d46df0b1a64c5ee6879aa09ea5818b36bcae5d39b941d7262bcff617be9873`  
		Last Modified: Tue, 12 Jan 2021 01:23:17 GMT  
		Size: 25.8 MB (25778695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5793705193bafef88f2e73d14ffad74a82df82eb504610af9e4317e2503abab`  
		Last Modified: Tue, 12 Jan 2021 05:55:38 GMT  
		Size: 15.7 MB (15687581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a046b9b47a317fbef9325c9df6ce038cf8e3b45de45ac125ef10922b340f951`  
		Last Modified: Tue, 12 Jan 2021 05:55:22 GMT  
		Size: 4.2 KB (4180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29b4995081445e06aaea12c5a1676c5fbfec79be31fd4ef6995273093a726f4`  
		Last Modified: Tue, 12 Jan 2021 05:55:27 GMT  
		Size: 6.3 MB (6290110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; ppc64le

```console
$ docker pull irssi@sha256:6842568cae6c8c6d79b417ba7b42fc08c09e9b8a5f44451f02e162cbb031af3e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.7 MB (54721702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32f18ae696de1cd0c23aadcb2ef012b92e8a46605f9d81908264954f5c2abcc6`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:44:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:44:42 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 02:44:55 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 02:45:06 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 02:45:15 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 02:53:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 02:53:59 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 02:54:02 GMT
USER user
# Tue, 12 Jan 2021 02:54:04 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d49326825512307a99b49b2bc483f9841c4196b0f020811e9ad66498bbe53f9`  
		Last Modified: Tue, 12 Jan 2021 02:54:45 GMT  
		Size: 17.4 MB (17403860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cddccfe8b27784a6c3bcc136f813e67d85217d590538a6b0f24b392a147c7c95`  
		Last Modified: Tue, 12 Jan 2021 02:54:38 GMT  
		Size: 4.2 KB (4224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fb7721e869a0a3572123da5a5a9d5b7795cf9332fa06b604b378c8faeb362a`  
		Last Modified: Tue, 12 Jan 2021 02:54:38 GMT  
		Size: 6.8 MB (6780781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; s390x

```console
$ docker pull irssi@sha256:ee350953d01f28ad635e1194152c20c0473f6e7bec4e6f4845c77cdd382238d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48997191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0365621040654b09bb5f1eea8657cdcca5cc5bcff9eecc979b39778390d29ee3`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Jan 2021 00:42:22 GMT
ADD file:c01d899d503187f788db0a7d658bf3f2b6541026a4c654707d3272f6d3ffaf58 in / 
# Tue, 12 Jan 2021 00:42:24 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:03:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:03:40 GMT
ENV HOME=/home/user
# Tue, 12 Jan 2021 03:03:42 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Jan 2021 03:03:43 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 03:03:43 GMT
ENV IRSSI_VERSION=1.2.2
# Tue, 12 Jan 2021 03:04:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Jan 2021 03:04:59 GMT
WORKDIR /home/user
# Tue, 12 Jan 2021 03:04:59 GMT
USER user
# Tue, 12 Jan 2021 03:04:59 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a0e3e06c0bd0347fefe8bde60780e7e551c0cdf1cbcf40be3d052e823d5ec118`  
		Last Modified: Tue, 12 Jan 2021 00:52:32 GMT  
		Size: 25.7 MB (25723406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b9fea8e4ca0ebc541e54ebc984bc5b2264637e7f0e8154e889fbf10a8774fe`  
		Last Modified: Tue, 12 Jan 2021 03:06:05 GMT  
		Size: 16.9 MB (16886327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d589abf4465e5265aca738df455a2f19f87b34932c190bbab36796c9633fe04`  
		Last Modified: Tue, 12 Jan 2021 03:06:05 GMT  
		Size: 4.2 KB (4219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:972f06fed78cf1528b81dc5167b378256a0153188898adfc443a2390f52c89ab`  
		Last Modified: Tue, 12 Jan 2021 03:06:06 GMT  
		Size: 6.4 MB (6383239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
