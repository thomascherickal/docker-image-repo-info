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
$ docker pull irssi@sha256:8cd808235b32389f3bdc481a70654f08582189b7eaf51633adda044135312271
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
$ docker pull irssi@sha256:44c777babe5699a8971eb5367dbd411e6eee21e8ed16a4ff7613b037af6f5ceb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76090686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33f1ddb1eb8c8968dc461872fe15016c247b14190fdf74279962255735dca784`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 20:24:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 20:24:47 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 20:24:48 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 20:24:48 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 20:24:48 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 20:25:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 20:25:28 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 20:25:28 GMT
USER user
# Wed, 11 Oct 2023 20:25:28 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3853166e834fc2c48aedc55edbe9e1f882a3d7949f309a967e85dc49845a888c`  
		Last Modified: Wed, 11 Oct 2023 20:26:01 GMT  
		Size: 18.3 MB (18258013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8712f3c7bad7100c6d37fcf7e3c5002d8d7678548bf0892ca23e4904b9c066`  
		Last Modified: Wed, 11 Oct 2023 20:25:57 GMT  
		Size: 3.4 KB (3374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8f213a94fe9accb515298e6053d1ff437041b2b2033156092b5365c7791601`  
		Last Modified: Wed, 11 Oct 2023 20:26:02 GMT  
		Size: 28.7 MB (28679425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm variant v5

```console
$ docker pull irssi@sha256:b49414becae5081d26d6eff6e214ce40e04aecbd6aa5ba63ebfda941497dd5a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70342849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a65606ee0e4cc323ad482840a06d50e1ba7e9d69faf54c5049c7c1fa6332a3f`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:43 GMT
ADD file:8c43adb3245fc6f2b10aa5a86c850db5dcf3515eaf7e46630922fe21f806bd2a in / 
# Wed, 11 Oct 2023 17:37:43 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:00:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:00:56 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 18:00:57 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 18:00:57 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 18:00:57 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 18:01:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 18:01:42 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 18:01:42 GMT
USER user
# Wed, 11 Oct 2023 18:01:42 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:904e6393ef1ee28b37171369eb4f7cb04714631c711799819fccb83886bd212b`  
		Last Modified: Wed, 11 Oct 2023 17:40:47 GMT  
		Size: 26.9 MB (26922150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107efe7ce893352f65dfb345d40ccf416fdb609825df68a2b3f8e02e6a0a3d56`  
		Last Modified: Wed, 11 Oct 2023 18:01:58 GMT  
		Size: 17.1 MB (17092623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317d45cff4b023ded2635c88d1801ee2d5e8911f9a7098ecc25aa7ef5949d566`  
		Last Modified: Wed, 11 Oct 2023 18:01:54 GMT  
		Size: 3.4 KB (3371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be15a5c4dd41a9defc1496cb7afa89616c007835aba62d34d7e38258f865e8e`  
		Last Modified: Wed, 11 Oct 2023 18:01:59 GMT  
		Size: 26.3 MB (26324705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm variant v7

```console
$ docker pull irssi@sha256:9acb53b918ce7218355b74aed1213e71f5126277b32e948808b45ae3424df9ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66653393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0fdfeb17d52fb8aecbbeffe1311c2184bb7fa3da76896c739fd02fe736d719b`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:12:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:12:48 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 19:12:48 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 19:12:48 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 19:12:48 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 19:13:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 19:13:29 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 19:13:29 GMT
USER user
# Wed, 11 Oct 2023 19:13:29 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5baaee56a9498d8e72131adb171dee5671edf350e3f83e1154b2d1651115385`  
		Last Modified: Wed, 11 Oct 2023 19:13:56 GMT  
		Size: 16.7 MB (16678815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ccc912053095badfc35dbd2f166cc2477b07f22b2a8ec2c38183c5c0277873d`  
		Last Modified: Wed, 11 Oct 2023 19:13:52 GMT  
		Size: 3.4 KB (3377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b622859b61c28bc5dbc1cca27e70e2473d2425378c3e3ba112546f6b0d1c70eb`  
		Last Modified: Wed, 11 Oct 2023 19:13:57 GMT  
		Size: 25.2 MB (25222276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:8edaae578605997a74c4364d46c96a3867c2054543a60b2f724913b6a4fa6754
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.8 MB (80788768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f32fcd8186f4b8d4af0b40f507e8f94ea2bfbd86b7fc41276659e2e7ab7ddfe`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:13 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Wed, 20 Sep 2023 02:44:14 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 11:22:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:22:14 GMT
ENV HOME=/home/user
# Wed, 20 Sep 2023 11:22:14 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Sep 2023 11:22:14 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 18:50:25 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 18:51:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 06 Oct 2023 18:51:03 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 18:51:03 GMT
USER user
# Fri, 06 Oct 2023 18:51:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e17a035c22a6860e7c120c60f7d2f84bf9834e6ebdef94bf9b9f044d9c93d69`  
		Last Modified: Wed, 20 Sep 2023 11:23:19 GMT  
		Size: 18.0 MB (18024704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f81b6709eee0366d7cb53c2306da1edae2817e93e99cdd35e7f36aa5e866c8e`  
		Last Modified: Wed, 20 Sep 2023 11:23:16 GMT  
		Size: 3.4 KB (3373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913009f5d7ce3f00561b3220a723826b84895260169d5eb98399e5b5e556cf3f`  
		Last Modified: Fri, 06 Oct 2023 18:51:38 GMT  
		Size: 33.6 MB (33603470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; 386

```console
$ docker pull irssi@sha256:63f96f9a3864f944849735f8de61f7b79f6e0523602340eb8af73f8e2bcca8e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76522799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7838aa7df5bd597e8394793aa77df15853878793a687685bf46ccbd60588a43`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:42 GMT
ADD file:31318c1b1f05d559cce42f5b12eef97d916932217e0b987fb07c0fc11bf0a14a in / 
# Wed, 11 Oct 2023 17:40:42 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:31:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:31:53 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 21:31:54 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 21:31:54 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 21:31:54 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 21:32:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 21:32:48 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 21:32:48 GMT
USER user
# Wed, 11 Oct 2023 21:32:48 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b27d0f1369837277a82877763487cdd2535037988fc27e16f11cf74e103ae4cd`  
		Last Modified: Wed, 11 Oct 2023 17:45:31 GMT  
		Size: 30.2 MB (30164118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5aabddc89a058b8444274e0ab7a7604dd6b19276ca05209051a7bd05996a97`  
		Last Modified: Wed, 11 Oct 2023 21:33:17 GMT  
		Size: 17.8 MB (17788766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674da66b6a6ab4b333d0fbf0c2731e6fcdfc0628ea6463fe2c8c298c2e4f5022`  
		Last Modified: Wed, 11 Oct 2023 21:33:10 GMT  
		Size: 3.4 KB (3373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be398748b24b800d52f805e4b55221b65ab68f63fa172620395b27d97f4cef62`  
		Last Modified: Wed, 11 Oct 2023 21:33:18 GMT  
		Size: 28.6 MB (28566542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; mips64le

```console
$ docker pull irssi@sha256:4622ced3be5a3c4e803c2594eaf6c13299ae0a9f6da133fcac361f6b46a6f62e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73893583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80f80aac1fac6ff7d115cd8d97db39021a1be94a7121a4fe70787e480a3d445f`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:49:32 GMT
ADD file:2abda0a72972a417d4f7f530ca8fa1ee7e85e25d4015fd4e70acf903cfd96d3d in / 
# Wed, 11 Oct 2023 17:49:36 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 20:05:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 20:05:10 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 20:05:16 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 20:05:19 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 20:05:23 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 20:09:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 20:09:27 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 20:09:31 GMT
USER user
# Wed, 11 Oct 2023 20:09:35 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f11870ec99d788b4b160d9f3f4c0a79904290083d8930b26e5d13579226e07f0`  
		Last Modified: Wed, 11 Oct 2023 18:00:43 GMT  
		Size: 29.1 MB (29142026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1f47bc243f41e66258f22f77a6d27afd7c49447f4867ab03737c1c00e055e5`  
		Last Modified: Wed, 11 Oct 2023 20:10:17 GMT  
		Size: 16.7 MB (16741536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528d2b189bddab2a8763fd33d4deba2040b0c2d28337893be13d77d751b745dd`  
		Last Modified: Wed, 11 Oct 2023 20:10:01 GMT  
		Size: 3.3 KB (3299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299c20205b3210d510f4fcb1678d9093fca2d25452b80816b0da15049cbb41d2`  
		Last Modified: Wed, 11 Oct 2023 20:10:22 GMT  
		Size: 28.0 MB (28006722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; ppc64le

```console
$ docker pull irssi@sha256:fe9ad83e93b168870c785b041cfbe670b128f99b8ed3e270c8d50bc9de07c5a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.9 MB (88901114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:132c9d6a4750e943c7033db5a5253d77f49da8681b15cc3af59b0459530997d5`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Sep 2023 07:52:54 GMT
ADD file:9a37b479e68a0d18babbef8dd04d09a0e6844a0080876d14144a34bfd9d0897a in / 
# Wed, 20 Sep 2023 07:52:55 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 11:46:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:46:25 GMT
ENV HOME=/home/user
# Wed, 20 Sep 2023 11:46:27 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Sep 2023 11:46:28 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 20:45:02 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 20:47:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 06 Oct 2023 20:47:27 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 20:47:28 GMT
USER user
# Fri, 06 Oct 2023 20:47:28 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:696a66e961f2033dcf69b003ad7faf28ed2248da58efa1c08a9d496739a8eeeb`  
		Last Modified: Wed, 20 Sep 2023 08:49:51 GMT  
		Size: 33.1 MB (33119461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30054596536297b2e58930c4fe17cb3dd9a484e48310a73810d633fb399b2ea4`  
		Last Modified: Wed, 20 Sep 2023 11:48:21 GMT  
		Size: 18.8 MB (18754188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53547fc5d9551d1c1a1f2ccd6a7125ea312eac162cb9f63b4cf854af65c77212`  
		Last Modified: Wed, 20 Sep 2023 11:48:14 GMT  
		Size: 3.4 KB (3376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c58b6669e0fac3c777f89f1c775613c7c4b79937cdbaa4f03d84f4779088902`  
		Last Modified: Fri, 06 Oct 2023 20:48:39 GMT  
		Size: 37.0 MB (37024089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; s390x

```console
$ docker pull irssi@sha256:adf3bc216988808a8cd8bc19d6474ceae3e63c68d9fb35a403ebc2880dc00605
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.4 MB (80399807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4a91ab3027978ac40b17ec8bcc5ed457b28d8b316732dafa175ccc524171687`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Sep 2023 02:54:26 GMT
ADD file:6ed982ad3e8566d63315a27a81b33069910952aef4b2d3e0b607bd2caeac7ca4 in / 
# Wed, 20 Sep 2023 02:54:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 08:50:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 08:50:11 GMT
ENV HOME=/home/user
# Wed, 20 Sep 2023 08:50:11 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Sep 2023 08:50:12 GMT
ENV LANG=C.UTF-8
# Tue, 10 Oct 2023 02:24:14 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 10 Oct 2023 02:34:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 10 Oct 2023 02:34:37 GMT
WORKDIR /home/user
# Tue, 10 Oct 2023 02:34:37 GMT
USER user
# Tue, 10 Oct 2023 02:34:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:26dcff366e33abcf08b812052a4c12496aa406aa267655e984aa7a84ca254cd8`  
		Last Modified: Wed, 20 Sep 2023 02:59:47 GMT  
		Size: 27.5 MB (27489966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9ab36ca6d32a38244529fb5d1341f679d66a581da57bc1e46bae74a2dac076`  
		Last Modified: Wed, 20 Sep 2023 08:51:27 GMT  
		Size: 18.2 MB (18205945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537016b33e97a91c754da6fb3df713bc111e51fdbd9e9967edfca9572cb96401`  
		Last Modified: Wed, 20 Sep 2023 08:51:24 GMT  
		Size: 3.4 KB (3372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f9e3389f5957a7bcdb6592475907b2611f851e3057e46ba4aa3c7143958e7b`  
		Last Modified: Tue, 10 Oct 2023 02:35:44 GMT  
		Size: 34.7 MB (34700524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1-alpine`

```console
$ docker pull irssi@sha256:38d806b8883cbc7d4ce632aa3b67d6d57415a6de9e8a1e24d78b5fa0dd4eb40c
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
$ docker pull irssi@sha256:1ee6ea9617f00ef85aec02096aeee93e253c1fce4f559a3739175f1412110887
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18840008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a7066a07c9e35db2f3641c82d1b1599ebb7ecfbba2d78659f3093927b81c6f9`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:07:22 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 23:07:22 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 23:07:23 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 23:07:23 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 20:05:43 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 20:06:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 20:06:02 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 20:06:02 GMT
USER user
# Fri, 06 Oct 2023 20:06:02 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af553cbaa1665f3df3ff9ed6df3fc8fdeef915391198875444aee02cb0f1dba`  
		Last Modified: Thu, 28 Sep 2023 23:08:01 GMT  
		Size: 9.6 MB (9638068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475821153744984a56837800be5e45c520da1740ad0e9e56b1a27abb64ab5677`  
		Last Modified: Thu, 28 Sep 2023 23:07:59 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6870b695db89ae46f18ed0a5ea51ba2cb82240d1c5b1c5219a7030798a3f67`  
		Last Modified: Fri, 06 Oct 2023 20:06:47 GMT  
		Size: 5.8 MB (5798688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:7118fc38d54f6deb6a8782357883da4a4cf756bdbfad659c9c1e763250c48d28
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17664781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:012fe6e595cbd84ddedfb4904315ce7f3714991ff90335a481bd48c1252e419c`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:01:23 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:01:24 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:01:24 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:01:24 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 18:54:46 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 18:55:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 18:55:03 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 18:55:03 GMT
USER user
# Fri, 06 Oct 2023 18:55:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:152af5fc5e35a15ab7dff7175a3d682681efedcdd033b4b6ba5e65c50b0ec64f`  
		Last Modified: Thu, 28 Sep 2023 22:01:58 GMT  
		Size: 8.9 MB (8873701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e78ce7c600d11081aaabe6fe5d3d25a6badae1aaa32d490a392cb1c418e0a4`  
		Last Modified: Thu, 28 Sep 2023 22:01:56 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1971284431ad2c2d645075809b4b98b4cf9f9e16ed619f22e95078036b79b731`  
		Last Modified: Fri, 06 Oct 2023 18:55:15 GMT  
		Size: 5.6 MB (5644504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:6553e184e6f2c2417e9f000d0234179c8c8a752d02eb3f2f0b26c675a256fe75
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16994937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0965965700d10cee279de650a20af25276316e23dcc59c4092e271285e7133ed`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:32:29 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 29 Sep 2023 00:32:30 GMT
ENV HOME=/home/user
# Fri, 29 Sep 2023 00:32:30 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 29 Sep 2023 00:32:30 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 19:06:51 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 19:07:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 19:07:06 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 19:07:07 GMT
USER user
# Fri, 06 Oct 2023 19:07:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666541fade74dbbeba8bc1dc2a6f59e496ee2556c1694f8d97e154861211eb4a`  
		Last Modified: Fri, 29 Sep 2023 00:33:18 GMT  
		Size: 8.7 MB (8713773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6786d679f064e76ebc61ea937d53f08e38f578e494b4f72907c4e1886737ccfa`  
		Last Modified: Fri, 29 Sep 2023 00:33:15 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c623f5de44c876517872695b3ea33e2cd0afd3becbd2ef6e84b03a5dacef1ef`  
		Last Modified: Fri, 06 Oct 2023 19:07:49 GMT  
		Size: 5.4 MB (5379973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:8e84ebd4f06676afeeff5d3df76c54b494e9225ad08af34c22405bbb1dfac624
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18715109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4acd348d9659d9e55521ba8e049504b24acb95e989e3c60ef45ce22819d3201c`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:57:36 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 21:57:36 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 21:57:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 21:57:36 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 18:51:05 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 18:51:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 18:51:19 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 18:51:19 GMT
USER user
# Fri, 06 Oct 2023 18:51:19 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb98c09201d772cdbd8ebf3b77e3767ba0112bb407e3fa992d4a5e162065862`  
		Last Modified: Thu, 28 Sep 2023 21:58:15 GMT  
		Size: 9.7 MB (9667003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3eb447534379436f487e6d6e2a8bfe8d3f4a55aaf3e65cd8c162ce04b733398`  
		Last Modified: Thu, 28 Sep 2023 21:58:14 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8285f819417a3875bfc576dd902248316d6bc296fa13316b6e8b1a5193ee0005`  
		Last Modified: Fri, 06 Oct 2023 18:51:59 GMT  
		Size: 5.7 MB (5714992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; 386

```console
$ docker pull irssi@sha256:69515832cd89cf3cc8728b14b7d7d45807fdbec718333af24fc6bf5a8278c54e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.9 MB (17949510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db319b5e7991efcb54c8e037e2cf8bf425d3120b5c5db3df57a4340e246f33dc`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:21:39 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:21:39 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:21:40 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:21:40 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 19:04:21 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 19:04:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 19:04:58 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 19:04:58 GMT
USER user
# Fri, 06 Oct 2023 19:04:58 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbc2dcf799f84aca231b4b6ee2ee6a7a58c3d7b06552d33525458178ce175e2`  
		Last Modified: Thu, 28 Sep 2023 22:22:42 GMT  
		Size: 8.9 MB (8896304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651ec124ac1e46e7e92bc912dfd7308d68d99665be7a2f45460942974926a5b1`  
		Last Modified: Thu, 28 Sep 2023 22:22:39 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a9a322c02a4abf355ad95df55379c7b4d60eba24e72dc90494c80090a1b592`  
		Last Modified: Fri, 06 Oct 2023 19:05:47 GMT  
		Size: 5.8 MB (5816163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:ff90811e849a6fab02c5de90bc84e4c443e3f3f0bb00de9e349725aa44244725
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19108084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c796f660963a32e2c420da0b32b935efdc163713b712139b85e90641d5cc03b2`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:30:38 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:30:40 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:30:41 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:30:42 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 20:47:41 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 20:48:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 20:48:10 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 20:48:10 GMT
USER user
# Fri, 06 Oct 2023 20:48:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765c74d616c6113799971e0b6fb6422b9d4f661cf327745b094cf89369df5fd4`  
		Last Modified: Thu, 28 Sep 2023 22:31:32 GMT  
		Size: 9.7 MB (9727392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfad26be399d4cd09dd2d4252d711e7870345b952b27faeb6f911e9ca449205b`  
		Last Modified: Thu, 28 Sep 2023 22:31:28 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a22d5c7ff0996c5ff524bb74b55e5db4d4a6f8d9bf364cea4a9a40c5ac4455d`  
		Last Modified: Fri, 06 Oct 2023 20:49:04 GMT  
		Size: 6.0 MB (6032900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:079255c123c85c24159e85a1eaf32b4e29a6d6a2e5f78f4d91eafa4e8a1678d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19110918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9b0678fe28100c4b753e58afa0b56102e537a694723ae5d01836a4dceeb40a3`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:18:20 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:18:21 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:18:22 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:18:22 GMT
ENV LANG=C.UTF-8
# Tue, 10 Oct 2023 02:34:46 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 10 Oct 2023 02:35:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 10 Oct 2023 02:35:16 GMT
WORKDIR /home/user
# Tue, 10 Oct 2023 02:35:16 GMT
USER user
# Tue, 10 Oct 2023 02:35:16 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91051e7453a3fcb401f58424e77fa5aa5ee6fee0cca8a5a32646f89a65360ce3`  
		Last Modified: Thu, 28 Sep 2023 22:19:09 GMT  
		Size: 10.1 MB (10078961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c731adf381a8e9331a2fea37d34da20a1359a905c7d7ccf7f166f464e39e5b42`  
		Last Modified: Thu, 28 Sep 2023 22:19:07 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adecf7d94f7048c67fd6041522959d98bf86eb9514cc1b44ede5da69ba7925a5`  
		Last Modified: Tue, 10 Oct 2023 02:37:07 GMT  
		Size: 5.8 MB (5815570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1-alpine3.18`

```console
$ docker pull irssi@sha256:38d806b8883cbc7d4ce632aa3b67d6d57415a6de9e8a1e24d78b5fa0dd4eb40c
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
$ docker pull irssi@sha256:1ee6ea9617f00ef85aec02096aeee93e253c1fce4f559a3739175f1412110887
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18840008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a7066a07c9e35db2f3641c82d1b1599ebb7ecfbba2d78659f3093927b81c6f9`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:07:22 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 23:07:22 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 23:07:23 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 23:07:23 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 20:05:43 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 20:06:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 20:06:02 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 20:06:02 GMT
USER user
# Fri, 06 Oct 2023 20:06:02 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af553cbaa1665f3df3ff9ed6df3fc8fdeef915391198875444aee02cb0f1dba`  
		Last Modified: Thu, 28 Sep 2023 23:08:01 GMT  
		Size: 9.6 MB (9638068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475821153744984a56837800be5e45c520da1740ad0e9e56b1a27abb64ab5677`  
		Last Modified: Thu, 28 Sep 2023 23:07:59 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6870b695db89ae46f18ed0a5ea51ba2cb82240d1c5b1c5219a7030798a3f67`  
		Last Modified: Fri, 06 Oct 2023 20:06:47 GMT  
		Size: 5.8 MB (5798688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine3.18` - linux; arm variant v6

```console
$ docker pull irssi@sha256:7118fc38d54f6deb6a8782357883da4a4cf756bdbfad659c9c1e763250c48d28
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17664781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:012fe6e595cbd84ddedfb4904315ce7f3714991ff90335a481bd48c1252e419c`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:01:23 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:01:24 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:01:24 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:01:24 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 18:54:46 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 18:55:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 18:55:03 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 18:55:03 GMT
USER user
# Fri, 06 Oct 2023 18:55:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:152af5fc5e35a15ab7dff7175a3d682681efedcdd033b4b6ba5e65c50b0ec64f`  
		Last Modified: Thu, 28 Sep 2023 22:01:58 GMT  
		Size: 8.9 MB (8873701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e78ce7c600d11081aaabe6fe5d3d25a6badae1aaa32d490a392cb1c418e0a4`  
		Last Modified: Thu, 28 Sep 2023 22:01:56 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1971284431ad2c2d645075809b4b98b4cf9f9e16ed619f22e95078036b79b731`  
		Last Modified: Fri, 06 Oct 2023 18:55:15 GMT  
		Size: 5.6 MB (5644504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine3.18` - linux; arm variant v7

```console
$ docker pull irssi@sha256:6553e184e6f2c2417e9f000d0234179c8c8a752d02eb3f2f0b26c675a256fe75
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16994937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0965965700d10cee279de650a20af25276316e23dcc59c4092e271285e7133ed`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:32:29 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 29 Sep 2023 00:32:30 GMT
ENV HOME=/home/user
# Fri, 29 Sep 2023 00:32:30 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 29 Sep 2023 00:32:30 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 19:06:51 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 19:07:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 19:07:06 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 19:07:07 GMT
USER user
# Fri, 06 Oct 2023 19:07:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666541fade74dbbeba8bc1dc2a6f59e496ee2556c1694f8d97e154861211eb4a`  
		Last Modified: Fri, 29 Sep 2023 00:33:18 GMT  
		Size: 8.7 MB (8713773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6786d679f064e76ebc61ea937d53f08e38f578e494b4f72907c4e1886737ccfa`  
		Last Modified: Fri, 29 Sep 2023 00:33:15 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c623f5de44c876517872695b3ea33e2cd0afd3becbd2ef6e84b03a5dacef1ef`  
		Last Modified: Fri, 06 Oct 2023 19:07:49 GMT  
		Size: 5.4 MB (5379973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:8e84ebd4f06676afeeff5d3df76c54b494e9225ad08af34c22405bbb1dfac624
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18715109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4acd348d9659d9e55521ba8e049504b24acb95e989e3c60ef45ce22819d3201c`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:57:36 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 21:57:36 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 21:57:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 21:57:36 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 18:51:05 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 18:51:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 18:51:19 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 18:51:19 GMT
USER user
# Fri, 06 Oct 2023 18:51:19 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb98c09201d772cdbd8ebf3b77e3767ba0112bb407e3fa992d4a5e162065862`  
		Last Modified: Thu, 28 Sep 2023 21:58:15 GMT  
		Size: 9.7 MB (9667003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3eb447534379436f487e6d6e2a8bfe8d3f4a55aaf3e65cd8c162ce04b733398`  
		Last Modified: Thu, 28 Sep 2023 21:58:14 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8285f819417a3875bfc576dd902248316d6bc296fa13316b6e8b1a5193ee0005`  
		Last Modified: Fri, 06 Oct 2023 18:51:59 GMT  
		Size: 5.7 MB (5714992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine3.18` - linux; 386

```console
$ docker pull irssi@sha256:69515832cd89cf3cc8728b14b7d7d45807fdbec718333af24fc6bf5a8278c54e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.9 MB (17949510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db319b5e7991efcb54c8e037e2cf8bf425d3120b5c5db3df57a4340e246f33dc`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:21:39 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:21:39 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:21:40 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:21:40 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 19:04:21 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 19:04:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 19:04:58 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 19:04:58 GMT
USER user
# Fri, 06 Oct 2023 19:04:58 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbc2dcf799f84aca231b4b6ee2ee6a7a58c3d7b06552d33525458178ce175e2`  
		Last Modified: Thu, 28 Sep 2023 22:22:42 GMT  
		Size: 8.9 MB (8896304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651ec124ac1e46e7e92bc912dfd7308d68d99665be7a2f45460942974926a5b1`  
		Last Modified: Thu, 28 Sep 2023 22:22:39 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a9a322c02a4abf355ad95df55379c7b4d60eba24e72dc90494c80090a1b592`  
		Last Modified: Fri, 06 Oct 2023 19:05:47 GMT  
		Size: 5.8 MB (5816163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine3.18` - linux; ppc64le

```console
$ docker pull irssi@sha256:ff90811e849a6fab02c5de90bc84e4c443e3f3f0bb00de9e349725aa44244725
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19108084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c796f660963a32e2c420da0b32b935efdc163713b712139b85e90641d5cc03b2`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:30:38 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:30:40 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:30:41 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:30:42 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 20:47:41 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 20:48:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 20:48:10 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 20:48:10 GMT
USER user
# Fri, 06 Oct 2023 20:48:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765c74d616c6113799971e0b6fb6422b9d4f661cf327745b094cf89369df5fd4`  
		Last Modified: Thu, 28 Sep 2023 22:31:32 GMT  
		Size: 9.7 MB (9727392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfad26be399d4cd09dd2d4252d711e7870345b952b27faeb6f911e9ca449205b`  
		Last Modified: Thu, 28 Sep 2023 22:31:28 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a22d5c7ff0996c5ff524bb74b55e5db4d4a6f8d9bf364cea4a9a40c5ac4455d`  
		Last Modified: Fri, 06 Oct 2023 20:49:04 GMT  
		Size: 6.0 MB (6032900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine3.18` - linux; s390x

```console
$ docker pull irssi@sha256:079255c123c85c24159e85a1eaf32b4e29a6d6a2e5f78f4d91eafa4e8a1678d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19110918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9b0678fe28100c4b753e58afa0b56102e537a694723ae5d01836a4dceeb40a3`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:18:20 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:18:21 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:18:22 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:18:22 GMT
ENV LANG=C.UTF-8
# Tue, 10 Oct 2023 02:34:46 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 10 Oct 2023 02:35:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 10 Oct 2023 02:35:16 GMT
WORKDIR /home/user
# Tue, 10 Oct 2023 02:35:16 GMT
USER user
# Tue, 10 Oct 2023 02:35:16 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91051e7453a3fcb401f58424e77fa5aa5ee6fee0cca8a5a32646f89a65360ce3`  
		Last Modified: Thu, 28 Sep 2023 22:19:09 GMT  
		Size: 10.1 MB (10078961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c731adf381a8e9331a2fea37d34da20a1359a905c7d7ccf7f166f464e39e5b42`  
		Last Modified: Thu, 28 Sep 2023 22:19:07 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adecf7d94f7048c67fd6041522959d98bf86eb9514cc1b44ede5da69ba7925a5`  
		Last Modified: Tue, 10 Oct 2023 02:37:07 GMT  
		Size: 5.8 MB (5815570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1-bookworm`

```console
$ docker pull irssi@sha256:8cd808235b32389f3bdc481a70654f08582189b7eaf51633adda044135312271
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
$ docker pull irssi@sha256:44c777babe5699a8971eb5367dbd411e6eee21e8ed16a4ff7613b037af6f5ceb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76090686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33f1ddb1eb8c8968dc461872fe15016c247b14190fdf74279962255735dca784`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 20:24:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 20:24:47 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 20:24:48 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 20:24:48 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 20:24:48 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 20:25:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 20:25:28 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 20:25:28 GMT
USER user
# Wed, 11 Oct 2023 20:25:28 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3853166e834fc2c48aedc55edbe9e1f882a3d7949f309a967e85dc49845a888c`  
		Last Modified: Wed, 11 Oct 2023 20:26:01 GMT  
		Size: 18.3 MB (18258013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8712f3c7bad7100c6d37fcf7e3c5002d8d7678548bf0892ca23e4904b9c066`  
		Last Modified: Wed, 11 Oct 2023 20:25:57 GMT  
		Size: 3.4 KB (3374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8f213a94fe9accb515298e6053d1ff437041b2b2033156092b5365c7791601`  
		Last Modified: Wed, 11 Oct 2023 20:26:02 GMT  
		Size: 28.7 MB (28679425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-bookworm` - linux; arm variant v5

```console
$ docker pull irssi@sha256:b49414becae5081d26d6eff6e214ce40e04aecbd6aa5ba63ebfda941497dd5a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70342849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a65606ee0e4cc323ad482840a06d50e1ba7e9d69faf54c5049c7c1fa6332a3f`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:43 GMT
ADD file:8c43adb3245fc6f2b10aa5a86c850db5dcf3515eaf7e46630922fe21f806bd2a in / 
# Wed, 11 Oct 2023 17:37:43 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:00:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:00:56 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 18:00:57 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 18:00:57 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 18:00:57 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 18:01:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 18:01:42 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 18:01:42 GMT
USER user
# Wed, 11 Oct 2023 18:01:42 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:904e6393ef1ee28b37171369eb4f7cb04714631c711799819fccb83886bd212b`  
		Last Modified: Wed, 11 Oct 2023 17:40:47 GMT  
		Size: 26.9 MB (26922150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107efe7ce893352f65dfb345d40ccf416fdb609825df68a2b3f8e02e6a0a3d56`  
		Last Modified: Wed, 11 Oct 2023 18:01:58 GMT  
		Size: 17.1 MB (17092623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317d45cff4b023ded2635c88d1801ee2d5e8911f9a7098ecc25aa7ef5949d566`  
		Last Modified: Wed, 11 Oct 2023 18:01:54 GMT  
		Size: 3.4 KB (3371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be15a5c4dd41a9defc1496cb7afa89616c007835aba62d34d7e38258f865e8e`  
		Last Modified: Wed, 11 Oct 2023 18:01:59 GMT  
		Size: 26.3 MB (26324705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-bookworm` - linux; arm variant v7

```console
$ docker pull irssi@sha256:9acb53b918ce7218355b74aed1213e71f5126277b32e948808b45ae3424df9ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66653393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0fdfeb17d52fb8aecbbeffe1311c2184bb7fa3da76896c739fd02fe736d719b`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:12:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:12:48 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 19:12:48 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 19:12:48 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 19:12:48 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 19:13:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 19:13:29 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 19:13:29 GMT
USER user
# Wed, 11 Oct 2023 19:13:29 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5baaee56a9498d8e72131adb171dee5671edf350e3f83e1154b2d1651115385`  
		Last Modified: Wed, 11 Oct 2023 19:13:56 GMT  
		Size: 16.7 MB (16678815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ccc912053095badfc35dbd2f166cc2477b07f22b2a8ec2c38183c5c0277873d`  
		Last Modified: Wed, 11 Oct 2023 19:13:52 GMT  
		Size: 3.4 KB (3377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b622859b61c28bc5dbc1cca27e70e2473d2425378c3e3ba112546f6b0d1c70eb`  
		Last Modified: Wed, 11 Oct 2023 19:13:57 GMT  
		Size: 25.2 MB (25222276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-bookworm` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:8edaae578605997a74c4364d46c96a3867c2054543a60b2f724913b6a4fa6754
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.8 MB (80788768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f32fcd8186f4b8d4af0b40f507e8f94ea2bfbd86b7fc41276659e2e7ab7ddfe`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:13 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Wed, 20 Sep 2023 02:44:14 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 11:22:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:22:14 GMT
ENV HOME=/home/user
# Wed, 20 Sep 2023 11:22:14 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Sep 2023 11:22:14 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 18:50:25 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 18:51:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 06 Oct 2023 18:51:03 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 18:51:03 GMT
USER user
# Fri, 06 Oct 2023 18:51:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e17a035c22a6860e7c120c60f7d2f84bf9834e6ebdef94bf9b9f044d9c93d69`  
		Last Modified: Wed, 20 Sep 2023 11:23:19 GMT  
		Size: 18.0 MB (18024704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f81b6709eee0366d7cb53c2306da1edae2817e93e99cdd35e7f36aa5e866c8e`  
		Last Modified: Wed, 20 Sep 2023 11:23:16 GMT  
		Size: 3.4 KB (3373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913009f5d7ce3f00561b3220a723826b84895260169d5eb98399e5b5e556cf3f`  
		Last Modified: Fri, 06 Oct 2023 18:51:38 GMT  
		Size: 33.6 MB (33603470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-bookworm` - linux; 386

```console
$ docker pull irssi@sha256:63f96f9a3864f944849735f8de61f7b79f6e0523602340eb8af73f8e2bcca8e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76522799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7838aa7df5bd597e8394793aa77df15853878793a687685bf46ccbd60588a43`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:42 GMT
ADD file:31318c1b1f05d559cce42f5b12eef97d916932217e0b987fb07c0fc11bf0a14a in / 
# Wed, 11 Oct 2023 17:40:42 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:31:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:31:53 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 21:31:54 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 21:31:54 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 21:31:54 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 21:32:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 21:32:48 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 21:32:48 GMT
USER user
# Wed, 11 Oct 2023 21:32:48 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b27d0f1369837277a82877763487cdd2535037988fc27e16f11cf74e103ae4cd`  
		Last Modified: Wed, 11 Oct 2023 17:45:31 GMT  
		Size: 30.2 MB (30164118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5aabddc89a058b8444274e0ab7a7604dd6b19276ca05209051a7bd05996a97`  
		Last Modified: Wed, 11 Oct 2023 21:33:17 GMT  
		Size: 17.8 MB (17788766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674da66b6a6ab4b333d0fbf0c2731e6fcdfc0628ea6463fe2c8c298c2e4f5022`  
		Last Modified: Wed, 11 Oct 2023 21:33:10 GMT  
		Size: 3.4 KB (3373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be398748b24b800d52f805e4b55221b65ab68f63fa172620395b27d97f4cef62`  
		Last Modified: Wed, 11 Oct 2023 21:33:18 GMT  
		Size: 28.6 MB (28566542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-bookworm` - linux; mips64le

```console
$ docker pull irssi@sha256:4622ced3be5a3c4e803c2594eaf6c13299ae0a9f6da133fcac361f6b46a6f62e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73893583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80f80aac1fac6ff7d115cd8d97db39021a1be94a7121a4fe70787e480a3d445f`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:49:32 GMT
ADD file:2abda0a72972a417d4f7f530ca8fa1ee7e85e25d4015fd4e70acf903cfd96d3d in / 
# Wed, 11 Oct 2023 17:49:36 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 20:05:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 20:05:10 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 20:05:16 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 20:05:19 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 20:05:23 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 20:09:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 20:09:27 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 20:09:31 GMT
USER user
# Wed, 11 Oct 2023 20:09:35 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f11870ec99d788b4b160d9f3f4c0a79904290083d8930b26e5d13579226e07f0`  
		Last Modified: Wed, 11 Oct 2023 18:00:43 GMT  
		Size: 29.1 MB (29142026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1f47bc243f41e66258f22f77a6d27afd7c49447f4867ab03737c1c00e055e5`  
		Last Modified: Wed, 11 Oct 2023 20:10:17 GMT  
		Size: 16.7 MB (16741536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528d2b189bddab2a8763fd33d4deba2040b0c2d28337893be13d77d751b745dd`  
		Last Modified: Wed, 11 Oct 2023 20:10:01 GMT  
		Size: 3.3 KB (3299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299c20205b3210d510f4fcb1678d9093fca2d25452b80816b0da15049cbb41d2`  
		Last Modified: Wed, 11 Oct 2023 20:10:22 GMT  
		Size: 28.0 MB (28006722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-bookworm` - linux; ppc64le

```console
$ docker pull irssi@sha256:fe9ad83e93b168870c785b041cfbe670b128f99b8ed3e270c8d50bc9de07c5a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.9 MB (88901114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:132c9d6a4750e943c7033db5a5253d77f49da8681b15cc3af59b0459530997d5`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Sep 2023 07:52:54 GMT
ADD file:9a37b479e68a0d18babbef8dd04d09a0e6844a0080876d14144a34bfd9d0897a in / 
# Wed, 20 Sep 2023 07:52:55 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 11:46:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:46:25 GMT
ENV HOME=/home/user
# Wed, 20 Sep 2023 11:46:27 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Sep 2023 11:46:28 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 20:45:02 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 20:47:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 06 Oct 2023 20:47:27 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 20:47:28 GMT
USER user
# Fri, 06 Oct 2023 20:47:28 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:696a66e961f2033dcf69b003ad7faf28ed2248da58efa1c08a9d496739a8eeeb`  
		Last Modified: Wed, 20 Sep 2023 08:49:51 GMT  
		Size: 33.1 MB (33119461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30054596536297b2e58930c4fe17cb3dd9a484e48310a73810d633fb399b2ea4`  
		Last Modified: Wed, 20 Sep 2023 11:48:21 GMT  
		Size: 18.8 MB (18754188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53547fc5d9551d1c1a1f2ccd6a7125ea312eac162cb9f63b4cf854af65c77212`  
		Last Modified: Wed, 20 Sep 2023 11:48:14 GMT  
		Size: 3.4 KB (3376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c58b6669e0fac3c777f89f1c775613c7c4b79937cdbaa4f03d84f4779088902`  
		Last Modified: Fri, 06 Oct 2023 20:48:39 GMT  
		Size: 37.0 MB (37024089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-bookworm` - linux; s390x

```console
$ docker pull irssi@sha256:adf3bc216988808a8cd8bc19d6474ceae3e63c68d9fb35a403ebc2880dc00605
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.4 MB (80399807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4a91ab3027978ac40b17ec8bcc5ed457b28d8b316732dafa175ccc524171687`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Sep 2023 02:54:26 GMT
ADD file:6ed982ad3e8566d63315a27a81b33069910952aef4b2d3e0b607bd2caeac7ca4 in / 
# Wed, 20 Sep 2023 02:54:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 08:50:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 08:50:11 GMT
ENV HOME=/home/user
# Wed, 20 Sep 2023 08:50:11 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Sep 2023 08:50:12 GMT
ENV LANG=C.UTF-8
# Tue, 10 Oct 2023 02:24:14 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 10 Oct 2023 02:34:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 10 Oct 2023 02:34:37 GMT
WORKDIR /home/user
# Tue, 10 Oct 2023 02:34:37 GMT
USER user
# Tue, 10 Oct 2023 02:34:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:26dcff366e33abcf08b812052a4c12496aa406aa267655e984aa7a84ca254cd8`  
		Last Modified: Wed, 20 Sep 2023 02:59:47 GMT  
		Size: 27.5 MB (27489966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9ab36ca6d32a38244529fb5d1341f679d66a581da57bc1e46bae74a2dac076`  
		Last Modified: Wed, 20 Sep 2023 08:51:27 GMT  
		Size: 18.2 MB (18205945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537016b33e97a91c754da6fb3df713bc111e51fdbd9e9967edfca9572cb96401`  
		Last Modified: Wed, 20 Sep 2023 08:51:24 GMT  
		Size: 3.4 KB (3372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f9e3389f5957a7bcdb6592475907b2611f851e3057e46ba4aa3c7143958e7b`  
		Last Modified: Tue, 10 Oct 2023 02:35:44 GMT  
		Size: 34.7 MB (34700524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4`

```console
$ docker pull irssi@sha256:8cd808235b32389f3bdc481a70654f08582189b7eaf51633adda044135312271
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
$ docker pull irssi@sha256:44c777babe5699a8971eb5367dbd411e6eee21e8ed16a4ff7613b037af6f5ceb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76090686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33f1ddb1eb8c8968dc461872fe15016c247b14190fdf74279962255735dca784`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 20:24:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 20:24:47 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 20:24:48 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 20:24:48 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 20:24:48 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 20:25:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 20:25:28 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 20:25:28 GMT
USER user
# Wed, 11 Oct 2023 20:25:28 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3853166e834fc2c48aedc55edbe9e1f882a3d7949f309a967e85dc49845a888c`  
		Last Modified: Wed, 11 Oct 2023 20:26:01 GMT  
		Size: 18.3 MB (18258013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8712f3c7bad7100c6d37fcf7e3c5002d8d7678548bf0892ca23e4904b9c066`  
		Last Modified: Wed, 11 Oct 2023 20:25:57 GMT  
		Size: 3.4 KB (3374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8f213a94fe9accb515298e6053d1ff437041b2b2033156092b5365c7791601`  
		Last Modified: Wed, 11 Oct 2023 20:26:02 GMT  
		Size: 28.7 MB (28679425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; arm variant v5

```console
$ docker pull irssi@sha256:b49414becae5081d26d6eff6e214ce40e04aecbd6aa5ba63ebfda941497dd5a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70342849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a65606ee0e4cc323ad482840a06d50e1ba7e9d69faf54c5049c7c1fa6332a3f`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:43 GMT
ADD file:8c43adb3245fc6f2b10aa5a86c850db5dcf3515eaf7e46630922fe21f806bd2a in / 
# Wed, 11 Oct 2023 17:37:43 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:00:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:00:56 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 18:00:57 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 18:00:57 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 18:00:57 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 18:01:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 18:01:42 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 18:01:42 GMT
USER user
# Wed, 11 Oct 2023 18:01:42 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:904e6393ef1ee28b37171369eb4f7cb04714631c711799819fccb83886bd212b`  
		Last Modified: Wed, 11 Oct 2023 17:40:47 GMT  
		Size: 26.9 MB (26922150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107efe7ce893352f65dfb345d40ccf416fdb609825df68a2b3f8e02e6a0a3d56`  
		Last Modified: Wed, 11 Oct 2023 18:01:58 GMT  
		Size: 17.1 MB (17092623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317d45cff4b023ded2635c88d1801ee2d5e8911f9a7098ecc25aa7ef5949d566`  
		Last Modified: Wed, 11 Oct 2023 18:01:54 GMT  
		Size: 3.4 KB (3371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be15a5c4dd41a9defc1496cb7afa89616c007835aba62d34d7e38258f865e8e`  
		Last Modified: Wed, 11 Oct 2023 18:01:59 GMT  
		Size: 26.3 MB (26324705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; arm variant v7

```console
$ docker pull irssi@sha256:9acb53b918ce7218355b74aed1213e71f5126277b32e948808b45ae3424df9ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66653393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0fdfeb17d52fb8aecbbeffe1311c2184bb7fa3da76896c739fd02fe736d719b`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:12:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:12:48 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 19:12:48 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 19:12:48 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 19:12:48 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 19:13:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 19:13:29 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 19:13:29 GMT
USER user
# Wed, 11 Oct 2023 19:13:29 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5baaee56a9498d8e72131adb171dee5671edf350e3f83e1154b2d1651115385`  
		Last Modified: Wed, 11 Oct 2023 19:13:56 GMT  
		Size: 16.7 MB (16678815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ccc912053095badfc35dbd2f166cc2477b07f22b2a8ec2c38183c5c0277873d`  
		Last Modified: Wed, 11 Oct 2023 19:13:52 GMT  
		Size: 3.4 KB (3377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b622859b61c28bc5dbc1cca27e70e2473d2425378c3e3ba112546f6b0d1c70eb`  
		Last Modified: Wed, 11 Oct 2023 19:13:57 GMT  
		Size: 25.2 MB (25222276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:8edaae578605997a74c4364d46c96a3867c2054543a60b2f724913b6a4fa6754
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.8 MB (80788768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f32fcd8186f4b8d4af0b40f507e8f94ea2bfbd86b7fc41276659e2e7ab7ddfe`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:13 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Wed, 20 Sep 2023 02:44:14 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 11:22:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:22:14 GMT
ENV HOME=/home/user
# Wed, 20 Sep 2023 11:22:14 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Sep 2023 11:22:14 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 18:50:25 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 18:51:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 06 Oct 2023 18:51:03 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 18:51:03 GMT
USER user
# Fri, 06 Oct 2023 18:51:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e17a035c22a6860e7c120c60f7d2f84bf9834e6ebdef94bf9b9f044d9c93d69`  
		Last Modified: Wed, 20 Sep 2023 11:23:19 GMT  
		Size: 18.0 MB (18024704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f81b6709eee0366d7cb53c2306da1edae2817e93e99cdd35e7f36aa5e866c8e`  
		Last Modified: Wed, 20 Sep 2023 11:23:16 GMT  
		Size: 3.4 KB (3373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913009f5d7ce3f00561b3220a723826b84895260169d5eb98399e5b5e556cf3f`  
		Last Modified: Fri, 06 Oct 2023 18:51:38 GMT  
		Size: 33.6 MB (33603470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; 386

```console
$ docker pull irssi@sha256:63f96f9a3864f944849735f8de61f7b79f6e0523602340eb8af73f8e2bcca8e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76522799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7838aa7df5bd597e8394793aa77df15853878793a687685bf46ccbd60588a43`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:42 GMT
ADD file:31318c1b1f05d559cce42f5b12eef97d916932217e0b987fb07c0fc11bf0a14a in / 
# Wed, 11 Oct 2023 17:40:42 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:31:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:31:53 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 21:31:54 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 21:31:54 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 21:31:54 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 21:32:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 21:32:48 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 21:32:48 GMT
USER user
# Wed, 11 Oct 2023 21:32:48 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b27d0f1369837277a82877763487cdd2535037988fc27e16f11cf74e103ae4cd`  
		Last Modified: Wed, 11 Oct 2023 17:45:31 GMT  
		Size: 30.2 MB (30164118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5aabddc89a058b8444274e0ab7a7604dd6b19276ca05209051a7bd05996a97`  
		Last Modified: Wed, 11 Oct 2023 21:33:17 GMT  
		Size: 17.8 MB (17788766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674da66b6a6ab4b333d0fbf0c2731e6fcdfc0628ea6463fe2c8c298c2e4f5022`  
		Last Modified: Wed, 11 Oct 2023 21:33:10 GMT  
		Size: 3.4 KB (3373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be398748b24b800d52f805e4b55221b65ab68f63fa172620395b27d97f4cef62`  
		Last Modified: Wed, 11 Oct 2023 21:33:18 GMT  
		Size: 28.6 MB (28566542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; mips64le

```console
$ docker pull irssi@sha256:4622ced3be5a3c4e803c2594eaf6c13299ae0a9f6da133fcac361f6b46a6f62e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73893583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80f80aac1fac6ff7d115cd8d97db39021a1be94a7121a4fe70787e480a3d445f`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:49:32 GMT
ADD file:2abda0a72972a417d4f7f530ca8fa1ee7e85e25d4015fd4e70acf903cfd96d3d in / 
# Wed, 11 Oct 2023 17:49:36 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 20:05:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 20:05:10 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 20:05:16 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 20:05:19 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 20:05:23 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 20:09:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 20:09:27 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 20:09:31 GMT
USER user
# Wed, 11 Oct 2023 20:09:35 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f11870ec99d788b4b160d9f3f4c0a79904290083d8930b26e5d13579226e07f0`  
		Last Modified: Wed, 11 Oct 2023 18:00:43 GMT  
		Size: 29.1 MB (29142026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1f47bc243f41e66258f22f77a6d27afd7c49447f4867ab03737c1c00e055e5`  
		Last Modified: Wed, 11 Oct 2023 20:10:17 GMT  
		Size: 16.7 MB (16741536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528d2b189bddab2a8763fd33d4deba2040b0c2d28337893be13d77d751b745dd`  
		Last Modified: Wed, 11 Oct 2023 20:10:01 GMT  
		Size: 3.3 KB (3299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299c20205b3210d510f4fcb1678d9093fca2d25452b80816b0da15049cbb41d2`  
		Last Modified: Wed, 11 Oct 2023 20:10:22 GMT  
		Size: 28.0 MB (28006722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; ppc64le

```console
$ docker pull irssi@sha256:fe9ad83e93b168870c785b041cfbe670b128f99b8ed3e270c8d50bc9de07c5a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.9 MB (88901114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:132c9d6a4750e943c7033db5a5253d77f49da8681b15cc3af59b0459530997d5`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Sep 2023 07:52:54 GMT
ADD file:9a37b479e68a0d18babbef8dd04d09a0e6844a0080876d14144a34bfd9d0897a in / 
# Wed, 20 Sep 2023 07:52:55 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 11:46:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:46:25 GMT
ENV HOME=/home/user
# Wed, 20 Sep 2023 11:46:27 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Sep 2023 11:46:28 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 20:45:02 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 20:47:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 06 Oct 2023 20:47:27 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 20:47:28 GMT
USER user
# Fri, 06 Oct 2023 20:47:28 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:696a66e961f2033dcf69b003ad7faf28ed2248da58efa1c08a9d496739a8eeeb`  
		Last Modified: Wed, 20 Sep 2023 08:49:51 GMT  
		Size: 33.1 MB (33119461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30054596536297b2e58930c4fe17cb3dd9a484e48310a73810d633fb399b2ea4`  
		Last Modified: Wed, 20 Sep 2023 11:48:21 GMT  
		Size: 18.8 MB (18754188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53547fc5d9551d1c1a1f2ccd6a7125ea312eac162cb9f63b4cf854af65c77212`  
		Last Modified: Wed, 20 Sep 2023 11:48:14 GMT  
		Size: 3.4 KB (3376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c58b6669e0fac3c777f89f1c775613c7c4b79937cdbaa4f03d84f4779088902`  
		Last Modified: Fri, 06 Oct 2023 20:48:39 GMT  
		Size: 37.0 MB (37024089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; s390x

```console
$ docker pull irssi@sha256:adf3bc216988808a8cd8bc19d6474ceae3e63c68d9fb35a403ebc2880dc00605
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.4 MB (80399807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4a91ab3027978ac40b17ec8bcc5ed457b28d8b316732dafa175ccc524171687`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Sep 2023 02:54:26 GMT
ADD file:6ed982ad3e8566d63315a27a81b33069910952aef4b2d3e0b607bd2caeac7ca4 in / 
# Wed, 20 Sep 2023 02:54:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 08:50:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 08:50:11 GMT
ENV HOME=/home/user
# Wed, 20 Sep 2023 08:50:11 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Sep 2023 08:50:12 GMT
ENV LANG=C.UTF-8
# Tue, 10 Oct 2023 02:24:14 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 10 Oct 2023 02:34:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 10 Oct 2023 02:34:37 GMT
WORKDIR /home/user
# Tue, 10 Oct 2023 02:34:37 GMT
USER user
# Tue, 10 Oct 2023 02:34:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:26dcff366e33abcf08b812052a4c12496aa406aa267655e984aa7a84ca254cd8`  
		Last Modified: Wed, 20 Sep 2023 02:59:47 GMT  
		Size: 27.5 MB (27489966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9ab36ca6d32a38244529fb5d1341f679d66a581da57bc1e46bae74a2dac076`  
		Last Modified: Wed, 20 Sep 2023 08:51:27 GMT  
		Size: 18.2 MB (18205945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537016b33e97a91c754da6fb3df713bc111e51fdbd9e9967edfca9572cb96401`  
		Last Modified: Wed, 20 Sep 2023 08:51:24 GMT  
		Size: 3.4 KB (3372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f9e3389f5957a7bcdb6592475907b2611f851e3057e46ba4aa3c7143958e7b`  
		Last Modified: Tue, 10 Oct 2023 02:35:44 GMT  
		Size: 34.7 MB (34700524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4-alpine`

```console
$ docker pull irssi@sha256:38d806b8883cbc7d4ce632aa3b67d6d57415a6de9e8a1e24d78b5fa0dd4eb40c
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
$ docker pull irssi@sha256:1ee6ea9617f00ef85aec02096aeee93e253c1fce4f559a3739175f1412110887
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18840008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a7066a07c9e35db2f3641c82d1b1599ebb7ecfbba2d78659f3093927b81c6f9`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:07:22 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 23:07:22 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 23:07:23 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 23:07:23 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 20:05:43 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 20:06:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 20:06:02 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 20:06:02 GMT
USER user
# Fri, 06 Oct 2023 20:06:02 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af553cbaa1665f3df3ff9ed6df3fc8fdeef915391198875444aee02cb0f1dba`  
		Last Modified: Thu, 28 Sep 2023 23:08:01 GMT  
		Size: 9.6 MB (9638068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475821153744984a56837800be5e45c520da1740ad0e9e56b1a27abb64ab5677`  
		Last Modified: Thu, 28 Sep 2023 23:07:59 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6870b695db89ae46f18ed0a5ea51ba2cb82240d1c5b1c5219a7030798a3f67`  
		Last Modified: Fri, 06 Oct 2023 20:06:47 GMT  
		Size: 5.8 MB (5798688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:7118fc38d54f6deb6a8782357883da4a4cf756bdbfad659c9c1e763250c48d28
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17664781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:012fe6e595cbd84ddedfb4904315ce7f3714991ff90335a481bd48c1252e419c`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:01:23 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:01:24 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:01:24 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:01:24 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 18:54:46 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 18:55:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 18:55:03 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 18:55:03 GMT
USER user
# Fri, 06 Oct 2023 18:55:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:152af5fc5e35a15ab7dff7175a3d682681efedcdd033b4b6ba5e65c50b0ec64f`  
		Last Modified: Thu, 28 Sep 2023 22:01:58 GMT  
		Size: 8.9 MB (8873701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e78ce7c600d11081aaabe6fe5d3d25a6badae1aaa32d490a392cb1c418e0a4`  
		Last Modified: Thu, 28 Sep 2023 22:01:56 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1971284431ad2c2d645075809b4b98b4cf9f9e16ed619f22e95078036b79b731`  
		Last Modified: Fri, 06 Oct 2023 18:55:15 GMT  
		Size: 5.6 MB (5644504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:6553e184e6f2c2417e9f000d0234179c8c8a752d02eb3f2f0b26c675a256fe75
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16994937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0965965700d10cee279de650a20af25276316e23dcc59c4092e271285e7133ed`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:32:29 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 29 Sep 2023 00:32:30 GMT
ENV HOME=/home/user
# Fri, 29 Sep 2023 00:32:30 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 29 Sep 2023 00:32:30 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 19:06:51 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 19:07:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 19:07:06 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 19:07:07 GMT
USER user
# Fri, 06 Oct 2023 19:07:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666541fade74dbbeba8bc1dc2a6f59e496ee2556c1694f8d97e154861211eb4a`  
		Last Modified: Fri, 29 Sep 2023 00:33:18 GMT  
		Size: 8.7 MB (8713773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6786d679f064e76ebc61ea937d53f08e38f578e494b4f72907c4e1886737ccfa`  
		Last Modified: Fri, 29 Sep 2023 00:33:15 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c623f5de44c876517872695b3ea33e2cd0afd3becbd2ef6e84b03a5dacef1ef`  
		Last Modified: Fri, 06 Oct 2023 19:07:49 GMT  
		Size: 5.4 MB (5379973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:8e84ebd4f06676afeeff5d3df76c54b494e9225ad08af34c22405bbb1dfac624
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18715109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4acd348d9659d9e55521ba8e049504b24acb95e989e3c60ef45ce22819d3201c`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:57:36 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 21:57:36 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 21:57:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 21:57:36 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 18:51:05 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 18:51:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 18:51:19 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 18:51:19 GMT
USER user
# Fri, 06 Oct 2023 18:51:19 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb98c09201d772cdbd8ebf3b77e3767ba0112bb407e3fa992d4a5e162065862`  
		Last Modified: Thu, 28 Sep 2023 21:58:15 GMT  
		Size: 9.7 MB (9667003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3eb447534379436f487e6d6e2a8bfe8d3f4a55aaf3e65cd8c162ce04b733398`  
		Last Modified: Thu, 28 Sep 2023 21:58:14 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8285f819417a3875bfc576dd902248316d6bc296fa13316b6e8b1a5193ee0005`  
		Last Modified: Fri, 06 Oct 2023 18:51:59 GMT  
		Size: 5.7 MB (5714992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine` - linux; 386

```console
$ docker pull irssi@sha256:69515832cd89cf3cc8728b14b7d7d45807fdbec718333af24fc6bf5a8278c54e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.9 MB (17949510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db319b5e7991efcb54c8e037e2cf8bf425d3120b5c5db3df57a4340e246f33dc`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:21:39 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:21:39 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:21:40 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:21:40 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 19:04:21 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 19:04:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 19:04:58 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 19:04:58 GMT
USER user
# Fri, 06 Oct 2023 19:04:58 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbc2dcf799f84aca231b4b6ee2ee6a7a58c3d7b06552d33525458178ce175e2`  
		Last Modified: Thu, 28 Sep 2023 22:22:42 GMT  
		Size: 8.9 MB (8896304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651ec124ac1e46e7e92bc912dfd7308d68d99665be7a2f45460942974926a5b1`  
		Last Modified: Thu, 28 Sep 2023 22:22:39 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a9a322c02a4abf355ad95df55379c7b4d60eba24e72dc90494c80090a1b592`  
		Last Modified: Fri, 06 Oct 2023 19:05:47 GMT  
		Size: 5.8 MB (5816163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:ff90811e849a6fab02c5de90bc84e4c443e3f3f0bb00de9e349725aa44244725
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19108084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c796f660963a32e2c420da0b32b935efdc163713b712139b85e90641d5cc03b2`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:30:38 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:30:40 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:30:41 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:30:42 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 20:47:41 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 20:48:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 20:48:10 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 20:48:10 GMT
USER user
# Fri, 06 Oct 2023 20:48:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765c74d616c6113799971e0b6fb6422b9d4f661cf327745b094cf89369df5fd4`  
		Last Modified: Thu, 28 Sep 2023 22:31:32 GMT  
		Size: 9.7 MB (9727392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfad26be399d4cd09dd2d4252d711e7870345b952b27faeb6f911e9ca449205b`  
		Last Modified: Thu, 28 Sep 2023 22:31:28 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a22d5c7ff0996c5ff524bb74b55e5db4d4a6f8d9bf364cea4a9a40c5ac4455d`  
		Last Modified: Fri, 06 Oct 2023 20:49:04 GMT  
		Size: 6.0 MB (6032900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:079255c123c85c24159e85a1eaf32b4e29a6d6a2e5f78f4d91eafa4e8a1678d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19110918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9b0678fe28100c4b753e58afa0b56102e537a694723ae5d01836a4dceeb40a3`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:18:20 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:18:21 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:18:22 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:18:22 GMT
ENV LANG=C.UTF-8
# Tue, 10 Oct 2023 02:34:46 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 10 Oct 2023 02:35:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 10 Oct 2023 02:35:16 GMT
WORKDIR /home/user
# Tue, 10 Oct 2023 02:35:16 GMT
USER user
# Tue, 10 Oct 2023 02:35:16 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91051e7453a3fcb401f58424e77fa5aa5ee6fee0cca8a5a32646f89a65360ce3`  
		Last Modified: Thu, 28 Sep 2023 22:19:09 GMT  
		Size: 10.1 MB (10078961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c731adf381a8e9331a2fea37d34da20a1359a905c7d7ccf7f166f464e39e5b42`  
		Last Modified: Thu, 28 Sep 2023 22:19:07 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adecf7d94f7048c67fd6041522959d98bf86eb9514cc1b44ede5da69ba7925a5`  
		Last Modified: Tue, 10 Oct 2023 02:37:07 GMT  
		Size: 5.8 MB (5815570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4-alpine3.18`

```console
$ docker pull irssi@sha256:38d806b8883cbc7d4ce632aa3b67d6d57415a6de9e8a1e24d78b5fa0dd4eb40c
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
$ docker pull irssi@sha256:1ee6ea9617f00ef85aec02096aeee93e253c1fce4f559a3739175f1412110887
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18840008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a7066a07c9e35db2f3641c82d1b1599ebb7ecfbba2d78659f3093927b81c6f9`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:07:22 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 23:07:22 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 23:07:23 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 23:07:23 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 20:05:43 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 20:06:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 20:06:02 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 20:06:02 GMT
USER user
# Fri, 06 Oct 2023 20:06:02 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af553cbaa1665f3df3ff9ed6df3fc8fdeef915391198875444aee02cb0f1dba`  
		Last Modified: Thu, 28 Sep 2023 23:08:01 GMT  
		Size: 9.6 MB (9638068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475821153744984a56837800be5e45c520da1740ad0e9e56b1a27abb64ab5677`  
		Last Modified: Thu, 28 Sep 2023 23:07:59 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6870b695db89ae46f18ed0a5ea51ba2cb82240d1c5b1c5219a7030798a3f67`  
		Last Modified: Fri, 06 Oct 2023 20:06:47 GMT  
		Size: 5.8 MB (5798688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine3.18` - linux; arm variant v6

```console
$ docker pull irssi@sha256:7118fc38d54f6deb6a8782357883da4a4cf756bdbfad659c9c1e763250c48d28
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17664781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:012fe6e595cbd84ddedfb4904315ce7f3714991ff90335a481bd48c1252e419c`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:01:23 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:01:24 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:01:24 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:01:24 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 18:54:46 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 18:55:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 18:55:03 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 18:55:03 GMT
USER user
# Fri, 06 Oct 2023 18:55:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:152af5fc5e35a15ab7dff7175a3d682681efedcdd033b4b6ba5e65c50b0ec64f`  
		Last Modified: Thu, 28 Sep 2023 22:01:58 GMT  
		Size: 8.9 MB (8873701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e78ce7c600d11081aaabe6fe5d3d25a6badae1aaa32d490a392cb1c418e0a4`  
		Last Modified: Thu, 28 Sep 2023 22:01:56 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1971284431ad2c2d645075809b4b98b4cf9f9e16ed619f22e95078036b79b731`  
		Last Modified: Fri, 06 Oct 2023 18:55:15 GMT  
		Size: 5.6 MB (5644504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine3.18` - linux; arm variant v7

```console
$ docker pull irssi@sha256:6553e184e6f2c2417e9f000d0234179c8c8a752d02eb3f2f0b26c675a256fe75
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16994937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0965965700d10cee279de650a20af25276316e23dcc59c4092e271285e7133ed`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:32:29 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 29 Sep 2023 00:32:30 GMT
ENV HOME=/home/user
# Fri, 29 Sep 2023 00:32:30 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 29 Sep 2023 00:32:30 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 19:06:51 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 19:07:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 19:07:06 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 19:07:07 GMT
USER user
# Fri, 06 Oct 2023 19:07:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666541fade74dbbeba8bc1dc2a6f59e496ee2556c1694f8d97e154861211eb4a`  
		Last Modified: Fri, 29 Sep 2023 00:33:18 GMT  
		Size: 8.7 MB (8713773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6786d679f064e76ebc61ea937d53f08e38f578e494b4f72907c4e1886737ccfa`  
		Last Modified: Fri, 29 Sep 2023 00:33:15 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c623f5de44c876517872695b3ea33e2cd0afd3becbd2ef6e84b03a5dacef1ef`  
		Last Modified: Fri, 06 Oct 2023 19:07:49 GMT  
		Size: 5.4 MB (5379973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:8e84ebd4f06676afeeff5d3df76c54b494e9225ad08af34c22405bbb1dfac624
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18715109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4acd348d9659d9e55521ba8e049504b24acb95e989e3c60ef45ce22819d3201c`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:57:36 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 21:57:36 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 21:57:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 21:57:36 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 18:51:05 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 18:51:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 18:51:19 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 18:51:19 GMT
USER user
# Fri, 06 Oct 2023 18:51:19 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb98c09201d772cdbd8ebf3b77e3767ba0112bb407e3fa992d4a5e162065862`  
		Last Modified: Thu, 28 Sep 2023 21:58:15 GMT  
		Size: 9.7 MB (9667003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3eb447534379436f487e6d6e2a8bfe8d3f4a55aaf3e65cd8c162ce04b733398`  
		Last Modified: Thu, 28 Sep 2023 21:58:14 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8285f819417a3875bfc576dd902248316d6bc296fa13316b6e8b1a5193ee0005`  
		Last Modified: Fri, 06 Oct 2023 18:51:59 GMT  
		Size: 5.7 MB (5714992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine3.18` - linux; 386

```console
$ docker pull irssi@sha256:69515832cd89cf3cc8728b14b7d7d45807fdbec718333af24fc6bf5a8278c54e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.9 MB (17949510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db319b5e7991efcb54c8e037e2cf8bf425d3120b5c5db3df57a4340e246f33dc`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:21:39 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:21:39 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:21:40 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:21:40 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 19:04:21 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 19:04:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 19:04:58 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 19:04:58 GMT
USER user
# Fri, 06 Oct 2023 19:04:58 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbc2dcf799f84aca231b4b6ee2ee6a7a58c3d7b06552d33525458178ce175e2`  
		Last Modified: Thu, 28 Sep 2023 22:22:42 GMT  
		Size: 8.9 MB (8896304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651ec124ac1e46e7e92bc912dfd7308d68d99665be7a2f45460942974926a5b1`  
		Last Modified: Thu, 28 Sep 2023 22:22:39 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a9a322c02a4abf355ad95df55379c7b4d60eba24e72dc90494c80090a1b592`  
		Last Modified: Fri, 06 Oct 2023 19:05:47 GMT  
		Size: 5.8 MB (5816163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine3.18` - linux; ppc64le

```console
$ docker pull irssi@sha256:ff90811e849a6fab02c5de90bc84e4c443e3f3f0bb00de9e349725aa44244725
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19108084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c796f660963a32e2c420da0b32b935efdc163713b712139b85e90641d5cc03b2`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:30:38 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:30:40 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:30:41 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:30:42 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 20:47:41 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 20:48:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 20:48:10 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 20:48:10 GMT
USER user
# Fri, 06 Oct 2023 20:48:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765c74d616c6113799971e0b6fb6422b9d4f661cf327745b094cf89369df5fd4`  
		Last Modified: Thu, 28 Sep 2023 22:31:32 GMT  
		Size: 9.7 MB (9727392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfad26be399d4cd09dd2d4252d711e7870345b952b27faeb6f911e9ca449205b`  
		Last Modified: Thu, 28 Sep 2023 22:31:28 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a22d5c7ff0996c5ff524bb74b55e5db4d4a6f8d9bf364cea4a9a40c5ac4455d`  
		Last Modified: Fri, 06 Oct 2023 20:49:04 GMT  
		Size: 6.0 MB (6032900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine3.18` - linux; s390x

```console
$ docker pull irssi@sha256:079255c123c85c24159e85a1eaf32b4e29a6d6a2e5f78f4d91eafa4e8a1678d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19110918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9b0678fe28100c4b753e58afa0b56102e537a694723ae5d01836a4dceeb40a3`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:18:20 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:18:21 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:18:22 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:18:22 GMT
ENV LANG=C.UTF-8
# Tue, 10 Oct 2023 02:34:46 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 10 Oct 2023 02:35:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 10 Oct 2023 02:35:16 GMT
WORKDIR /home/user
# Tue, 10 Oct 2023 02:35:16 GMT
USER user
# Tue, 10 Oct 2023 02:35:16 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91051e7453a3fcb401f58424e77fa5aa5ee6fee0cca8a5a32646f89a65360ce3`  
		Last Modified: Thu, 28 Sep 2023 22:19:09 GMT  
		Size: 10.1 MB (10078961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c731adf381a8e9331a2fea37d34da20a1359a905c7d7ccf7f166f464e39e5b42`  
		Last Modified: Thu, 28 Sep 2023 22:19:07 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adecf7d94f7048c67fd6041522959d98bf86eb9514cc1b44ede5da69ba7925a5`  
		Last Modified: Tue, 10 Oct 2023 02:37:07 GMT  
		Size: 5.8 MB (5815570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4-bookworm`

```console
$ docker pull irssi@sha256:8cd808235b32389f3bdc481a70654f08582189b7eaf51633adda044135312271
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
$ docker pull irssi@sha256:44c777babe5699a8971eb5367dbd411e6eee21e8ed16a4ff7613b037af6f5ceb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76090686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33f1ddb1eb8c8968dc461872fe15016c247b14190fdf74279962255735dca784`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 20:24:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 20:24:47 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 20:24:48 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 20:24:48 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 20:24:48 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 20:25:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 20:25:28 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 20:25:28 GMT
USER user
# Wed, 11 Oct 2023 20:25:28 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3853166e834fc2c48aedc55edbe9e1f882a3d7949f309a967e85dc49845a888c`  
		Last Modified: Wed, 11 Oct 2023 20:26:01 GMT  
		Size: 18.3 MB (18258013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8712f3c7bad7100c6d37fcf7e3c5002d8d7678548bf0892ca23e4904b9c066`  
		Last Modified: Wed, 11 Oct 2023 20:25:57 GMT  
		Size: 3.4 KB (3374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8f213a94fe9accb515298e6053d1ff437041b2b2033156092b5365c7791601`  
		Last Modified: Wed, 11 Oct 2023 20:26:02 GMT  
		Size: 28.7 MB (28679425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-bookworm` - linux; arm variant v5

```console
$ docker pull irssi@sha256:b49414becae5081d26d6eff6e214ce40e04aecbd6aa5ba63ebfda941497dd5a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70342849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a65606ee0e4cc323ad482840a06d50e1ba7e9d69faf54c5049c7c1fa6332a3f`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:43 GMT
ADD file:8c43adb3245fc6f2b10aa5a86c850db5dcf3515eaf7e46630922fe21f806bd2a in / 
# Wed, 11 Oct 2023 17:37:43 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:00:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:00:56 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 18:00:57 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 18:00:57 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 18:00:57 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 18:01:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 18:01:42 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 18:01:42 GMT
USER user
# Wed, 11 Oct 2023 18:01:42 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:904e6393ef1ee28b37171369eb4f7cb04714631c711799819fccb83886bd212b`  
		Last Modified: Wed, 11 Oct 2023 17:40:47 GMT  
		Size: 26.9 MB (26922150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107efe7ce893352f65dfb345d40ccf416fdb609825df68a2b3f8e02e6a0a3d56`  
		Last Modified: Wed, 11 Oct 2023 18:01:58 GMT  
		Size: 17.1 MB (17092623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317d45cff4b023ded2635c88d1801ee2d5e8911f9a7098ecc25aa7ef5949d566`  
		Last Modified: Wed, 11 Oct 2023 18:01:54 GMT  
		Size: 3.4 KB (3371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be15a5c4dd41a9defc1496cb7afa89616c007835aba62d34d7e38258f865e8e`  
		Last Modified: Wed, 11 Oct 2023 18:01:59 GMT  
		Size: 26.3 MB (26324705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-bookworm` - linux; arm variant v7

```console
$ docker pull irssi@sha256:9acb53b918ce7218355b74aed1213e71f5126277b32e948808b45ae3424df9ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66653393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0fdfeb17d52fb8aecbbeffe1311c2184bb7fa3da76896c739fd02fe736d719b`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:12:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:12:48 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 19:12:48 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 19:12:48 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 19:12:48 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 19:13:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 19:13:29 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 19:13:29 GMT
USER user
# Wed, 11 Oct 2023 19:13:29 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5baaee56a9498d8e72131adb171dee5671edf350e3f83e1154b2d1651115385`  
		Last Modified: Wed, 11 Oct 2023 19:13:56 GMT  
		Size: 16.7 MB (16678815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ccc912053095badfc35dbd2f166cc2477b07f22b2a8ec2c38183c5c0277873d`  
		Last Modified: Wed, 11 Oct 2023 19:13:52 GMT  
		Size: 3.4 KB (3377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b622859b61c28bc5dbc1cca27e70e2473d2425378c3e3ba112546f6b0d1c70eb`  
		Last Modified: Wed, 11 Oct 2023 19:13:57 GMT  
		Size: 25.2 MB (25222276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-bookworm` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:8edaae578605997a74c4364d46c96a3867c2054543a60b2f724913b6a4fa6754
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.8 MB (80788768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f32fcd8186f4b8d4af0b40f507e8f94ea2bfbd86b7fc41276659e2e7ab7ddfe`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:13 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Wed, 20 Sep 2023 02:44:14 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 11:22:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:22:14 GMT
ENV HOME=/home/user
# Wed, 20 Sep 2023 11:22:14 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Sep 2023 11:22:14 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 18:50:25 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 18:51:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 06 Oct 2023 18:51:03 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 18:51:03 GMT
USER user
# Fri, 06 Oct 2023 18:51:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e17a035c22a6860e7c120c60f7d2f84bf9834e6ebdef94bf9b9f044d9c93d69`  
		Last Modified: Wed, 20 Sep 2023 11:23:19 GMT  
		Size: 18.0 MB (18024704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f81b6709eee0366d7cb53c2306da1edae2817e93e99cdd35e7f36aa5e866c8e`  
		Last Modified: Wed, 20 Sep 2023 11:23:16 GMT  
		Size: 3.4 KB (3373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913009f5d7ce3f00561b3220a723826b84895260169d5eb98399e5b5e556cf3f`  
		Last Modified: Fri, 06 Oct 2023 18:51:38 GMT  
		Size: 33.6 MB (33603470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-bookworm` - linux; 386

```console
$ docker pull irssi@sha256:63f96f9a3864f944849735f8de61f7b79f6e0523602340eb8af73f8e2bcca8e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76522799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7838aa7df5bd597e8394793aa77df15853878793a687685bf46ccbd60588a43`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:42 GMT
ADD file:31318c1b1f05d559cce42f5b12eef97d916932217e0b987fb07c0fc11bf0a14a in / 
# Wed, 11 Oct 2023 17:40:42 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:31:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:31:53 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 21:31:54 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 21:31:54 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 21:31:54 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 21:32:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 21:32:48 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 21:32:48 GMT
USER user
# Wed, 11 Oct 2023 21:32:48 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b27d0f1369837277a82877763487cdd2535037988fc27e16f11cf74e103ae4cd`  
		Last Modified: Wed, 11 Oct 2023 17:45:31 GMT  
		Size: 30.2 MB (30164118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5aabddc89a058b8444274e0ab7a7604dd6b19276ca05209051a7bd05996a97`  
		Last Modified: Wed, 11 Oct 2023 21:33:17 GMT  
		Size: 17.8 MB (17788766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674da66b6a6ab4b333d0fbf0c2731e6fcdfc0628ea6463fe2c8c298c2e4f5022`  
		Last Modified: Wed, 11 Oct 2023 21:33:10 GMT  
		Size: 3.4 KB (3373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be398748b24b800d52f805e4b55221b65ab68f63fa172620395b27d97f4cef62`  
		Last Modified: Wed, 11 Oct 2023 21:33:18 GMT  
		Size: 28.6 MB (28566542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-bookworm` - linux; mips64le

```console
$ docker pull irssi@sha256:4622ced3be5a3c4e803c2594eaf6c13299ae0a9f6da133fcac361f6b46a6f62e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73893583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80f80aac1fac6ff7d115cd8d97db39021a1be94a7121a4fe70787e480a3d445f`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:49:32 GMT
ADD file:2abda0a72972a417d4f7f530ca8fa1ee7e85e25d4015fd4e70acf903cfd96d3d in / 
# Wed, 11 Oct 2023 17:49:36 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 20:05:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 20:05:10 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 20:05:16 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 20:05:19 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 20:05:23 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 20:09:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 20:09:27 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 20:09:31 GMT
USER user
# Wed, 11 Oct 2023 20:09:35 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f11870ec99d788b4b160d9f3f4c0a79904290083d8930b26e5d13579226e07f0`  
		Last Modified: Wed, 11 Oct 2023 18:00:43 GMT  
		Size: 29.1 MB (29142026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1f47bc243f41e66258f22f77a6d27afd7c49447f4867ab03737c1c00e055e5`  
		Last Modified: Wed, 11 Oct 2023 20:10:17 GMT  
		Size: 16.7 MB (16741536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528d2b189bddab2a8763fd33d4deba2040b0c2d28337893be13d77d751b745dd`  
		Last Modified: Wed, 11 Oct 2023 20:10:01 GMT  
		Size: 3.3 KB (3299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299c20205b3210d510f4fcb1678d9093fca2d25452b80816b0da15049cbb41d2`  
		Last Modified: Wed, 11 Oct 2023 20:10:22 GMT  
		Size: 28.0 MB (28006722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-bookworm` - linux; ppc64le

```console
$ docker pull irssi@sha256:fe9ad83e93b168870c785b041cfbe670b128f99b8ed3e270c8d50bc9de07c5a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.9 MB (88901114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:132c9d6a4750e943c7033db5a5253d77f49da8681b15cc3af59b0459530997d5`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Sep 2023 07:52:54 GMT
ADD file:9a37b479e68a0d18babbef8dd04d09a0e6844a0080876d14144a34bfd9d0897a in / 
# Wed, 20 Sep 2023 07:52:55 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 11:46:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:46:25 GMT
ENV HOME=/home/user
# Wed, 20 Sep 2023 11:46:27 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Sep 2023 11:46:28 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 20:45:02 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 20:47:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 06 Oct 2023 20:47:27 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 20:47:28 GMT
USER user
# Fri, 06 Oct 2023 20:47:28 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:696a66e961f2033dcf69b003ad7faf28ed2248da58efa1c08a9d496739a8eeeb`  
		Last Modified: Wed, 20 Sep 2023 08:49:51 GMT  
		Size: 33.1 MB (33119461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30054596536297b2e58930c4fe17cb3dd9a484e48310a73810d633fb399b2ea4`  
		Last Modified: Wed, 20 Sep 2023 11:48:21 GMT  
		Size: 18.8 MB (18754188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53547fc5d9551d1c1a1f2ccd6a7125ea312eac162cb9f63b4cf854af65c77212`  
		Last Modified: Wed, 20 Sep 2023 11:48:14 GMT  
		Size: 3.4 KB (3376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c58b6669e0fac3c777f89f1c775613c7c4b79937cdbaa4f03d84f4779088902`  
		Last Modified: Fri, 06 Oct 2023 20:48:39 GMT  
		Size: 37.0 MB (37024089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-bookworm` - linux; s390x

```console
$ docker pull irssi@sha256:adf3bc216988808a8cd8bc19d6474ceae3e63c68d9fb35a403ebc2880dc00605
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.4 MB (80399807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4a91ab3027978ac40b17ec8bcc5ed457b28d8b316732dafa175ccc524171687`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Sep 2023 02:54:26 GMT
ADD file:6ed982ad3e8566d63315a27a81b33069910952aef4b2d3e0b607bd2caeac7ca4 in / 
# Wed, 20 Sep 2023 02:54:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 08:50:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 08:50:11 GMT
ENV HOME=/home/user
# Wed, 20 Sep 2023 08:50:11 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Sep 2023 08:50:12 GMT
ENV LANG=C.UTF-8
# Tue, 10 Oct 2023 02:24:14 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 10 Oct 2023 02:34:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 10 Oct 2023 02:34:37 GMT
WORKDIR /home/user
# Tue, 10 Oct 2023 02:34:37 GMT
USER user
# Tue, 10 Oct 2023 02:34:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:26dcff366e33abcf08b812052a4c12496aa406aa267655e984aa7a84ca254cd8`  
		Last Modified: Wed, 20 Sep 2023 02:59:47 GMT  
		Size: 27.5 MB (27489966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9ab36ca6d32a38244529fb5d1341f679d66a581da57bc1e46bae74a2dac076`  
		Last Modified: Wed, 20 Sep 2023 08:51:27 GMT  
		Size: 18.2 MB (18205945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537016b33e97a91c754da6fb3df713bc111e51fdbd9e9967edfca9572cb96401`  
		Last Modified: Wed, 20 Sep 2023 08:51:24 GMT  
		Size: 3.4 KB (3372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f9e3389f5957a7bcdb6592475907b2611f851e3057e46ba4aa3c7143958e7b`  
		Last Modified: Tue, 10 Oct 2023 02:35:44 GMT  
		Size: 34.7 MB (34700524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4.5`

```console
$ docker pull irssi@sha256:8cd808235b32389f3bdc481a70654f08582189b7eaf51633adda044135312271
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
$ docker pull irssi@sha256:44c777babe5699a8971eb5367dbd411e6eee21e8ed16a4ff7613b037af6f5ceb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76090686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33f1ddb1eb8c8968dc461872fe15016c247b14190fdf74279962255735dca784`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 20:24:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 20:24:47 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 20:24:48 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 20:24:48 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 20:24:48 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 20:25:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 20:25:28 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 20:25:28 GMT
USER user
# Wed, 11 Oct 2023 20:25:28 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3853166e834fc2c48aedc55edbe9e1f882a3d7949f309a967e85dc49845a888c`  
		Last Modified: Wed, 11 Oct 2023 20:26:01 GMT  
		Size: 18.3 MB (18258013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8712f3c7bad7100c6d37fcf7e3c5002d8d7678548bf0892ca23e4904b9c066`  
		Last Modified: Wed, 11 Oct 2023 20:25:57 GMT  
		Size: 3.4 KB (3374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8f213a94fe9accb515298e6053d1ff437041b2b2033156092b5365c7791601`  
		Last Modified: Wed, 11 Oct 2023 20:26:02 GMT  
		Size: 28.7 MB (28679425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5` - linux; arm variant v5

```console
$ docker pull irssi@sha256:b49414becae5081d26d6eff6e214ce40e04aecbd6aa5ba63ebfda941497dd5a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70342849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a65606ee0e4cc323ad482840a06d50e1ba7e9d69faf54c5049c7c1fa6332a3f`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:43 GMT
ADD file:8c43adb3245fc6f2b10aa5a86c850db5dcf3515eaf7e46630922fe21f806bd2a in / 
# Wed, 11 Oct 2023 17:37:43 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:00:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:00:56 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 18:00:57 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 18:00:57 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 18:00:57 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 18:01:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 18:01:42 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 18:01:42 GMT
USER user
# Wed, 11 Oct 2023 18:01:42 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:904e6393ef1ee28b37171369eb4f7cb04714631c711799819fccb83886bd212b`  
		Last Modified: Wed, 11 Oct 2023 17:40:47 GMT  
		Size: 26.9 MB (26922150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107efe7ce893352f65dfb345d40ccf416fdb609825df68a2b3f8e02e6a0a3d56`  
		Last Modified: Wed, 11 Oct 2023 18:01:58 GMT  
		Size: 17.1 MB (17092623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317d45cff4b023ded2635c88d1801ee2d5e8911f9a7098ecc25aa7ef5949d566`  
		Last Modified: Wed, 11 Oct 2023 18:01:54 GMT  
		Size: 3.4 KB (3371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be15a5c4dd41a9defc1496cb7afa89616c007835aba62d34d7e38258f865e8e`  
		Last Modified: Wed, 11 Oct 2023 18:01:59 GMT  
		Size: 26.3 MB (26324705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5` - linux; arm variant v7

```console
$ docker pull irssi@sha256:9acb53b918ce7218355b74aed1213e71f5126277b32e948808b45ae3424df9ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66653393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0fdfeb17d52fb8aecbbeffe1311c2184bb7fa3da76896c739fd02fe736d719b`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:12:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:12:48 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 19:12:48 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 19:12:48 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 19:12:48 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 19:13:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 19:13:29 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 19:13:29 GMT
USER user
# Wed, 11 Oct 2023 19:13:29 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5baaee56a9498d8e72131adb171dee5671edf350e3f83e1154b2d1651115385`  
		Last Modified: Wed, 11 Oct 2023 19:13:56 GMT  
		Size: 16.7 MB (16678815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ccc912053095badfc35dbd2f166cc2477b07f22b2a8ec2c38183c5c0277873d`  
		Last Modified: Wed, 11 Oct 2023 19:13:52 GMT  
		Size: 3.4 KB (3377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b622859b61c28bc5dbc1cca27e70e2473d2425378c3e3ba112546f6b0d1c70eb`  
		Last Modified: Wed, 11 Oct 2023 19:13:57 GMT  
		Size: 25.2 MB (25222276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:8edaae578605997a74c4364d46c96a3867c2054543a60b2f724913b6a4fa6754
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.8 MB (80788768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f32fcd8186f4b8d4af0b40f507e8f94ea2bfbd86b7fc41276659e2e7ab7ddfe`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:13 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Wed, 20 Sep 2023 02:44:14 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 11:22:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:22:14 GMT
ENV HOME=/home/user
# Wed, 20 Sep 2023 11:22:14 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Sep 2023 11:22:14 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 18:50:25 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 18:51:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 06 Oct 2023 18:51:03 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 18:51:03 GMT
USER user
# Fri, 06 Oct 2023 18:51:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e17a035c22a6860e7c120c60f7d2f84bf9834e6ebdef94bf9b9f044d9c93d69`  
		Last Modified: Wed, 20 Sep 2023 11:23:19 GMT  
		Size: 18.0 MB (18024704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f81b6709eee0366d7cb53c2306da1edae2817e93e99cdd35e7f36aa5e866c8e`  
		Last Modified: Wed, 20 Sep 2023 11:23:16 GMT  
		Size: 3.4 KB (3373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913009f5d7ce3f00561b3220a723826b84895260169d5eb98399e5b5e556cf3f`  
		Last Modified: Fri, 06 Oct 2023 18:51:38 GMT  
		Size: 33.6 MB (33603470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5` - linux; 386

```console
$ docker pull irssi@sha256:63f96f9a3864f944849735f8de61f7b79f6e0523602340eb8af73f8e2bcca8e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76522799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7838aa7df5bd597e8394793aa77df15853878793a687685bf46ccbd60588a43`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:42 GMT
ADD file:31318c1b1f05d559cce42f5b12eef97d916932217e0b987fb07c0fc11bf0a14a in / 
# Wed, 11 Oct 2023 17:40:42 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:31:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:31:53 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 21:31:54 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 21:31:54 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 21:31:54 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 21:32:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 21:32:48 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 21:32:48 GMT
USER user
# Wed, 11 Oct 2023 21:32:48 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b27d0f1369837277a82877763487cdd2535037988fc27e16f11cf74e103ae4cd`  
		Last Modified: Wed, 11 Oct 2023 17:45:31 GMT  
		Size: 30.2 MB (30164118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5aabddc89a058b8444274e0ab7a7604dd6b19276ca05209051a7bd05996a97`  
		Last Modified: Wed, 11 Oct 2023 21:33:17 GMT  
		Size: 17.8 MB (17788766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674da66b6a6ab4b333d0fbf0c2731e6fcdfc0628ea6463fe2c8c298c2e4f5022`  
		Last Modified: Wed, 11 Oct 2023 21:33:10 GMT  
		Size: 3.4 KB (3373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be398748b24b800d52f805e4b55221b65ab68f63fa172620395b27d97f4cef62`  
		Last Modified: Wed, 11 Oct 2023 21:33:18 GMT  
		Size: 28.6 MB (28566542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5` - linux; mips64le

```console
$ docker pull irssi@sha256:4622ced3be5a3c4e803c2594eaf6c13299ae0a9f6da133fcac361f6b46a6f62e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73893583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80f80aac1fac6ff7d115cd8d97db39021a1be94a7121a4fe70787e480a3d445f`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:49:32 GMT
ADD file:2abda0a72972a417d4f7f530ca8fa1ee7e85e25d4015fd4e70acf903cfd96d3d in / 
# Wed, 11 Oct 2023 17:49:36 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 20:05:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 20:05:10 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 20:05:16 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 20:05:19 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 20:05:23 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 20:09:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 20:09:27 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 20:09:31 GMT
USER user
# Wed, 11 Oct 2023 20:09:35 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f11870ec99d788b4b160d9f3f4c0a79904290083d8930b26e5d13579226e07f0`  
		Last Modified: Wed, 11 Oct 2023 18:00:43 GMT  
		Size: 29.1 MB (29142026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1f47bc243f41e66258f22f77a6d27afd7c49447f4867ab03737c1c00e055e5`  
		Last Modified: Wed, 11 Oct 2023 20:10:17 GMT  
		Size: 16.7 MB (16741536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528d2b189bddab2a8763fd33d4deba2040b0c2d28337893be13d77d751b745dd`  
		Last Modified: Wed, 11 Oct 2023 20:10:01 GMT  
		Size: 3.3 KB (3299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299c20205b3210d510f4fcb1678d9093fca2d25452b80816b0da15049cbb41d2`  
		Last Modified: Wed, 11 Oct 2023 20:10:22 GMT  
		Size: 28.0 MB (28006722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5` - linux; ppc64le

```console
$ docker pull irssi@sha256:fe9ad83e93b168870c785b041cfbe670b128f99b8ed3e270c8d50bc9de07c5a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.9 MB (88901114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:132c9d6a4750e943c7033db5a5253d77f49da8681b15cc3af59b0459530997d5`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Sep 2023 07:52:54 GMT
ADD file:9a37b479e68a0d18babbef8dd04d09a0e6844a0080876d14144a34bfd9d0897a in / 
# Wed, 20 Sep 2023 07:52:55 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 11:46:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:46:25 GMT
ENV HOME=/home/user
# Wed, 20 Sep 2023 11:46:27 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Sep 2023 11:46:28 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 20:45:02 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 20:47:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 06 Oct 2023 20:47:27 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 20:47:28 GMT
USER user
# Fri, 06 Oct 2023 20:47:28 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:696a66e961f2033dcf69b003ad7faf28ed2248da58efa1c08a9d496739a8eeeb`  
		Last Modified: Wed, 20 Sep 2023 08:49:51 GMT  
		Size: 33.1 MB (33119461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30054596536297b2e58930c4fe17cb3dd9a484e48310a73810d633fb399b2ea4`  
		Last Modified: Wed, 20 Sep 2023 11:48:21 GMT  
		Size: 18.8 MB (18754188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53547fc5d9551d1c1a1f2ccd6a7125ea312eac162cb9f63b4cf854af65c77212`  
		Last Modified: Wed, 20 Sep 2023 11:48:14 GMT  
		Size: 3.4 KB (3376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c58b6669e0fac3c777f89f1c775613c7c4b79937cdbaa4f03d84f4779088902`  
		Last Modified: Fri, 06 Oct 2023 20:48:39 GMT  
		Size: 37.0 MB (37024089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5` - linux; s390x

```console
$ docker pull irssi@sha256:adf3bc216988808a8cd8bc19d6474ceae3e63c68d9fb35a403ebc2880dc00605
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.4 MB (80399807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4a91ab3027978ac40b17ec8bcc5ed457b28d8b316732dafa175ccc524171687`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Sep 2023 02:54:26 GMT
ADD file:6ed982ad3e8566d63315a27a81b33069910952aef4b2d3e0b607bd2caeac7ca4 in / 
# Wed, 20 Sep 2023 02:54:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 08:50:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 08:50:11 GMT
ENV HOME=/home/user
# Wed, 20 Sep 2023 08:50:11 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Sep 2023 08:50:12 GMT
ENV LANG=C.UTF-8
# Tue, 10 Oct 2023 02:24:14 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 10 Oct 2023 02:34:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 10 Oct 2023 02:34:37 GMT
WORKDIR /home/user
# Tue, 10 Oct 2023 02:34:37 GMT
USER user
# Tue, 10 Oct 2023 02:34:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:26dcff366e33abcf08b812052a4c12496aa406aa267655e984aa7a84ca254cd8`  
		Last Modified: Wed, 20 Sep 2023 02:59:47 GMT  
		Size: 27.5 MB (27489966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9ab36ca6d32a38244529fb5d1341f679d66a581da57bc1e46bae74a2dac076`  
		Last Modified: Wed, 20 Sep 2023 08:51:27 GMT  
		Size: 18.2 MB (18205945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537016b33e97a91c754da6fb3df713bc111e51fdbd9e9967edfca9572cb96401`  
		Last Modified: Wed, 20 Sep 2023 08:51:24 GMT  
		Size: 3.4 KB (3372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f9e3389f5957a7bcdb6592475907b2611f851e3057e46ba4aa3c7143958e7b`  
		Last Modified: Tue, 10 Oct 2023 02:35:44 GMT  
		Size: 34.7 MB (34700524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4.5-alpine`

```console
$ docker pull irssi@sha256:38d806b8883cbc7d4ce632aa3b67d6d57415a6de9e8a1e24d78b5fa0dd4eb40c
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
$ docker pull irssi@sha256:1ee6ea9617f00ef85aec02096aeee93e253c1fce4f559a3739175f1412110887
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18840008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a7066a07c9e35db2f3641c82d1b1599ebb7ecfbba2d78659f3093927b81c6f9`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:07:22 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 23:07:22 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 23:07:23 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 23:07:23 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 20:05:43 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 20:06:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 20:06:02 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 20:06:02 GMT
USER user
# Fri, 06 Oct 2023 20:06:02 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af553cbaa1665f3df3ff9ed6df3fc8fdeef915391198875444aee02cb0f1dba`  
		Last Modified: Thu, 28 Sep 2023 23:08:01 GMT  
		Size: 9.6 MB (9638068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475821153744984a56837800be5e45c520da1740ad0e9e56b1a27abb64ab5677`  
		Last Modified: Thu, 28 Sep 2023 23:07:59 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6870b695db89ae46f18ed0a5ea51ba2cb82240d1c5b1c5219a7030798a3f67`  
		Last Modified: Fri, 06 Oct 2023 20:06:47 GMT  
		Size: 5.8 MB (5798688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:7118fc38d54f6deb6a8782357883da4a4cf756bdbfad659c9c1e763250c48d28
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17664781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:012fe6e595cbd84ddedfb4904315ce7f3714991ff90335a481bd48c1252e419c`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:01:23 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:01:24 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:01:24 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:01:24 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 18:54:46 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 18:55:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 18:55:03 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 18:55:03 GMT
USER user
# Fri, 06 Oct 2023 18:55:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:152af5fc5e35a15ab7dff7175a3d682681efedcdd033b4b6ba5e65c50b0ec64f`  
		Last Modified: Thu, 28 Sep 2023 22:01:58 GMT  
		Size: 8.9 MB (8873701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e78ce7c600d11081aaabe6fe5d3d25a6badae1aaa32d490a392cb1c418e0a4`  
		Last Modified: Thu, 28 Sep 2023 22:01:56 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1971284431ad2c2d645075809b4b98b4cf9f9e16ed619f22e95078036b79b731`  
		Last Modified: Fri, 06 Oct 2023 18:55:15 GMT  
		Size: 5.6 MB (5644504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:6553e184e6f2c2417e9f000d0234179c8c8a752d02eb3f2f0b26c675a256fe75
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16994937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0965965700d10cee279de650a20af25276316e23dcc59c4092e271285e7133ed`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:32:29 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 29 Sep 2023 00:32:30 GMT
ENV HOME=/home/user
# Fri, 29 Sep 2023 00:32:30 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 29 Sep 2023 00:32:30 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 19:06:51 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 19:07:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 19:07:06 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 19:07:07 GMT
USER user
# Fri, 06 Oct 2023 19:07:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666541fade74dbbeba8bc1dc2a6f59e496ee2556c1694f8d97e154861211eb4a`  
		Last Modified: Fri, 29 Sep 2023 00:33:18 GMT  
		Size: 8.7 MB (8713773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6786d679f064e76ebc61ea937d53f08e38f578e494b4f72907c4e1886737ccfa`  
		Last Modified: Fri, 29 Sep 2023 00:33:15 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c623f5de44c876517872695b3ea33e2cd0afd3becbd2ef6e84b03a5dacef1ef`  
		Last Modified: Fri, 06 Oct 2023 19:07:49 GMT  
		Size: 5.4 MB (5379973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:8e84ebd4f06676afeeff5d3df76c54b494e9225ad08af34c22405bbb1dfac624
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18715109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4acd348d9659d9e55521ba8e049504b24acb95e989e3c60ef45ce22819d3201c`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:57:36 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 21:57:36 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 21:57:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 21:57:36 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 18:51:05 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 18:51:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 18:51:19 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 18:51:19 GMT
USER user
# Fri, 06 Oct 2023 18:51:19 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb98c09201d772cdbd8ebf3b77e3767ba0112bb407e3fa992d4a5e162065862`  
		Last Modified: Thu, 28 Sep 2023 21:58:15 GMT  
		Size: 9.7 MB (9667003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3eb447534379436f487e6d6e2a8bfe8d3f4a55aaf3e65cd8c162ce04b733398`  
		Last Modified: Thu, 28 Sep 2023 21:58:14 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8285f819417a3875bfc576dd902248316d6bc296fa13316b6e8b1a5193ee0005`  
		Last Modified: Fri, 06 Oct 2023 18:51:59 GMT  
		Size: 5.7 MB (5714992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-alpine` - linux; 386

```console
$ docker pull irssi@sha256:69515832cd89cf3cc8728b14b7d7d45807fdbec718333af24fc6bf5a8278c54e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.9 MB (17949510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db319b5e7991efcb54c8e037e2cf8bf425d3120b5c5db3df57a4340e246f33dc`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:21:39 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:21:39 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:21:40 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:21:40 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 19:04:21 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 19:04:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 19:04:58 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 19:04:58 GMT
USER user
# Fri, 06 Oct 2023 19:04:58 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbc2dcf799f84aca231b4b6ee2ee6a7a58c3d7b06552d33525458178ce175e2`  
		Last Modified: Thu, 28 Sep 2023 22:22:42 GMT  
		Size: 8.9 MB (8896304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651ec124ac1e46e7e92bc912dfd7308d68d99665be7a2f45460942974926a5b1`  
		Last Modified: Thu, 28 Sep 2023 22:22:39 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a9a322c02a4abf355ad95df55379c7b4d60eba24e72dc90494c80090a1b592`  
		Last Modified: Fri, 06 Oct 2023 19:05:47 GMT  
		Size: 5.8 MB (5816163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:ff90811e849a6fab02c5de90bc84e4c443e3f3f0bb00de9e349725aa44244725
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19108084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c796f660963a32e2c420da0b32b935efdc163713b712139b85e90641d5cc03b2`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:30:38 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:30:40 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:30:41 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:30:42 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 20:47:41 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 20:48:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 20:48:10 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 20:48:10 GMT
USER user
# Fri, 06 Oct 2023 20:48:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765c74d616c6113799971e0b6fb6422b9d4f661cf327745b094cf89369df5fd4`  
		Last Modified: Thu, 28 Sep 2023 22:31:32 GMT  
		Size: 9.7 MB (9727392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfad26be399d4cd09dd2d4252d711e7870345b952b27faeb6f911e9ca449205b`  
		Last Modified: Thu, 28 Sep 2023 22:31:28 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a22d5c7ff0996c5ff524bb74b55e5db4d4a6f8d9bf364cea4a9a40c5ac4455d`  
		Last Modified: Fri, 06 Oct 2023 20:49:04 GMT  
		Size: 6.0 MB (6032900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:079255c123c85c24159e85a1eaf32b4e29a6d6a2e5f78f4d91eafa4e8a1678d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19110918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9b0678fe28100c4b753e58afa0b56102e537a694723ae5d01836a4dceeb40a3`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:18:20 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:18:21 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:18:22 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:18:22 GMT
ENV LANG=C.UTF-8
# Tue, 10 Oct 2023 02:34:46 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 10 Oct 2023 02:35:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 10 Oct 2023 02:35:16 GMT
WORKDIR /home/user
# Tue, 10 Oct 2023 02:35:16 GMT
USER user
# Tue, 10 Oct 2023 02:35:16 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91051e7453a3fcb401f58424e77fa5aa5ee6fee0cca8a5a32646f89a65360ce3`  
		Last Modified: Thu, 28 Sep 2023 22:19:09 GMT  
		Size: 10.1 MB (10078961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c731adf381a8e9331a2fea37d34da20a1359a905c7d7ccf7f166f464e39e5b42`  
		Last Modified: Thu, 28 Sep 2023 22:19:07 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adecf7d94f7048c67fd6041522959d98bf86eb9514cc1b44ede5da69ba7925a5`  
		Last Modified: Tue, 10 Oct 2023 02:37:07 GMT  
		Size: 5.8 MB (5815570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4.5-alpine3.18`

```console
$ docker pull irssi@sha256:38d806b8883cbc7d4ce632aa3b67d6d57415a6de9e8a1e24d78b5fa0dd4eb40c
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
$ docker pull irssi@sha256:1ee6ea9617f00ef85aec02096aeee93e253c1fce4f559a3739175f1412110887
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18840008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a7066a07c9e35db2f3641c82d1b1599ebb7ecfbba2d78659f3093927b81c6f9`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:07:22 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 23:07:22 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 23:07:23 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 23:07:23 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 20:05:43 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 20:06:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 20:06:02 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 20:06:02 GMT
USER user
# Fri, 06 Oct 2023 20:06:02 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af553cbaa1665f3df3ff9ed6df3fc8fdeef915391198875444aee02cb0f1dba`  
		Last Modified: Thu, 28 Sep 2023 23:08:01 GMT  
		Size: 9.6 MB (9638068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475821153744984a56837800be5e45c520da1740ad0e9e56b1a27abb64ab5677`  
		Last Modified: Thu, 28 Sep 2023 23:07:59 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6870b695db89ae46f18ed0a5ea51ba2cb82240d1c5b1c5219a7030798a3f67`  
		Last Modified: Fri, 06 Oct 2023 20:06:47 GMT  
		Size: 5.8 MB (5798688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-alpine3.18` - linux; arm variant v6

```console
$ docker pull irssi@sha256:7118fc38d54f6deb6a8782357883da4a4cf756bdbfad659c9c1e763250c48d28
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17664781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:012fe6e595cbd84ddedfb4904315ce7f3714991ff90335a481bd48c1252e419c`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:01:23 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:01:24 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:01:24 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:01:24 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 18:54:46 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 18:55:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 18:55:03 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 18:55:03 GMT
USER user
# Fri, 06 Oct 2023 18:55:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:152af5fc5e35a15ab7dff7175a3d682681efedcdd033b4b6ba5e65c50b0ec64f`  
		Last Modified: Thu, 28 Sep 2023 22:01:58 GMT  
		Size: 8.9 MB (8873701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e78ce7c600d11081aaabe6fe5d3d25a6badae1aaa32d490a392cb1c418e0a4`  
		Last Modified: Thu, 28 Sep 2023 22:01:56 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1971284431ad2c2d645075809b4b98b4cf9f9e16ed619f22e95078036b79b731`  
		Last Modified: Fri, 06 Oct 2023 18:55:15 GMT  
		Size: 5.6 MB (5644504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-alpine3.18` - linux; arm variant v7

```console
$ docker pull irssi@sha256:6553e184e6f2c2417e9f000d0234179c8c8a752d02eb3f2f0b26c675a256fe75
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16994937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0965965700d10cee279de650a20af25276316e23dcc59c4092e271285e7133ed`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:32:29 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 29 Sep 2023 00:32:30 GMT
ENV HOME=/home/user
# Fri, 29 Sep 2023 00:32:30 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 29 Sep 2023 00:32:30 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 19:06:51 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 19:07:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 19:07:06 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 19:07:07 GMT
USER user
# Fri, 06 Oct 2023 19:07:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666541fade74dbbeba8bc1dc2a6f59e496ee2556c1694f8d97e154861211eb4a`  
		Last Modified: Fri, 29 Sep 2023 00:33:18 GMT  
		Size: 8.7 MB (8713773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6786d679f064e76ebc61ea937d53f08e38f578e494b4f72907c4e1886737ccfa`  
		Last Modified: Fri, 29 Sep 2023 00:33:15 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c623f5de44c876517872695b3ea33e2cd0afd3becbd2ef6e84b03a5dacef1ef`  
		Last Modified: Fri, 06 Oct 2023 19:07:49 GMT  
		Size: 5.4 MB (5379973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:8e84ebd4f06676afeeff5d3df76c54b494e9225ad08af34c22405bbb1dfac624
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18715109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4acd348d9659d9e55521ba8e049504b24acb95e989e3c60ef45ce22819d3201c`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:57:36 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 21:57:36 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 21:57:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 21:57:36 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 18:51:05 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 18:51:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 18:51:19 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 18:51:19 GMT
USER user
# Fri, 06 Oct 2023 18:51:19 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb98c09201d772cdbd8ebf3b77e3767ba0112bb407e3fa992d4a5e162065862`  
		Last Modified: Thu, 28 Sep 2023 21:58:15 GMT  
		Size: 9.7 MB (9667003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3eb447534379436f487e6d6e2a8bfe8d3f4a55aaf3e65cd8c162ce04b733398`  
		Last Modified: Thu, 28 Sep 2023 21:58:14 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8285f819417a3875bfc576dd902248316d6bc296fa13316b6e8b1a5193ee0005`  
		Last Modified: Fri, 06 Oct 2023 18:51:59 GMT  
		Size: 5.7 MB (5714992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-alpine3.18` - linux; 386

```console
$ docker pull irssi@sha256:69515832cd89cf3cc8728b14b7d7d45807fdbec718333af24fc6bf5a8278c54e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.9 MB (17949510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db319b5e7991efcb54c8e037e2cf8bf425d3120b5c5db3df57a4340e246f33dc`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:21:39 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:21:39 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:21:40 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:21:40 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 19:04:21 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 19:04:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 19:04:58 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 19:04:58 GMT
USER user
# Fri, 06 Oct 2023 19:04:58 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbc2dcf799f84aca231b4b6ee2ee6a7a58c3d7b06552d33525458178ce175e2`  
		Last Modified: Thu, 28 Sep 2023 22:22:42 GMT  
		Size: 8.9 MB (8896304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651ec124ac1e46e7e92bc912dfd7308d68d99665be7a2f45460942974926a5b1`  
		Last Modified: Thu, 28 Sep 2023 22:22:39 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a9a322c02a4abf355ad95df55379c7b4d60eba24e72dc90494c80090a1b592`  
		Last Modified: Fri, 06 Oct 2023 19:05:47 GMT  
		Size: 5.8 MB (5816163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-alpine3.18` - linux; ppc64le

```console
$ docker pull irssi@sha256:ff90811e849a6fab02c5de90bc84e4c443e3f3f0bb00de9e349725aa44244725
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19108084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c796f660963a32e2c420da0b32b935efdc163713b712139b85e90641d5cc03b2`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:30:38 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:30:40 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:30:41 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:30:42 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 20:47:41 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 20:48:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 20:48:10 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 20:48:10 GMT
USER user
# Fri, 06 Oct 2023 20:48:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765c74d616c6113799971e0b6fb6422b9d4f661cf327745b094cf89369df5fd4`  
		Last Modified: Thu, 28 Sep 2023 22:31:32 GMT  
		Size: 9.7 MB (9727392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfad26be399d4cd09dd2d4252d711e7870345b952b27faeb6f911e9ca449205b`  
		Last Modified: Thu, 28 Sep 2023 22:31:28 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a22d5c7ff0996c5ff524bb74b55e5db4d4a6f8d9bf364cea4a9a40c5ac4455d`  
		Last Modified: Fri, 06 Oct 2023 20:49:04 GMT  
		Size: 6.0 MB (6032900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-alpine3.18` - linux; s390x

```console
$ docker pull irssi@sha256:079255c123c85c24159e85a1eaf32b4e29a6d6a2e5f78f4d91eafa4e8a1678d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19110918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9b0678fe28100c4b753e58afa0b56102e537a694723ae5d01836a4dceeb40a3`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:18:20 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:18:21 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:18:22 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:18:22 GMT
ENV LANG=C.UTF-8
# Tue, 10 Oct 2023 02:34:46 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 10 Oct 2023 02:35:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 10 Oct 2023 02:35:16 GMT
WORKDIR /home/user
# Tue, 10 Oct 2023 02:35:16 GMT
USER user
# Tue, 10 Oct 2023 02:35:16 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91051e7453a3fcb401f58424e77fa5aa5ee6fee0cca8a5a32646f89a65360ce3`  
		Last Modified: Thu, 28 Sep 2023 22:19:09 GMT  
		Size: 10.1 MB (10078961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c731adf381a8e9331a2fea37d34da20a1359a905c7d7ccf7f166f464e39e5b42`  
		Last Modified: Thu, 28 Sep 2023 22:19:07 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adecf7d94f7048c67fd6041522959d98bf86eb9514cc1b44ede5da69ba7925a5`  
		Last Modified: Tue, 10 Oct 2023 02:37:07 GMT  
		Size: 5.8 MB (5815570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4.5-bookworm`

```console
$ docker pull irssi@sha256:8cd808235b32389f3bdc481a70654f08582189b7eaf51633adda044135312271
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
$ docker pull irssi@sha256:44c777babe5699a8971eb5367dbd411e6eee21e8ed16a4ff7613b037af6f5ceb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76090686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33f1ddb1eb8c8968dc461872fe15016c247b14190fdf74279962255735dca784`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 20:24:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 20:24:47 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 20:24:48 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 20:24:48 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 20:24:48 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 20:25:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 20:25:28 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 20:25:28 GMT
USER user
# Wed, 11 Oct 2023 20:25:28 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3853166e834fc2c48aedc55edbe9e1f882a3d7949f309a967e85dc49845a888c`  
		Last Modified: Wed, 11 Oct 2023 20:26:01 GMT  
		Size: 18.3 MB (18258013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8712f3c7bad7100c6d37fcf7e3c5002d8d7678548bf0892ca23e4904b9c066`  
		Last Modified: Wed, 11 Oct 2023 20:25:57 GMT  
		Size: 3.4 KB (3374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8f213a94fe9accb515298e6053d1ff437041b2b2033156092b5365c7791601`  
		Last Modified: Wed, 11 Oct 2023 20:26:02 GMT  
		Size: 28.7 MB (28679425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-bookworm` - linux; arm variant v5

```console
$ docker pull irssi@sha256:b49414becae5081d26d6eff6e214ce40e04aecbd6aa5ba63ebfda941497dd5a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70342849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a65606ee0e4cc323ad482840a06d50e1ba7e9d69faf54c5049c7c1fa6332a3f`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:43 GMT
ADD file:8c43adb3245fc6f2b10aa5a86c850db5dcf3515eaf7e46630922fe21f806bd2a in / 
# Wed, 11 Oct 2023 17:37:43 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:00:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:00:56 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 18:00:57 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 18:00:57 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 18:00:57 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 18:01:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 18:01:42 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 18:01:42 GMT
USER user
# Wed, 11 Oct 2023 18:01:42 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:904e6393ef1ee28b37171369eb4f7cb04714631c711799819fccb83886bd212b`  
		Last Modified: Wed, 11 Oct 2023 17:40:47 GMT  
		Size: 26.9 MB (26922150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107efe7ce893352f65dfb345d40ccf416fdb609825df68a2b3f8e02e6a0a3d56`  
		Last Modified: Wed, 11 Oct 2023 18:01:58 GMT  
		Size: 17.1 MB (17092623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317d45cff4b023ded2635c88d1801ee2d5e8911f9a7098ecc25aa7ef5949d566`  
		Last Modified: Wed, 11 Oct 2023 18:01:54 GMT  
		Size: 3.4 KB (3371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be15a5c4dd41a9defc1496cb7afa89616c007835aba62d34d7e38258f865e8e`  
		Last Modified: Wed, 11 Oct 2023 18:01:59 GMT  
		Size: 26.3 MB (26324705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-bookworm` - linux; arm variant v7

```console
$ docker pull irssi@sha256:9acb53b918ce7218355b74aed1213e71f5126277b32e948808b45ae3424df9ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66653393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0fdfeb17d52fb8aecbbeffe1311c2184bb7fa3da76896c739fd02fe736d719b`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:12:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:12:48 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 19:12:48 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 19:12:48 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 19:12:48 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 19:13:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 19:13:29 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 19:13:29 GMT
USER user
# Wed, 11 Oct 2023 19:13:29 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5baaee56a9498d8e72131adb171dee5671edf350e3f83e1154b2d1651115385`  
		Last Modified: Wed, 11 Oct 2023 19:13:56 GMT  
		Size: 16.7 MB (16678815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ccc912053095badfc35dbd2f166cc2477b07f22b2a8ec2c38183c5c0277873d`  
		Last Modified: Wed, 11 Oct 2023 19:13:52 GMT  
		Size: 3.4 KB (3377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b622859b61c28bc5dbc1cca27e70e2473d2425378c3e3ba112546f6b0d1c70eb`  
		Last Modified: Wed, 11 Oct 2023 19:13:57 GMT  
		Size: 25.2 MB (25222276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-bookworm` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:8edaae578605997a74c4364d46c96a3867c2054543a60b2f724913b6a4fa6754
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.8 MB (80788768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f32fcd8186f4b8d4af0b40f507e8f94ea2bfbd86b7fc41276659e2e7ab7ddfe`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:13 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Wed, 20 Sep 2023 02:44:14 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 11:22:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:22:14 GMT
ENV HOME=/home/user
# Wed, 20 Sep 2023 11:22:14 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Sep 2023 11:22:14 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 18:50:25 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 18:51:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 06 Oct 2023 18:51:03 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 18:51:03 GMT
USER user
# Fri, 06 Oct 2023 18:51:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e17a035c22a6860e7c120c60f7d2f84bf9834e6ebdef94bf9b9f044d9c93d69`  
		Last Modified: Wed, 20 Sep 2023 11:23:19 GMT  
		Size: 18.0 MB (18024704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f81b6709eee0366d7cb53c2306da1edae2817e93e99cdd35e7f36aa5e866c8e`  
		Last Modified: Wed, 20 Sep 2023 11:23:16 GMT  
		Size: 3.4 KB (3373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913009f5d7ce3f00561b3220a723826b84895260169d5eb98399e5b5e556cf3f`  
		Last Modified: Fri, 06 Oct 2023 18:51:38 GMT  
		Size: 33.6 MB (33603470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-bookworm` - linux; 386

```console
$ docker pull irssi@sha256:63f96f9a3864f944849735f8de61f7b79f6e0523602340eb8af73f8e2bcca8e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76522799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7838aa7df5bd597e8394793aa77df15853878793a687685bf46ccbd60588a43`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:42 GMT
ADD file:31318c1b1f05d559cce42f5b12eef97d916932217e0b987fb07c0fc11bf0a14a in / 
# Wed, 11 Oct 2023 17:40:42 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:31:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:31:53 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 21:31:54 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 21:31:54 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 21:31:54 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 21:32:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 21:32:48 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 21:32:48 GMT
USER user
# Wed, 11 Oct 2023 21:32:48 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b27d0f1369837277a82877763487cdd2535037988fc27e16f11cf74e103ae4cd`  
		Last Modified: Wed, 11 Oct 2023 17:45:31 GMT  
		Size: 30.2 MB (30164118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5aabddc89a058b8444274e0ab7a7604dd6b19276ca05209051a7bd05996a97`  
		Last Modified: Wed, 11 Oct 2023 21:33:17 GMT  
		Size: 17.8 MB (17788766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674da66b6a6ab4b333d0fbf0c2731e6fcdfc0628ea6463fe2c8c298c2e4f5022`  
		Last Modified: Wed, 11 Oct 2023 21:33:10 GMT  
		Size: 3.4 KB (3373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be398748b24b800d52f805e4b55221b65ab68f63fa172620395b27d97f4cef62`  
		Last Modified: Wed, 11 Oct 2023 21:33:18 GMT  
		Size: 28.6 MB (28566542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-bookworm` - linux; mips64le

```console
$ docker pull irssi@sha256:4622ced3be5a3c4e803c2594eaf6c13299ae0a9f6da133fcac361f6b46a6f62e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73893583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80f80aac1fac6ff7d115cd8d97db39021a1be94a7121a4fe70787e480a3d445f`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:49:32 GMT
ADD file:2abda0a72972a417d4f7f530ca8fa1ee7e85e25d4015fd4e70acf903cfd96d3d in / 
# Wed, 11 Oct 2023 17:49:36 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 20:05:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 20:05:10 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 20:05:16 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 20:05:19 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 20:05:23 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 20:09:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 20:09:27 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 20:09:31 GMT
USER user
# Wed, 11 Oct 2023 20:09:35 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f11870ec99d788b4b160d9f3f4c0a79904290083d8930b26e5d13579226e07f0`  
		Last Modified: Wed, 11 Oct 2023 18:00:43 GMT  
		Size: 29.1 MB (29142026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1f47bc243f41e66258f22f77a6d27afd7c49447f4867ab03737c1c00e055e5`  
		Last Modified: Wed, 11 Oct 2023 20:10:17 GMT  
		Size: 16.7 MB (16741536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528d2b189bddab2a8763fd33d4deba2040b0c2d28337893be13d77d751b745dd`  
		Last Modified: Wed, 11 Oct 2023 20:10:01 GMT  
		Size: 3.3 KB (3299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299c20205b3210d510f4fcb1678d9093fca2d25452b80816b0da15049cbb41d2`  
		Last Modified: Wed, 11 Oct 2023 20:10:22 GMT  
		Size: 28.0 MB (28006722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-bookworm` - linux; ppc64le

```console
$ docker pull irssi@sha256:fe9ad83e93b168870c785b041cfbe670b128f99b8ed3e270c8d50bc9de07c5a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.9 MB (88901114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:132c9d6a4750e943c7033db5a5253d77f49da8681b15cc3af59b0459530997d5`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Sep 2023 07:52:54 GMT
ADD file:9a37b479e68a0d18babbef8dd04d09a0e6844a0080876d14144a34bfd9d0897a in / 
# Wed, 20 Sep 2023 07:52:55 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 11:46:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:46:25 GMT
ENV HOME=/home/user
# Wed, 20 Sep 2023 11:46:27 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Sep 2023 11:46:28 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 20:45:02 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 20:47:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 06 Oct 2023 20:47:27 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 20:47:28 GMT
USER user
# Fri, 06 Oct 2023 20:47:28 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:696a66e961f2033dcf69b003ad7faf28ed2248da58efa1c08a9d496739a8eeeb`  
		Last Modified: Wed, 20 Sep 2023 08:49:51 GMT  
		Size: 33.1 MB (33119461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30054596536297b2e58930c4fe17cb3dd9a484e48310a73810d633fb399b2ea4`  
		Last Modified: Wed, 20 Sep 2023 11:48:21 GMT  
		Size: 18.8 MB (18754188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53547fc5d9551d1c1a1f2ccd6a7125ea312eac162cb9f63b4cf854af65c77212`  
		Last Modified: Wed, 20 Sep 2023 11:48:14 GMT  
		Size: 3.4 KB (3376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c58b6669e0fac3c777f89f1c775613c7c4b79937cdbaa4f03d84f4779088902`  
		Last Modified: Fri, 06 Oct 2023 20:48:39 GMT  
		Size: 37.0 MB (37024089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-bookworm` - linux; s390x

```console
$ docker pull irssi@sha256:adf3bc216988808a8cd8bc19d6474ceae3e63c68d9fb35a403ebc2880dc00605
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.4 MB (80399807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4a91ab3027978ac40b17ec8bcc5ed457b28d8b316732dafa175ccc524171687`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Sep 2023 02:54:26 GMT
ADD file:6ed982ad3e8566d63315a27a81b33069910952aef4b2d3e0b607bd2caeac7ca4 in / 
# Wed, 20 Sep 2023 02:54:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 08:50:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 08:50:11 GMT
ENV HOME=/home/user
# Wed, 20 Sep 2023 08:50:11 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Sep 2023 08:50:12 GMT
ENV LANG=C.UTF-8
# Tue, 10 Oct 2023 02:24:14 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 10 Oct 2023 02:34:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 10 Oct 2023 02:34:37 GMT
WORKDIR /home/user
# Tue, 10 Oct 2023 02:34:37 GMT
USER user
# Tue, 10 Oct 2023 02:34:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:26dcff366e33abcf08b812052a4c12496aa406aa267655e984aa7a84ca254cd8`  
		Last Modified: Wed, 20 Sep 2023 02:59:47 GMT  
		Size: 27.5 MB (27489966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9ab36ca6d32a38244529fb5d1341f679d66a581da57bc1e46bae74a2dac076`  
		Last Modified: Wed, 20 Sep 2023 08:51:27 GMT  
		Size: 18.2 MB (18205945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537016b33e97a91c754da6fb3df713bc111e51fdbd9e9967edfca9572cb96401`  
		Last Modified: Wed, 20 Sep 2023 08:51:24 GMT  
		Size: 3.4 KB (3372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f9e3389f5957a7bcdb6592475907b2611f851e3057e46ba4aa3c7143958e7b`  
		Last Modified: Tue, 10 Oct 2023 02:35:44 GMT  
		Size: 34.7 MB (34700524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:alpine`

```console
$ docker pull irssi@sha256:38d806b8883cbc7d4ce632aa3b67d6d57415a6de9e8a1e24d78b5fa0dd4eb40c
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
$ docker pull irssi@sha256:1ee6ea9617f00ef85aec02096aeee93e253c1fce4f559a3739175f1412110887
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18840008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a7066a07c9e35db2f3641c82d1b1599ebb7ecfbba2d78659f3093927b81c6f9`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:07:22 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 23:07:22 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 23:07:23 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 23:07:23 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 20:05:43 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 20:06:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 20:06:02 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 20:06:02 GMT
USER user
# Fri, 06 Oct 2023 20:06:02 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af553cbaa1665f3df3ff9ed6df3fc8fdeef915391198875444aee02cb0f1dba`  
		Last Modified: Thu, 28 Sep 2023 23:08:01 GMT  
		Size: 9.6 MB (9638068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475821153744984a56837800be5e45c520da1740ad0e9e56b1a27abb64ab5677`  
		Last Modified: Thu, 28 Sep 2023 23:07:59 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6870b695db89ae46f18ed0a5ea51ba2cb82240d1c5b1c5219a7030798a3f67`  
		Last Modified: Fri, 06 Oct 2023 20:06:47 GMT  
		Size: 5.8 MB (5798688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:7118fc38d54f6deb6a8782357883da4a4cf756bdbfad659c9c1e763250c48d28
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17664781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:012fe6e595cbd84ddedfb4904315ce7f3714991ff90335a481bd48c1252e419c`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:01:23 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:01:24 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:01:24 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:01:24 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 18:54:46 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 18:55:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 18:55:03 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 18:55:03 GMT
USER user
# Fri, 06 Oct 2023 18:55:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:152af5fc5e35a15ab7dff7175a3d682681efedcdd033b4b6ba5e65c50b0ec64f`  
		Last Modified: Thu, 28 Sep 2023 22:01:58 GMT  
		Size: 8.9 MB (8873701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e78ce7c600d11081aaabe6fe5d3d25a6badae1aaa32d490a392cb1c418e0a4`  
		Last Modified: Thu, 28 Sep 2023 22:01:56 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1971284431ad2c2d645075809b4b98b4cf9f9e16ed619f22e95078036b79b731`  
		Last Modified: Fri, 06 Oct 2023 18:55:15 GMT  
		Size: 5.6 MB (5644504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:6553e184e6f2c2417e9f000d0234179c8c8a752d02eb3f2f0b26c675a256fe75
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16994937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0965965700d10cee279de650a20af25276316e23dcc59c4092e271285e7133ed`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:32:29 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 29 Sep 2023 00:32:30 GMT
ENV HOME=/home/user
# Fri, 29 Sep 2023 00:32:30 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 29 Sep 2023 00:32:30 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 19:06:51 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 19:07:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 19:07:06 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 19:07:07 GMT
USER user
# Fri, 06 Oct 2023 19:07:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666541fade74dbbeba8bc1dc2a6f59e496ee2556c1694f8d97e154861211eb4a`  
		Last Modified: Fri, 29 Sep 2023 00:33:18 GMT  
		Size: 8.7 MB (8713773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6786d679f064e76ebc61ea937d53f08e38f578e494b4f72907c4e1886737ccfa`  
		Last Modified: Fri, 29 Sep 2023 00:33:15 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c623f5de44c876517872695b3ea33e2cd0afd3becbd2ef6e84b03a5dacef1ef`  
		Last Modified: Fri, 06 Oct 2023 19:07:49 GMT  
		Size: 5.4 MB (5379973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:8e84ebd4f06676afeeff5d3df76c54b494e9225ad08af34c22405bbb1dfac624
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18715109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4acd348d9659d9e55521ba8e049504b24acb95e989e3c60ef45ce22819d3201c`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:57:36 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 21:57:36 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 21:57:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 21:57:36 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 18:51:05 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 18:51:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 18:51:19 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 18:51:19 GMT
USER user
# Fri, 06 Oct 2023 18:51:19 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb98c09201d772cdbd8ebf3b77e3767ba0112bb407e3fa992d4a5e162065862`  
		Last Modified: Thu, 28 Sep 2023 21:58:15 GMT  
		Size: 9.7 MB (9667003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3eb447534379436f487e6d6e2a8bfe8d3f4a55aaf3e65cd8c162ce04b733398`  
		Last Modified: Thu, 28 Sep 2023 21:58:14 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8285f819417a3875bfc576dd902248316d6bc296fa13316b6e8b1a5193ee0005`  
		Last Modified: Fri, 06 Oct 2023 18:51:59 GMT  
		Size: 5.7 MB (5714992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; 386

```console
$ docker pull irssi@sha256:69515832cd89cf3cc8728b14b7d7d45807fdbec718333af24fc6bf5a8278c54e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.9 MB (17949510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db319b5e7991efcb54c8e037e2cf8bf425d3120b5c5db3df57a4340e246f33dc`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:21:39 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:21:39 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:21:40 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:21:40 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 19:04:21 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 19:04:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 19:04:58 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 19:04:58 GMT
USER user
# Fri, 06 Oct 2023 19:04:58 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbc2dcf799f84aca231b4b6ee2ee6a7a58c3d7b06552d33525458178ce175e2`  
		Last Modified: Thu, 28 Sep 2023 22:22:42 GMT  
		Size: 8.9 MB (8896304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651ec124ac1e46e7e92bc912dfd7308d68d99665be7a2f45460942974926a5b1`  
		Last Modified: Thu, 28 Sep 2023 22:22:39 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a9a322c02a4abf355ad95df55379c7b4d60eba24e72dc90494c80090a1b592`  
		Last Modified: Fri, 06 Oct 2023 19:05:47 GMT  
		Size: 5.8 MB (5816163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:ff90811e849a6fab02c5de90bc84e4c443e3f3f0bb00de9e349725aa44244725
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19108084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c796f660963a32e2c420da0b32b935efdc163713b712139b85e90641d5cc03b2`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:30:38 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:30:40 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:30:41 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:30:42 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 20:47:41 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 20:48:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 20:48:10 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 20:48:10 GMT
USER user
# Fri, 06 Oct 2023 20:48:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765c74d616c6113799971e0b6fb6422b9d4f661cf327745b094cf89369df5fd4`  
		Last Modified: Thu, 28 Sep 2023 22:31:32 GMT  
		Size: 9.7 MB (9727392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfad26be399d4cd09dd2d4252d711e7870345b952b27faeb6f911e9ca449205b`  
		Last Modified: Thu, 28 Sep 2023 22:31:28 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a22d5c7ff0996c5ff524bb74b55e5db4d4a6f8d9bf364cea4a9a40c5ac4455d`  
		Last Modified: Fri, 06 Oct 2023 20:49:04 GMT  
		Size: 6.0 MB (6032900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; s390x

```console
$ docker pull irssi@sha256:079255c123c85c24159e85a1eaf32b4e29a6d6a2e5f78f4d91eafa4e8a1678d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19110918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9b0678fe28100c4b753e58afa0b56102e537a694723ae5d01836a4dceeb40a3`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:18:20 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:18:21 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:18:22 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:18:22 GMT
ENV LANG=C.UTF-8
# Tue, 10 Oct 2023 02:34:46 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 10 Oct 2023 02:35:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 10 Oct 2023 02:35:16 GMT
WORKDIR /home/user
# Tue, 10 Oct 2023 02:35:16 GMT
USER user
# Tue, 10 Oct 2023 02:35:16 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91051e7453a3fcb401f58424e77fa5aa5ee6fee0cca8a5a32646f89a65360ce3`  
		Last Modified: Thu, 28 Sep 2023 22:19:09 GMT  
		Size: 10.1 MB (10078961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c731adf381a8e9331a2fea37d34da20a1359a905c7d7ccf7f166f464e39e5b42`  
		Last Modified: Thu, 28 Sep 2023 22:19:07 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adecf7d94f7048c67fd6041522959d98bf86eb9514cc1b44ede5da69ba7925a5`  
		Last Modified: Tue, 10 Oct 2023 02:37:07 GMT  
		Size: 5.8 MB (5815570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:alpine3.18`

```console
$ docker pull irssi@sha256:38d806b8883cbc7d4ce632aa3b67d6d57415a6de9e8a1e24d78b5fa0dd4eb40c
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
$ docker pull irssi@sha256:1ee6ea9617f00ef85aec02096aeee93e253c1fce4f559a3739175f1412110887
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18840008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a7066a07c9e35db2f3641c82d1b1599ebb7ecfbba2d78659f3093927b81c6f9`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:07:22 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 23:07:22 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 23:07:23 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 23:07:23 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 20:05:43 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 20:06:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 20:06:02 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 20:06:02 GMT
USER user
# Fri, 06 Oct 2023 20:06:02 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af553cbaa1665f3df3ff9ed6df3fc8fdeef915391198875444aee02cb0f1dba`  
		Last Modified: Thu, 28 Sep 2023 23:08:01 GMT  
		Size: 9.6 MB (9638068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475821153744984a56837800be5e45c520da1740ad0e9e56b1a27abb64ab5677`  
		Last Modified: Thu, 28 Sep 2023 23:07:59 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6870b695db89ae46f18ed0a5ea51ba2cb82240d1c5b1c5219a7030798a3f67`  
		Last Modified: Fri, 06 Oct 2023 20:06:47 GMT  
		Size: 5.8 MB (5798688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine3.18` - linux; arm variant v6

```console
$ docker pull irssi@sha256:7118fc38d54f6deb6a8782357883da4a4cf756bdbfad659c9c1e763250c48d28
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17664781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:012fe6e595cbd84ddedfb4904315ce7f3714991ff90335a481bd48c1252e419c`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:01:23 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:01:24 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:01:24 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:01:24 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 18:54:46 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 18:55:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 18:55:03 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 18:55:03 GMT
USER user
# Fri, 06 Oct 2023 18:55:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:152af5fc5e35a15ab7dff7175a3d682681efedcdd033b4b6ba5e65c50b0ec64f`  
		Last Modified: Thu, 28 Sep 2023 22:01:58 GMT  
		Size: 8.9 MB (8873701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e78ce7c600d11081aaabe6fe5d3d25a6badae1aaa32d490a392cb1c418e0a4`  
		Last Modified: Thu, 28 Sep 2023 22:01:56 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1971284431ad2c2d645075809b4b98b4cf9f9e16ed619f22e95078036b79b731`  
		Last Modified: Fri, 06 Oct 2023 18:55:15 GMT  
		Size: 5.6 MB (5644504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine3.18` - linux; arm variant v7

```console
$ docker pull irssi@sha256:6553e184e6f2c2417e9f000d0234179c8c8a752d02eb3f2f0b26c675a256fe75
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16994937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0965965700d10cee279de650a20af25276316e23dcc59c4092e271285e7133ed`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:32:29 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 29 Sep 2023 00:32:30 GMT
ENV HOME=/home/user
# Fri, 29 Sep 2023 00:32:30 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 29 Sep 2023 00:32:30 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 19:06:51 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 19:07:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 19:07:06 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 19:07:07 GMT
USER user
# Fri, 06 Oct 2023 19:07:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666541fade74dbbeba8bc1dc2a6f59e496ee2556c1694f8d97e154861211eb4a`  
		Last Modified: Fri, 29 Sep 2023 00:33:18 GMT  
		Size: 8.7 MB (8713773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6786d679f064e76ebc61ea937d53f08e38f578e494b4f72907c4e1886737ccfa`  
		Last Modified: Fri, 29 Sep 2023 00:33:15 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c623f5de44c876517872695b3ea33e2cd0afd3becbd2ef6e84b03a5dacef1ef`  
		Last Modified: Fri, 06 Oct 2023 19:07:49 GMT  
		Size: 5.4 MB (5379973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine3.18` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:8e84ebd4f06676afeeff5d3df76c54b494e9225ad08af34c22405bbb1dfac624
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18715109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4acd348d9659d9e55521ba8e049504b24acb95e989e3c60ef45ce22819d3201c`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:57:36 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 21:57:36 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 21:57:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 21:57:36 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 18:51:05 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 18:51:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 18:51:19 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 18:51:19 GMT
USER user
# Fri, 06 Oct 2023 18:51:19 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb98c09201d772cdbd8ebf3b77e3767ba0112bb407e3fa992d4a5e162065862`  
		Last Modified: Thu, 28 Sep 2023 21:58:15 GMT  
		Size: 9.7 MB (9667003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3eb447534379436f487e6d6e2a8bfe8d3f4a55aaf3e65cd8c162ce04b733398`  
		Last Modified: Thu, 28 Sep 2023 21:58:14 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8285f819417a3875bfc576dd902248316d6bc296fa13316b6e8b1a5193ee0005`  
		Last Modified: Fri, 06 Oct 2023 18:51:59 GMT  
		Size: 5.7 MB (5714992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine3.18` - linux; 386

```console
$ docker pull irssi@sha256:69515832cd89cf3cc8728b14b7d7d45807fdbec718333af24fc6bf5a8278c54e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.9 MB (17949510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db319b5e7991efcb54c8e037e2cf8bf425d3120b5c5db3df57a4340e246f33dc`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:21:39 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:21:39 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:21:40 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:21:40 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 19:04:21 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 19:04:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 19:04:58 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 19:04:58 GMT
USER user
# Fri, 06 Oct 2023 19:04:58 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbc2dcf799f84aca231b4b6ee2ee6a7a58c3d7b06552d33525458178ce175e2`  
		Last Modified: Thu, 28 Sep 2023 22:22:42 GMT  
		Size: 8.9 MB (8896304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651ec124ac1e46e7e92bc912dfd7308d68d99665be7a2f45460942974926a5b1`  
		Last Modified: Thu, 28 Sep 2023 22:22:39 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a9a322c02a4abf355ad95df55379c7b4d60eba24e72dc90494c80090a1b592`  
		Last Modified: Fri, 06 Oct 2023 19:05:47 GMT  
		Size: 5.8 MB (5816163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine3.18` - linux; ppc64le

```console
$ docker pull irssi@sha256:ff90811e849a6fab02c5de90bc84e4c443e3f3f0bb00de9e349725aa44244725
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19108084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c796f660963a32e2c420da0b32b935efdc163713b712139b85e90641d5cc03b2`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:30:38 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:30:40 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:30:41 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:30:42 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 20:47:41 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 20:48:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 06 Oct 2023 20:48:10 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 20:48:10 GMT
USER user
# Fri, 06 Oct 2023 20:48:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765c74d616c6113799971e0b6fb6422b9d4f661cf327745b094cf89369df5fd4`  
		Last Modified: Thu, 28 Sep 2023 22:31:32 GMT  
		Size: 9.7 MB (9727392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfad26be399d4cd09dd2d4252d711e7870345b952b27faeb6f911e9ca449205b`  
		Last Modified: Thu, 28 Sep 2023 22:31:28 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a22d5c7ff0996c5ff524bb74b55e5db4d4a6f8d9bf364cea4a9a40c5ac4455d`  
		Last Modified: Fri, 06 Oct 2023 20:49:04 GMT  
		Size: 6.0 MB (6032900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine3.18` - linux; s390x

```console
$ docker pull irssi@sha256:079255c123c85c24159e85a1eaf32b4e29a6d6a2e5f78f4d91eafa4e8a1678d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19110918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9b0678fe28100c4b753e58afa0b56102e537a694723ae5d01836a4dceeb40a3`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:18:20 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 28 Sep 2023 22:18:21 GMT
ENV HOME=/home/user
# Thu, 28 Sep 2023 22:18:22 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 28 Sep 2023 22:18:22 GMT
ENV LANG=C.UTF-8
# Tue, 10 Oct 2023 02:34:46 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 10 Oct 2023 02:35:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 10 Oct 2023 02:35:16 GMT
WORKDIR /home/user
# Tue, 10 Oct 2023 02:35:16 GMT
USER user
# Tue, 10 Oct 2023 02:35:16 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91051e7453a3fcb401f58424e77fa5aa5ee6fee0cca8a5a32646f89a65360ce3`  
		Last Modified: Thu, 28 Sep 2023 22:19:09 GMT  
		Size: 10.1 MB (10078961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c731adf381a8e9331a2fea37d34da20a1359a905c7d7ccf7f166f464e39e5b42`  
		Last Modified: Thu, 28 Sep 2023 22:19:07 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adecf7d94f7048c67fd6041522959d98bf86eb9514cc1b44ede5da69ba7925a5`  
		Last Modified: Tue, 10 Oct 2023 02:37:07 GMT  
		Size: 5.8 MB (5815570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:bookworm`

```console
$ docker pull irssi@sha256:8cd808235b32389f3bdc481a70654f08582189b7eaf51633adda044135312271
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
$ docker pull irssi@sha256:44c777babe5699a8971eb5367dbd411e6eee21e8ed16a4ff7613b037af6f5ceb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76090686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33f1ddb1eb8c8968dc461872fe15016c247b14190fdf74279962255735dca784`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 20:24:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 20:24:47 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 20:24:48 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 20:24:48 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 20:24:48 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 20:25:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 20:25:28 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 20:25:28 GMT
USER user
# Wed, 11 Oct 2023 20:25:28 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3853166e834fc2c48aedc55edbe9e1f882a3d7949f309a967e85dc49845a888c`  
		Last Modified: Wed, 11 Oct 2023 20:26:01 GMT  
		Size: 18.3 MB (18258013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8712f3c7bad7100c6d37fcf7e3c5002d8d7678548bf0892ca23e4904b9c066`  
		Last Modified: Wed, 11 Oct 2023 20:25:57 GMT  
		Size: 3.4 KB (3374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8f213a94fe9accb515298e6053d1ff437041b2b2033156092b5365c7791601`  
		Last Modified: Wed, 11 Oct 2023 20:26:02 GMT  
		Size: 28.7 MB (28679425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:bookworm` - linux; arm variant v5

```console
$ docker pull irssi@sha256:b49414becae5081d26d6eff6e214ce40e04aecbd6aa5ba63ebfda941497dd5a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70342849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a65606ee0e4cc323ad482840a06d50e1ba7e9d69faf54c5049c7c1fa6332a3f`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:43 GMT
ADD file:8c43adb3245fc6f2b10aa5a86c850db5dcf3515eaf7e46630922fe21f806bd2a in / 
# Wed, 11 Oct 2023 17:37:43 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:00:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:00:56 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 18:00:57 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 18:00:57 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 18:00:57 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 18:01:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 18:01:42 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 18:01:42 GMT
USER user
# Wed, 11 Oct 2023 18:01:42 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:904e6393ef1ee28b37171369eb4f7cb04714631c711799819fccb83886bd212b`  
		Last Modified: Wed, 11 Oct 2023 17:40:47 GMT  
		Size: 26.9 MB (26922150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107efe7ce893352f65dfb345d40ccf416fdb609825df68a2b3f8e02e6a0a3d56`  
		Last Modified: Wed, 11 Oct 2023 18:01:58 GMT  
		Size: 17.1 MB (17092623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317d45cff4b023ded2635c88d1801ee2d5e8911f9a7098ecc25aa7ef5949d566`  
		Last Modified: Wed, 11 Oct 2023 18:01:54 GMT  
		Size: 3.4 KB (3371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be15a5c4dd41a9defc1496cb7afa89616c007835aba62d34d7e38258f865e8e`  
		Last Modified: Wed, 11 Oct 2023 18:01:59 GMT  
		Size: 26.3 MB (26324705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:bookworm` - linux; arm variant v7

```console
$ docker pull irssi@sha256:9acb53b918ce7218355b74aed1213e71f5126277b32e948808b45ae3424df9ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66653393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0fdfeb17d52fb8aecbbeffe1311c2184bb7fa3da76896c739fd02fe736d719b`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:12:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:12:48 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 19:12:48 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 19:12:48 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 19:12:48 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 19:13:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 19:13:29 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 19:13:29 GMT
USER user
# Wed, 11 Oct 2023 19:13:29 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5baaee56a9498d8e72131adb171dee5671edf350e3f83e1154b2d1651115385`  
		Last Modified: Wed, 11 Oct 2023 19:13:56 GMT  
		Size: 16.7 MB (16678815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ccc912053095badfc35dbd2f166cc2477b07f22b2a8ec2c38183c5c0277873d`  
		Last Modified: Wed, 11 Oct 2023 19:13:52 GMT  
		Size: 3.4 KB (3377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b622859b61c28bc5dbc1cca27e70e2473d2425378c3e3ba112546f6b0d1c70eb`  
		Last Modified: Wed, 11 Oct 2023 19:13:57 GMT  
		Size: 25.2 MB (25222276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:bookworm` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:8edaae578605997a74c4364d46c96a3867c2054543a60b2f724913b6a4fa6754
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.8 MB (80788768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f32fcd8186f4b8d4af0b40f507e8f94ea2bfbd86b7fc41276659e2e7ab7ddfe`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:13 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Wed, 20 Sep 2023 02:44:14 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 11:22:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:22:14 GMT
ENV HOME=/home/user
# Wed, 20 Sep 2023 11:22:14 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Sep 2023 11:22:14 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 18:50:25 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 18:51:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 06 Oct 2023 18:51:03 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 18:51:03 GMT
USER user
# Fri, 06 Oct 2023 18:51:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e17a035c22a6860e7c120c60f7d2f84bf9834e6ebdef94bf9b9f044d9c93d69`  
		Last Modified: Wed, 20 Sep 2023 11:23:19 GMT  
		Size: 18.0 MB (18024704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f81b6709eee0366d7cb53c2306da1edae2817e93e99cdd35e7f36aa5e866c8e`  
		Last Modified: Wed, 20 Sep 2023 11:23:16 GMT  
		Size: 3.4 KB (3373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913009f5d7ce3f00561b3220a723826b84895260169d5eb98399e5b5e556cf3f`  
		Last Modified: Fri, 06 Oct 2023 18:51:38 GMT  
		Size: 33.6 MB (33603470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:bookworm` - linux; 386

```console
$ docker pull irssi@sha256:63f96f9a3864f944849735f8de61f7b79f6e0523602340eb8af73f8e2bcca8e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76522799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7838aa7df5bd597e8394793aa77df15853878793a687685bf46ccbd60588a43`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:42 GMT
ADD file:31318c1b1f05d559cce42f5b12eef97d916932217e0b987fb07c0fc11bf0a14a in / 
# Wed, 11 Oct 2023 17:40:42 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:31:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:31:53 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 21:31:54 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 21:31:54 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 21:31:54 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 21:32:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 21:32:48 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 21:32:48 GMT
USER user
# Wed, 11 Oct 2023 21:32:48 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b27d0f1369837277a82877763487cdd2535037988fc27e16f11cf74e103ae4cd`  
		Last Modified: Wed, 11 Oct 2023 17:45:31 GMT  
		Size: 30.2 MB (30164118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5aabddc89a058b8444274e0ab7a7604dd6b19276ca05209051a7bd05996a97`  
		Last Modified: Wed, 11 Oct 2023 21:33:17 GMT  
		Size: 17.8 MB (17788766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674da66b6a6ab4b333d0fbf0c2731e6fcdfc0628ea6463fe2c8c298c2e4f5022`  
		Last Modified: Wed, 11 Oct 2023 21:33:10 GMT  
		Size: 3.4 KB (3373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be398748b24b800d52f805e4b55221b65ab68f63fa172620395b27d97f4cef62`  
		Last Modified: Wed, 11 Oct 2023 21:33:18 GMT  
		Size: 28.6 MB (28566542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:bookworm` - linux; mips64le

```console
$ docker pull irssi@sha256:4622ced3be5a3c4e803c2594eaf6c13299ae0a9f6da133fcac361f6b46a6f62e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73893583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80f80aac1fac6ff7d115cd8d97db39021a1be94a7121a4fe70787e480a3d445f`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:49:32 GMT
ADD file:2abda0a72972a417d4f7f530ca8fa1ee7e85e25d4015fd4e70acf903cfd96d3d in / 
# Wed, 11 Oct 2023 17:49:36 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 20:05:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 20:05:10 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 20:05:16 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 20:05:19 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 20:05:23 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 20:09:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 20:09:27 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 20:09:31 GMT
USER user
# Wed, 11 Oct 2023 20:09:35 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f11870ec99d788b4b160d9f3f4c0a79904290083d8930b26e5d13579226e07f0`  
		Last Modified: Wed, 11 Oct 2023 18:00:43 GMT  
		Size: 29.1 MB (29142026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1f47bc243f41e66258f22f77a6d27afd7c49447f4867ab03737c1c00e055e5`  
		Last Modified: Wed, 11 Oct 2023 20:10:17 GMT  
		Size: 16.7 MB (16741536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528d2b189bddab2a8763fd33d4deba2040b0c2d28337893be13d77d751b745dd`  
		Last Modified: Wed, 11 Oct 2023 20:10:01 GMT  
		Size: 3.3 KB (3299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299c20205b3210d510f4fcb1678d9093fca2d25452b80816b0da15049cbb41d2`  
		Last Modified: Wed, 11 Oct 2023 20:10:22 GMT  
		Size: 28.0 MB (28006722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:bookworm` - linux; ppc64le

```console
$ docker pull irssi@sha256:fe9ad83e93b168870c785b041cfbe670b128f99b8ed3e270c8d50bc9de07c5a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.9 MB (88901114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:132c9d6a4750e943c7033db5a5253d77f49da8681b15cc3af59b0459530997d5`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Sep 2023 07:52:54 GMT
ADD file:9a37b479e68a0d18babbef8dd04d09a0e6844a0080876d14144a34bfd9d0897a in / 
# Wed, 20 Sep 2023 07:52:55 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 11:46:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:46:25 GMT
ENV HOME=/home/user
# Wed, 20 Sep 2023 11:46:27 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Sep 2023 11:46:28 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 20:45:02 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 20:47:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 06 Oct 2023 20:47:27 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 20:47:28 GMT
USER user
# Fri, 06 Oct 2023 20:47:28 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:696a66e961f2033dcf69b003ad7faf28ed2248da58efa1c08a9d496739a8eeeb`  
		Last Modified: Wed, 20 Sep 2023 08:49:51 GMT  
		Size: 33.1 MB (33119461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30054596536297b2e58930c4fe17cb3dd9a484e48310a73810d633fb399b2ea4`  
		Last Modified: Wed, 20 Sep 2023 11:48:21 GMT  
		Size: 18.8 MB (18754188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53547fc5d9551d1c1a1f2ccd6a7125ea312eac162cb9f63b4cf854af65c77212`  
		Last Modified: Wed, 20 Sep 2023 11:48:14 GMT  
		Size: 3.4 KB (3376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c58b6669e0fac3c777f89f1c775613c7c4b79937cdbaa4f03d84f4779088902`  
		Last Modified: Fri, 06 Oct 2023 20:48:39 GMT  
		Size: 37.0 MB (37024089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:bookworm` - linux; s390x

```console
$ docker pull irssi@sha256:adf3bc216988808a8cd8bc19d6474ceae3e63c68d9fb35a403ebc2880dc00605
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.4 MB (80399807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4a91ab3027978ac40b17ec8bcc5ed457b28d8b316732dafa175ccc524171687`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Sep 2023 02:54:26 GMT
ADD file:6ed982ad3e8566d63315a27a81b33069910952aef4b2d3e0b607bd2caeac7ca4 in / 
# Wed, 20 Sep 2023 02:54:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 08:50:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 08:50:11 GMT
ENV HOME=/home/user
# Wed, 20 Sep 2023 08:50:11 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Sep 2023 08:50:12 GMT
ENV LANG=C.UTF-8
# Tue, 10 Oct 2023 02:24:14 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 10 Oct 2023 02:34:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 10 Oct 2023 02:34:37 GMT
WORKDIR /home/user
# Tue, 10 Oct 2023 02:34:37 GMT
USER user
# Tue, 10 Oct 2023 02:34:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:26dcff366e33abcf08b812052a4c12496aa406aa267655e984aa7a84ca254cd8`  
		Last Modified: Wed, 20 Sep 2023 02:59:47 GMT  
		Size: 27.5 MB (27489966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9ab36ca6d32a38244529fb5d1341f679d66a581da57bc1e46bae74a2dac076`  
		Last Modified: Wed, 20 Sep 2023 08:51:27 GMT  
		Size: 18.2 MB (18205945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537016b33e97a91c754da6fb3df713bc111e51fdbd9e9967edfca9572cb96401`  
		Last Modified: Wed, 20 Sep 2023 08:51:24 GMT  
		Size: 3.4 KB (3372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f9e3389f5957a7bcdb6592475907b2611f851e3057e46ba4aa3c7143958e7b`  
		Last Modified: Tue, 10 Oct 2023 02:35:44 GMT  
		Size: 34.7 MB (34700524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:latest`

```console
$ docker pull irssi@sha256:8cd808235b32389f3bdc481a70654f08582189b7eaf51633adda044135312271
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
$ docker pull irssi@sha256:44c777babe5699a8971eb5367dbd411e6eee21e8ed16a4ff7613b037af6f5ceb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76090686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33f1ddb1eb8c8968dc461872fe15016c247b14190fdf74279962255735dca784`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 20:24:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 20:24:47 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 20:24:48 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 20:24:48 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 20:24:48 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 20:25:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 20:25:28 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 20:25:28 GMT
USER user
# Wed, 11 Oct 2023 20:25:28 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3853166e834fc2c48aedc55edbe9e1f882a3d7949f309a967e85dc49845a888c`  
		Last Modified: Wed, 11 Oct 2023 20:26:01 GMT  
		Size: 18.3 MB (18258013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8712f3c7bad7100c6d37fcf7e3c5002d8d7678548bf0892ca23e4904b9c066`  
		Last Modified: Wed, 11 Oct 2023 20:25:57 GMT  
		Size: 3.4 KB (3374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8f213a94fe9accb515298e6053d1ff437041b2b2033156092b5365c7791601`  
		Last Modified: Wed, 11 Oct 2023 20:26:02 GMT  
		Size: 28.7 MB (28679425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm variant v5

```console
$ docker pull irssi@sha256:b49414becae5081d26d6eff6e214ce40e04aecbd6aa5ba63ebfda941497dd5a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70342849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a65606ee0e4cc323ad482840a06d50e1ba7e9d69faf54c5049c7c1fa6332a3f`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:43 GMT
ADD file:8c43adb3245fc6f2b10aa5a86c850db5dcf3515eaf7e46630922fe21f806bd2a in / 
# Wed, 11 Oct 2023 17:37:43 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:00:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:00:56 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 18:00:57 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 18:00:57 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 18:00:57 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 18:01:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 18:01:42 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 18:01:42 GMT
USER user
# Wed, 11 Oct 2023 18:01:42 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:904e6393ef1ee28b37171369eb4f7cb04714631c711799819fccb83886bd212b`  
		Last Modified: Wed, 11 Oct 2023 17:40:47 GMT  
		Size: 26.9 MB (26922150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107efe7ce893352f65dfb345d40ccf416fdb609825df68a2b3f8e02e6a0a3d56`  
		Last Modified: Wed, 11 Oct 2023 18:01:58 GMT  
		Size: 17.1 MB (17092623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317d45cff4b023ded2635c88d1801ee2d5e8911f9a7098ecc25aa7ef5949d566`  
		Last Modified: Wed, 11 Oct 2023 18:01:54 GMT  
		Size: 3.4 KB (3371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be15a5c4dd41a9defc1496cb7afa89616c007835aba62d34d7e38258f865e8e`  
		Last Modified: Wed, 11 Oct 2023 18:01:59 GMT  
		Size: 26.3 MB (26324705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm variant v7

```console
$ docker pull irssi@sha256:9acb53b918ce7218355b74aed1213e71f5126277b32e948808b45ae3424df9ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66653393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0fdfeb17d52fb8aecbbeffe1311c2184bb7fa3da76896c739fd02fe736d719b`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:12:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:12:48 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 19:12:48 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 19:12:48 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 19:12:48 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 19:13:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 19:13:29 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 19:13:29 GMT
USER user
# Wed, 11 Oct 2023 19:13:29 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5baaee56a9498d8e72131adb171dee5671edf350e3f83e1154b2d1651115385`  
		Last Modified: Wed, 11 Oct 2023 19:13:56 GMT  
		Size: 16.7 MB (16678815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ccc912053095badfc35dbd2f166cc2477b07f22b2a8ec2c38183c5c0277873d`  
		Last Modified: Wed, 11 Oct 2023 19:13:52 GMT  
		Size: 3.4 KB (3377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b622859b61c28bc5dbc1cca27e70e2473d2425378c3e3ba112546f6b0d1c70eb`  
		Last Modified: Wed, 11 Oct 2023 19:13:57 GMT  
		Size: 25.2 MB (25222276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:8edaae578605997a74c4364d46c96a3867c2054543a60b2f724913b6a4fa6754
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.8 MB (80788768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f32fcd8186f4b8d4af0b40f507e8f94ea2bfbd86b7fc41276659e2e7ab7ddfe`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:13 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Wed, 20 Sep 2023 02:44:14 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 11:22:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:22:14 GMT
ENV HOME=/home/user
# Wed, 20 Sep 2023 11:22:14 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Sep 2023 11:22:14 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 18:50:25 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 18:51:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 06 Oct 2023 18:51:03 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 18:51:03 GMT
USER user
# Fri, 06 Oct 2023 18:51:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e17a035c22a6860e7c120c60f7d2f84bf9834e6ebdef94bf9b9f044d9c93d69`  
		Last Modified: Wed, 20 Sep 2023 11:23:19 GMT  
		Size: 18.0 MB (18024704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f81b6709eee0366d7cb53c2306da1edae2817e93e99cdd35e7f36aa5e866c8e`  
		Last Modified: Wed, 20 Sep 2023 11:23:16 GMT  
		Size: 3.4 KB (3373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913009f5d7ce3f00561b3220a723826b84895260169d5eb98399e5b5e556cf3f`  
		Last Modified: Fri, 06 Oct 2023 18:51:38 GMT  
		Size: 33.6 MB (33603470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; 386

```console
$ docker pull irssi@sha256:63f96f9a3864f944849735f8de61f7b79f6e0523602340eb8af73f8e2bcca8e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76522799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7838aa7df5bd597e8394793aa77df15853878793a687685bf46ccbd60588a43`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:42 GMT
ADD file:31318c1b1f05d559cce42f5b12eef97d916932217e0b987fb07c0fc11bf0a14a in / 
# Wed, 11 Oct 2023 17:40:42 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:31:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:31:53 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 21:31:54 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 21:31:54 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 21:31:54 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 21:32:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 21:32:48 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 21:32:48 GMT
USER user
# Wed, 11 Oct 2023 21:32:48 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b27d0f1369837277a82877763487cdd2535037988fc27e16f11cf74e103ae4cd`  
		Last Modified: Wed, 11 Oct 2023 17:45:31 GMT  
		Size: 30.2 MB (30164118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5aabddc89a058b8444274e0ab7a7604dd6b19276ca05209051a7bd05996a97`  
		Last Modified: Wed, 11 Oct 2023 21:33:17 GMT  
		Size: 17.8 MB (17788766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674da66b6a6ab4b333d0fbf0c2731e6fcdfc0628ea6463fe2c8c298c2e4f5022`  
		Last Modified: Wed, 11 Oct 2023 21:33:10 GMT  
		Size: 3.4 KB (3373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be398748b24b800d52f805e4b55221b65ab68f63fa172620395b27d97f4cef62`  
		Last Modified: Wed, 11 Oct 2023 21:33:18 GMT  
		Size: 28.6 MB (28566542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; mips64le

```console
$ docker pull irssi@sha256:4622ced3be5a3c4e803c2594eaf6c13299ae0a9f6da133fcac361f6b46a6f62e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73893583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80f80aac1fac6ff7d115cd8d97db39021a1be94a7121a4fe70787e480a3d445f`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 Oct 2023 17:49:32 GMT
ADD file:2abda0a72972a417d4f7f530ca8fa1ee7e85e25d4015fd4e70acf903cfd96d3d in / 
# Wed, 11 Oct 2023 17:49:36 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 20:05:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 20:05:10 GMT
ENV HOME=/home/user
# Wed, 11 Oct 2023 20:05:16 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 Oct 2023 20:05:19 GMT
ENV LANG=C.UTF-8
# Wed, 11 Oct 2023 20:05:23 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 11 Oct 2023 20:09:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 Oct 2023 20:09:27 GMT
WORKDIR /home/user
# Wed, 11 Oct 2023 20:09:31 GMT
USER user
# Wed, 11 Oct 2023 20:09:35 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f11870ec99d788b4b160d9f3f4c0a79904290083d8930b26e5d13579226e07f0`  
		Last Modified: Wed, 11 Oct 2023 18:00:43 GMT  
		Size: 29.1 MB (29142026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1f47bc243f41e66258f22f77a6d27afd7c49447f4867ab03737c1c00e055e5`  
		Last Modified: Wed, 11 Oct 2023 20:10:17 GMT  
		Size: 16.7 MB (16741536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528d2b189bddab2a8763fd33d4deba2040b0c2d28337893be13d77d751b745dd`  
		Last Modified: Wed, 11 Oct 2023 20:10:01 GMT  
		Size: 3.3 KB (3299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299c20205b3210d510f4fcb1678d9093fca2d25452b80816b0da15049cbb41d2`  
		Last Modified: Wed, 11 Oct 2023 20:10:22 GMT  
		Size: 28.0 MB (28006722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; ppc64le

```console
$ docker pull irssi@sha256:fe9ad83e93b168870c785b041cfbe670b128f99b8ed3e270c8d50bc9de07c5a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.9 MB (88901114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:132c9d6a4750e943c7033db5a5253d77f49da8681b15cc3af59b0459530997d5`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Sep 2023 07:52:54 GMT
ADD file:9a37b479e68a0d18babbef8dd04d09a0e6844a0080876d14144a34bfd9d0897a in / 
# Wed, 20 Sep 2023 07:52:55 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 11:46:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:46:25 GMT
ENV HOME=/home/user
# Wed, 20 Sep 2023 11:46:27 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Sep 2023 11:46:28 GMT
ENV LANG=C.UTF-8
# Fri, 06 Oct 2023 20:45:02 GMT
ENV IRSSI_VERSION=1.4.5
# Fri, 06 Oct 2023 20:47:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 06 Oct 2023 20:47:27 GMT
WORKDIR /home/user
# Fri, 06 Oct 2023 20:47:28 GMT
USER user
# Fri, 06 Oct 2023 20:47:28 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:696a66e961f2033dcf69b003ad7faf28ed2248da58efa1c08a9d496739a8eeeb`  
		Last Modified: Wed, 20 Sep 2023 08:49:51 GMT  
		Size: 33.1 MB (33119461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30054596536297b2e58930c4fe17cb3dd9a484e48310a73810d633fb399b2ea4`  
		Last Modified: Wed, 20 Sep 2023 11:48:21 GMT  
		Size: 18.8 MB (18754188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53547fc5d9551d1c1a1f2ccd6a7125ea312eac162cb9f63b4cf854af65c77212`  
		Last Modified: Wed, 20 Sep 2023 11:48:14 GMT  
		Size: 3.4 KB (3376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c58b6669e0fac3c777f89f1c775613c7c4b79937cdbaa4f03d84f4779088902`  
		Last Modified: Fri, 06 Oct 2023 20:48:39 GMT  
		Size: 37.0 MB (37024089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; s390x

```console
$ docker pull irssi@sha256:adf3bc216988808a8cd8bc19d6474ceae3e63c68d9fb35a403ebc2880dc00605
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.4 MB (80399807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4a91ab3027978ac40b17ec8bcc5ed457b28d8b316732dafa175ccc524171687`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Sep 2023 02:54:26 GMT
ADD file:6ed982ad3e8566d63315a27a81b33069910952aef4b2d3e0b607bd2caeac7ca4 in / 
# Wed, 20 Sep 2023 02:54:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 08:50:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 08:50:11 GMT
ENV HOME=/home/user
# Wed, 20 Sep 2023 08:50:11 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Sep 2023 08:50:12 GMT
ENV LANG=C.UTF-8
# Tue, 10 Oct 2023 02:24:14 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 10 Oct 2023 02:34:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 10 Oct 2023 02:34:37 GMT
WORKDIR /home/user
# Tue, 10 Oct 2023 02:34:37 GMT
USER user
# Tue, 10 Oct 2023 02:34:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:26dcff366e33abcf08b812052a4c12496aa406aa267655e984aa7a84ca254cd8`  
		Last Modified: Wed, 20 Sep 2023 02:59:47 GMT  
		Size: 27.5 MB (27489966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9ab36ca6d32a38244529fb5d1341f679d66a581da57bc1e46bae74a2dac076`  
		Last Modified: Wed, 20 Sep 2023 08:51:27 GMT  
		Size: 18.2 MB (18205945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537016b33e97a91c754da6fb3df713bc111e51fdbd9e9967edfca9572cb96401`  
		Last Modified: Wed, 20 Sep 2023 08:51:24 GMT  
		Size: 3.4 KB (3372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f9e3389f5957a7bcdb6592475907b2611f851e3057e46ba4aa3c7143958e7b`  
		Last Modified: Tue, 10 Oct 2023 02:35:44 GMT  
		Size: 34.7 MB (34700524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
