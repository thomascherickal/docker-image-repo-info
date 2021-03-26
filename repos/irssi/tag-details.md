<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `irssi`

-	[`irssi:1`](#irssi1)
-	[`irssi:1-alpine`](#irssi1-alpine)
-	[`irssi:1.2`](#irssi12)
-	[`irssi:1.2-alpine`](#irssi12-alpine)
-	[`irssi:1.2.2`](#irssi122)
-	[`irssi:1.2.2-alpine`](#irssi122-alpine)
-	[`irssi:alpine`](#irssialpine)
-	[`irssi:latest`](#irssilatest)

## `irssi:1`

```console
$ docker pull irssi@sha256:575d68fdda2e48da8abc975a602afab57a32dcd210101706492cb6c2fe9a0bde
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
$ docker pull irssi@sha256:7d442244c3d5d97b95ac0c0ca9be95165bd30b909621e572bed3f954cbdd3389
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50568077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5911d6f3416365bd18470b92a5ceca377f1b3c9337c0c9fbaec9891141aad195`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 11:04:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 11:04:57 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 11:04:59 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 11:04:59 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 11:04:59 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 11:06:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 11:06:38 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 11:06:39 GMT
USER user
# Fri, 12 Mar 2021 11:06:39 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa82220b80b6fa32a82277cdcf2e1a8b7350d3eb49dd723043dd4dfee38a4d7c`  
		Last Modified: Fri, 12 Mar 2021 11:08:48 GMT  
		Size: 17.0 MB (17033440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cab4a877a41e1cfdc916be3c7625c0f914119e3ad2abc2ad4b159e3baa1e0e`  
		Last Modified: Fri, 12 Mar 2021 11:08:42 GMT  
		Size: 4.2 KB (4208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a6c2e5e877ecd200d4c003252a7db5a9797a0f90feeadeded09ddd3a2f1eae`  
		Last Modified: Fri, 12 Mar 2021 11:08:44 GMT  
		Size: 6.4 MB (6429428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm variant v5

```console
$ docker pull irssi@sha256:9e24e92190db23a06e2692b1a49ce3438288a26b7bd501bd58fb0f84caf11185
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46843846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7aaa632856c778560f9f55abbd065b8f2980a83ed0420f7607c9c2879be3124`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 01:52:27 GMT
ADD file:8e357182800adfe658856515726f1e012cc120349f0f305692cf50282f6d8b7b in / 
# Fri, 12 Mar 2021 01:52:29 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:50:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:50:23 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 02:50:26 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 02:50:26 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 02:50:27 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 02:52:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 02:52:15 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 02:52:16 GMT
USER user
# Fri, 12 Mar 2021 02:52:17 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:9babb1be2e38b3bddad5a4e05bb34173369ae3472c0c0d8668853011cd65969f`  
		Last Modified: Fri, 12 Mar 2021 02:02:01 GMT  
		Size: 24.8 MB (24845925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e25b60c55c4d12e692a0e8d8966b14cc0e5085187f8a343a4d84956e316ffb6`  
		Last Modified: Fri, 12 Mar 2021 02:52:43 GMT  
		Size: 15.9 MB (15931049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67829e638098b8d79aa01cad5ded7c1cb12071840410b02090c62c9f8edd7fa`  
		Last Modified: Fri, 12 Mar 2021 02:52:36 GMT  
		Size: 4.2 KB (4196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd508527cc93ad08df450347b6d21d5032a28fa0488016291c8abe88d2de5ce`  
		Last Modified: Fri, 12 Mar 2021 02:52:38 GMT  
		Size: 6.1 MB (6062676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm variant v7

```console
$ docker pull irssi@sha256:32f2605101fe727c1455d51042f015e19827a7866ddedc3d22d5ad735064ba81
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44234132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8977a6c44287eae4a76289108e4ce0b1ac7425a4f5c9b9e02d8eea74df22d92e`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 02:00:12 GMT
ADD file:123da9848f87c8ed4c5122a104b8650564c09767725916f822def7b645a019f1 in / 
# Fri, 12 Mar 2021 02:00:14 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 04:56:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 04:56:26 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 04:56:28 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 04:56:29 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 04:56:29 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 04:57:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 04:58:00 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 04:58:01 GMT
USER user
# Fri, 12 Mar 2021 04:58:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:e12d26f75fe8b7fd14712965ff5178762227d07d2151bb35fa21105ddfc4a14a`  
		Last Modified: Fri, 12 Mar 2021 02:10:28 GMT  
		Size: 22.7 MB (22709467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f1dc2c6549f399aec326fad72f414b645d8f953321c14032de6b908cb94b42`  
		Last Modified: Fri, 12 Mar 2021 04:58:35 GMT  
		Size: 15.6 MB (15590035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f0a2c1c5574bae60fc820eb688fd9317c9fb76c8fbc8127760891fb60261f65`  
		Last Modified: Fri, 12 Mar 2021 04:58:27 GMT  
		Size: 4.2 KB (4195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc5f47c56a02365fc5a6dfa4ce63062636df3340e67756c0413eaab1feed334`  
		Last Modified: Fri, 12 Mar 2021 04:58:29 GMT  
		Size: 5.9 MB (5930435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:02686cdc34ce5dd16345df7292a3064f22a074585de5547ad7e4691b5547fea9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49052058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d3942313a1f6e377d074ac70be91b98b22f099283c005a45801c8b265bce22b`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 01:53:53 GMT
ADD file:6130ddc0a939dd72c0614de4aa77de47aa16fe211274bacb31995aa1a0526164 in / 
# Fri, 12 Mar 2021 01:53:56 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 17:43:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 17:43:25 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 17:43:27 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 17:43:28 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 17:43:29 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 17:45:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 17:45:04 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 17:45:05 GMT
USER user
# Fri, 12 Mar 2021 17:45:06 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:706ee5d0a6b53d9257cbea22d8409fb22c867ab3a001c65f6b8bfd37dace0e58`  
		Last Modified: Fri, 12 Mar 2021 02:01:39 GMT  
		Size: 25.9 MB (25856512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc1a0fcfd5b5c8a6304adad324f44c13c6ebe3062940f9da8318bbbc1b57a6d`  
		Last Modified: Fri, 12 Mar 2021 17:45:35 GMT  
		Size: 16.8 MB (16803429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d79819a4c69ccab094f2aaee1ee4c383589114a44ea07437262e24e3335b026`  
		Last Modified: Fri, 12 Mar 2021 17:45:28 GMT  
		Size: 4.2 KB (4219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4834bc87f80d7b0ee15ef328f8981b1fa7cdc1e1f761286aa1e57e32fe2c2194`  
		Last Modified: Fri, 12 Mar 2021 17:45:31 GMT  
		Size: 6.4 MB (6387898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; 386

```console
$ docker pull irssi@sha256:1c1a9780a77d5593848ec9f66c0c4a1db62d6c1ab536b03499426dc3230db8aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50425172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4233b7a266ca3253ce68dd157a42b68fce5841ab7212bd92ad8c98df61c29a9d`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 01:44:27 GMT
ADD file:90c103e04bd6fe0f39733cbf8eb2d8845aed3e4fc3fd1e5c3354df69e40aa615 in / 
# Fri, 12 Mar 2021 01:44:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 21:13:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 21:13:08 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 21:13:09 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 21:13:09 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 21:13:09 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 21:14:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 21:14:46 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 21:14:46 GMT
USER user
# Fri, 12 Mar 2021 21:14:46 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:0898aa7472f57f223652846337cf862f142e109d0c039b41886e7f20c345f85e`  
		Last Modified: Fri, 12 Mar 2021 01:52:08 GMT  
		Size: 27.8 MB (27760948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7adad1dd74fcd0ecb398e894c7f8861e0f07cfc0bdb77cbc12e24b5cb793c68c`  
		Last Modified: Fri, 12 Mar 2021 21:16:47 GMT  
		Size: 16.6 MB (16558205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b2cf9a9a3e742c4c14027ae25b0d3325b123f048d89744ac861296cfdcfb46c`  
		Last Modified: Fri, 12 Mar 2021 21:16:37 GMT  
		Size: 4.2 KB (4192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c8264777e37ece315309662ef9c2042aed482ebfe6288ccebe91922fcc072fb`  
		Last Modified: Fri, 12 Mar 2021 21:16:41 GMT  
		Size: 6.1 MB (6101827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; mips64le

```console
$ docker pull irssi@sha256:11dcb1ea1f6a694137f6869a3a5d24e9c73d1d5e898b9feaf60779bc9d7ea9f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47775886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd123eb9b8194e1dce76a162a06d55a66f76c4a1947e7375174754f54dd208b9`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 02:10:02 GMT
ADD file:491c5ca15fe098b83de42861289c216c693d788a1f9e739a78acefb0cad453c8 in / 
# Fri, 12 Mar 2021 02:10:03 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 03:00:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 03:00:09 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 03:00:11 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 03:00:12 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 03:00:12 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 03:02:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 03:02:45 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 03:02:45 GMT
USER user
# Fri, 12 Mar 2021 03:02:45 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:d0b6b2cc51bdde474395b8c32ff8012e471727bba69f221cfb79b46e8283f047`  
		Last Modified: Fri, 12 Mar 2021 02:17:07 GMT  
		Size: 25.8 MB (25772338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f07eae8650e63d8e5c5c11fa467c8cb401e24859b6c3eb97d1cb4beb77ca33f`  
		Last Modified: Fri, 12 Mar 2021 03:03:23 GMT  
		Size: 15.7 MB (15709110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069673a50a0626dfb618561bcc33174f5af67375b61426deebf65feeb686a270`  
		Last Modified: Fri, 12 Mar 2021 03:03:06 GMT  
		Size: 4.2 KB (4179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0e23988c6b3499aefb8ddcbd10d127bd56e8d4c22e34889250b9602c012f9e`  
		Last Modified: Fri, 12 Mar 2021 03:03:11 GMT  
		Size: 6.3 MB (6290259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; ppc64le

```console
$ docker pull irssi@sha256:042a76fc7d37dc6e7fe106e64a43037de8d4f6162bed9362f02ce1cb46d89b05
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.7 MB (54748353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e21ad9386f16b76532f9ca7679ab7b1a1b7ae07c665005d3540d630efb08a2e`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 02:32:43 GMT
ADD file:6a0c0cfa71979cf6fdd859dce1e32582f0e55ed382b9e17b77a2001defc2c9db in / 
# Fri, 12 Mar 2021 02:32:50 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 05:21:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 05:21:53 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 05:22:19 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 05:22:33 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 05:22:47 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 05:33:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 05:33:07 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 05:33:15 GMT
USER user
# Fri, 12 Mar 2021 05:33:35 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1d686056fdac1848f4fd78ba2b335502055ffe98c79619e21d0c2fb7db95257e`  
		Last Modified: Fri, 12 Mar 2021 02:45:35 GMT  
		Size: 30.5 MB (30525728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ece5dc65262bccb6252440d8c5e1a3dca0ec3603abb9e8b49d82f97d6cb85b9`  
		Last Modified: Fri, 12 Mar 2021 05:34:13 GMT  
		Size: 17.4 MB (17437414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc49adb12fb0cd54dc637a9532fbc83cb4e037e6b2bd4e5971948ffbf5f5d8a`  
		Last Modified: Fri, 12 Mar 2021 05:34:08 GMT  
		Size: 4.2 KB (4214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559c20b0868126ced94ac9ef5df1d609e27bd8abfc99fde3a2676da11e98a227`  
		Last Modified: Fri, 12 Mar 2021 05:34:11 GMT  
		Size: 6.8 MB (6780997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; s390x

```console
$ docker pull irssi@sha256:5d0796552e1559a6f77853b1e52d7e7ae5b2a7ea5a36c11cee0ef8f99a528f74
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49012748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f31d157ba631157ab487f5b32e1ef32f016af19318e4009606af63816fcc1530`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 01:46:04 GMT
ADD file:afec039adf230a9186a38b57eed85262696f8d178ac649a445657066f16fe806 in / 
# Fri, 12 Mar 2021 01:46:07 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:53:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:54:00 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 02:54:00 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 02:54:01 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 02:54:01 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 02:54:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 02:54:49 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 02:54:50 GMT
USER user
# Fri, 12 Mar 2021 02:54:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:d41215965c091534e809ab2e8f4a2c1cebee3de536c2c74a7bc8302bbc8af7e1`  
		Last Modified: Fri, 12 Mar 2021 01:50:30 GMT  
		Size: 25.7 MB (25716294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1928942d4ca75c8bd9f793f48c56b77ad65491e9dcaf8f62e83eabffc0e2cd`  
		Last Modified: Fri, 12 Mar 2021 02:55:16 GMT  
		Size: 16.9 MB (16908957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e83765cc93c78e150ab9768d197c9d289926fe154516b60c0ac8e2d9eb17add`  
		Last Modified: Fri, 12 Mar 2021 02:55:13 GMT  
		Size: 4.2 KB (4212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9e5915a1e5381a069146b20a3141656c4e9aa3b2de62aa599e87e3c0661289`  
		Last Modified: Fri, 12 Mar 2021 02:55:14 GMT  
		Size: 6.4 MB (6383285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1-alpine`

```console
$ docker pull irssi@sha256:eda9ee756ac46d776ad5ff176894bedc8dfd6f8fb347b1e187714a263c54c7e5
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
$ docker pull irssi@sha256:e9f7fca8e1035fed887c65299debd1c144dc2795ed2cd70897ea33a94537a663
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18637035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:200fcb1a18950b1666d02171cfd5fc98329498d7b47076b8c551e632f92cbb37`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Fri, 12 Mar 2021 11:06:48 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 12 Mar 2021 11:06:49 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 11:06:50 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 11:06:51 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 11:06:51 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 11:08:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 12 Mar 2021 11:08:21 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 11:08:21 GMT
USER user
# Fri, 12 Mar 2021 11:08:22 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ceb86e4dfc3e51177b0c9bebe5e21c4f62846f82bb31e9c3df05d61b12686b`  
		Last Modified: Fri, 12 Mar 2021 11:09:08 GMT  
		Size: 9.5 MB (9546291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcdb0e3bcaae9496a4170e17023710d0c83a9b50295582212ab80da6b1fea415`  
		Last Modified: Fri, 12 Mar 2021 11:09:05 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef393ac458300cb54e5348a4fad9fdacb7e8ff40df4246c6beec666e09f6bf22`  
		Last Modified: Fri, 12 Mar 2021 11:09:08 GMT  
		Size: 6.3 MB (6277814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:1f5c7f3acf830fde5a0b1b2a03c8d4c241c16f80075fa9354eee2fedcda705e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17380720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71696b9d35a21e30b8716ccac8b96700bd5f52f029875b05bbae25c07cf2482a`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 21:24:35 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 17 Feb 2021 21:24:36 GMT
ENV HOME=/home/user
# Wed, 17 Feb 2021 21:24:39 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 17 Feb 2021 21:24:40 GMT
ENV LANG=C.UTF-8
# Wed, 17 Feb 2021 21:24:41 GMT
ENV IRSSI_VERSION=1.2.2
# Wed, 17 Feb 2021 21:25:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 17 Feb 2021 21:25:34 GMT
WORKDIR /home/user
# Wed, 17 Feb 2021 21:25:35 GMT
USER user
# Wed, 17 Feb 2021 21:25:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ff4c5d9d970b7aea5a3154a048a8dffdecaa2ba25b1ca324fe17c97846b341`  
		Last Modified: Wed, 17 Feb 2021 21:25:58 GMT  
		Size: 8.8 MB (8779079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762491e3840e0e26a34e0b701ff53443ad7810f8597293077dc34d419566d287`  
		Last Modified: Wed, 17 Feb 2021 21:25:54 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8ff637f1f0558e9446a89673d71ef57ac31f70c30723de693a929ae08bef99`  
		Last Modified: Wed, 17 Feb 2021 21:25:56 GMT  
		Size: 6.0 MB (5978332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:115a46cdc50bac16442fd75d0074f03fb6cd0a34fbed184d1c54c510721362f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16827376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca8749a9d6b447f282bbe9655d0f57d542f83ba2d22f455135da140d63b51ccc`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 25 Mar 2021 22:05:53 GMT
ADD file:44ef6cff6e7d37a67c5846eb792fec65025702c00c56ff96801ac79bf81b0cc3 in / 
# Thu, 25 Mar 2021 22:05:55 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:34:24 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 26 Mar 2021 01:34:27 GMT
ENV HOME=/home/user
# Fri, 26 Mar 2021 01:34:43 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 26 Mar 2021 01:34:57 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:34:58 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 26 Mar 2021 01:36:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 26 Mar 2021 01:36:30 GMT
WORKDIR /home/user
# Fri, 26 Mar 2021 01:36:32 GMT
USER user
# Fri, 26 Mar 2021 01:36:33 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6c1162af251f0d5ab4945f8506f3265b86d0a03cda37f703c2446a71a233bc20`  
		Last Modified: Thu, 25 Mar 2021 22:07:21 GMT  
		Size: 2.4 MB (2423999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc3e3c0e1237dab78d7546291ec3af3710654eb21a6a41d24735358183e2ef4`  
		Last Modified: Fri, 26 Mar 2021 01:37:10 GMT  
		Size: 8.6 MB (8630420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46da2938095dda6c27bc8a3751401e2068f53541132e174a7ab8d3da0c47260e`  
		Last Modified: Fri, 26 Mar 2021 01:37:03 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b70fe4c17acc8e06c03a1657b143ba9dcfb902d3e8bb458944dc57ad752b3f`  
		Last Modified: Fri, 26 Mar 2021 01:37:07 GMT  
		Size: 5.8 MB (5771687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:7e952f73bc19dba012551a010556a9f2830354aafeabc65ab98b99fb46b78be0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18484286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fba76d5f44622ab0ff706b71f209a569b5444a6d04f17ffb9db797df41fa954`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:25:09 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 26 Mar 2021 01:25:11 GMT
ENV HOME=/home/user
# Fri, 26 Mar 2021 01:25:14 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 26 Mar 2021 01:25:15 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:25:16 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 26 Mar 2021 01:26:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 26 Mar 2021 01:26:17 GMT
WORKDIR /home/user
# Fri, 26 Mar 2021 01:26:19 GMT
USER user
# Fri, 26 Mar 2021 01:26:20 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26913993fc81df5a50e2d87a7112af3450e67ba4062fd5b9165a12009ab102f2`  
		Last Modified: Fri, 26 Mar 2021 01:26:54 GMT  
		Size: 9.5 MB (9542280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7fd25418e612aa429275628f3f13f275019cecdb3a1fb98b1afa34d975ca4d7`  
		Last Modified: Fri, 26 Mar 2021 01:26:50 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9349288f06be1425b975ad9bdf02398a063d15cadeb878a254a09595abc9d5f9`  
		Last Modified: Fri, 26 Mar 2021 01:26:52 GMT  
		Size: 6.2 MB (6228838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; 386

```console
$ docker pull irssi@sha256:6a0279ffd88af96276b4e6f77f91af191a67083b06160756a00f6fd1e3009982
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17697705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:227f5732bdf7871068257a1c48d0bb2904bccbbbea092e0f8cae703b70f791cb`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 25 Mar 2021 22:38:25 GMT
ADD file:8953415d4b98f486af17a39ba53b38f7262aa590734c18ff9318927e5a705baf in / 
# Thu, 25 Mar 2021 22:38:26 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:59:51 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 26 Mar 2021 01:59:52 GMT
ENV HOME=/home/user
# Fri, 26 Mar 2021 01:59:53 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 26 Mar 2021 01:59:53 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:59:53 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 26 Mar 2021 02:00:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 26 Mar 2021 02:00:50 GMT
WORKDIR /home/user
# Fri, 26 Mar 2021 02:00:50 GMT
USER user
# Fri, 26 Mar 2021 02:00:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1fbd1c9912b638ce64a4740e3af7a3a03452f8705b8103950d677f1d79ae8164`  
		Last Modified: Thu, 25 Mar 2021 22:39:34 GMT  
		Size: 2.8 MB (2818129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1a8934e2dc515a457fca6334af810a53eb34db25494b16839f0b133883627c`  
		Last Modified: Fri, 26 Mar 2021 02:01:26 GMT  
		Size: 8.9 MB (8913129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2783e7c652bc8b874a3a033a780ab09a31d28cfee03a5b91e6c08f0d46c28db`  
		Last Modified: Fri, 26 Mar 2021 02:01:23 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6391518bf9cffe8e3d6ce27412a2de4c2fd1d1d0cb4da142b31eb2a2b507f7`  
		Last Modified: Fri, 26 Mar 2021 02:01:25 GMT  
		Size: 6.0 MB (5965177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:3d1948a0ceda5993a4cfdeefa7dd4d31fd815055235e99ae4c1e0d904dd1412a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18937265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe6dfa6dd0254312eba3b51ef834249b06061fa100633addef7bbbf84c42b637`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:28 GMT
ADD file:f91f8e0aa646cb847f6e210056280f9332382ad2f8d6a8839fd9aa69b81c4a2a in / 
# Thu, 25 Mar 2021 22:22:30 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:18:40 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 26 Mar 2021 01:18:48 GMT
ENV HOME=/home/user
# Fri, 26 Mar 2021 01:19:13 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 26 Mar 2021 01:19:21 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:19:27 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 26 Mar 2021 01:20:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 26 Mar 2021 01:20:35 GMT
WORKDIR /home/user
# Fri, 26 Mar 2021 01:20:45 GMT
USER user
# Fri, 26 Mar 2021 01:20:55 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f3b2866c25f0a9167af050d646a7a740ccc88d46e068c90ff28a5c2ec2ee0030`  
		Last Modified: Thu, 25 Mar 2021 22:24:08 GMT  
		Size: 2.8 MB (2813115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c86a2b2846b9a05e2deb4452ef826e8aa09d0d3b0b0ad866470ca47fcc0010b`  
		Last Modified: Fri, 26 Mar 2021 01:21:23 GMT  
		Size: 9.6 MB (9642108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f273ec2efe1d38112809f70cfe7a4c8f2912c0d43d784b03bfd2584665034e`  
		Last Modified: Fri, 26 Mar 2021 01:21:18 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a46d376716d33d6040dc26a63f40a6c19a9ea7b6a3680fc69e4bc7405792b55`  
		Last Modified: Fri, 26 Mar 2021 01:21:22 GMT  
		Size: 6.5 MB (6480769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:3c9d5482055f570989dac4b779ed2dd61aa3962b700a0a86135c9e9bb94205f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18849651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d3485e43acc5bf841c450ebc9d4ec75ea06ba436106b891755b7f4395339b5`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:34 GMT
ADD file:44e2c7cd992fc98df702bef7022e0f8c4ee86312c311ab5ae185fd5fc878edf9 in / 
# Thu, 25 Mar 2021 22:41:34 GMT
CMD ["/bin/sh"]
# Thu, 25 Mar 2021 23:59:56 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 25 Mar 2021 23:59:57 GMT
ENV HOME=/home/user
# Thu, 25 Mar 2021 23:59:58 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 25 Mar 2021 23:59:58 GMT
ENV LANG=C.UTF-8
# Thu, 25 Mar 2021 23:59:58 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 26 Mar 2021 00:00:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 26 Mar 2021 00:00:48 GMT
WORKDIR /home/user
# Fri, 26 Mar 2021 00:00:49 GMT
USER user
# Fri, 26 Mar 2021 00:00:49 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a266c0a9554add02ea09a46b8584cb36b7f606b7b4398b9ad7369f899f8360df`  
		Last Modified: Thu, 25 Mar 2021 22:42:07 GMT  
		Size: 2.6 MB (2602387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3247e0e05b318025a2d06f5368689c9847b298d64ed74c4f1595537be0b5c108`  
		Last Modified: Fri, 26 Mar 2021 00:01:17 GMT  
		Size: 10.0 MB (9983489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc605ff0a3f649f05afe38576d87bcc3ec1b087706cf95b44cfba2fdec1d77f`  
		Last Modified: Fri, 26 Mar 2021 00:01:15 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed45869f07cd143be2d9406f2a3ea7493dd8536819c152ecea64b0ad8c9da02`  
		Last Modified: Fri, 26 Mar 2021 00:01:16 GMT  
		Size: 6.3 MB (6262509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2`

```console
$ docker pull irssi@sha256:575d68fdda2e48da8abc975a602afab57a32dcd210101706492cb6c2fe9a0bde
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
$ docker pull irssi@sha256:7d442244c3d5d97b95ac0c0ca9be95165bd30b909621e572bed3f954cbdd3389
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50568077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5911d6f3416365bd18470b92a5ceca377f1b3c9337c0c9fbaec9891141aad195`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 11:04:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 11:04:57 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 11:04:59 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 11:04:59 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 11:04:59 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 11:06:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 11:06:38 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 11:06:39 GMT
USER user
# Fri, 12 Mar 2021 11:06:39 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa82220b80b6fa32a82277cdcf2e1a8b7350d3eb49dd723043dd4dfee38a4d7c`  
		Last Modified: Fri, 12 Mar 2021 11:08:48 GMT  
		Size: 17.0 MB (17033440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cab4a877a41e1cfdc916be3c7625c0f914119e3ad2abc2ad4b159e3baa1e0e`  
		Last Modified: Fri, 12 Mar 2021 11:08:42 GMT  
		Size: 4.2 KB (4208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a6c2e5e877ecd200d4c003252a7db5a9797a0f90feeadeded09ddd3a2f1eae`  
		Last Modified: Fri, 12 Mar 2021 11:08:44 GMT  
		Size: 6.4 MB (6429428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; arm variant v5

```console
$ docker pull irssi@sha256:9e24e92190db23a06e2692b1a49ce3438288a26b7bd501bd58fb0f84caf11185
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46843846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7aaa632856c778560f9f55abbd065b8f2980a83ed0420f7607c9c2879be3124`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 01:52:27 GMT
ADD file:8e357182800adfe658856515726f1e012cc120349f0f305692cf50282f6d8b7b in / 
# Fri, 12 Mar 2021 01:52:29 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:50:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:50:23 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 02:50:26 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 02:50:26 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 02:50:27 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 02:52:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 02:52:15 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 02:52:16 GMT
USER user
# Fri, 12 Mar 2021 02:52:17 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:9babb1be2e38b3bddad5a4e05bb34173369ae3472c0c0d8668853011cd65969f`  
		Last Modified: Fri, 12 Mar 2021 02:02:01 GMT  
		Size: 24.8 MB (24845925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e25b60c55c4d12e692a0e8d8966b14cc0e5085187f8a343a4d84956e316ffb6`  
		Last Modified: Fri, 12 Mar 2021 02:52:43 GMT  
		Size: 15.9 MB (15931049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67829e638098b8d79aa01cad5ded7c1cb12071840410b02090c62c9f8edd7fa`  
		Last Modified: Fri, 12 Mar 2021 02:52:36 GMT  
		Size: 4.2 KB (4196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd508527cc93ad08df450347b6d21d5032a28fa0488016291c8abe88d2de5ce`  
		Last Modified: Fri, 12 Mar 2021 02:52:38 GMT  
		Size: 6.1 MB (6062676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; arm variant v7

```console
$ docker pull irssi@sha256:32f2605101fe727c1455d51042f015e19827a7866ddedc3d22d5ad735064ba81
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44234132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8977a6c44287eae4a76289108e4ce0b1ac7425a4f5c9b9e02d8eea74df22d92e`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 02:00:12 GMT
ADD file:123da9848f87c8ed4c5122a104b8650564c09767725916f822def7b645a019f1 in / 
# Fri, 12 Mar 2021 02:00:14 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 04:56:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 04:56:26 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 04:56:28 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 04:56:29 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 04:56:29 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 04:57:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 04:58:00 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 04:58:01 GMT
USER user
# Fri, 12 Mar 2021 04:58:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:e12d26f75fe8b7fd14712965ff5178762227d07d2151bb35fa21105ddfc4a14a`  
		Last Modified: Fri, 12 Mar 2021 02:10:28 GMT  
		Size: 22.7 MB (22709467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f1dc2c6549f399aec326fad72f414b645d8f953321c14032de6b908cb94b42`  
		Last Modified: Fri, 12 Mar 2021 04:58:35 GMT  
		Size: 15.6 MB (15590035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f0a2c1c5574bae60fc820eb688fd9317c9fb76c8fbc8127760891fb60261f65`  
		Last Modified: Fri, 12 Mar 2021 04:58:27 GMT  
		Size: 4.2 KB (4195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc5f47c56a02365fc5a6dfa4ce63062636df3340e67756c0413eaab1feed334`  
		Last Modified: Fri, 12 Mar 2021 04:58:29 GMT  
		Size: 5.9 MB (5930435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:02686cdc34ce5dd16345df7292a3064f22a074585de5547ad7e4691b5547fea9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49052058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d3942313a1f6e377d074ac70be91b98b22f099283c005a45801c8b265bce22b`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 01:53:53 GMT
ADD file:6130ddc0a939dd72c0614de4aa77de47aa16fe211274bacb31995aa1a0526164 in / 
# Fri, 12 Mar 2021 01:53:56 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 17:43:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 17:43:25 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 17:43:27 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 17:43:28 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 17:43:29 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 17:45:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 17:45:04 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 17:45:05 GMT
USER user
# Fri, 12 Mar 2021 17:45:06 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:706ee5d0a6b53d9257cbea22d8409fb22c867ab3a001c65f6b8bfd37dace0e58`  
		Last Modified: Fri, 12 Mar 2021 02:01:39 GMT  
		Size: 25.9 MB (25856512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc1a0fcfd5b5c8a6304adad324f44c13c6ebe3062940f9da8318bbbc1b57a6d`  
		Last Modified: Fri, 12 Mar 2021 17:45:35 GMT  
		Size: 16.8 MB (16803429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d79819a4c69ccab094f2aaee1ee4c383589114a44ea07437262e24e3335b026`  
		Last Modified: Fri, 12 Mar 2021 17:45:28 GMT  
		Size: 4.2 KB (4219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4834bc87f80d7b0ee15ef328f8981b1fa7cdc1e1f761286aa1e57e32fe2c2194`  
		Last Modified: Fri, 12 Mar 2021 17:45:31 GMT  
		Size: 6.4 MB (6387898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; 386

```console
$ docker pull irssi@sha256:1c1a9780a77d5593848ec9f66c0c4a1db62d6c1ab536b03499426dc3230db8aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50425172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4233b7a266ca3253ce68dd157a42b68fce5841ab7212bd92ad8c98df61c29a9d`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 01:44:27 GMT
ADD file:90c103e04bd6fe0f39733cbf8eb2d8845aed3e4fc3fd1e5c3354df69e40aa615 in / 
# Fri, 12 Mar 2021 01:44:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 21:13:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 21:13:08 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 21:13:09 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 21:13:09 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 21:13:09 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 21:14:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 21:14:46 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 21:14:46 GMT
USER user
# Fri, 12 Mar 2021 21:14:46 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:0898aa7472f57f223652846337cf862f142e109d0c039b41886e7f20c345f85e`  
		Last Modified: Fri, 12 Mar 2021 01:52:08 GMT  
		Size: 27.8 MB (27760948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7adad1dd74fcd0ecb398e894c7f8861e0f07cfc0bdb77cbc12e24b5cb793c68c`  
		Last Modified: Fri, 12 Mar 2021 21:16:47 GMT  
		Size: 16.6 MB (16558205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b2cf9a9a3e742c4c14027ae25b0d3325b123f048d89744ac861296cfdcfb46c`  
		Last Modified: Fri, 12 Mar 2021 21:16:37 GMT  
		Size: 4.2 KB (4192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c8264777e37ece315309662ef9c2042aed482ebfe6288ccebe91922fcc072fb`  
		Last Modified: Fri, 12 Mar 2021 21:16:41 GMT  
		Size: 6.1 MB (6101827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; mips64le

```console
$ docker pull irssi@sha256:11dcb1ea1f6a694137f6869a3a5d24e9c73d1d5e898b9feaf60779bc9d7ea9f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47775886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd123eb9b8194e1dce76a162a06d55a66f76c4a1947e7375174754f54dd208b9`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 02:10:02 GMT
ADD file:491c5ca15fe098b83de42861289c216c693d788a1f9e739a78acefb0cad453c8 in / 
# Fri, 12 Mar 2021 02:10:03 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 03:00:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 03:00:09 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 03:00:11 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 03:00:12 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 03:00:12 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 03:02:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 03:02:45 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 03:02:45 GMT
USER user
# Fri, 12 Mar 2021 03:02:45 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:d0b6b2cc51bdde474395b8c32ff8012e471727bba69f221cfb79b46e8283f047`  
		Last Modified: Fri, 12 Mar 2021 02:17:07 GMT  
		Size: 25.8 MB (25772338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f07eae8650e63d8e5c5c11fa467c8cb401e24859b6c3eb97d1cb4beb77ca33f`  
		Last Modified: Fri, 12 Mar 2021 03:03:23 GMT  
		Size: 15.7 MB (15709110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069673a50a0626dfb618561bcc33174f5af67375b61426deebf65feeb686a270`  
		Last Modified: Fri, 12 Mar 2021 03:03:06 GMT  
		Size: 4.2 KB (4179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0e23988c6b3499aefb8ddcbd10d127bd56e8d4c22e34889250b9602c012f9e`  
		Last Modified: Fri, 12 Mar 2021 03:03:11 GMT  
		Size: 6.3 MB (6290259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; ppc64le

```console
$ docker pull irssi@sha256:042a76fc7d37dc6e7fe106e64a43037de8d4f6162bed9362f02ce1cb46d89b05
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.7 MB (54748353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e21ad9386f16b76532f9ca7679ab7b1a1b7ae07c665005d3540d630efb08a2e`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 02:32:43 GMT
ADD file:6a0c0cfa71979cf6fdd859dce1e32582f0e55ed382b9e17b77a2001defc2c9db in / 
# Fri, 12 Mar 2021 02:32:50 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 05:21:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 05:21:53 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 05:22:19 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 05:22:33 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 05:22:47 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 05:33:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 05:33:07 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 05:33:15 GMT
USER user
# Fri, 12 Mar 2021 05:33:35 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1d686056fdac1848f4fd78ba2b335502055ffe98c79619e21d0c2fb7db95257e`  
		Last Modified: Fri, 12 Mar 2021 02:45:35 GMT  
		Size: 30.5 MB (30525728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ece5dc65262bccb6252440d8c5e1a3dca0ec3603abb9e8b49d82f97d6cb85b9`  
		Last Modified: Fri, 12 Mar 2021 05:34:13 GMT  
		Size: 17.4 MB (17437414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc49adb12fb0cd54dc637a9532fbc83cb4e037e6b2bd4e5971948ffbf5f5d8a`  
		Last Modified: Fri, 12 Mar 2021 05:34:08 GMT  
		Size: 4.2 KB (4214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559c20b0868126ced94ac9ef5df1d609e27bd8abfc99fde3a2676da11e98a227`  
		Last Modified: Fri, 12 Mar 2021 05:34:11 GMT  
		Size: 6.8 MB (6780997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; s390x

```console
$ docker pull irssi@sha256:5d0796552e1559a6f77853b1e52d7e7ae5b2a7ea5a36c11cee0ef8f99a528f74
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49012748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f31d157ba631157ab487f5b32e1ef32f016af19318e4009606af63816fcc1530`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 01:46:04 GMT
ADD file:afec039adf230a9186a38b57eed85262696f8d178ac649a445657066f16fe806 in / 
# Fri, 12 Mar 2021 01:46:07 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:53:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:54:00 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 02:54:00 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 02:54:01 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 02:54:01 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 02:54:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 02:54:49 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 02:54:50 GMT
USER user
# Fri, 12 Mar 2021 02:54:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:d41215965c091534e809ab2e8f4a2c1cebee3de536c2c74a7bc8302bbc8af7e1`  
		Last Modified: Fri, 12 Mar 2021 01:50:30 GMT  
		Size: 25.7 MB (25716294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1928942d4ca75c8bd9f793f48c56b77ad65491e9dcaf8f62e83eabffc0e2cd`  
		Last Modified: Fri, 12 Mar 2021 02:55:16 GMT  
		Size: 16.9 MB (16908957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e83765cc93c78e150ab9768d197c9d289926fe154516b60c0ac8e2d9eb17add`  
		Last Modified: Fri, 12 Mar 2021 02:55:13 GMT  
		Size: 4.2 KB (4212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9e5915a1e5381a069146b20a3141656c4e9aa3b2de62aa599e87e3c0661289`  
		Last Modified: Fri, 12 Mar 2021 02:55:14 GMT  
		Size: 6.4 MB (6383285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2-alpine`

```console
$ docker pull irssi@sha256:eda9ee756ac46d776ad5ff176894bedc8dfd6f8fb347b1e187714a263c54c7e5
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
$ docker pull irssi@sha256:e9f7fca8e1035fed887c65299debd1c144dc2795ed2cd70897ea33a94537a663
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18637035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:200fcb1a18950b1666d02171cfd5fc98329498d7b47076b8c551e632f92cbb37`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Fri, 12 Mar 2021 11:06:48 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 12 Mar 2021 11:06:49 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 11:06:50 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 11:06:51 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 11:06:51 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 11:08:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 12 Mar 2021 11:08:21 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 11:08:21 GMT
USER user
# Fri, 12 Mar 2021 11:08:22 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ceb86e4dfc3e51177b0c9bebe5e21c4f62846f82bb31e9c3df05d61b12686b`  
		Last Modified: Fri, 12 Mar 2021 11:09:08 GMT  
		Size: 9.5 MB (9546291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcdb0e3bcaae9496a4170e17023710d0c83a9b50295582212ab80da6b1fea415`  
		Last Modified: Fri, 12 Mar 2021 11:09:05 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef393ac458300cb54e5348a4fad9fdacb7e8ff40df4246c6beec666e09f6bf22`  
		Last Modified: Fri, 12 Mar 2021 11:09:08 GMT  
		Size: 6.3 MB (6277814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:1f5c7f3acf830fde5a0b1b2a03c8d4c241c16f80075fa9354eee2fedcda705e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17380720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71696b9d35a21e30b8716ccac8b96700bd5f52f029875b05bbae25c07cf2482a`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 21:24:35 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 17 Feb 2021 21:24:36 GMT
ENV HOME=/home/user
# Wed, 17 Feb 2021 21:24:39 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 17 Feb 2021 21:24:40 GMT
ENV LANG=C.UTF-8
# Wed, 17 Feb 2021 21:24:41 GMT
ENV IRSSI_VERSION=1.2.2
# Wed, 17 Feb 2021 21:25:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 17 Feb 2021 21:25:34 GMT
WORKDIR /home/user
# Wed, 17 Feb 2021 21:25:35 GMT
USER user
# Wed, 17 Feb 2021 21:25:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ff4c5d9d970b7aea5a3154a048a8dffdecaa2ba25b1ca324fe17c97846b341`  
		Last Modified: Wed, 17 Feb 2021 21:25:58 GMT  
		Size: 8.8 MB (8779079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762491e3840e0e26a34e0b701ff53443ad7810f8597293077dc34d419566d287`  
		Last Modified: Wed, 17 Feb 2021 21:25:54 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8ff637f1f0558e9446a89673d71ef57ac31f70c30723de693a929ae08bef99`  
		Last Modified: Wed, 17 Feb 2021 21:25:56 GMT  
		Size: 6.0 MB (5978332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:115a46cdc50bac16442fd75d0074f03fb6cd0a34fbed184d1c54c510721362f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16827376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca8749a9d6b447f282bbe9655d0f57d542f83ba2d22f455135da140d63b51ccc`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 25 Mar 2021 22:05:53 GMT
ADD file:44ef6cff6e7d37a67c5846eb792fec65025702c00c56ff96801ac79bf81b0cc3 in / 
# Thu, 25 Mar 2021 22:05:55 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:34:24 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 26 Mar 2021 01:34:27 GMT
ENV HOME=/home/user
# Fri, 26 Mar 2021 01:34:43 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 26 Mar 2021 01:34:57 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:34:58 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 26 Mar 2021 01:36:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 26 Mar 2021 01:36:30 GMT
WORKDIR /home/user
# Fri, 26 Mar 2021 01:36:32 GMT
USER user
# Fri, 26 Mar 2021 01:36:33 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6c1162af251f0d5ab4945f8506f3265b86d0a03cda37f703c2446a71a233bc20`  
		Last Modified: Thu, 25 Mar 2021 22:07:21 GMT  
		Size: 2.4 MB (2423999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc3e3c0e1237dab78d7546291ec3af3710654eb21a6a41d24735358183e2ef4`  
		Last Modified: Fri, 26 Mar 2021 01:37:10 GMT  
		Size: 8.6 MB (8630420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46da2938095dda6c27bc8a3751401e2068f53541132e174a7ab8d3da0c47260e`  
		Last Modified: Fri, 26 Mar 2021 01:37:03 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b70fe4c17acc8e06c03a1657b143ba9dcfb902d3e8bb458944dc57ad752b3f`  
		Last Modified: Fri, 26 Mar 2021 01:37:07 GMT  
		Size: 5.8 MB (5771687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:7e952f73bc19dba012551a010556a9f2830354aafeabc65ab98b99fb46b78be0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18484286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fba76d5f44622ab0ff706b71f209a569b5444a6d04f17ffb9db797df41fa954`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:25:09 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 26 Mar 2021 01:25:11 GMT
ENV HOME=/home/user
# Fri, 26 Mar 2021 01:25:14 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 26 Mar 2021 01:25:15 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:25:16 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 26 Mar 2021 01:26:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 26 Mar 2021 01:26:17 GMT
WORKDIR /home/user
# Fri, 26 Mar 2021 01:26:19 GMT
USER user
# Fri, 26 Mar 2021 01:26:20 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26913993fc81df5a50e2d87a7112af3450e67ba4062fd5b9165a12009ab102f2`  
		Last Modified: Fri, 26 Mar 2021 01:26:54 GMT  
		Size: 9.5 MB (9542280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7fd25418e612aa429275628f3f13f275019cecdb3a1fb98b1afa34d975ca4d7`  
		Last Modified: Fri, 26 Mar 2021 01:26:50 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9349288f06be1425b975ad9bdf02398a063d15cadeb878a254a09595abc9d5f9`  
		Last Modified: Fri, 26 Mar 2021 01:26:52 GMT  
		Size: 6.2 MB (6228838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; 386

```console
$ docker pull irssi@sha256:6a0279ffd88af96276b4e6f77f91af191a67083b06160756a00f6fd1e3009982
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17697705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:227f5732bdf7871068257a1c48d0bb2904bccbbbea092e0f8cae703b70f791cb`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 25 Mar 2021 22:38:25 GMT
ADD file:8953415d4b98f486af17a39ba53b38f7262aa590734c18ff9318927e5a705baf in / 
# Thu, 25 Mar 2021 22:38:26 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:59:51 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 26 Mar 2021 01:59:52 GMT
ENV HOME=/home/user
# Fri, 26 Mar 2021 01:59:53 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 26 Mar 2021 01:59:53 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:59:53 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 26 Mar 2021 02:00:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 26 Mar 2021 02:00:50 GMT
WORKDIR /home/user
# Fri, 26 Mar 2021 02:00:50 GMT
USER user
# Fri, 26 Mar 2021 02:00:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1fbd1c9912b638ce64a4740e3af7a3a03452f8705b8103950d677f1d79ae8164`  
		Last Modified: Thu, 25 Mar 2021 22:39:34 GMT  
		Size: 2.8 MB (2818129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1a8934e2dc515a457fca6334af810a53eb34db25494b16839f0b133883627c`  
		Last Modified: Fri, 26 Mar 2021 02:01:26 GMT  
		Size: 8.9 MB (8913129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2783e7c652bc8b874a3a033a780ab09a31d28cfee03a5b91e6c08f0d46c28db`  
		Last Modified: Fri, 26 Mar 2021 02:01:23 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6391518bf9cffe8e3d6ce27412a2de4c2fd1d1d0cb4da142b31eb2a2b507f7`  
		Last Modified: Fri, 26 Mar 2021 02:01:25 GMT  
		Size: 6.0 MB (5965177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:3d1948a0ceda5993a4cfdeefa7dd4d31fd815055235e99ae4c1e0d904dd1412a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18937265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe6dfa6dd0254312eba3b51ef834249b06061fa100633addef7bbbf84c42b637`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:28 GMT
ADD file:f91f8e0aa646cb847f6e210056280f9332382ad2f8d6a8839fd9aa69b81c4a2a in / 
# Thu, 25 Mar 2021 22:22:30 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:18:40 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 26 Mar 2021 01:18:48 GMT
ENV HOME=/home/user
# Fri, 26 Mar 2021 01:19:13 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 26 Mar 2021 01:19:21 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:19:27 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 26 Mar 2021 01:20:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 26 Mar 2021 01:20:35 GMT
WORKDIR /home/user
# Fri, 26 Mar 2021 01:20:45 GMT
USER user
# Fri, 26 Mar 2021 01:20:55 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f3b2866c25f0a9167af050d646a7a740ccc88d46e068c90ff28a5c2ec2ee0030`  
		Last Modified: Thu, 25 Mar 2021 22:24:08 GMT  
		Size: 2.8 MB (2813115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c86a2b2846b9a05e2deb4452ef826e8aa09d0d3b0b0ad866470ca47fcc0010b`  
		Last Modified: Fri, 26 Mar 2021 01:21:23 GMT  
		Size: 9.6 MB (9642108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f273ec2efe1d38112809f70cfe7a4c8f2912c0d43d784b03bfd2584665034e`  
		Last Modified: Fri, 26 Mar 2021 01:21:18 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a46d376716d33d6040dc26a63f40a6c19a9ea7b6a3680fc69e4bc7405792b55`  
		Last Modified: Fri, 26 Mar 2021 01:21:22 GMT  
		Size: 6.5 MB (6480769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:3c9d5482055f570989dac4b779ed2dd61aa3962b700a0a86135c9e9bb94205f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18849651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d3485e43acc5bf841c450ebc9d4ec75ea06ba436106b891755b7f4395339b5`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:34 GMT
ADD file:44e2c7cd992fc98df702bef7022e0f8c4ee86312c311ab5ae185fd5fc878edf9 in / 
# Thu, 25 Mar 2021 22:41:34 GMT
CMD ["/bin/sh"]
# Thu, 25 Mar 2021 23:59:56 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 25 Mar 2021 23:59:57 GMT
ENV HOME=/home/user
# Thu, 25 Mar 2021 23:59:58 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 25 Mar 2021 23:59:58 GMT
ENV LANG=C.UTF-8
# Thu, 25 Mar 2021 23:59:58 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 26 Mar 2021 00:00:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 26 Mar 2021 00:00:48 GMT
WORKDIR /home/user
# Fri, 26 Mar 2021 00:00:49 GMT
USER user
# Fri, 26 Mar 2021 00:00:49 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a266c0a9554add02ea09a46b8584cb36b7f606b7b4398b9ad7369f899f8360df`  
		Last Modified: Thu, 25 Mar 2021 22:42:07 GMT  
		Size: 2.6 MB (2602387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3247e0e05b318025a2d06f5368689c9847b298d64ed74c4f1595537be0b5c108`  
		Last Modified: Fri, 26 Mar 2021 00:01:17 GMT  
		Size: 10.0 MB (9983489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc605ff0a3f649f05afe38576d87bcc3ec1b087706cf95b44cfba2fdec1d77f`  
		Last Modified: Fri, 26 Mar 2021 00:01:15 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed45869f07cd143be2d9406f2a3ea7493dd8536819c152ecea64b0ad8c9da02`  
		Last Modified: Fri, 26 Mar 2021 00:01:16 GMT  
		Size: 6.3 MB (6262509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2.2`

```console
$ docker pull irssi@sha256:575d68fdda2e48da8abc975a602afab57a32dcd210101706492cb6c2fe9a0bde
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
$ docker pull irssi@sha256:7d442244c3d5d97b95ac0c0ca9be95165bd30b909621e572bed3f954cbdd3389
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50568077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5911d6f3416365bd18470b92a5ceca377f1b3c9337c0c9fbaec9891141aad195`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 11:04:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 11:04:57 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 11:04:59 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 11:04:59 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 11:04:59 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 11:06:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 11:06:38 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 11:06:39 GMT
USER user
# Fri, 12 Mar 2021 11:06:39 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa82220b80b6fa32a82277cdcf2e1a8b7350d3eb49dd723043dd4dfee38a4d7c`  
		Last Modified: Fri, 12 Mar 2021 11:08:48 GMT  
		Size: 17.0 MB (17033440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cab4a877a41e1cfdc916be3c7625c0f914119e3ad2abc2ad4b159e3baa1e0e`  
		Last Modified: Fri, 12 Mar 2021 11:08:42 GMT  
		Size: 4.2 KB (4208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a6c2e5e877ecd200d4c003252a7db5a9797a0f90feeadeded09ddd3a2f1eae`  
		Last Modified: Fri, 12 Mar 2021 11:08:44 GMT  
		Size: 6.4 MB (6429428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2` - linux; arm variant v5

```console
$ docker pull irssi@sha256:9e24e92190db23a06e2692b1a49ce3438288a26b7bd501bd58fb0f84caf11185
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46843846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7aaa632856c778560f9f55abbd065b8f2980a83ed0420f7607c9c2879be3124`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 01:52:27 GMT
ADD file:8e357182800adfe658856515726f1e012cc120349f0f305692cf50282f6d8b7b in / 
# Fri, 12 Mar 2021 01:52:29 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:50:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:50:23 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 02:50:26 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 02:50:26 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 02:50:27 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 02:52:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 02:52:15 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 02:52:16 GMT
USER user
# Fri, 12 Mar 2021 02:52:17 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:9babb1be2e38b3bddad5a4e05bb34173369ae3472c0c0d8668853011cd65969f`  
		Last Modified: Fri, 12 Mar 2021 02:02:01 GMT  
		Size: 24.8 MB (24845925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e25b60c55c4d12e692a0e8d8966b14cc0e5085187f8a343a4d84956e316ffb6`  
		Last Modified: Fri, 12 Mar 2021 02:52:43 GMT  
		Size: 15.9 MB (15931049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67829e638098b8d79aa01cad5ded7c1cb12071840410b02090c62c9f8edd7fa`  
		Last Modified: Fri, 12 Mar 2021 02:52:36 GMT  
		Size: 4.2 KB (4196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd508527cc93ad08df450347b6d21d5032a28fa0488016291c8abe88d2de5ce`  
		Last Modified: Fri, 12 Mar 2021 02:52:38 GMT  
		Size: 6.1 MB (6062676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2` - linux; arm variant v7

```console
$ docker pull irssi@sha256:32f2605101fe727c1455d51042f015e19827a7866ddedc3d22d5ad735064ba81
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44234132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8977a6c44287eae4a76289108e4ce0b1ac7425a4f5c9b9e02d8eea74df22d92e`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 02:00:12 GMT
ADD file:123da9848f87c8ed4c5122a104b8650564c09767725916f822def7b645a019f1 in / 
# Fri, 12 Mar 2021 02:00:14 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 04:56:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 04:56:26 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 04:56:28 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 04:56:29 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 04:56:29 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 04:57:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 04:58:00 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 04:58:01 GMT
USER user
# Fri, 12 Mar 2021 04:58:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:e12d26f75fe8b7fd14712965ff5178762227d07d2151bb35fa21105ddfc4a14a`  
		Last Modified: Fri, 12 Mar 2021 02:10:28 GMT  
		Size: 22.7 MB (22709467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f1dc2c6549f399aec326fad72f414b645d8f953321c14032de6b908cb94b42`  
		Last Modified: Fri, 12 Mar 2021 04:58:35 GMT  
		Size: 15.6 MB (15590035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f0a2c1c5574bae60fc820eb688fd9317c9fb76c8fbc8127760891fb60261f65`  
		Last Modified: Fri, 12 Mar 2021 04:58:27 GMT  
		Size: 4.2 KB (4195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc5f47c56a02365fc5a6dfa4ce63062636df3340e67756c0413eaab1feed334`  
		Last Modified: Fri, 12 Mar 2021 04:58:29 GMT  
		Size: 5.9 MB (5930435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:02686cdc34ce5dd16345df7292a3064f22a074585de5547ad7e4691b5547fea9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49052058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d3942313a1f6e377d074ac70be91b98b22f099283c005a45801c8b265bce22b`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 01:53:53 GMT
ADD file:6130ddc0a939dd72c0614de4aa77de47aa16fe211274bacb31995aa1a0526164 in / 
# Fri, 12 Mar 2021 01:53:56 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 17:43:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 17:43:25 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 17:43:27 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 17:43:28 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 17:43:29 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 17:45:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 17:45:04 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 17:45:05 GMT
USER user
# Fri, 12 Mar 2021 17:45:06 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:706ee5d0a6b53d9257cbea22d8409fb22c867ab3a001c65f6b8bfd37dace0e58`  
		Last Modified: Fri, 12 Mar 2021 02:01:39 GMT  
		Size: 25.9 MB (25856512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc1a0fcfd5b5c8a6304adad324f44c13c6ebe3062940f9da8318bbbc1b57a6d`  
		Last Modified: Fri, 12 Mar 2021 17:45:35 GMT  
		Size: 16.8 MB (16803429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d79819a4c69ccab094f2aaee1ee4c383589114a44ea07437262e24e3335b026`  
		Last Modified: Fri, 12 Mar 2021 17:45:28 GMT  
		Size: 4.2 KB (4219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4834bc87f80d7b0ee15ef328f8981b1fa7cdc1e1f761286aa1e57e32fe2c2194`  
		Last Modified: Fri, 12 Mar 2021 17:45:31 GMT  
		Size: 6.4 MB (6387898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2` - linux; 386

```console
$ docker pull irssi@sha256:1c1a9780a77d5593848ec9f66c0c4a1db62d6c1ab536b03499426dc3230db8aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50425172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4233b7a266ca3253ce68dd157a42b68fce5841ab7212bd92ad8c98df61c29a9d`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 01:44:27 GMT
ADD file:90c103e04bd6fe0f39733cbf8eb2d8845aed3e4fc3fd1e5c3354df69e40aa615 in / 
# Fri, 12 Mar 2021 01:44:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 21:13:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 21:13:08 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 21:13:09 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 21:13:09 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 21:13:09 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 21:14:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 21:14:46 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 21:14:46 GMT
USER user
# Fri, 12 Mar 2021 21:14:46 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:0898aa7472f57f223652846337cf862f142e109d0c039b41886e7f20c345f85e`  
		Last Modified: Fri, 12 Mar 2021 01:52:08 GMT  
		Size: 27.8 MB (27760948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7adad1dd74fcd0ecb398e894c7f8861e0f07cfc0bdb77cbc12e24b5cb793c68c`  
		Last Modified: Fri, 12 Mar 2021 21:16:47 GMT  
		Size: 16.6 MB (16558205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b2cf9a9a3e742c4c14027ae25b0d3325b123f048d89744ac861296cfdcfb46c`  
		Last Modified: Fri, 12 Mar 2021 21:16:37 GMT  
		Size: 4.2 KB (4192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c8264777e37ece315309662ef9c2042aed482ebfe6288ccebe91922fcc072fb`  
		Last Modified: Fri, 12 Mar 2021 21:16:41 GMT  
		Size: 6.1 MB (6101827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2` - linux; mips64le

```console
$ docker pull irssi@sha256:11dcb1ea1f6a694137f6869a3a5d24e9c73d1d5e898b9feaf60779bc9d7ea9f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47775886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd123eb9b8194e1dce76a162a06d55a66f76c4a1947e7375174754f54dd208b9`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 02:10:02 GMT
ADD file:491c5ca15fe098b83de42861289c216c693d788a1f9e739a78acefb0cad453c8 in / 
# Fri, 12 Mar 2021 02:10:03 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 03:00:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 03:00:09 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 03:00:11 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 03:00:12 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 03:00:12 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 03:02:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 03:02:45 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 03:02:45 GMT
USER user
# Fri, 12 Mar 2021 03:02:45 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:d0b6b2cc51bdde474395b8c32ff8012e471727bba69f221cfb79b46e8283f047`  
		Last Modified: Fri, 12 Mar 2021 02:17:07 GMT  
		Size: 25.8 MB (25772338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f07eae8650e63d8e5c5c11fa467c8cb401e24859b6c3eb97d1cb4beb77ca33f`  
		Last Modified: Fri, 12 Mar 2021 03:03:23 GMT  
		Size: 15.7 MB (15709110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069673a50a0626dfb618561bcc33174f5af67375b61426deebf65feeb686a270`  
		Last Modified: Fri, 12 Mar 2021 03:03:06 GMT  
		Size: 4.2 KB (4179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0e23988c6b3499aefb8ddcbd10d127bd56e8d4c22e34889250b9602c012f9e`  
		Last Modified: Fri, 12 Mar 2021 03:03:11 GMT  
		Size: 6.3 MB (6290259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2` - linux; ppc64le

```console
$ docker pull irssi@sha256:042a76fc7d37dc6e7fe106e64a43037de8d4f6162bed9362f02ce1cb46d89b05
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.7 MB (54748353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e21ad9386f16b76532f9ca7679ab7b1a1b7ae07c665005d3540d630efb08a2e`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 02:32:43 GMT
ADD file:6a0c0cfa71979cf6fdd859dce1e32582f0e55ed382b9e17b77a2001defc2c9db in / 
# Fri, 12 Mar 2021 02:32:50 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 05:21:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 05:21:53 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 05:22:19 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 05:22:33 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 05:22:47 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 05:33:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 05:33:07 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 05:33:15 GMT
USER user
# Fri, 12 Mar 2021 05:33:35 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1d686056fdac1848f4fd78ba2b335502055ffe98c79619e21d0c2fb7db95257e`  
		Last Modified: Fri, 12 Mar 2021 02:45:35 GMT  
		Size: 30.5 MB (30525728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ece5dc65262bccb6252440d8c5e1a3dca0ec3603abb9e8b49d82f97d6cb85b9`  
		Last Modified: Fri, 12 Mar 2021 05:34:13 GMT  
		Size: 17.4 MB (17437414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc49adb12fb0cd54dc637a9532fbc83cb4e037e6b2bd4e5971948ffbf5f5d8a`  
		Last Modified: Fri, 12 Mar 2021 05:34:08 GMT  
		Size: 4.2 KB (4214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559c20b0868126ced94ac9ef5df1d609e27bd8abfc99fde3a2676da11e98a227`  
		Last Modified: Fri, 12 Mar 2021 05:34:11 GMT  
		Size: 6.8 MB (6780997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2` - linux; s390x

```console
$ docker pull irssi@sha256:5d0796552e1559a6f77853b1e52d7e7ae5b2a7ea5a36c11cee0ef8f99a528f74
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49012748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f31d157ba631157ab487f5b32e1ef32f016af19318e4009606af63816fcc1530`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 01:46:04 GMT
ADD file:afec039adf230a9186a38b57eed85262696f8d178ac649a445657066f16fe806 in / 
# Fri, 12 Mar 2021 01:46:07 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:53:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:54:00 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 02:54:00 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 02:54:01 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 02:54:01 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 02:54:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 02:54:49 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 02:54:50 GMT
USER user
# Fri, 12 Mar 2021 02:54:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:d41215965c091534e809ab2e8f4a2c1cebee3de536c2c74a7bc8302bbc8af7e1`  
		Last Modified: Fri, 12 Mar 2021 01:50:30 GMT  
		Size: 25.7 MB (25716294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1928942d4ca75c8bd9f793f48c56b77ad65491e9dcaf8f62e83eabffc0e2cd`  
		Last Modified: Fri, 12 Mar 2021 02:55:16 GMT  
		Size: 16.9 MB (16908957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e83765cc93c78e150ab9768d197c9d289926fe154516b60c0ac8e2d9eb17add`  
		Last Modified: Fri, 12 Mar 2021 02:55:13 GMT  
		Size: 4.2 KB (4212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9e5915a1e5381a069146b20a3141656c4e9aa3b2de62aa599e87e3c0661289`  
		Last Modified: Fri, 12 Mar 2021 02:55:14 GMT  
		Size: 6.4 MB (6383285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2.2-alpine`

```console
$ docker pull irssi@sha256:eda9ee756ac46d776ad5ff176894bedc8dfd6f8fb347b1e187714a263c54c7e5
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
$ docker pull irssi@sha256:e9f7fca8e1035fed887c65299debd1c144dc2795ed2cd70897ea33a94537a663
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18637035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:200fcb1a18950b1666d02171cfd5fc98329498d7b47076b8c551e632f92cbb37`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Fri, 12 Mar 2021 11:06:48 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 12 Mar 2021 11:06:49 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 11:06:50 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 11:06:51 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 11:06:51 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 11:08:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 12 Mar 2021 11:08:21 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 11:08:21 GMT
USER user
# Fri, 12 Mar 2021 11:08:22 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ceb86e4dfc3e51177b0c9bebe5e21c4f62846f82bb31e9c3df05d61b12686b`  
		Last Modified: Fri, 12 Mar 2021 11:09:08 GMT  
		Size: 9.5 MB (9546291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcdb0e3bcaae9496a4170e17023710d0c83a9b50295582212ab80da6b1fea415`  
		Last Modified: Fri, 12 Mar 2021 11:09:05 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef393ac458300cb54e5348a4fad9fdacb7e8ff40df4246c6beec666e09f6bf22`  
		Last Modified: Fri, 12 Mar 2021 11:09:08 GMT  
		Size: 6.3 MB (6277814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:1f5c7f3acf830fde5a0b1b2a03c8d4c241c16f80075fa9354eee2fedcda705e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17380720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71696b9d35a21e30b8716ccac8b96700bd5f52f029875b05bbae25c07cf2482a`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 21:24:35 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 17 Feb 2021 21:24:36 GMT
ENV HOME=/home/user
# Wed, 17 Feb 2021 21:24:39 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 17 Feb 2021 21:24:40 GMT
ENV LANG=C.UTF-8
# Wed, 17 Feb 2021 21:24:41 GMT
ENV IRSSI_VERSION=1.2.2
# Wed, 17 Feb 2021 21:25:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 17 Feb 2021 21:25:34 GMT
WORKDIR /home/user
# Wed, 17 Feb 2021 21:25:35 GMT
USER user
# Wed, 17 Feb 2021 21:25:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ff4c5d9d970b7aea5a3154a048a8dffdecaa2ba25b1ca324fe17c97846b341`  
		Last Modified: Wed, 17 Feb 2021 21:25:58 GMT  
		Size: 8.8 MB (8779079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762491e3840e0e26a34e0b701ff53443ad7810f8597293077dc34d419566d287`  
		Last Modified: Wed, 17 Feb 2021 21:25:54 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8ff637f1f0558e9446a89673d71ef57ac31f70c30723de693a929ae08bef99`  
		Last Modified: Wed, 17 Feb 2021 21:25:56 GMT  
		Size: 6.0 MB (5978332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:115a46cdc50bac16442fd75d0074f03fb6cd0a34fbed184d1c54c510721362f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16827376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca8749a9d6b447f282bbe9655d0f57d542f83ba2d22f455135da140d63b51ccc`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 25 Mar 2021 22:05:53 GMT
ADD file:44ef6cff6e7d37a67c5846eb792fec65025702c00c56ff96801ac79bf81b0cc3 in / 
# Thu, 25 Mar 2021 22:05:55 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:34:24 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 26 Mar 2021 01:34:27 GMT
ENV HOME=/home/user
# Fri, 26 Mar 2021 01:34:43 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 26 Mar 2021 01:34:57 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:34:58 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 26 Mar 2021 01:36:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 26 Mar 2021 01:36:30 GMT
WORKDIR /home/user
# Fri, 26 Mar 2021 01:36:32 GMT
USER user
# Fri, 26 Mar 2021 01:36:33 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6c1162af251f0d5ab4945f8506f3265b86d0a03cda37f703c2446a71a233bc20`  
		Last Modified: Thu, 25 Mar 2021 22:07:21 GMT  
		Size: 2.4 MB (2423999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc3e3c0e1237dab78d7546291ec3af3710654eb21a6a41d24735358183e2ef4`  
		Last Modified: Fri, 26 Mar 2021 01:37:10 GMT  
		Size: 8.6 MB (8630420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46da2938095dda6c27bc8a3751401e2068f53541132e174a7ab8d3da0c47260e`  
		Last Modified: Fri, 26 Mar 2021 01:37:03 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b70fe4c17acc8e06c03a1657b143ba9dcfb902d3e8bb458944dc57ad752b3f`  
		Last Modified: Fri, 26 Mar 2021 01:37:07 GMT  
		Size: 5.8 MB (5771687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:7e952f73bc19dba012551a010556a9f2830354aafeabc65ab98b99fb46b78be0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18484286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fba76d5f44622ab0ff706b71f209a569b5444a6d04f17ffb9db797df41fa954`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:25:09 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 26 Mar 2021 01:25:11 GMT
ENV HOME=/home/user
# Fri, 26 Mar 2021 01:25:14 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 26 Mar 2021 01:25:15 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:25:16 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 26 Mar 2021 01:26:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 26 Mar 2021 01:26:17 GMT
WORKDIR /home/user
# Fri, 26 Mar 2021 01:26:19 GMT
USER user
# Fri, 26 Mar 2021 01:26:20 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26913993fc81df5a50e2d87a7112af3450e67ba4062fd5b9165a12009ab102f2`  
		Last Modified: Fri, 26 Mar 2021 01:26:54 GMT  
		Size: 9.5 MB (9542280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7fd25418e612aa429275628f3f13f275019cecdb3a1fb98b1afa34d975ca4d7`  
		Last Modified: Fri, 26 Mar 2021 01:26:50 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9349288f06be1425b975ad9bdf02398a063d15cadeb878a254a09595abc9d5f9`  
		Last Modified: Fri, 26 Mar 2021 01:26:52 GMT  
		Size: 6.2 MB (6228838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2-alpine` - linux; 386

```console
$ docker pull irssi@sha256:6a0279ffd88af96276b4e6f77f91af191a67083b06160756a00f6fd1e3009982
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17697705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:227f5732bdf7871068257a1c48d0bb2904bccbbbea092e0f8cae703b70f791cb`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 25 Mar 2021 22:38:25 GMT
ADD file:8953415d4b98f486af17a39ba53b38f7262aa590734c18ff9318927e5a705baf in / 
# Thu, 25 Mar 2021 22:38:26 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:59:51 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 26 Mar 2021 01:59:52 GMT
ENV HOME=/home/user
# Fri, 26 Mar 2021 01:59:53 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 26 Mar 2021 01:59:53 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:59:53 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 26 Mar 2021 02:00:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 26 Mar 2021 02:00:50 GMT
WORKDIR /home/user
# Fri, 26 Mar 2021 02:00:50 GMT
USER user
# Fri, 26 Mar 2021 02:00:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1fbd1c9912b638ce64a4740e3af7a3a03452f8705b8103950d677f1d79ae8164`  
		Last Modified: Thu, 25 Mar 2021 22:39:34 GMT  
		Size: 2.8 MB (2818129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1a8934e2dc515a457fca6334af810a53eb34db25494b16839f0b133883627c`  
		Last Modified: Fri, 26 Mar 2021 02:01:26 GMT  
		Size: 8.9 MB (8913129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2783e7c652bc8b874a3a033a780ab09a31d28cfee03a5b91e6c08f0d46c28db`  
		Last Modified: Fri, 26 Mar 2021 02:01:23 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6391518bf9cffe8e3d6ce27412a2de4c2fd1d1d0cb4da142b31eb2a2b507f7`  
		Last Modified: Fri, 26 Mar 2021 02:01:25 GMT  
		Size: 6.0 MB (5965177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:3d1948a0ceda5993a4cfdeefa7dd4d31fd815055235e99ae4c1e0d904dd1412a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18937265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe6dfa6dd0254312eba3b51ef834249b06061fa100633addef7bbbf84c42b637`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:28 GMT
ADD file:f91f8e0aa646cb847f6e210056280f9332382ad2f8d6a8839fd9aa69b81c4a2a in / 
# Thu, 25 Mar 2021 22:22:30 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:18:40 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 26 Mar 2021 01:18:48 GMT
ENV HOME=/home/user
# Fri, 26 Mar 2021 01:19:13 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 26 Mar 2021 01:19:21 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:19:27 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 26 Mar 2021 01:20:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 26 Mar 2021 01:20:35 GMT
WORKDIR /home/user
# Fri, 26 Mar 2021 01:20:45 GMT
USER user
# Fri, 26 Mar 2021 01:20:55 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f3b2866c25f0a9167af050d646a7a740ccc88d46e068c90ff28a5c2ec2ee0030`  
		Last Modified: Thu, 25 Mar 2021 22:24:08 GMT  
		Size: 2.8 MB (2813115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c86a2b2846b9a05e2deb4452ef826e8aa09d0d3b0b0ad866470ca47fcc0010b`  
		Last Modified: Fri, 26 Mar 2021 01:21:23 GMT  
		Size: 9.6 MB (9642108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f273ec2efe1d38112809f70cfe7a4c8f2912c0d43d784b03bfd2584665034e`  
		Last Modified: Fri, 26 Mar 2021 01:21:18 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a46d376716d33d6040dc26a63f40a6c19a9ea7b6a3680fc69e4bc7405792b55`  
		Last Modified: Fri, 26 Mar 2021 01:21:22 GMT  
		Size: 6.5 MB (6480769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:3c9d5482055f570989dac4b779ed2dd61aa3962b700a0a86135c9e9bb94205f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18849651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d3485e43acc5bf841c450ebc9d4ec75ea06ba436106b891755b7f4395339b5`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:34 GMT
ADD file:44e2c7cd992fc98df702bef7022e0f8c4ee86312c311ab5ae185fd5fc878edf9 in / 
# Thu, 25 Mar 2021 22:41:34 GMT
CMD ["/bin/sh"]
# Thu, 25 Mar 2021 23:59:56 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 25 Mar 2021 23:59:57 GMT
ENV HOME=/home/user
# Thu, 25 Mar 2021 23:59:58 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 25 Mar 2021 23:59:58 GMT
ENV LANG=C.UTF-8
# Thu, 25 Mar 2021 23:59:58 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 26 Mar 2021 00:00:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 26 Mar 2021 00:00:48 GMT
WORKDIR /home/user
# Fri, 26 Mar 2021 00:00:49 GMT
USER user
# Fri, 26 Mar 2021 00:00:49 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a266c0a9554add02ea09a46b8584cb36b7f606b7b4398b9ad7369f899f8360df`  
		Last Modified: Thu, 25 Mar 2021 22:42:07 GMT  
		Size: 2.6 MB (2602387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3247e0e05b318025a2d06f5368689c9847b298d64ed74c4f1595537be0b5c108`  
		Last Modified: Fri, 26 Mar 2021 00:01:17 GMT  
		Size: 10.0 MB (9983489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc605ff0a3f649f05afe38576d87bcc3ec1b087706cf95b44cfba2fdec1d77f`  
		Last Modified: Fri, 26 Mar 2021 00:01:15 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed45869f07cd143be2d9406f2a3ea7493dd8536819c152ecea64b0ad8c9da02`  
		Last Modified: Fri, 26 Mar 2021 00:01:16 GMT  
		Size: 6.3 MB (6262509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:alpine`

```console
$ docker pull irssi@sha256:eda9ee756ac46d776ad5ff176894bedc8dfd6f8fb347b1e187714a263c54c7e5
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
$ docker pull irssi@sha256:e9f7fca8e1035fed887c65299debd1c144dc2795ed2cd70897ea33a94537a663
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18637035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:200fcb1a18950b1666d02171cfd5fc98329498d7b47076b8c551e632f92cbb37`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Fri, 12 Mar 2021 11:06:48 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 12 Mar 2021 11:06:49 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 11:06:50 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 11:06:51 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 11:06:51 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 11:08:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 12 Mar 2021 11:08:21 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 11:08:21 GMT
USER user
# Fri, 12 Mar 2021 11:08:22 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ceb86e4dfc3e51177b0c9bebe5e21c4f62846f82bb31e9c3df05d61b12686b`  
		Last Modified: Fri, 12 Mar 2021 11:09:08 GMT  
		Size: 9.5 MB (9546291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcdb0e3bcaae9496a4170e17023710d0c83a9b50295582212ab80da6b1fea415`  
		Last Modified: Fri, 12 Mar 2021 11:09:05 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef393ac458300cb54e5348a4fad9fdacb7e8ff40df4246c6beec666e09f6bf22`  
		Last Modified: Fri, 12 Mar 2021 11:09:08 GMT  
		Size: 6.3 MB (6277814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:1f5c7f3acf830fde5a0b1b2a03c8d4c241c16f80075fa9354eee2fedcda705e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17380720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71696b9d35a21e30b8716ccac8b96700bd5f52f029875b05bbae25c07cf2482a`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 21:24:35 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 17 Feb 2021 21:24:36 GMT
ENV HOME=/home/user
# Wed, 17 Feb 2021 21:24:39 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 17 Feb 2021 21:24:40 GMT
ENV LANG=C.UTF-8
# Wed, 17 Feb 2021 21:24:41 GMT
ENV IRSSI_VERSION=1.2.2
# Wed, 17 Feb 2021 21:25:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 17 Feb 2021 21:25:34 GMT
WORKDIR /home/user
# Wed, 17 Feb 2021 21:25:35 GMT
USER user
# Wed, 17 Feb 2021 21:25:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ff4c5d9d970b7aea5a3154a048a8dffdecaa2ba25b1ca324fe17c97846b341`  
		Last Modified: Wed, 17 Feb 2021 21:25:58 GMT  
		Size: 8.8 MB (8779079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762491e3840e0e26a34e0b701ff53443ad7810f8597293077dc34d419566d287`  
		Last Modified: Wed, 17 Feb 2021 21:25:54 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8ff637f1f0558e9446a89673d71ef57ac31f70c30723de693a929ae08bef99`  
		Last Modified: Wed, 17 Feb 2021 21:25:56 GMT  
		Size: 6.0 MB (5978332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:115a46cdc50bac16442fd75d0074f03fb6cd0a34fbed184d1c54c510721362f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16827376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca8749a9d6b447f282bbe9655d0f57d542f83ba2d22f455135da140d63b51ccc`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 25 Mar 2021 22:05:53 GMT
ADD file:44ef6cff6e7d37a67c5846eb792fec65025702c00c56ff96801ac79bf81b0cc3 in / 
# Thu, 25 Mar 2021 22:05:55 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:34:24 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 26 Mar 2021 01:34:27 GMT
ENV HOME=/home/user
# Fri, 26 Mar 2021 01:34:43 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 26 Mar 2021 01:34:57 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:34:58 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 26 Mar 2021 01:36:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 26 Mar 2021 01:36:30 GMT
WORKDIR /home/user
# Fri, 26 Mar 2021 01:36:32 GMT
USER user
# Fri, 26 Mar 2021 01:36:33 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6c1162af251f0d5ab4945f8506f3265b86d0a03cda37f703c2446a71a233bc20`  
		Last Modified: Thu, 25 Mar 2021 22:07:21 GMT  
		Size: 2.4 MB (2423999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc3e3c0e1237dab78d7546291ec3af3710654eb21a6a41d24735358183e2ef4`  
		Last Modified: Fri, 26 Mar 2021 01:37:10 GMT  
		Size: 8.6 MB (8630420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46da2938095dda6c27bc8a3751401e2068f53541132e174a7ab8d3da0c47260e`  
		Last Modified: Fri, 26 Mar 2021 01:37:03 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b70fe4c17acc8e06c03a1657b143ba9dcfb902d3e8bb458944dc57ad752b3f`  
		Last Modified: Fri, 26 Mar 2021 01:37:07 GMT  
		Size: 5.8 MB (5771687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:7e952f73bc19dba012551a010556a9f2830354aafeabc65ab98b99fb46b78be0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18484286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fba76d5f44622ab0ff706b71f209a569b5444a6d04f17ffb9db797df41fa954`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:25:09 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 26 Mar 2021 01:25:11 GMT
ENV HOME=/home/user
# Fri, 26 Mar 2021 01:25:14 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 26 Mar 2021 01:25:15 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:25:16 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 26 Mar 2021 01:26:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 26 Mar 2021 01:26:17 GMT
WORKDIR /home/user
# Fri, 26 Mar 2021 01:26:19 GMT
USER user
# Fri, 26 Mar 2021 01:26:20 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26913993fc81df5a50e2d87a7112af3450e67ba4062fd5b9165a12009ab102f2`  
		Last Modified: Fri, 26 Mar 2021 01:26:54 GMT  
		Size: 9.5 MB (9542280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7fd25418e612aa429275628f3f13f275019cecdb3a1fb98b1afa34d975ca4d7`  
		Last Modified: Fri, 26 Mar 2021 01:26:50 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9349288f06be1425b975ad9bdf02398a063d15cadeb878a254a09595abc9d5f9`  
		Last Modified: Fri, 26 Mar 2021 01:26:52 GMT  
		Size: 6.2 MB (6228838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; 386

```console
$ docker pull irssi@sha256:6a0279ffd88af96276b4e6f77f91af191a67083b06160756a00f6fd1e3009982
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17697705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:227f5732bdf7871068257a1c48d0bb2904bccbbbea092e0f8cae703b70f791cb`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 25 Mar 2021 22:38:25 GMT
ADD file:8953415d4b98f486af17a39ba53b38f7262aa590734c18ff9318927e5a705baf in / 
# Thu, 25 Mar 2021 22:38:26 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:59:51 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 26 Mar 2021 01:59:52 GMT
ENV HOME=/home/user
# Fri, 26 Mar 2021 01:59:53 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 26 Mar 2021 01:59:53 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:59:53 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 26 Mar 2021 02:00:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 26 Mar 2021 02:00:50 GMT
WORKDIR /home/user
# Fri, 26 Mar 2021 02:00:50 GMT
USER user
# Fri, 26 Mar 2021 02:00:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1fbd1c9912b638ce64a4740e3af7a3a03452f8705b8103950d677f1d79ae8164`  
		Last Modified: Thu, 25 Mar 2021 22:39:34 GMT  
		Size: 2.8 MB (2818129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1a8934e2dc515a457fca6334af810a53eb34db25494b16839f0b133883627c`  
		Last Modified: Fri, 26 Mar 2021 02:01:26 GMT  
		Size: 8.9 MB (8913129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2783e7c652bc8b874a3a033a780ab09a31d28cfee03a5b91e6c08f0d46c28db`  
		Last Modified: Fri, 26 Mar 2021 02:01:23 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6391518bf9cffe8e3d6ce27412a2de4c2fd1d1d0cb4da142b31eb2a2b507f7`  
		Last Modified: Fri, 26 Mar 2021 02:01:25 GMT  
		Size: 6.0 MB (5965177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:3d1948a0ceda5993a4cfdeefa7dd4d31fd815055235e99ae4c1e0d904dd1412a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18937265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe6dfa6dd0254312eba3b51ef834249b06061fa100633addef7bbbf84c42b637`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:28 GMT
ADD file:f91f8e0aa646cb847f6e210056280f9332382ad2f8d6a8839fd9aa69b81c4a2a in / 
# Thu, 25 Mar 2021 22:22:30 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:18:40 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 26 Mar 2021 01:18:48 GMT
ENV HOME=/home/user
# Fri, 26 Mar 2021 01:19:13 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 26 Mar 2021 01:19:21 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:19:27 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 26 Mar 2021 01:20:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 26 Mar 2021 01:20:35 GMT
WORKDIR /home/user
# Fri, 26 Mar 2021 01:20:45 GMT
USER user
# Fri, 26 Mar 2021 01:20:55 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f3b2866c25f0a9167af050d646a7a740ccc88d46e068c90ff28a5c2ec2ee0030`  
		Last Modified: Thu, 25 Mar 2021 22:24:08 GMT  
		Size: 2.8 MB (2813115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c86a2b2846b9a05e2deb4452ef826e8aa09d0d3b0b0ad866470ca47fcc0010b`  
		Last Modified: Fri, 26 Mar 2021 01:21:23 GMT  
		Size: 9.6 MB (9642108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f273ec2efe1d38112809f70cfe7a4c8f2912c0d43d784b03bfd2584665034e`  
		Last Modified: Fri, 26 Mar 2021 01:21:18 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a46d376716d33d6040dc26a63f40a6c19a9ea7b6a3680fc69e4bc7405792b55`  
		Last Modified: Fri, 26 Mar 2021 01:21:22 GMT  
		Size: 6.5 MB (6480769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; s390x

```console
$ docker pull irssi@sha256:3c9d5482055f570989dac4b779ed2dd61aa3962b700a0a86135c9e9bb94205f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18849651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d3485e43acc5bf841c450ebc9d4ec75ea06ba436106b891755b7f4395339b5`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:34 GMT
ADD file:44e2c7cd992fc98df702bef7022e0f8c4ee86312c311ab5ae185fd5fc878edf9 in / 
# Thu, 25 Mar 2021 22:41:34 GMT
CMD ["/bin/sh"]
# Thu, 25 Mar 2021 23:59:56 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 25 Mar 2021 23:59:57 GMT
ENV HOME=/home/user
# Thu, 25 Mar 2021 23:59:58 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 25 Mar 2021 23:59:58 GMT
ENV LANG=C.UTF-8
# Thu, 25 Mar 2021 23:59:58 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 26 Mar 2021 00:00:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 26 Mar 2021 00:00:48 GMT
WORKDIR /home/user
# Fri, 26 Mar 2021 00:00:49 GMT
USER user
# Fri, 26 Mar 2021 00:00:49 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a266c0a9554add02ea09a46b8584cb36b7f606b7b4398b9ad7369f899f8360df`  
		Last Modified: Thu, 25 Mar 2021 22:42:07 GMT  
		Size: 2.6 MB (2602387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3247e0e05b318025a2d06f5368689c9847b298d64ed74c4f1595537be0b5c108`  
		Last Modified: Fri, 26 Mar 2021 00:01:17 GMT  
		Size: 10.0 MB (9983489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc605ff0a3f649f05afe38576d87bcc3ec1b087706cf95b44cfba2fdec1d77f`  
		Last Modified: Fri, 26 Mar 2021 00:01:15 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed45869f07cd143be2d9406f2a3ea7493dd8536819c152ecea64b0ad8c9da02`  
		Last Modified: Fri, 26 Mar 2021 00:01:16 GMT  
		Size: 6.3 MB (6262509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:latest`

```console
$ docker pull irssi@sha256:575d68fdda2e48da8abc975a602afab57a32dcd210101706492cb6c2fe9a0bde
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
$ docker pull irssi@sha256:7d442244c3d5d97b95ac0c0ca9be95165bd30b909621e572bed3f954cbdd3389
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50568077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5911d6f3416365bd18470b92a5ceca377f1b3c9337c0c9fbaec9891141aad195`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 11:04:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 11:04:57 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 11:04:59 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 11:04:59 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 11:04:59 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 11:06:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 11:06:38 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 11:06:39 GMT
USER user
# Fri, 12 Mar 2021 11:06:39 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa82220b80b6fa32a82277cdcf2e1a8b7350d3eb49dd723043dd4dfee38a4d7c`  
		Last Modified: Fri, 12 Mar 2021 11:08:48 GMT  
		Size: 17.0 MB (17033440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cab4a877a41e1cfdc916be3c7625c0f914119e3ad2abc2ad4b159e3baa1e0e`  
		Last Modified: Fri, 12 Mar 2021 11:08:42 GMT  
		Size: 4.2 KB (4208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a6c2e5e877ecd200d4c003252a7db5a9797a0f90feeadeded09ddd3a2f1eae`  
		Last Modified: Fri, 12 Mar 2021 11:08:44 GMT  
		Size: 6.4 MB (6429428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm variant v5

```console
$ docker pull irssi@sha256:9e24e92190db23a06e2692b1a49ce3438288a26b7bd501bd58fb0f84caf11185
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46843846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7aaa632856c778560f9f55abbd065b8f2980a83ed0420f7607c9c2879be3124`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 01:52:27 GMT
ADD file:8e357182800adfe658856515726f1e012cc120349f0f305692cf50282f6d8b7b in / 
# Fri, 12 Mar 2021 01:52:29 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:50:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:50:23 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 02:50:26 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 02:50:26 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 02:50:27 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 02:52:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 02:52:15 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 02:52:16 GMT
USER user
# Fri, 12 Mar 2021 02:52:17 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:9babb1be2e38b3bddad5a4e05bb34173369ae3472c0c0d8668853011cd65969f`  
		Last Modified: Fri, 12 Mar 2021 02:02:01 GMT  
		Size: 24.8 MB (24845925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e25b60c55c4d12e692a0e8d8966b14cc0e5085187f8a343a4d84956e316ffb6`  
		Last Modified: Fri, 12 Mar 2021 02:52:43 GMT  
		Size: 15.9 MB (15931049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67829e638098b8d79aa01cad5ded7c1cb12071840410b02090c62c9f8edd7fa`  
		Last Modified: Fri, 12 Mar 2021 02:52:36 GMT  
		Size: 4.2 KB (4196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd508527cc93ad08df450347b6d21d5032a28fa0488016291c8abe88d2de5ce`  
		Last Modified: Fri, 12 Mar 2021 02:52:38 GMT  
		Size: 6.1 MB (6062676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm variant v7

```console
$ docker pull irssi@sha256:32f2605101fe727c1455d51042f015e19827a7866ddedc3d22d5ad735064ba81
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44234132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8977a6c44287eae4a76289108e4ce0b1ac7425a4f5c9b9e02d8eea74df22d92e`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 02:00:12 GMT
ADD file:123da9848f87c8ed4c5122a104b8650564c09767725916f822def7b645a019f1 in / 
# Fri, 12 Mar 2021 02:00:14 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 04:56:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 04:56:26 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 04:56:28 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 04:56:29 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 04:56:29 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 04:57:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 04:58:00 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 04:58:01 GMT
USER user
# Fri, 12 Mar 2021 04:58:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:e12d26f75fe8b7fd14712965ff5178762227d07d2151bb35fa21105ddfc4a14a`  
		Last Modified: Fri, 12 Mar 2021 02:10:28 GMT  
		Size: 22.7 MB (22709467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f1dc2c6549f399aec326fad72f414b645d8f953321c14032de6b908cb94b42`  
		Last Modified: Fri, 12 Mar 2021 04:58:35 GMT  
		Size: 15.6 MB (15590035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f0a2c1c5574bae60fc820eb688fd9317c9fb76c8fbc8127760891fb60261f65`  
		Last Modified: Fri, 12 Mar 2021 04:58:27 GMT  
		Size: 4.2 KB (4195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc5f47c56a02365fc5a6dfa4ce63062636df3340e67756c0413eaab1feed334`  
		Last Modified: Fri, 12 Mar 2021 04:58:29 GMT  
		Size: 5.9 MB (5930435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:02686cdc34ce5dd16345df7292a3064f22a074585de5547ad7e4691b5547fea9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49052058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d3942313a1f6e377d074ac70be91b98b22f099283c005a45801c8b265bce22b`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 01:53:53 GMT
ADD file:6130ddc0a939dd72c0614de4aa77de47aa16fe211274bacb31995aa1a0526164 in / 
# Fri, 12 Mar 2021 01:53:56 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 17:43:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 17:43:25 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 17:43:27 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 17:43:28 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 17:43:29 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 17:45:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 17:45:04 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 17:45:05 GMT
USER user
# Fri, 12 Mar 2021 17:45:06 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:706ee5d0a6b53d9257cbea22d8409fb22c867ab3a001c65f6b8bfd37dace0e58`  
		Last Modified: Fri, 12 Mar 2021 02:01:39 GMT  
		Size: 25.9 MB (25856512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc1a0fcfd5b5c8a6304adad324f44c13c6ebe3062940f9da8318bbbc1b57a6d`  
		Last Modified: Fri, 12 Mar 2021 17:45:35 GMT  
		Size: 16.8 MB (16803429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d79819a4c69ccab094f2aaee1ee4c383589114a44ea07437262e24e3335b026`  
		Last Modified: Fri, 12 Mar 2021 17:45:28 GMT  
		Size: 4.2 KB (4219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4834bc87f80d7b0ee15ef328f8981b1fa7cdc1e1f761286aa1e57e32fe2c2194`  
		Last Modified: Fri, 12 Mar 2021 17:45:31 GMT  
		Size: 6.4 MB (6387898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; 386

```console
$ docker pull irssi@sha256:1c1a9780a77d5593848ec9f66c0c4a1db62d6c1ab536b03499426dc3230db8aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50425172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4233b7a266ca3253ce68dd157a42b68fce5841ab7212bd92ad8c98df61c29a9d`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 01:44:27 GMT
ADD file:90c103e04bd6fe0f39733cbf8eb2d8845aed3e4fc3fd1e5c3354df69e40aa615 in / 
# Fri, 12 Mar 2021 01:44:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 21:13:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 21:13:08 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 21:13:09 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 21:13:09 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 21:13:09 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 21:14:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 21:14:46 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 21:14:46 GMT
USER user
# Fri, 12 Mar 2021 21:14:46 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:0898aa7472f57f223652846337cf862f142e109d0c039b41886e7f20c345f85e`  
		Last Modified: Fri, 12 Mar 2021 01:52:08 GMT  
		Size: 27.8 MB (27760948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7adad1dd74fcd0ecb398e894c7f8861e0f07cfc0bdb77cbc12e24b5cb793c68c`  
		Last Modified: Fri, 12 Mar 2021 21:16:47 GMT  
		Size: 16.6 MB (16558205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b2cf9a9a3e742c4c14027ae25b0d3325b123f048d89744ac861296cfdcfb46c`  
		Last Modified: Fri, 12 Mar 2021 21:16:37 GMT  
		Size: 4.2 KB (4192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c8264777e37ece315309662ef9c2042aed482ebfe6288ccebe91922fcc072fb`  
		Last Modified: Fri, 12 Mar 2021 21:16:41 GMT  
		Size: 6.1 MB (6101827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; mips64le

```console
$ docker pull irssi@sha256:11dcb1ea1f6a694137f6869a3a5d24e9c73d1d5e898b9feaf60779bc9d7ea9f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47775886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd123eb9b8194e1dce76a162a06d55a66f76c4a1947e7375174754f54dd208b9`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 02:10:02 GMT
ADD file:491c5ca15fe098b83de42861289c216c693d788a1f9e739a78acefb0cad453c8 in / 
# Fri, 12 Mar 2021 02:10:03 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 03:00:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 03:00:09 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 03:00:11 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 03:00:12 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 03:00:12 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 03:02:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 03:02:45 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 03:02:45 GMT
USER user
# Fri, 12 Mar 2021 03:02:45 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:d0b6b2cc51bdde474395b8c32ff8012e471727bba69f221cfb79b46e8283f047`  
		Last Modified: Fri, 12 Mar 2021 02:17:07 GMT  
		Size: 25.8 MB (25772338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f07eae8650e63d8e5c5c11fa467c8cb401e24859b6c3eb97d1cb4beb77ca33f`  
		Last Modified: Fri, 12 Mar 2021 03:03:23 GMT  
		Size: 15.7 MB (15709110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069673a50a0626dfb618561bcc33174f5af67375b61426deebf65feeb686a270`  
		Last Modified: Fri, 12 Mar 2021 03:03:06 GMT  
		Size: 4.2 KB (4179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0e23988c6b3499aefb8ddcbd10d127bd56e8d4c22e34889250b9602c012f9e`  
		Last Modified: Fri, 12 Mar 2021 03:03:11 GMT  
		Size: 6.3 MB (6290259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; ppc64le

```console
$ docker pull irssi@sha256:042a76fc7d37dc6e7fe106e64a43037de8d4f6162bed9362f02ce1cb46d89b05
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.7 MB (54748353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e21ad9386f16b76532f9ca7679ab7b1a1b7ae07c665005d3540d630efb08a2e`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 02:32:43 GMT
ADD file:6a0c0cfa71979cf6fdd859dce1e32582f0e55ed382b9e17b77a2001defc2c9db in / 
# Fri, 12 Mar 2021 02:32:50 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 05:21:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 05:21:53 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 05:22:19 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 05:22:33 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 05:22:47 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 05:33:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 05:33:07 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 05:33:15 GMT
USER user
# Fri, 12 Mar 2021 05:33:35 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1d686056fdac1848f4fd78ba2b335502055ffe98c79619e21d0c2fb7db95257e`  
		Last Modified: Fri, 12 Mar 2021 02:45:35 GMT  
		Size: 30.5 MB (30525728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ece5dc65262bccb6252440d8c5e1a3dca0ec3603abb9e8b49d82f97d6cb85b9`  
		Last Modified: Fri, 12 Mar 2021 05:34:13 GMT  
		Size: 17.4 MB (17437414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc49adb12fb0cd54dc637a9532fbc83cb4e037e6b2bd4e5971948ffbf5f5d8a`  
		Last Modified: Fri, 12 Mar 2021 05:34:08 GMT  
		Size: 4.2 KB (4214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559c20b0868126ced94ac9ef5df1d609e27bd8abfc99fde3a2676da11e98a227`  
		Last Modified: Fri, 12 Mar 2021 05:34:11 GMT  
		Size: 6.8 MB (6780997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; s390x

```console
$ docker pull irssi@sha256:5d0796552e1559a6f77853b1e52d7e7ae5b2a7ea5a36c11cee0ef8f99a528f74
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49012748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f31d157ba631157ab487f5b32e1ef32f016af19318e4009606af63816fcc1530`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Mar 2021 01:46:04 GMT
ADD file:afec039adf230a9186a38b57eed85262696f8d178ac649a445657066f16fe806 in / 
# Fri, 12 Mar 2021 01:46:07 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:53:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:54:00 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 02:54:00 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 02:54:01 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 02:54:01 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 02:54:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Fri, 12 Mar 2021 02:54:49 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 02:54:50 GMT
USER user
# Fri, 12 Mar 2021 02:54:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:d41215965c091534e809ab2e8f4a2c1cebee3de536c2c74a7bc8302bbc8af7e1`  
		Last Modified: Fri, 12 Mar 2021 01:50:30 GMT  
		Size: 25.7 MB (25716294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1928942d4ca75c8bd9f793f48c56b77ad65491e9dcaf8f62e83eabffc0e2cd`  
		Last Modified: Fri, 12 Mar 2021 02:55:16 GMT  
		Size: 16.9 MB (16908957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e83765cc93c78e150ab9768d197c9d289926fe154516b60c0ac8e2d9eb17add`  
		Last Modified: Fri, 12 Mar 2021 02:55:13 GMT  
		Size: 4.2 KB (4212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9e5915a1e5381a069146b20a3141656c4e9aa3b2de62aa599e87e3c0661289`  
		Last Modified: Fri, 12 Mar 2021 02:55:14 GMT  
		Size: 6.4 MB (6383285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
