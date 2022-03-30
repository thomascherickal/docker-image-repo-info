<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `irssi`

-	[`irssi:1`](#irssi1)
-	[`irssi:1-alpine`](#irssi1-alpine)
-	[`irssi:1.2`](#irssi12)
-	[`irssi:1.2-alpine`](#irssi12-alpine)
-	[`irssi:1.2.3`](#irssi123)
-	[`irssi:1.2.3-alpine`](#irssi123-alpine)
-	[`irssi:alpine`](#irssialpine)
-	[`irssi:latest`](#irssilatest)

## `irssi:1`

```console
$ docker pull irssi@sha256:480c39b4457078a69d69e8cc069a98f87278350e1f6ca14d4cbe79616f0e00b1
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
$ docker pull irssi@sha256:898197fd559f9b169fa4d36cb9424351490be12245aa2e2c4e85838db057306d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50628334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a33ad04f436ec45a3cc476c2c220e7d42ce40687a2c41dc99cc020453041b3`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 16:39:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 16:39:05 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 16:39:06 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 16:39:06 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 16:39:06 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 16:39:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 16:39:57 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 16:39:57 GMT
USER user
# Tue, 29 Mar 2022 16:39:57 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd2cdd5c22666980d61bf83c478dfc880881556673a21e118f955376664ea2a`  
		Last Modified: Tue, 29 Mar 2022 16:41:14 GMT  
		Size: 17.0 MB (17038736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2861ba30751829fb2555bb33ca9170f484208f0049973581aa13988f65bcce`  
		Last Modified: Tue, 29 Mar 2022 16:41:10 GMT  
		Size: 4.2 KB (4209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bcc182247f746f92a6a75dee26bc22a8d50acc4c3286802af9e38fdd1c0b90`  
		Last Modified: Tue, 29 Mar 2022 16:41:12 GMT  
		Size: 6.4 MB (6433419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm variant v5

```console
$ docker pull irssi@sha256:ce001569547e34819fdf079112b88f49e44b499ed10726ae591cc6c5a0ea2bc9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46893537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f038e776a2c3d5a6f454656fe59c07165ac40653fc18ea19e3ce095e5a5056d`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:51:36 GMT
ADD file:7ac5498e2c44686d7eb272ef7645a0a64486cf942610f6754aa4a932f5b1a4be in / 
# Tue, 29 Mar 2022 00:51:37 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 08:47:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 08:47:02 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 08:47:04 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 08:47:04 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 08:47:05 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 08:48:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 08:48:51 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 08:48:52 GMT
USER user
# Tue, 29 Mar 2022 08:48:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8f10b1b67f0119a2dd5f838a3e98ab2c412e4b51fb1e4841e2b79fd4cae86105`  
		Last Modified: Tue, 29 Mar 2022 01:06:51 GMT  
		Size: 24.9 MB (24887495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb68688aa70be630bab2170a39e77d005f229ab6390b76e8d3b9a89acf825b8`  
		Last Modified: Tue, 29 Mar 2022 08:49:39 GMT  
		Size: 15.9 MB (15937355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f462c871b83b3653daf80a7cec6d9d06057396022a1e2b36a5764dcc29588a3`  
		Last Modified: Tue, 29 Mar 2022 08:49:28 GMT  
		Size: 4.2 KB (4199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae06e20e90eb68e6394cd65e5487477d7353a5816b39fa872fac1074888de42c`  
		Last Modified: Tue, 29 Mar 2022 08:49:31 GMT  
		Size: 6.1 MB (6064488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm variant v7

```console
$ docker pull irssi@sha256:3db3ddfc45fb2ccf78e4b7349fa0fd23aa6e59eaf69371032c89f4b995b2baf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44287695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8432232c7fa73842270a6402575d03dcd1af079cced86028166d84a2623f94cc`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 02:19:40 GMT
ADD file:8d54e000817531229c35a32eee074105c7b4d3c08b7ca56b1abdd80571687f28 in / 
# Tue, 29 Mar 2022 02:19:41 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:21:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:21:34 GMT
ENV HOME=/home/user
# Wed, 30 Mar 2022 02:21:36 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 30 Mar 2022 02:21:37 GMT
ENV LANG=C.UTF-8
# Wed, 30 Mar 2022 02:21:37 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 30 Mar 2022 02:23:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 30 Mar 2022 02:23:23 GMT
WORKDIR /home/user
# Wed, 30 Mar 2022 02:23:23 GMT
USER user
# Wed, 30 Mar 2022 02:23:24 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:d4bf0b27c669e589de33695047d638174fc2ca819a4366d5f80d1ad6b01c0c0e`  
		Last Modified: Tue, 29 Mar 2022 02:35:26 GMT  
		Size: 22.8 MB (22753045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac8262be381607606ea917e05e243851b4d99f2c3b81758f6312dfd87969356`  
		Last Modified: Wed, 30 Mar 2022 02:26:12 GMT  
		Size: 15.6 MB (15597948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62dbb031a500a927ff9934a53e57156d7a1faa17d61c5bd2e83339d685db97a8`  
		Last Modified: Wed, 30 Mar 2022 02:25:56 GMT  
		Size: 4.2 KB (4196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:489ce9745374ad929508ff3be1139e1d7e92b1035939d613574df8757f45f1ba`  
		Last Modified: Wed, 30 Mar 2022 02:26:00 GMT  
		Size: 5.9 MB (5932506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:8c11bc795decb16053eee4599521d727932b0b65a6043eb2d753763f6a0fcba8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48915028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:325958a38fb96c65a0cbe50172b3b831b9e521e2f46956e55bf1228253f6885e`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:42 GMT
ADD file:fdc8a5391a75cbf8c121f8f799ca08e94d2b3967b2546b36231c9297f7ce2151 in / 
# Tue, 29 Mar 2022 00:43:43 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 11:58:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 11:58:23 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 11:58:24 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 11:58:25 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 11:58:26 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 11:59:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 11:59:24 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 11:59:25 GMT
USER user
# Tue, 29 Mar 2022 11:59:26 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:5022906f515a0d4ec6bc1d0e5e7a01f47b1fbbb912e7e3f1ace27987169a9a21`  
		Last Modified: Tue, 29 Mar 2022 00:50:58 GMT  
		Size: 25.9 MB (25919777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99733c8db8c4371f3d274a989271d20844041e6ee266e8f74fa0a52e8e126277`  
		Last Modified: Tue, 29 Mar 2022 12:01:08 GMT  
		Size: 16.8 MB (16815150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b028d71796d54b96aa2ef9143f43950b86a4c6451c7da2b4836a693416e08660`  
		Last Modified: Tue, 29 Mar 2022 12:01:04 GMT  
		Size: 4.1 KB (4075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e78bd4b4962d8db2ae26337c77d821e36a0b186d875a7d5626aabe15e2be8e0`  
		Last Modified: Tue, 29 Mar 2022 12:01:05 GMT  
		Size: 6.2 MB (6176026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; 386

```console
$ docker pull irssi@sha256:406c82696ff47006adf53f11781be3f504cc4fe335a780106844f23f6a799af2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50264307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6ac23335fd4259a5aa45431e78631ccb7ba153d3b8b30da64cdff5bdafe99cb`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:42:26 GMT
ADD file:bcf3d504dc285de8b639c7f4017c41a4593a6c2aa6f046c9be79e587d05b5120 in / 
# Tue, 29 Mar 2022 00:42:27 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 05:48:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 05:48:43 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 05:48:44 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 05:48:45 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 05:48:46 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 05:49:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 05:49:35 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 05:49:36 GMT
USER user
# Tue, 29 Mar 2022 05:49:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:65b92490caa5e2c0588fab60d39315a2a8c09aa8ea0fe208d23f6984a47ecc03`  
		Last Modified: Tue, 29 Mar 2022 00:50:02 GMT  
		Size: 27.8 MB (27801252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65153b3620d7c8324690f0556ea546e098d1c5abea0de04cec331abe652fd6cc`  
		Last Modified: Tue, 29 Mar 2022 05:51:09 GMT  
		Size: 16.6 MB (16565592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f81e51b798316e6dddef7d44c46adbbfac04c8639c9c6d7fc569722558240ce`  
		Last Modified: Tue, 29 Mar 2022 05:51:05 GMT  
		Size: 4.1 KB (4052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb19cd58e039f1ea121d78c3603e8bcfac093136e3b920a3ab1df0bbf9ecd21d`  
		Last Modified: Tue, 29 Mar 2022 05:51:06 GMT  
		Size: 5.9 MB (5893411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; mips64le

```console
$ docker pull irssi@sha256:eed1cd2fe79ac4ab10dee6870ffa2be2cec900112d6a0a5d01b0474c5e8301f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47634326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b493b1d75e78f56f629ff77cc840485832b6f90136f061ceff8a2788aa90025`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 07:43:36 GMT
ADD file:7827dc4070f09537c063b825b0b7a5b076fac295f9afa415dee6c5346c38d46b in / 
# Tue, 29 Mar 2022 07:43:40 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 10:26:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 10:26:25 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 10:26:33 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 10:26:36 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 10:26:39 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 10:31:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 10:31:16 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 10:31:19 GMT
USER user
# Tue, 29 Mar 2022 10:31:23 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4a3e27ca4ec7041c36d0e9cbc672ce565851ce1a0cc90120d7a923a938fb3c18`  
		Last Modified: Tue, 29 Mar 2022 07:54:19 GMT  
		Size: 25.8 MB (25818066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2023bef9f22712b6457705ea84614163a3d0a854f38d7f2f13f388c262fd8d68`  
		Last Modified: Tue, 29 Mar 2022 10:31:51 GMT  
		Size: 15.7 MB (15731870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783dfb57d1278d639db4a6acd55eea930b6387da357be8c4e1ef6af2c734ff13`  
		Last Modified: Tue, 29 Mar 2022 10:31:37 GMT  
		Size: 4.1 KB (4069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e297148bdf9b4491afc8d6b2898998918425c1e35865b360d93b281abe77ce`  
		Last Modified: Tue, 29 Mar 2022 10:31:40 GMT  
		Size: 6.1 MB (6080321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; ppc64le

```console
$ docker pull irssi@sha256:a460c3520546307e352a19d055007a7fcba927f322c545e3e7296c1bfdf74592
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54787995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f694d959fe967b7564e8a7cdaf212e3d814c5d6b79c1d3696f77b35c476d8ea`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:59 GMT
ADD file:7271d778d432a07f57fedf8d50d83699ef545acc9db9346f6fe75b0054af4cd1 in / 
# Tue, 29 Mar 2022 00:23:00 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 07:34:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 07:35:01 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 07:35:09 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 07:35:12 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 07:35:15 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 07:39:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 07:39:58 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 07:39:59 GMT
USER user
# Tue, 29 Mar 2022 07:40:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:7db831386ce67ac1cf2b4f1513fe3746c9ea2b8d4c82efca75be638eaf533614`  
		Last Modified: Tue, 29 Mar 2022 00:34:41 GMT  
		Size: 30.6 MB (30560163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6f0e2fb83c5287040e529ec1e0cc34c5383697a80a278632cddf17a110ab26`  
		Last Modified: Tue, 29 Mar 2022 07:42:17 GMT  
		Size: 17.4 MB (17440827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9798211288cab71997a2ba40949386224112d0754a517ece37e3cfc68ccc5ad0`  
		Last Modified: Tue, 29 Mar 2022 07:42:12 GMT  
		Size: 4.2 KB (4216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dadee1dc4117b4a1068f72e957d68471ff9f516c4db70a938e36a427e6f45b7`  
		Last Modified: Tue, 29 Mar 2022 07:42:14 GMT  
		Size: 6.8 MB (6782789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; s390x

```console
$ docker pull irssi@sha256:8aa6207ef3bc8833bb6a35d3870a604c6e90fc607bf1bbebab6688fb11f2d4ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49068950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9b140f48665cda5494c089acdb6eae60f96d15c3fb4dd0ba4b19d99953db655`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:52:27 GMT
ADD file:dbf01085079906b34f3ec9db0b9ce31aa1466b935a47e8e30772a5488f76fec0 in / 
# Tue, 29 Mar 2022 00:52:29 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 15:57:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 15:57:55 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 15:57:56 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 15:57:56 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 15:57:56 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 15:58:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 15:58:46 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 15:58:46 GMT
USER user
# Tue, 29 Mar 2022 15:58:46 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:66ccc81b275f683f44a0f40ddce6992117eefe92dca84fadf6d2e51c22d11a64`  
		Last Modified: Tue, 29 Mar 2022 01:10:22 GMT  
		Size: 25.8 MB (25765916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f745ab618468906119bb54aef0c97df6677ebed5694c4d839b8103c60531d8`  
		Last Modified: Tue, 29 Mar 2022 16:00:54 GMT  
		Size: 16.9 MB (16914174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e65abef5df82c79a408eb80534564b0361dc35744b6aa982b493c4f0e59e55d4`  
		Last Modified: Tue, 29 Mar 2022 16:00:54 GMT  
		Size: 4.2 KB (4216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a6b20318811928ca8b7d3a3a3229cab3b5ac4bd24212ec30916433aef99d73`  
		Last Modified: Tue, 29 Mar 2022 16:00:54 GMT  
		Size: 6.4 MB (6384644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1-alpine`

```console
$ docker pull irssi@sha256:fc0f0ae29aedc3e3dfee43d698d4de461180f8959428023f3a5bd95b61433f18
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
$ docker pull irssi@sha256:d7bbd05aae77230148f9a3af4a07717c5626cdb254caa1dc239bfc8866124f3e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18648371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b63678d9d2827a5a4d447b135a05921b9b618d639a9641f3970ce71fbad41c58`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:46 GMT
ADD file:a2ef39a587aac85256b55bee81f17d73aaa7154b2a32a31527c7803fb889f2e7 in / 
# Tue, 29 Mar 2022 00:19:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 16:40:04 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 16:40:04 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 16:40:05 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 16:40:05 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 16:40:05 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 16:40:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 16:40:49 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 16:40:49 GMT
USER user
# Tue, 29 Mar 2022 16:40:49 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b9c05db88786fd3c89b78787631257301391f898c03ba50553b556630046a741`  
		Last Modified: Tue, 29 Mar 2022 00:20:43 GMT  
		Size: 2.8 MB (2819223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c516145633461419b5a658706a7453eb731aaf449afd25b5996b275b8692bb0e`  
		Last Modified: Tue, 29 Mar 2022 16:41:30 GMT  
		Size: 9.5 MB (9540598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d5246be564bab1c71a70cfe50bdab883825a0ec36ed4a79b2c6730ee23849f`  
		Last Modified: Tue, 29 Mar 2022 16:41:28 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0543c4eb94b3e7485a55ed115e70d48d246fc300c3430bf71f774b156b56f7`  
		Last Modified: Tue, 29 Mar 2022 16:41:29 GMT  
		Size: 6.3 MB (6287279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:8f4fc787e0e6164fcc251c034c9fbff27d3a81fdda0c2a82c859312e16aa677a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17385391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:facc4fa1f84eebf576961df4f191b9e7763fd7f790ee44517915d56ab994e139`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:56 GMT
ADD file:23d913551f75313e359a4e93592ea0a9655e1a7c2bec5fddd210717d70c3114b in / 
# Tue, 29 Mar 2022 00:49:57 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 14:24:05 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 14:24:06 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 14:24:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 14:24:08 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 14:24:08 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 14:25:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 14:25:17 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 14:25:18 GMT
USER user
# Tue, 29 Mar 2022 14:25:18 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:eba0847afba90891ea7dae672f5dadfa405a822df0bc9c00b9e3328fd5fd889c`  
		Last Modified: Tue, 29 Mar 2022 00:51:57 GMT  
		Size: 2.6 MB (2625139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475d9671ce28a72461f25c4368162f9eac018ffced5ee61d17852dac61f60923`  
		Last Modified: Tue, 29 Mar 2022 14:25:59 GMT  
		Size: 8.8 MB (8771957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223ba1931ceb81e998f74a59ac08d88367fa3be50d7864242a41937e0a744bb8`  
		Last Modified: Tue, 29 Mar 2022 14:25:51 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9769077f19f3aaf8bd8f635611ddc58ab0133ca7a4207c1e68a6b84b68056afa`  
		Last Modified: Tue, 29 Mar 2022 14:25:55 GMT  
		Size: 6.0 MB (5987025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:645f3bdeef2e0deedf6315612f78330153c94d47580d86102653f44c653cbcfb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16839519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c53528eb26529ee3c99677c1271b1f6fe9b45db594e0a4d5f16d5bb51dd858cf`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 02:13:57 GMT
ADD file:9995ada53dfe4b82c6c01a9143cdcf8aa3aabac359fa023f5fa4da85e7a88704 in / 
# Tue, 29 Mar 2022 02:13:58 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 02:23:53 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 30 Mar 2022 02:23:53 GMT
ENV HOME=/home/user
# Wed, 30 Mar 2022 02:23:55 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 30 Mar 2022 02:23:55 GMT
ENV LANG=C.UTF-8
# Wed, 30 Mar 2022 02:23:56 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 30 Mar 2022 02:25:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 30 Mar 2022 02:25:01 GMT
WORKDIR /home/user
# Wed, 30 Mar 2022 02:25:01 GMT
USER user
# Wed, 30 Mar 2022 02:25:02 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:9e629c3986cd97398b7f233a377ad62b7d37cbccbcba0bbae7c5bc600ea73620`  
		Last Modified: Tue, 29 Mar 2022 02:15:59 GMT  
		Size: 2.4 MB (2427878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef6405d47acdbe9f502c4db8aa5db79963974eb33c7c7db6367815d922d0d34`  
		Last Modified: Wed, 30 Mar 2022 02:26:38 GMT  
		Size: 8.6 MB (8626355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360bcdf4cc43bbde189db2de03107a0ef571fdf754c37919f41990fba758ab25`  
		Last Modified: Wed, 30 Mar 2022 02:26:31 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3419b023d43ddc842375a10a3b44776c2694b31cdb493104714b3331e346e099`  
		Last Modified: Wed, 30 Mar 2022 02:26:34 GMT  
		Size: 5.8 MB (5784017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:dfc50492eaf70eaec1101ec66e1039ff67a7db7dd5800d74dc45a4a739e02c20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18505715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39eb77e04653f1fe9557fb01ddbcf5aa051eb2f6c3c10529e6e8c1dda25085a7`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:18 GMT
ADD file:3b8e0dac20ca40faf2aaf084b69476a222952f177c0e6ec90804a10c91a51feb in / 
# Tue, 29 Mar 2022 00:40:19 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:59:34 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 11:59:35 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 11:59:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 11:59:37 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 11:59:38 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 12:00:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 12:00:38 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 12:00:39 GMT
USER user
# Tue, 29 Mar 2022 12:00:40 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4e7dd0becbc2dc968b69cba46c81a25fa500c88a644832ce17a5bb090925fa79`  
		Last Modified: Tue, 29 Mar 2022 00:41:37 GMT  
		Size: 2.7 MB (2720845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac63509931e219bc0df384426086bba93e5441adbe04844a6c56a7735dac3694`  
		Last Modified: Tue, 29 Mar 2022 12:01:26 GMT  
		Size: 9.5 MB (9536372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a61c76a95903e39d6d820ac1aa943f60dadb3928830a7cdca8225e25f8adef9`  
		Last Modified: Tue, 29 Mar 2022 12:01:24 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a666811bc4a9b90ef3fd8809c2eee8110d7113f8ec0ff856025534ae9399d8`  
		Last Modified: Tue, 29 Mar 2022 12:01:25 GMT  
		Size: 6.2 MB (6247254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; 386

```console
$ docker pull irssi@sha256:2bf221ef68d0a83a2116f20883a82c6ce6a7e0b4a5dfd71aa071b1db35aba964
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17703944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9afa5090692aa67a79e6c4008981e2926490e0d02199c568434f36da260714c`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:38:45 GMT
ADD file:f1abe5c2930209c2d735059c8e767e630c0818cc18a4fd10b0b90e6efbc675e2 in / 
# Tue, 29 Mar 2022 00:38:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 05:49:58 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 05:49:58 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 05:49:59 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 05:50:00 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 05:50:01 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 05:50:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 05:50:35 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 05:50:36 GMT
USER user
# Tue, 29 Mar 2022 05:50:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:dadad3128a09e6d507e89afe042cb1d48da14a72b28ca79dec7c6acf971bd9e6`  
		Last Modified: Tue, 29 Mar 2022 00:40:03 GMT  
		Size: 2.8 MB (2820388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101c682f90c53e18b63f7d30a8a7307eac0253f42c2fd84242c34fe251569421`  
		Last Modified: Tue, 29 Mar 2022 05:51:27 GMT  
		Size: 8.9 MB (8904321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:749bdf2ce2f439246606355222bf5bc711659dab2fa692f263642488f30cf45a`  
		Last Modified: Tue, 29 Mar 2022 05:51:26 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83177ea77693953b946bef5957dce55878d366d9332cb8cb61db7f190ce662f4`  
		Last Modified: Tue, 29 Mar 2022 05:51:27 GMT  
		Size: 6.0 MB (5977991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:977677327cf46ebee97c359921786db207de5c7cb4ab7d9b116d4c1d33ce4a80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18941144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:608f69d4d0976fd802228409ecdc55faff220c9aee1b43137f96bf8338f677f6`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:17:21 GMT
ADD file:0f301305d95e2e1e0580ec71f76edab57a1c18ed0adba5d09708b587ec19e622 in / 
# Tue, 29 Mar 2022 00:17:25 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:40:24 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 07:40:29 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 07:40:34 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 07:40:36 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 07:40:39 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 07:41:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 07:41:37 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 07:41:39 GMT
USER user
# Tue, 29 Mar 2022 07:41:41 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:77fcf2c0cc10658b5d6b4e43a75682b8bebbdc2e47895412dd1241c0422b8368`  
		Last Modified: Tue, 29 Mar 2022 00:18:56 GMT  
		Size: 2.8 MB (2814846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02339d74c6ee81495a0e118ded4e0419f26ccf80513936bca81454dcccb4a9ef`  
		Last Modified: Tue, 29 Mar 2022 07:42:43 GMT  
		Size: 9.6 MB (9632820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a2e134a3a26a9a610f884b36fc8c7c4515c3f8a6e496e0b30c88fe5bc2334d`  
		Last Modified: Tue, 29 Mar 2022 07:42:41 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b666408c25fa0d0d140d842ae855c147d353f9dfec2689327143be5d97c77a34`  
		Last Modified: Tue, 29 Mar 2022 07:42:42 GMT  
		Size: 6.5 MB (6492208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:a1996310e95fe58903b86881db102fc711c686616d690e464a1201242c01da6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18854963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bd0c6b0836f9d3340e3865bed234d2efe13b8dd8a243f3a3d4eb695106c636f`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:45 GMT
ADD file:08b65c73088f2cc387829e0ce9aa160db404a3e5fa0e4fda048cdbc02d8f64c2 in / 
# Tue, 29 Mar 2022 00:41:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 15:59:07 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 15:59:08 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 15:59:08 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 15:59:08 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 15:59:08 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 15:59:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 15:59:44 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 15:59:44 GMT
USER user
# Tue, 29 Mar 2022 15:59:44 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:89a2ea5c1a3e1d541ae66fbd95d215b39b560c537460c3fc76ad6826582893fe`  
		Last Modified: Tue, 29 Mar 2022 00:47:35 GMT  
		Size: 2.6 MB (2605074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1a5a4806a9221ab47409adcf5e27285f18845563e348e4bff66f36a4ec7727`  
		Last Modified: Tue, 29 Mar 2022 16:03:04 GMT  
		Size: 10.0 MB (9971979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ef67480f26d7536af4b650290ddd1955b0ef1afd6b33b3cdb1fcf4f4756f42`  
		Last Modified: Tue, 29 Mar 2022 16:03:04 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffa0c352647c43ea9c6e7c65920a410f592c9417d32b6fba1f0bad1646fc40e`  
		Last Modified: Tue, 29 Mar 2022 16:03:05 GMT  
		Size: 6.3 MB (6276640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2`

```console
$ docker pull irssi@sha256:480c39b4457078a69d69e8cc069a98f87278350e1f6ca14d4cbe79616f0e00b1
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

### `irssi:1.2` - linux; amd64

```console
$ docker pull irssi@sha256:898197fd559f9b169fa4d36cb9424351490be12245aa2e2c4e85838db057306d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50628334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a33ad04f436ec45a3cc476c2c220e7d42ce40687a2c41dc99cc020453041b3`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 16:39:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 16:39:05 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 16:39:06 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 16:39:06 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 16:39:06 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 16:39:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 16:39:57 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 16:39:57 GMT
USER user
# Tue, 29 Mar 2022 16:39:57 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd2cdd5c22666980d61bf83c478dfc880881556673a21e118f955376664ea2a`  
		Last Modified: Tue, 29 Mar 2022 16:41:14 GMT  
		Size: 17.0 MB (17038736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2861ba30751829fb2555bb33ca9170f484208f0049973581aa13988f65bcce`  
		Last Modified: Tue, 29 Mar 2022 16:41:10 GMT  
		Size: 4.2 KB (4209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bcc182247f746f92a6a75dee26bc22a8d50acc4c3286802af9e38fdd1c0b90`  
		Last Modified: Tue, 29 Mar 2022 16:41:12 GMT  
		Size: 6.4 MB (6433419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; arm variant v5

```console
$ docker pull irssi@sha256:ce001569547e34819fdf079112b88f49e44b499ed10726ae591cc6c5a0ea2bc9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46893537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f038e776a2c3d5a6f454656fe59c07165ac40653fc18ea19e3ce095e5a5056d`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:51:36 GMT
ADD file:7ac5498e2c44686d7eb272ef7645a0a64486cf942610f6754aa4a932f5b1a4be in / 
# Tue, 29 Mar 2022 00:51:37 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 08:47:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 08:47:02 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 08:47:04 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 08:47:04 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 08:47:05 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 08:48:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 08:48:51 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 08:48:52 GMT
USER user
# Tue, 29 Mar 2022 08:48:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8f10b1b67f0119a2dd5f838a3e98ab2c412e4b51fb1e4841e2b79fd4cae86105`  
		Last Modified: Tue, 29 Mar 2022 01:06:51 GMT  
		Size: 24.9 MB (24887495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb68688aa70be630bab2170a39e77d005f229ab6390b76e8d3b9a89acf825b8`  
		Last Modified: Tue, 29 Mar 2022 08:49:39 GMT  
		Size: 15.9 MB (15937355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f462c871b83b3653daf80a7cec6d9d06057396022a1e2b36a5764dcc29588a3`  
		Last Modified: Tue, 29 Mar 2022 08:49:28 GMT  
		Size: 4.2 KB (4199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae06e20e90eb68e6394cd65e5487477d7353a5816b39fa872fac1074888de42c`  
		Last Modified: Tue, 29 Mar 2022 08:49:31 GMT  
		Size: 6.1 MB (6064488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; arm variant v7

```console
$ docker pull irssi@sha256:3db3ddfc45fb2ccf78e4b7349fa0fd23aa6e59eaf69371032c89f4b995b2baf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44287695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8432232c7fa73842270a6402575d03dcd1af079cced86028166d84a2623f94cc`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 02:19:40 GMT
ADD file:8d54e000817531229c35a32eee074105c7b4d3c08b7ca56b1abdd80571687f28 in / 
# Tue, 29 Mar 2022 02:19:41 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:21:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:21:34 GMT
ENV HOME=/home/user
# Wed, 30 Mar 2022 02:21:36 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 30 Mar 2022 02:21:37 GMT
ENV LANG=C.UTF-8
# Wed, 30 Mar 2022 02:21:37 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 30 Mar 2022 02:23:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 30 Mar 2022 02:23:23 GMT
WORKDIR /home/user
# Wed, 30 Mar 2022 02:23:23 GMT
USER user
# Wed, 30 Mar 2022 02:23:24 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:d4bf0b27c669e589de33695047d638174fc2ca819a4366d5f80d1ad6b01c0c0e`  
		Last Modified: Tue, 29 Mar 2022 02:35:26 GMT  
		Size: 22.8 MB (22753045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac8262be381607606ea917e05e243851b4d99f2c3b81758f6312dfd87969356`  
		Last Modified: Wed, 30 Mar 2022 02:26:12 GMT  
		Size: 15.6 MB (15597948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62dbb031a500a927ff9934a53e57156d7a1faa17d61c5bd2e83339d685db97a8`  
		Last Modified: Wed, 30 Mar 2022 02:25:56 GMT  
		Size: 4.2 KB (4196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:489ce9745374ad929508ff3be1139e1d7e92b1035939d613574df8757f45f1ba`  
		Last Modified: Wed, 30 Mar 2022 02:26:00 GMT  
		Size: 5.9 MB (5932506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:8c11bc795decb16053eee4599521d727932b0b65a6043eb2d753763f6a0fcba8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48915028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:325958a38fb96c65a0cbe50172b3b831b9e521e2f46956e55bf1228253f6885e`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:42 GMT
ADD file:fdc8a5391a75cbf8c121f8f799ca08e94d2b3967b2546b36231c9297f7ce2151 in / 
# Tue, 29 Mar 2022 00:43:43 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 11:58:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 11:58:23 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 11:58:24 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 11:58:25 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 11:58:26 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 11:59:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 11:59:24 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 11:59:25 GMT
USER user
# Tue, 29 Mar 2022 11:59:26 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:5022906f515a0d4ec6bc1d0e5e7a01f47b1fbbb912e7e3f1ace27987169a9a21`  
		Last Modified: Tue, 29 Mar 2022 00:50:58 GMT  
		Size: 25.9 MB (25919777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99733c8db8c4371f3d274a989271d20844041e6ee266e8f74fa0a52e8e126277`  
		Last Modified: Tue, 29 Mar 2022 12:01:08 GMT  
		Size: 16.8 MB (16815150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b028d71796d54b96aa2ef9143f43950b86a4c6451c7da2b4836a693416e08660`  
		Last Modified: Tue, 29 Mar 2022 12:01:04 GMT  
		Size: 4.1 KB (4075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e78bd4b4962d8db2ae26337c77d821e36a0b186d875a7d5626aabe15e2be8e0`  
		Last Modified: Tue, 29 Mar 2022 12:01:05 GMT  
		Size: 6.2 MB (6176026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; 386

```console
$ docker pull irssi@sha256:406c82696ff47006adf53f11781be3f504cc4fe335a780106844f23f6a799af2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50264307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6ac23335fd4259a5aa45431e78631ccb7ba153d3b8b30da64cdff5bdafe99cb`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:42:26 GMT
ADD file:bcf3d504dc285de8b639c7f4017c41a4593a6c2aa6f046c9be79e587d05b5120 in / 
# Tue, 29 Mar 2022 00:42:27 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 05:48:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 05:48:43 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 05:48:44 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 05:48:45 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 05:48:46 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 05:49:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 05:49:35 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 05:49:36 GMT
USER user
# Tue, 29 Mar 2022 05:49:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:65b92490caa5e2c0588fab60d39315a2a8c09aa8ea0fe208d23f6984a47ecc03`  
		Last Modified: Tue, 29 Mar 2022 00:50:02 GMT  
		Size: 27.8 MB (27801252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65153b3620d7c8324690f0556ea546e098d1c5abea0de04cec331abe652fd6cc`  
		Last Modified: Tue, 29 Mar 2022 05:51:09 GMT  
		Size: 16.6 MB (16565592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f81e51b798316e6dddef7d44c46adbbfac04c8639c9c6d7fc569722558240ce`  
		Last Modified: Tue, 29 Mar 2022 05:51:05 GMT  
		Size: 4.1 KB (4052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb19cd58e039f1ea121d78c3603e8bcfac093136e3b920a3ab1df0bbf9ecd21d`  
		Last Modified: Tue, 29 Mar 2022 05:51:06 GMT  
		Size: 5.9 MB (5893411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; mips64le

```console
$ docker pull irssi@sha256:eed1cd2fe79ac4ab10dee6870ffa2be2cec900112d6a0a5d01b0474c5e8301f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47634326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b493b1d75e78f56f629ff77cc840485832b6f90136f061ceff8a2788aa90025`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 07:43:36 GMT
ADD file:7827dc4070f09537c063b825b0b7a5b076fac295f9afa415dee6c5346c38d46b in / 
# Tue, 29 Mar 2022 07:43:40 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 10:26:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 10:26:25 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 10:26:33 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 10:26:36 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 10:26:39 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 10:31:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 10:31:16 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 10:31:19 GMT
USER user
# Tue, 29 Mar 2022 10:31:23 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4a3e27ca4ec7041c36d0e9cbc672ce565851ce1a0cc90120d7a923a938fb3c18`  
		Last Modified: Tue, 29 Mar 2022 07:54:19 GMT  
		Size: 25.8 MB (25818066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2023bef9f22712b6457705ea84614163a3d0a854f38d7f2f13f388c262fd8d68`  
		Last Modified: Tue, 29 Mar 2022 10:31:51 GMT  
		Size: 15.7 MB (15731870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783dfb57d1278d639db4a6acd55eea930b6387da357be8c4e1ef6af2c734ff13`  
		Last Modified: Tue, 29 Mar 2022 10:31:37 GMT  
		Size: 4.1 KB (4069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e297148bdf9b4491afc8d6b2898998918425c1e35865b360d93b281abe77ce`  
		Last Modified: Tue, 29 Mar 2022 10:31:40 GMT  
		Size: 6.1 MB (6080321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; ppc64le

```console
$ docker pull irssi@sha256:a460c3520546307e352a19d055007a7fcba927f322c545e3e7296c1bfdf74592
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54787995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f694d959fe967b7564e8a7cdaf212e3d814c5d6b79c1d3696f77b35c476d8ea`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:59 GMT
ADD file:7271d778d432a07f57fedf8d50d83699ef545acc9db9346f6fe75b0054af4cd1 in / 
# Tue, 29 Mar 2022 00:23:00 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 07:34:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 07:35:01 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 07:35:09 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 07:35:12 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 07:35:15 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 07:39:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 07:39:58 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 07:39:59 GMT
USER user
# Tue, 29 Mar 2022 07:40:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:7db831386ce67ac1cf2b4f1513fe3746c9ea2b8d4c82efca75be638eaf533614`  
		Last Modified: Tue, 29 Mar 2022 00:34:41 GMT  
		Size: 30.6 MB (30560163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6f0e2fb83c5287040e529ec1e0cc34c5383697a80a278632cddf17a110ab26`  
		Last Modified: Tue, 29 Mar 2022 07:42:17 GMT  
		Size: 17.4 MB (17440827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9798211288cab71997a2ba40949386224112d0754a517ece37e3cfc68ccc5ad0`  
		Last Modified: Tue, 29 Mar 2022 07:42:12 GMT  
		Size: 4.2 KB (4216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dadee1dc4117b4a1068f72e957d68471ff9f516c4db70a938e36a427e6f45b7`  
		Last Modified: Tue, 29 Mar 2022 07:42:14 GMT  
		Size: 6.8 MB (6782789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; s390x

```console
$ docker pull irssi@sha256:8aa6207ef3bc8833bb6a35d3870a604c6e90fc607bf1bbebab6688fb11f2d4ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49068950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9b140f48665cda5494c089acdb6eae60f96d15c3fb4dd0ba4b19d99953db655`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:52:27 GMT
ADD file:dbf01085079906b34f3ec9db0b9ce31aa1466b935a47e8e30772a5488f76fec0 in / 
# Tue, 29 Mar 2022 00:52:29 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 15:57:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 15:57:55 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 15:57:56 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 15:57:56 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 15:57:56 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 15:58:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 15:58:46 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 15:58:46 GMT
USER user
# Tue, 29 Mar 2022 15:58:46 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:66ccc81b275f683f44a0f40ddce6992117eefe92dca84fadf6d2e51c22d11a64`  
		Last Modified: Tue, 29 Mar 2022 01:10:22 GMT  
		Size: 25.8 MB (25765916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f745ab618468906119bb54aef0c97df6677ebed5694c4d839b8103c60531d8`  
		Last Modified: Tue, 29 Mar 2022 16:00:54 GMT  
		Size: 16.9 MB (16914174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e65abef5df82c79a408eb80534564b0361dc35744b6aa982b493c4f0e59e55d4`  
		Last Modified: Tue, 29 Mar 2022 16:00:54 GMT  
		Size: 4.2 KB (4216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a6b20318811928ca8b7d3a3a3229cab3b5ac4bd24212ec30916433aef99d73`  
		Last Modified: Tue, 29 Mar 2022 16:00:54 GMT  
		Size: 6.4 MB (6384644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2-alpine`

```console
$ docker pull irssi@sha256:fc0f0ae29aedc3e3dfee43d698d4de461180f8959428023f3a5bd95b61433f18
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

### `irssi:1.2-alpine` - linux; amd64

```console
$ docker pull irssi@sha256:d7bbd05aae77230148f9a3af4a07717c5626cdb254caa1dc239bfc8866124f3e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18648371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b63678d9d2827a5a4d447b135a05921b9b618d639a9641f3970ce71fbad41c58`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:46 GMT
ADD file:a2ef39a587aac85256b55bee81f17d73aaa7154b2a32a31527c7803fb889f2e7 in / 
# Tue, 29 Mar 2022 00:19:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 16:40:04 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 16:40:04 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 16:40:05 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 16:40:05 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 16:40:05 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 16:40:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 16:40:49 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 16:40:49 GMT
USER user
# Tue, 29 Mar 2022 16:40:49 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b9c05db88786fd3c89b78787631257301391f898c03ba50553b556630046a741`  
		Last Modified: Tue, 29 Mar 2022 00:20:43 GMT  
		Size: 2.8 MB (2819223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c516145633461419b5a658706a7453eb731aaf449afd25b5996b275b8692bb0e`  
		Last Modified: Tue, 29 Mar 2022 16:41:30 GMT  
		Size: 9.5 MB (9540598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d5246be564bab1c71a70cfe50bdab883825a0ec36ed4a79b2c6730ee23849f`  
		Last Modified: Tue, 29 Mar 2022 16:41:28 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0543c4eb94b3e7485a55ed115e70d48d246fc300c3430bf71f774b156b56f7`  
		Last Modified: Tue, 29 Mar 2022 16:41:29 GMT  
		Size: 6.3 MB (6287279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:8f4fc787e0e6164fcc251c034c9fbff27d3a81fdda0c2a82c859312e16aa677a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17385391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:facc4fa1f84eebf576961df4f191b9e7763fd7f790ee44517915d56ab994e139`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:56 GMT
ADD file:23d913551f75313e359a4e93592ea0a9655e1a7c2bec5fddd210717d70c3114b in / 
# Tue, 29 Mar 2022 00:49:57 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 14:24:05 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 14:24:06 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 14:24:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 14:24:08 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 14:24:08 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 14:25:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 14:25:17 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 14:25:18 GMT
USER user
# Tue, 29 Mar 2022 14:25:18 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:eba0847afba90891ea7dae672f5dadfa405a822df0bc9c00b9e3328fd5fd889c`  
		Last Modified: Tue, 29 Mar 2022 00:51:57 GMT  
		Size: 2.6 MB (2625139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475d9671ce28a72461f25c4368162f9eac018ffced5ee61d17852dac61f60923`  
		Last Modified: Tue, 29 Mar 2022 14:25:59 GMT  
		Size: 8.8 MB (8771957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223ba1931ceb81e998f74a59ac08d88367fa3be50d7864242a41937e0a744bb8`  
		Last Modified: Tue, 29 Mar 2022 14:25:51 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9769077f19f3aaf8bd8f635611ddc58ab0133ca7a4207c1e68a6b84b68056afa`  
		Last Modified: Tue, 29 Mar 2022 14:25:55 GMT  
		Size: 6.0 MB (5987025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:645f3bdeef2e0deedf6315612f78330153c94d47580d86102653f44c653cbcfb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16839519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c53528eb26529ee3c99677c1271b1f6fe9b45db594e0a4d5f16d5bb51dd858cf`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 02:13:57 GMT
ADD file:9995ada53dfe4b82c6c01a9143cdcf8aa3aabac359fa023f5fa4da85e7a88704 in / 
# Tue, 29 Mar 2022 02:13:58 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 02:23:53 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 30 Mar 2022 02:23:53 GMT
ENV HOME=/home/user
# Wed, 30 Mar 2022 02:23:55 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 30 Mar 2022 02:23:55 GMT
ENV LANG=C.UTF-8
# Wed, 30 Mar 2022 02:23:56 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 30 Mar 2022 02:25:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 30 Mar 2022 02:25:01 GMT
WORKDIR /home/user
# Wed, 30 Mar 2022 02:25:01 GMT
USER user
# Wed, 30 Mar 2022 02:25:02 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:9e629c3986cd97398b7f233a377ad62b7d37cbccbcba0bbae7c5bc600ea73620`  
		Last Modified: Tue, 29 Mar 2022 02:15:59 GMT  
		Size: 2.4 MB (2427878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef6405d47acdbe9f502c4db8aa5db79963974eb33c7c7db6367815d922d0d34`  
		Last Modified: Wed, 30 Mar 2022 02:26:38 GMT  
		Size: 8.6 MB (8626355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360bcdf4cc43bbde189db2de03107a0ef571fdf754c37919f41990fba758ab25`  
		Last Modified: Wed, 30 Mar 2022 02:26:31 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3419b023d43ddc842375a10a3b44776c2694b31cdb493104714b3331e346e099`  
		Last Modified: Wed, 30 Mar 2022 02:26:34 GMT  
		Size: 5.8 MB (5784017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:dfc50492eaf70eaec1101ec66e1039ff67a7db7dd5800d74dc45a4a739e02c20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18505715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39eb77e04653f1fe9557fb01ddbcf5aa051eb2f6c3c10529e6e8c1dda25085a7`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:18 GMT
ADD file:3b8e0dac20ca40faf2aaf084b69476a222952f177c0e6ec90804a10c91a51feb in / 
# Tue, 29 Mar 2022 00:40:19 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:59:34 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 11:59:35 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 11:59:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 11:59:37 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 11:59:38 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 12:00:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 12:00:38 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 12:00:39 GMT
USER user
# Tue, 29 Mar 2022 12:00:40 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4e7dd0becbc2dc968b69cba46c81a25fa500c88a644832ce17a5bb090925fa79`  
		Last Modified: Tue, 29 Mar 2022 00:41:37 GMT  
		Size: 2.7 MB (2720845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac63509931e219bc0df384426086bba93e5441adbe04844a6c56a7735dac3694`  
		Last Modified: Tue, 29 Mar 2022 12:01:26 GMT  
		Size: 9.5 MB (9536372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a61c76a95903e39d6d820ac1aa943f60dadb3928830a7cdca8225e25f8adef9`  
		Last Modified: Tue, 29 Mar 2022 12:01:24 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a666811bc4a9b90ef3fd8809c2eee8110d7113f8ec0ff856025534ae9399d8`  
		Last Modified: Tue, 29 Mar 2022 12:01:25 GMT  
		Size: 6.2 MB (6247254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; 386

```console
$ docker pull irssi@sha256:2bf221ef68d0a83a2116f20883a82c6ce6a7e0b4a5dfd71aa071b1db35aba964
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17703944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9afa5090692aa67a79e6c4008981e2926490e0d02199c568434f36da260714c`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:38:45 GMT
ADD file:f1abe5c2930209c2d735059c8e767e630c0818cc18a4fd10b0b90e6efbc675e2 in / 
# Tue, 29 Mar 2022 00:38:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 05:49:58 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 05:49:58 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 05:49:59 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 05:50:00 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 05:50:01 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 05:50:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 05:50:35 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 05:50:36 GMT
USER user
# Tue, 29 Mar 2022 05:50:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:dadad3128a09e6d507e89afe042cb1d48da14a72b28ca79dec7c6acf971bd9e6`  
		Last Modified: Tue, 29 Mar 2022 00:40:03 GMT  
		Size: 2.8 MB (2820388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101c682f90c53e18b63f7d30a8a7307eac0253f42c2fd84242c34fe251569421`  
		Last Modified: Tue, 29 Mar 2022 05:51:27 GMT  
		Size: 8.9 MB (8904321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:749bdf2ce2f439246606355222bf5bc711659dab2fa692f263642488f30cf45a`  
		Last Modified: Tue, 29 Mar 2022 05:51:26 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83177ea77693953b946bef5957dce55878d366d9332cb8cb61db7f190ce662f4`  
		Last Modified: Tue, 29 Mar 2022 05:51:27 GMT  
		Size: 6.0 MB (5977991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:977677327cf46ebee97c359921786db207de5c7cb4ab7d9b116d4c1d33ce4a80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18941144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:608f69d4d0976fd802228409ecdc55faff220c9aee1b43137f96bf8338f677f6`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:17:21 GMT
ADD file:0f301305d95e2e1e0580ec71f76edab57a1c18ed0adba5d09708b587ec19e622 in / 
# Tue, 29 Mar 2022 00:17:25 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:40:24 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 07:40:29 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 07:40:34 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 07:40:36 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 07:40:39 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 07:41:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 07:41:37 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 07:41:39 GMT
USER user
# Tue, 29 Mar 2022 07:41:41 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:77fcf2c0cc10658b5d6b4e43a75682b8bebbdc2e47895412dd1241c0422b8368`  
		Last Modified: Tue, 29 Mar 2022 00:18:56 GMT  
		Size: 2.8 MB (2814846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02339d74c6ee81495a0e118ded4e0419f26ccf80513936bca81454dcccb4a9ef`  
		Last Modified: Tue, 29 Mar 2022 07:42:43 GMT  
		Size: 9.6 MB (9632820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a2e134a3a26a9a610f884b36fc8c7c4515c3f8a6e496e0b30c88fe5bc2334d`  
		Last Modified: Tue, 29 Mar 2022 07:42:41 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b666408c25fa0d0d140d842ae855c147d353f9dfec2689327143be5d97c77a34`  
		Last Modified: Tue, 29 Mar 2022 07:42:42 GMT  
		Size: 6.5 MB (6492208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:a1996310e95fe58903b86881db102fc711c686616d690e464a1201242c01da6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18854963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bd0c6b0836f9d3340e3865bed234d2efe13b8dd8a243f3a3d4eb695106c636f`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:45 GMT
ADD file:08b65c73088f2cc387829e0ce9aa160db404a3e5fa0e4fda048cdbc02d8f64c2 in / 
# Tue, 29 Mar 2022 00:41:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 15:59:07 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 15:59:08 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 15:59:08 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 15:59:08 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 15:59:08 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 15:59:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 15:59:44 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 15:59:44 GMT
USER user
# Tue, 29 Mar 2022 15:59:44 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:89a2ea5c1a3e1d541ae66fbd95d215b39b560c537460c3fc76ad6826582893fe`  
		Last Modified: Tue, 29 Mar 2022 00:47:35 GMT  
		Size: 2.6 MB (2605074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1a5a4806a9221ab47409adcf5e27285f18845563e348e4bff66f36a4ec7727`  
		Last Modified: Tue, 29 Mar 2022 16:03:04 GMT  
		Size: 10.0 MB (9971979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ef67480f26d7536af4b650290ddd1955b0ef1afd6b33b3cdb1fcf4f4756f42`  
		Last Modified: Tue, 29 Mar 2022 16:03:04 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffa0c352647c43ea9c6e7c65920a410f592c9417d32b6fba1f0bad1646fc40e`  
		Last Modified: Tue, 29 Mar 2022 16:03:05 GMT  
		Size: 6.3 MB (6276640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2.3`

```console
$ docker pull irssi@sha256:480c39b4457078a69d69e8cc069a98f87278350e1f6ca14d4cbe79616f0e00b1
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

### `irssi:1.2.3` - linux; amd64

```console
$ docker pull irssi@sha256:898197fd559f9b169fa4d36cb9424351490be12245aa2e2c4e85838db057306d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50628334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a33ad04f436ec45a3cc476c2c220e7d42ce40687a2c41dc99cc020453041b3`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 16:39:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 16:39:05 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 16:39:06 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 16:39:06 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 16:39:06 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 16:39:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 16:39:57 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 16:39:57 GMT
USER user
# Tue, 29 Mar 2022 16:39:57 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd2cdd5c22666980d61bf83c478dfc880881556673a21e118f955376664ea2a`  
		Last Modified: Tue, 29 Mar 2022 16:41:14 GMT  
		Size: 17.0 MB (17038736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2861ba30751829fb2555bb33ca9170f484208f0049973581aa13988f65bcce`  
		Last Modified: Tue, 29 Mar 2022 16:41:10 GMT  
		Size: 4.2 KB (4209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bcc182247f746f92a6a75dee26bc22a8d50acc4c3286802af9e38fdd1c0b90`  
		Last Modified: Tue, 29 Mar 2022 16:41:12 GMT  
		Size: 6.4 MB (6433419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; arm variant v5

```console
$ docker pull irssi@sha256:ce001569547e34819fdf079112b88f49e44b499ed10726ae591cc6c5a0ea2bc9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46893537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f038e776a2c3d5a6f454656fe59c07165ac40653fc18ea19e3ce095e5a5056d`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:51:36 GMT
ADD file:7ac5498e2c44686d7eb272ef7645a0a64486cf942610f6754aa4a932f5b1a4be in / 
# Tue, 29 Mar 2022 00:51:37 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 08:47:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 08:47:02 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 08:47:04 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 08:47:04 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 08:47:05 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 08:48:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 08:48:51 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 08:48:52 GMT
USER user
# Tue, 29 Mar 2022 08:48:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8f10b1b67f0119a2dd5f838a3e98ab2c412e4b51fb1e4841e2b79fd4cae86105`  
		Last Modified: Tue, 29 Mar 2022 01:06:51 GMT  
		Size: 24.9 MB (24887495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb68688aa70be630bab2170a39e77d005f229ab6390b76e8d3b9a89acf825b8`  
		Last Modified: Tue, 29 Mar 2022 08:49:39 GMT  
		Size: 15.9 MB (15937355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f462c871b83b3653daf80a7cec6d9d06057396022a1e2b36a5764dcc29588a3`  
		Last Modified: Tue, 29 Mar 2022 08:49:28 GMT  
		Size: 4.2 KB (4199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae06e20e90eb68e6394cd65e5487477d7353a5816b39fa872fac1074888de42c`  
		Last Modified: Tue, 29 Mar 2022 08:49:31 GMT  
		Size: 6.1 MB (6064488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; arm variant v7

```console
$ docker pull irssi@sha256:3db3ddfc45fb2ccf78e4b7349fa0fd23aa6e59eaf69371032c89f4b995b2baf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44287695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8432232c7fa73842270a6402575d03dcd1af079cced86028166d84a2623f94cc`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 02:19:40 GMT
ADD file:8d54e000817531229c35a32eee074105c7b4d3c08b7ca56b1abdd80571687f28 in / 
# Tue, 29 Mar 2022 02:19:41 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:21:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:21:34 GMT
ENV HOME=/home/user
# Wed, 30 Mar 2022 02:21:36 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 30 Mar 2022 02:21:37 GMT
ENV LANG=C.UTF-8
# Wed, 30 Mar 2022 02:21:37 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 30 Mar 2022 02:23:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 30 Mar 2022 02:23:23 GMT
WORKDIR /home/user
# Wed, 30 Mar 2022 02:23:23 GMT
USER user
# Wed, 30 Mar 2022 02:23:24 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:d4bf0b27c669e589de33695047d638174fc2ca819a4366d5f80d1ad6b01c0c0e`  
		Last Modified: Tue, 29 Mar 2022 02:35:26 GMT  
		Size: 22.8 MB (22753045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac8262be381607606ea917e05e243851b4d99f2c3b81758f6312dfd87969356`  
		Last Modified: Wed, 30 Mar 2022 02:26:12 GMT  
		Size: 15.6 MB (15597948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62dbb031a500a927ff9934a53e57156d7a1faa17d61c5bd2e83339d685db97a8`  
		Last Modified: Wed, 30 Mar 2022 02:25:56 GMT  
		Size: 4.2 KB (4196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:489ce9745374ad929508ff3be1139e1d7e92b1035939d613574df8757f45f1ba`  
		Last Modified: Wed, 30 Mar 2022 02:26:00 GMT  
		Size: 5.9 MB (5932506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:8c11bc795decb16053eee4599521d727932b0b65a6043eb2d753763f6a0fcba8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48915028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:325958a38fb96c65a0cbe50172b3b831b9e521e2f46956e55bf1228253f6885e`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:42 GMT
ADD file:fdc8a5391a75cbf8c121f8f799ca08e94d2b3967b2546b36231c9297f7ce2151 in / 
# Tue, 29 Mar 2022 00:43:43 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 11:58:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 11:58:23 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 11:58:24 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 11:58:25 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 11:58:26 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 11:59:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 11:59:24 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 11:59:25 GMT
USER user
# Tue, 29 Mar 2022 11:59:26 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:5022906f515a0d4ec6bc1d0e5e7a01f47b1fbbb912e7e3f1ace27987169a9a21`  
		Last Modified: Tue, 29 Mar 2022 00:50:58 GMT  
		Size: 25.9 MB (25919777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99733c8db8c4371f3d274a989271d20844041e6ee266e8f74fa0a52e8e126277`  
		Last Modified: Tue, 29 Mar 2022 12:01:08 GMT  
		Size: 16.8 MB (16815150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b028d71796d54b96aa2ef9143f43950b86a4c6451c7da2b4836a693416e08660`  
		Last Modified: Tue, 29 Mar 2022 12:01:04 GMT  
		Size: 4.1 KB (4075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e78bd4b4962d8db2ae26337c77d821e36a0b186d875a7d5626aabe15e2be8e0`  
		Last Modified: Tue, 29 Mar 2022 12:01:05 GMT  
		Size: 6.2 MB (6176026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; 386

```console
$ docker pull irssi@sha256:406c82696ff47006adf53f11781be3f504cc4fe335a780106844f23f6a799af2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50264307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6ac23335fd4259a5aa45431e78631ccb7ba153d3b8b30da64cdff5bdafe99cb`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:42:26 GMT
ADD file:bcf3d504dc285de8b639c7f4017c41a4593a6c2aa6f046c9be79e587d05b5120 in / 
# Tue, 29 Mar 2022 00:42:27 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 05:48:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 05:48:43 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 05:48:44 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 05:48:45 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 05:48:46 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 05:49:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 05:49:35 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 05:49:36 GMT
USER user
# Tue, 29 Mar 2022 05:49:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:65b92490caa5e2c0588fab60d39315a2a8c09aa8ea0fe208d23f6984a47ecc03`  
		Last Modified: Tue, 29 Mar 2022 00:50:02 GMT  
		Size: 27.8 MB (27801252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65153b3620d7c8324690f0556ea546e098d1c5abea0de04cec331abe652fd6cc`  
		Last Modified: Tue, 29 Mar 2022 05:51:09 GMT  
		Size: 16.6 MB (16565592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f81e51b798316e6dddef7d44c46adbbfac04c8639c9c6d7fc569722558240ce`  
		Last Modified: Tue, 29 Mar 2022 05:51:05 GMT  
		Size: 4.1 KB (4052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb19cd58e039f1ea121d78c3603e8bcfac093136e3b920a3ab1df0bbf9ecd21d`  
		Last Modified: Tue, 29 Mar 2022 05:51:06 GMT  
		Size: 5.9 MB (5893411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; mips64le

```console
$ docker pull irssi@sha256:eed1cd2fe79ac4ab10dee6870ffa2be2cec900112d6a0a5d01b0474c5e8301f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47634326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b493b1d75e78f56f629ff77cc840485832b6f90136f061ceff8a2788aa90025`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 07:43:36 GMT
ADD file:7827dc4070f09537c063b825b0b7a5b076fac295f9afa415dee6c5346c38d46b in / 
# Tue, 29 Mar 2022 07:43:40 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 10:26:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 10:26:25 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 10:26:33 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 10:26:36 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 10:26:39 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 10:31:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 10:31:16 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 10:31:19 GMT
USER user
# Tue, 29 Mar 2022 10:31:23 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4a3e27ca4ec7041c36d0e9cbc672ce565851ce1a0cc90120d7a923a938fb3c18`  
		Last Modified: Tue, 29 Mar 2022 07:54:19 GMT  
		Size: 25.8 MB (25818066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2023bef9f22712b6457705ea84614163a3d0a854f38d7f2f13f388c262fd8d68`  
		Last Modified: Tue, 29 Mar 2022 10:31:51 GMT  
		Size: 15.7 MB (15731870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783dfb57d1278d639db4a6acd55eea930b6387da357be8c4e1ef6af2c734ff13`  
		Last Modified: Tue, 29 Mar 2022 10:31:37 GMT  
		Size: 4.1 KB (4069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e297148bdf9b4491afc8d6b2898998918425c1e35865b360d93b281abe77ce`  
		Last Modified: Tue, 29 Mar 2022 10:31:40 GMT  
		Size: 6.1 MB (6080321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; ppc64le

```console
$ docker pull irssi@sha256:a460c3520546307e352a19d055007a7fcba927f322c545e3e7296c1bfdf74592
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54787995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f694d959fe967b7564e8a7cdaf212e3d814c5d6b79c1d3696f77b35c476d8ea`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:59 GMT
ADD file:7271d778d432a07f57fedf8d50d83699ef545acc9db9346f6fe75b0054af4cd1 in / 
# Tue, 29 Mar 2022 00:23:00 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 07:34:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 07:35:01 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 07:35:09 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 07:35:12 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 07:35:15 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 07:39:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 07:39:58 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 07:39:59 GMT
USER user
# Tue, 29 Mar 2022 07:40:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:7db831386ce67ac1cf2b4f1513fe3746c9ea2b8d4c82efca75be638eaf533614`  
		Last Modified: Tue, 29 Mar 2022 00:34:41 GMT  
		Size: 30.6 MB (30560163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6f0e2fb83c5287040e529ec1e0cc34c5383697a80a278632cddf17a110ab26`  
		Last Modified: Tue, 29 Mar 2022 07:42:17 GMT  
		Size: 17.4 MB (17440827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9798211288cab71997a2ba40949386224112d0754a517ece37e3cfc68ccc5ad0`  
		Last Modified: Tue, 29 Mar 2022 07:42:12 GMT  
		Size: 4.2 KB (4216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dadee1dc4117b4a1068f72e957d68471ff9f516c4db70a938e36a427e6f45b7`  
		Last Modified: Tue, 29 Mar 2022 07:42:14 GMT  
		Size: 6.8 MB (6782789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; s390x

```console
$ docker pull irssi@sha256:8aa6207ef3bc8833bb6a35d3870a604c6e90fc607bf1bbebab6688fb11f2d4ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49068950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9b140f48665cda5494c089acdb6eae60f96d15c3fb4dd0ba4b19d99953db655`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:52:27 GMT
ADD file:dbf01085079906b34f3ec9db0b9ce31aa1466b935a47e8e30772a5488f76fec0 in / 
# Tue, 29 Mar 2022 00:52:29 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 15:57:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 15:57:55 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 15:57:56 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 15:57:56 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 15:57:56 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 15:58:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 15:58:46 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 15:58:46 GMT
USER user
# Tue, 29 Mar 2022 15:58:46 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:66ccc81b275f683f44a0f40ddce6992117eefe92dca84fadf6d2e51c22d11a64`  
		Last Modified: Tue, 29 Mar 2022 01:10:22 GMT  
		Size: 25.8 MB (25765916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f745ab618468906119bb54aef0c97df6677ebed5694c4d839b8103c60531d8`  
		Last Modified: Tue, 29 Mar 2022 16:00:54 GMT  
		Size: 16.9 MB (16914174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e65abef5df82c79a408eb80534564b0361dc35744b6aa982b493c4f0e59e55d4`  
		Last Modified: Tue, 29 Mar 2022 16:00:54 GMT  
		Size: 4.2 KB (4216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a6b20318811928ca8b7d3a3a3229cab3b5ac4bd24212ec30916433aef99d73`  
		Last Modified: Tue, 29 Mar 2022 16:00:54 GMT  
		Size: 6.4 MB (6384644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2.3-alpine`

```console
$ docker pull irssi@sha256:fc0f0ae29aedc3e3dfee43d698d4de461180f8959428023f3a5bd95b61433f18
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

### `irssi:1.2.3-alpine` - linux; amd64

```console
$ docker pull irssi@sha256:d7bbd05aae77230148f9a3af4a07717c5626cdb254caa1dc239bfc8866124f3e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18648371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b63678d9d2827a5a4d447b135a05921b9b618d639a9641f3970ce71fbad41c58`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:46 GMT
ADD file:a2ef39a587aac85256b55bee81f17d73aaa7154b2a32a31527c7803fb889f2e7 in / 
# Tue, 29 Mar 2022 00:19:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 16:40:04 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 16:40:04 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 16:40:05 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 16:40:05 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 16:40:05 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 16:40:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 16:40:49 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 16:40:49 GMT
USER user
# Tue, 29 Mar 2022 16:40:49 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b9c05db88786fd3c89b78787631257301391f898c03ba50553b556630046a741`  
		Last Modified: Tue, 29 Mar 2022 00:20:43 GMT  
		Size: 2.8 MB (2819223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c516145633461419b5a658706a7453eb731aaf449afd25b5996b275b8692bb0e`  
		Last Modified: Tue, 29 Mar 2022 16:41:30 GMT  
		Size: 9.5 MB (9540598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d5246be564bab1c71a70cfe50bdab883825a0ec36ed4a79b2c6730ee23849f`  
		Last Modified: Tue, 29 Mar 2022 16:41:28 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0543c4eb94b3e7485a55ed115e70d48d246fc300c3430bf71f774b156b56f7`  
		Last Modified: Tue, 29 Mar 2022 16:41:29 GMT  
		Size: 6.3 MB (6287279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:8f4fc787e0e6164fcc251c034c9fbff27d3a81fdda0c2a82c859312e16aa677a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17385391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:facc4fa1f84eebf576961df4f191b9e7763fd7f790ee44517915d56ab994e139`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:56 GMT
ADD file:23d913551f75313e359a4e93592ea0a9655e1a7c2bec5fddd210717d70c3114b in / 
# Tue, 29 Mar 2022 00:49:57 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 14:24:05 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 14:24:06 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 14:24:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 14:24:08 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 14:24:08 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 14:25:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 14:25:17 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 14:25:18 GMT
USER user
# Tue, 29 Mar 2022 14:25:18 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:eba0847afba90891ea7dae672f5dadfa405a822df0bc9c00b9e3328fd5fd889c`  
		Last Modified: Tue, 29 Mar 2022 00:51:57 GMT  
		Size: 2.6 MB (2625139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475d9671ce28a72461f25c4368162f9eac018ffced5ee61d17852dac61f60923`  
		Last Modified: Tue, 29 Mar 2022 14:25:59 GMT  
		Size: 8.8 MB (8771957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223ba1931ceb81e998f74a59ac08d88367fa3be50d7864242a41937e0a744bb8`  
		Last Modified: Tue, 29 Mar 2022 14:25:51 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9769077f19f3aaf8bd8f635611ddc58ab0133ca7a4207c1e68a6b84b68056afa`  
		Last Modified: Tue, 29 Mar 2022 14:25:55 GMT  
		Size: 6.0 MB (5987025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:645f3bdeef2e0deedf6315612f78330153c94d47580d86102653f44c653cbcfb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16839519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c53528eb26529ee3c99677c1271b1f6fe9b45db594e0a4d5f16d5bb51dd858cf`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 02:13:57 GMT
ADD file:9995ada53dfe4b82c6c01a9143cdcf8aa3aabac359fa023f5fa4da85e7a88704 in / 
# Tue, 29 Mar 2022 02:13:58 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 02:23:53 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 30 Mar 2022 02:23:53 GMT
ENV HOME=/home/user
# Wed, 30 Mar 2022 02:23:55 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 30 Mar 2022 02:23:55 GMT
ENV LANG=C.UTF-8
# Wed, 30 Mar 2022 02:23:56 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 30 Mar 2022 02:25:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 30 Mar 2022 02:25:01 GMT
WORKDIR /home/user
# Wed, 30 Mar 2022 02:25:01 GMT
USER user
# Wed, 30 Mar 2022 02:25:02 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:9e629c3986cd97398b7f233a377ad62b7d37cbccbcba0bbae7c5bc600ea73620`  
		Last Modified: Tue, 29 Mar 2022 02:15:59 GMT  
		Size: 2.4 MB (2427878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef6405d47acdbe9f502c4db8aa5db79963974eb33c7c7db6367815d922d0d34`  
		Last Modified: Wed, 30 Mar 2022 02:26:38 GMT  
		Size: 8.6 MB (8626355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360bcdf4cc43bbde189db2de03107a0ef571fdf754c37919f41990fba758ab25`  
		Last Modified: Wed, 30 Mar 2022 02:26:31 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3419b023d43ddc842375a10a3b44776c2694b31cdb493104714b3331e346e099`  
		Last Modified: Wed, 30 Mar 2022 02:26:34 GMT  
		Size: 5.8 MB (5784017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:dfc50492eaf70eaec1101ec66e1039ff67a7db7dd5800d74dc45a4a739e02c20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18505715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39eb77e04653f1fe9557fb01ddbcf5aa051eb2f6c3c10529e6e8c1dda25085a7`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:18 GMT
ADD file:3b8e0dac20ca40faf2aaf084b69476a222952f177c0e6ec90804a10c91a51feb in / 
# Tue, 29 Mar 2022 00:40:19 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:59:34 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 11:59:35 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 11:59:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 11:59:37 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 11:59:38 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 12:00:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 12:00:38 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 12:00:39 GMT
USER user
# Tue, 29 Mar 2022 12:00:40 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4e7dd0becbc2dc968b69cba46c81a25fa500c88a644832ce17a5bb090925fa79`  
		Last Modified: Tue, 29 Mar 2022 00:41:37 GMT  
		Size: 2.7 MB (2720845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac63509931e219bc0df384426086bba93e5441adbe04844a6c56a7735dac3694`  
		Last Modified: Tue, 29 Mar 2022 12:01:26 GMT  
		Size: 9.5 MB (9536372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a61c76a95903e39d6d820ac1aa943f60dadb3928830a7cdca8225e25f8adef9`  
		Last Modified: Tue, 29 Mar 2022 12:01:24 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a666811bc4a9b90ef3fd8809c2eee8110d7113f8ec0ff856025534ae9399d8`  
		Last Modified: Tue, 29 Mar 2022 12:01:25 GMT  
		Size: 6.2 MB (6247254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; 386

```console
$ docker pull irssi@sha256:2bf221ef68d0a83a2116f20883a82c6ce6a7e0b4a5dfd71aa071b1db35aba964
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17703944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9afa5090692aa67a79e6c4008981e2926490e0d02199c568434f36da260714c`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:38:45 GMT
ADD file:f1abe5c2930209c2d735059c8e767e630c0818cc18a4fd10b0b90e6efbc675e2 in / 
# Tue, 29 Mar 2022 00:38:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 05:49:58 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 05:49:58 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 05:49:59 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 05:50:00 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 05:50:01 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 05:50:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 05:50:35 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 05:50:36 GMT
USER user
# Tue, 29 Mar 2022 05:50:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:dadad3128a09e6d507e89afe042cb1d48da14a72b28ca79dec7c6acf971bd9e6`  
		Last Modified: Tue, 29 Mar 2022 00:40:03 GMT  
		Size: 2.8 MB (2820388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101c682f90c53e18b63f7d30a8a7307eac0253f42c2fd84242c34fe251569421`  
		Last Modified: Tue, 29 Mar 2022 05:51:27 GMT  
		Size: 8.9 MB (8904321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:749bdf2ce2f439246606355222bf5bc711659dab2fa692f263642488f30cf45a`  
		Last Modified: Tue, 29 Mar 2022 05:51:26 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83177ea77693953b946bef5957dce55878d366d9332cb8cb61db7f190ce662f4`  
		Last Modified: Tue, 29 Mar 2022 05:51:27 GMT  
		Size: 6.0 MB (5977991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:977677327cf46ebee97c359921786db207de5c7cb4ab7d9b116d4c1d33ce4a80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18941144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:608f69d4d0976fd802228409ecdc55faff220c9aee1b43137f96bf8338f677f6`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:17:21 GMT
ADD file:0f301305d95e2e1e0580ec71f76edab57a1c18ed0adba5d09708b587ec19e622 in / 
# Tue, 29 Mar 2022 00:17:25 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:40:24 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 07:40:29 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 07:40:34 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 07:40:36 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 07:40:39 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 07:41:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 07:41:37 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 07:41:39 GMT
USER user
# Tue, 29 Mar 2022 07:41:41 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:77fcf2c0cc10658b5d6b4e43a75682b8bebbdc2e47895412dd1241c0422b8368`  
		Last Modified: Tue, 29 Mar 2022 00:18:56 GMT  
		Size: 2.8 MB (2814846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02339d74c6ee81495a0e118ded4e0419f26ccf80513936bca81454dcccb4a9ef`  
		Last Modified: Tue, 29 Mar 2022 07:42:43 GMT  
		Size: 9.6 MB (9632820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a2e134a3a26a9a610f884b36fc8c7c4515c3f8a6e496e0b30c88fe5bc2334d`  
		Last Modified: Tue, 29 Mar 2022 07:42:41 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b666408c25fa0d0d140d842ae855c147d353f9dfec2689327143be5d97c77a34`  
		Last Modified: Tue, 29 Mar 2022 07:42:42 GMT  
		Size: 6.5 MB (6492208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:a1996310e95fe58903b86881db102fc711c686616d690e464a1201242c01da6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18854963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bd0c6b0836f9d3340e3865bed234d2efe13b8dd8a243f3a3d4eb695106c636f`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:45 GMT
ADD file:08b65c73088f2cc387829e0ce9aa160db404a3e5fa0e4fda048cdbc02d8f64c2 in / 
# Tue, 29 Mar 2022 00:41:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 15:59:07 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 15:59:08 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 15:59:08 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 15:59:08 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 15:59:08 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 15:59:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 15:59:44 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 15:59:44 GMT
USER user
# Tue, 29 Mar 2022 15:59:44 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:89a2ea5c1a3e1d541ae66fbd95d215b39b560c537460c3fc76ad6826582893fe`  
		Last Modified: Tue, 29 Mar 2022 00:47:35 GMT  
		Size: 2.6 MB (2605074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1a5a4806a9221ab47409adcf5e27285f18845563e348e4bff66f36a4ec7727`  
		Last Modified: Tue, 29 Mar 2022 16:03:04 GMT  
		Size: 10.0 MB (9971979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ef67480f26d7536af4b650290ddd1955b0ef1afd6b33b3cdb1fcf4f4756f42`  
		Last Modified: Tue, 29 Mar 2022 16:03:04 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffa0c352647c43ea9c6e7c65920a410f592c9417d32b6fba1f0bad1646fc40e`  
		Last Modified: Tue, 29 Mar 2022 16:03:05 GMT  
		Size: 6.3 MB (6276640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:alpine`

```console
$ docker pull irssi@sha256:fc0f0ae29aedc3e3dfee43d698d4de461180f8959428023f3a5bd95b61433f18
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
$ docker pull irssi@sha256:d7bbd05aae77230148f9a3af4a07717c5626cdb254caa1dc239bfc8866124f3e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18648371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b63678d9d2827a5a4d447b135a05921b9b618d639a9641f3970ce71fbad41c58`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:46 GMT
ADD file:a2ef39a587aac85256b55bee81f17d73aaa7154b2a32a31527c7803fb889f2e7 in / 
# Tue, 29 Mar 2022 00:19:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 16:40:04 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 16:40:04 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 16:40:05 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 16:40:05 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 16:40:05 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 16:40:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 16:40:49 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 16:40:49 GMT
USER user
# Tue, 29 Mar 2022 16:40:49 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b9c05db88786fd3c89b78787631257301391f898c03ba50553b556630046a741`  
		Last Modified: Tue, 29 Mar 2022 00:20:43 GMT  
		Size: 2.8 MB (2819223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c516145633461419b5a658706a7453eb731aaf449afd25b5996b275b8692bb0e`  
		Last Modified: Tue, 29 Mar 2022 16:41:30 GMT  
		Size: 9.5 MB (9540598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d5246be564bab1c71a70cfe50bdab883825a0ec36ed4a79b2c6730ee23849f`  
		Last Modified: Tue, 29 Mar 2022 16:41:28 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0543c4eb94b3e7485a55ed115e70d48d246fc300c3430bf71f774b156b56f7`  
		Last Modified: Tue, 29 Mar 2022 16:41:29 GMT  
		Size: 6.3 MB (6287279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:8f4fc787e0e6164fcc251c034c9fbff27d3a81fdda0c2a82c859312e16aa677a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17385391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:facc4fa1f84eebf576961df4f191b9e7763fd7f790ee44517915d56ab994e139`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:56 GMT
ADD file:23d913551f75313e359a4e93592ea0a9655e1a7c2bec5fddd210717d70c3114b in / 
# Tue, 29 Mar 2022 00:49:57 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 14:24:05 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 14:24:06 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 14:24:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 14:24:08 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 14:24:08 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 14:25:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 14:25:17 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 14:25:18 GMT
USER user
# Tue, 29 Mar 2022 14:25:18 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:eba0847afba90891ea7dae672f5dadfa405a822df0bc9c00b9e3328fd5fd889c`  
		Last Modified: Tue, 29 Mar 2022 00:51:57 GMT  
		Size: 2.6 MB (2625139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475d9671ce28a72461f25c4368162f9eac018ffced5ee61d17852dac61f60923`  
		Last Modified: Tue, 29 Mar 2022 14:25:59 GMT  
		Size: 8.8 MB (8771957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223ba1931ceb81e998f74a59ac08d88367fa3be50d7864242a41937e0a744bb8`  
		Last Modified: Tue, 29 Mar 2022 14:25:51 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9769077f19f3aaf8bd8f635611ddc58ab0133ca7a4207c1e68a6b84b68056afa`  
		Last Modified: Tue, 29 Mar 2022 14:25:55 GMT  
		Size: 6.0 MB (5987025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:645f3bdeef2e0deedf6315612f78330153c94d47580d86102653f44c653cbcfb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16839519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c53528eb26529ee3c99677c1271b1f6fe9b45db594e0a4d5f16d5bb51dd858cf`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 02:13:57 GMT
ADD file:9995ada53dfe4b82c6c01a9143cdcf8aa3aabac359fa023f5fa4da85e7a88704 in / 
# Tue, 29 Mar 2022 02:13:58 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 02:23:53 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 30 Mar 2022 02:23:53 GMT
ENV HOME=/home/user
# Wed, 30 Mar 2022 02:23:55 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 30 Mar 2022 02:23:55 GMT
ENV LANG=C.UTF-8
# Wed, 30 Mar 2022 02:23:56 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 30 Mar 2022 02:25:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 30 Mar 2022 02:25:01 GMT
WORKDIR /home/user
# Wed, 30 Mar 2022 02:25:01 GMT
USER user
# Wed, 30 Mar 2022 02:25:02 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:9e629c3986cd97398b7f233a377ad62b7d37cbccbcba0bbae7c5bc600ea73620`  
		Last Modified: Tue, 29 Mar 2022 02:15:59 GMT  
		Size: 2.4 MB (2427878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef6405d47acdbe9f502c4db8aa5db79963974eb33c7c7db6367815d922d0d34`  
		Last Modified: Wed, 30 Mar 2022 02:26:38 GMT  
		Size: 8.6 MB (8626355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360bcdf4cc43bbde189db2de03107a0ef571fdf754c37919f41990fba758ab25`  
		Last Modified: Wed, 30 Mar 2022 02:26:31 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3419b023d43ddc842375a10a3b44776c2694b31cdb493104714b3331e346e099`  
		Last Modified: Wed, 30 Mar 2022 02:26:34 GMT  
		Size: 5.8 MB (5784017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:dfc50492eaf70eaec1101ec66e1039ff67a7db7dd5800d74dc45a4a739e02c20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18505715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39eb77e04653f1fe9557fb01ddbcf5aa051eb2f6c3c10529e6e8c1dda25085a7`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:18 GMT
ADD file:3b8e0dac20ca40faf2aaf084b69476a222952f177c0e6ec90804a10c91a51feb in / 
# Tue, 29 Mar 2022 00:40:19 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:59:34 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 11:59:35 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 11:59:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 11:59:37 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 11:59:38 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 12:00:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 12:00:38 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 12:00:39 GMT
USER user
# Tue, 29 Mar 2022 12:00:40 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4e7dd0becbc2dc968b69cba46c81a25fa500c88a644832ce17a5bb090925fa79`  
		Last Modified: Tue, 29 Mar 2022 00:41:37 GMT  
		Size: 2.7 MB (2720845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac63509931e219bc0df384426086bba93e5441adbe04844a6c56a7735dac3694`  
		Last Modified: Tue, 29 Mar 2022 12:01:26 GMT  
		Size: 9.5 MB (9536372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a61c76a95903e39d6d820ac1aa943f60dadb3928830a7cdca8225e25f8adef9`  
		Last Modified: Tue, 29 Mar 2022 12:01:24 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a666811bc4a9b90ef3fd8809c2eee8110d7113f8ec0ff856025534ae9399d8`  
		Last Modified: Tue, 29 Mar 2022 12:01:25 GMT  
		Size: 6.2 MB (6247254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; 386

```console
$ docker pull irssi@sha256:2bf221ef68d0a83a2116f20883a82c6ce6a7e0b4a5dfd71aa071b1db35aba964
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17703944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9afa5090692aa67a79e6c4008981e2926490e0d02199c568434f36da260714c`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:38:45 GMT
ADD file:f1abe5c2930209c2d735059c8e767e630c0818cc18a4fd10b0b90e6efbc675e2 in / 
# Tue, 29 Mar 2022 00:38:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 05:49:58 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 05:49:58 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 05:49:59 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 05:50:00 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 05:50:01 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 05:50:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 05:50:35 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 05:50:36 GMT
USER user
# Tue, 29 Mar 2022 05:50:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:dadad3128a09e6d507e89afe042cb1d48da14a72b28ca79dec7c6acf971bd9e6`  
		Last Modified: Tue, 29 Mar 2022 00:40:03 GMT  
		Size: 2.8 MB (2820388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101c682f90c53e18b63f7d30a8a7307eac0253f42c2fd84242c34fe251569421`  
		Last Modified: Tue, 29 Mar 2022 05:51:27 GMT  
		Size: 8.9 MB (8904321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:749bdf2ce2f439246606355222bf5bc711659dab2fa692f263642488f30cf45a`  
		Last Modified: Tue, 29 Mar 2022 05:51:26 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83177ea77693953b946bef5957dce55878d366d9332cb8cb61db7f190ce662f4`  
		Last Modified: Tue, 29 Mar 2022 05:51:27 GMT  
		Size: 6.0 MB (5977991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:977677327cf46ebee97c359921786db207de5c7cb4ab7d9b116d4c1d33ce4a80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18941144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:608f69d4d0976fd802228409ecdc55faff220c9aee1b43137f96bf8338f677f6`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:17:21 GMT
ADD file:0f301305d95e2e1e0580ec71f76edab57a1c18ed0adba5d09708b587ec19e622 in / 
# Tue, 29 Mar 2022 00:17:25 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:40:24 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 07:40:29 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 07:40:34 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 07:40:36 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 07:40:39 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 07:41:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 07:41:37 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 07:41:39 GMT
USER user
# Tue, 29 Mar 2022 07:41:41 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:77fcf2c0cc10658b5d6b4e43a75682b8bebbdc2e47895412dd1241c0422b8368`  
		Last Modified: Tue, 29 Mar 2022 00:18:56 GMT  
		Size: 2.8 MB (2814846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02339d74c6ee81495a0e118ded4e0419f26ccf80513936bca81454dcccb4a9ef`  
		Last Modified: Tue, 29 Mar 2022 07:42:43 GMT  
		Size: 9.6 MB (9632820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a2e134a3a26a9a610f884b36fc8c7c4515c3f8a6e496e0b30c88fe5bc2334d`  
		Last Modified: Tue, 29 Mar 2022 07:42:41 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b666408c25fa0d0d140d842ae855c147d353f9dfec2689327143be5d97c77a34`  
		Last Modified: Tue, 29 Mar 2022 07:42:42 GMT  
		Size: 6.5 MB (6492208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; s390x

```console
$ docker pull irssi@sha256:a1996310e95fe58903b86881db102fc711c686616d690e464a1201242c01da6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18854963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bd0c6b0836f9d3340e3865bed234d2efe13b8dd8a243f3a3d4eb695106c636f`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:45 GMT
ADD file:08b65c73088f2cc387829e0ce9aa160db404a3e5fa0e4fda048cdbc02d8f64c2 in / 
# Tue, 29 Mar 2022 00:41:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 15:59:07 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 15:59:08 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 15:59:08 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 15:59:08 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 15:59:08 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 15:59:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 15:59:44 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 15:59:44 GMT
USER user
# Tue, 29 Mar 2022 15:59:44 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:89a2ea5c1a3e1d541ae66fbd95d215b39b560c537460c3fc76ad6826582893fe`  
		Last Modified: Tue, 29 Mar 2022 00:47:35 GMT  
		Size: 2.6 MB (2605074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1a5a4806a9221ab47409adcf5e27285f18845563e348e4bff66f36a4ec7727`  
		Last Modified: Tue, 29 Mar 2022 16:03:04 GMT  
		Size: 10.0 MB (9971979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ef67480f26d7536af4b650290ddd1955b0ef1afd6b33b3cdb1fcf4f4756f42`  
		Last Modified: Tue, 29 Mar 2022 16:03:04 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffa0c352647c43ea9c6e7c65920a410f592c9417d32b6fba1f0bad1646fc40e`  
		Last Modified: Tue, 29 Mar 2022 16:03:05 GMT  
		Size: 6.3 MB (6276640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:latest`

```console
$ docker pull irssi@sha256:480c39b4457078a69d69e8cc069a98f87278350e1f6ca14d4cbe79616f0e00b1
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
$ docker pull irssi@sha256:898197fd559f9b169fa4d36cb9424351490be12245aa2e2c4e85838db057306d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50628334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a33ad04f436ec45a3cc476c2c220e7d42ce40687a2c41dc99cc020453041b3`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 16:39:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 16:39:05 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 16:39:06 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 16:39:06 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 16:39:06 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 16:39:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 16:39:57 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 16:39:57 GMT
USER user
# Tue, 29 Mar 2022 16:39:57 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd2cdd5c22666980d61bf83c478dfc880881556673a21e118f955376664ea2a`  
		Last Modified: Tue, 29 Mar 2022 16:41:14 GMT  
		Size: 17.0 MB (17038736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2861ba30751829fb2555bb33ca9170f484208f0049973581aa13988f65bcce`  
		Last Modified: Tue, 29 Mar 2022 16:41:10 GMT  
		Size: 4.2 KB (4209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bcc182247f746f92a6a75dee26bc22a8d50acc4c3286802af9e38fdd1c0b90`  
		Last Modified: Tue, 29 Mar 2022 16:41:12 GMT  
		Size: 6.4 MB (6433419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm variant v5

```console
$ docker pull irssi@sha256:ce001569547e34819fdf079112b88f49e44b499ed10726ae591cc6c5a0ea2bc9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46893537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f038e776a2c3d5a6f454656fe59c07165ac40653fc18ea19e3ce095e5a5056d`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:51:36 GMT
ADD file:7ac5498e2c44686d7eb272ef7645a0a64486cf942610f6754aa4a932f5b1a4be in / 
# Tue, 29 Mar 2022 00:51:37 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 08:47:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 08:47:02 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 08:47:04 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 08:47:04 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 08:47:05 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 08:48:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 08:48:51 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 08:48:52 GMT
USER user
# Tue, 29 Mar 2022 08:48:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8f10b1b67f0119a2dd5f838a3e98ab2c412e4b51fb1e4841e2b79fd4cae86105`  
		Last Modified: Tue, 29 Mar 2022 01:06:51 GMT  
		Size: 24.9 MB (24887495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb68688aa70be630bab2170a39e77d005f229ab6390b76e8d3b9a89acf825b8`  
		Last Modified: Tue, 29 Mar 2022 08:49:39 GMT  
		Size: 15.9 MB (15937355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f462c871b83b3653daf80a7cec6d9d06057396022a1e2b36a5764dcc29588a3`  
		Last Modified: Tue, 29 Mar 2022 08:49:28 GMT  
		Size: 4.2 KB (4199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae06e20e90eb68e6394cd65e5487477d7353a5816b39fa872fac1074888de42c`  
		Last Modified: Tue, 29 Mar 2022 08:49:31 GMT  
		Size: 6.1 MB (6064488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm variant v7

```console
$ docker pull irssi@sha256:3db3ddfc45fb2ccf78e4b7349fa0fd23aa6e59eaf69371032c89f4b995b2baf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44287695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8432232c7fa73842270a6402575d03dcd1af079cced86028166d84a2623f94cc`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 02:19:40 GMT
ADD file:8d54e000817531229c35a32eee074105c7b4d3c08b7ca56b1abdd80571687f28 in / 
# Tue, 29 Mar 2022 02:19:41 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:21:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:21:34 GMT
ENV HOME=/home/user
# Wed, 30 Mar 2022 02:21:36 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 30 Mar 2022 02:21:37 GMT
ENV LANG=C.UTF-8
# Wed, 30 Mar 2022 02:21:37 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 30 Mar 2022 02:23:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 30 Mar 2022 02:23:23 GMT
WORKDIR /home/user
# Wed, 30 Mar 2022 02:23:23 GMT
USER user
# Wed, 30 Mar 2022 02:23:24 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:d4bf0b27c669e589de33695047d638174fc2ca819a4366d5f80d1ad6b01c0c0e`  
		Last Modified: Tue, 29 Mar 2022 02:35:26 GMT  
		Size: 22.8 MB (22753045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac8262be381607606ea917e05e243851b4d99f2c3b81758f6312dfd87969356`  
		Last Modified: Wed, 30 Mar 2022 02:26:12 GMT  
		Size: 15.6 MB (15597948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62dbb031a500a927ff9934a53e57156d7a1faa17d61c5bd2e83339d685db97a8`  
		Last Modified: Wed, 30 Mar 2022 02:25:56 GMT  
		Size: 4.2 KB (4196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:489ce9745374ad929508ff3be1139e1d7e92b1035939d613574df8757f45f1ba`  
		Last Modified: Wed, 30 Mar 2022 02:26:00 GMT  
		Size: 5.9 MB (5932506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:8c11bc795decb16053eee4599521d727932b0b65a6043eb2d753763f6a0fcba8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48915028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:325958a38fb96c65a0cbe50172b3b831b9e521e2f46956e55bf1228253f6885e`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:42 GMT
ADD file:fdc8a5391a75cbf8c121f8f799ca08e94d2b3967b2546b36231c9297f7ce2151 in / 
# Tue, 29 Mar 2022 00:43:43 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 11:58:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 11:58:23 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 11:58:24 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 11:58:25 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 11:58:26 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 11:59:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 11:59:24 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 11:59:25 GMT
USER user
# Tue, 29 Mar 2022 11:59:26 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:5022906f515a0d4ec6bc1d0e5e7a01f47b1fbbb912e7e3f1ace27987169a9a21`  
		Last Modified: Tue, 29 Mar 2022 00:50:58 GMT  
		Size: 25.9 MB (25919777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99733c8db8c4371f3d274a989271d20844041e6ee266e8f74fa0a52e8e126277`  
		Last Modified: Tue, 29 Mar 2022 12:01:08 GMT  
		Size: 16.8 MB (16815150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b028d71796d54b96aa2ef9143f43950b86a4c6451c7da2b4836a693416e08660`  
		Last Modified: Tue, 29 Mar 2022 12:01:04 GMT  
		Size: 4.1 KB (4075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e78bd4b4962d8db2ae26337c77d821e36a0b186d875a7d5626aabe15e2be8e0`  
		Last Modified: Tue, 29 Mar 2022 12:01:05 GMT  
		Size: 6.2 MB (6176026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; 386

```console
$ docker pull irssi@sha256:406c82696ff47006adf53f11781be3f504cc4fe335a780106844f23f6a799af2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50264307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6ac23335fd4259a5aa45431e78631ccb7ba153d3b8b30da64cdff5bdafe99cb`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:42:26 GMT
ADD file:bcf3d504dc285de8b639c7f4017c41a4593a6c2aa6f046c9be79e587d05b5120 in / 
# Tue, 29 Mar 2022 00:42:27 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 05:48:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 05:48:43 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 05:48:44 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 05:48:45 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 05:48:46 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 05:49:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 05:49:35 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 05:49:36 GMT
USER user
# Tue, 29 Mar 2022 05:49:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:65b92490caa5e2c0588fab60d39315a2a8c09aa8ea0fe208d23f6984a47ecc03`  
		Last Modified: Tue, 29 Mar 2022 00:50:02 GMT  
		Size: 27.8 MB (27801252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65153b3620d7c8324690f0556ea546e098d1c5abea0de04cec331abe652fd6cc`  
		Last Modified: Tue, 29 Mar 2022 05:51:09 GMT  
		Size: 16.6 MB (16565592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f81e51b798316e6dddef7d44c46adbbfac04c8639c9c6d7fc569722558240ce`  
		Last Modified: Tue, 29 Mar 2022 05:51:05 GMT  
		Size: 4.1 KB (4052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb19cd58e039f1ea121d78c3603e8bcfac093136e3b920a3ab1df0bbf9ecd21d`  
		Last Modified: Tue, 29 Mar 2022 05:51:06 GMT  
		Size: 5.9 MB (5893411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; mips64le

```console
$ docker pull irssi@sha256:eed1cd2fe79ac4ab10dee6870ffa2be2cec900112d6a0a5d01b0474c5e8301f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47634326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b493b1d75e78f56f629ff77cc840485832b6f90136f061ceff8a2788aa90025`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 07:43:36 GMT
ADD file:7827dc4070f09537c063b825b0b7a5b076fac295f9afa415dee6c5346c38d46b in / 
# Tue, 29 Mar 2022 07:43:40 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 10:26:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 10:26:25 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 10:26:33 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 10:26:36 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 10:26:39 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 10:31:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 10:31:16 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 10:31:19 GMT
USER user
# Tue, 29 Mar 2022 10:31:23 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4a3e27ca4ec7041c36d0e9cbc672ce565851ce1a0cc90120d7a923a938fb3c18`  
		Last Modified: Tue, 29 Mar 2022 07:54:19 GMT  
		Size: 25.8 MB (25818066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2023bef9f22712b6457705ea84614163a3d0a854f38d7f2f13f388c262fd8d68`  
		Last Modified: Tue, 29 Mar 2022 10:31:51 GMT  
		Size: 15.7 MB (15731870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783dfb57d1278d639db4a6acd55eea930b6387da357be8c4e1ef6af2c734ff13`  
		Last Modified: Tue, 29 Mar 2022 10:31:37 GMT  
		Size: 4.1 KB (4069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e297148bdf9b4491afc8d6b2898998918425c1e35865b360d93b281abe77ce`  
		Last Modified: Tue, 29 Mar 2022 10:31:40 GMT  
		Size: 6.1 MB (6080321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; ppc64le

```console
$ docker pull irssi@sha256:a460c3520546307e352a19d055007a7fcba927f322c545e3e7296c1bfdf74592
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54787995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f694d959fe967b7564e8a7cdaf212e3d814c5d6b79c1d3696f77b35c476d8ea`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:59 GMT
ADD file:7271d778d432a07f57fedf8d50d83699ef545acc9db9346f6fe75b0054af4cd1 in / 
# Tue, 29 Mar 2022 00:23:00 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 07:34:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 07:35:01 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 07:35:09 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 07:35:12 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 07:35:15 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 07:39:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 07:39:58 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 07:39:59 GMT
USER user
# Tue, 29 Mar 2022 07:40:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:7db831386ce67ac1cf2b4f1513fe3746c9ea2b8d4c82efca75be638eaf533614`  
		Last Modified: Tue, 29 Mar 2022 00:34:41 GMT  
		Size: 30.6 MB (30560163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6f0e2fb83c5287040e529ec1e0cc34c5383697a80a278632cddf17a110ab26`  
		Last Modified: Tue, 29 Mar 2022 07:42:17 GMT  
		Size: 17.4 MB (17440827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9798211288cab71997a2ba40949386224112d0754a517ece37e3cfc68ccc5ad0`  
		Last Modified: Tue, 29 Mar 2022 07:42:12 GMT  
		Size: 4.2 KB (4216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dadee1dc4117b4a1068f72e957d68471ff9f516c4db70a938e36a427e6f45b7`  
		Last Modified: Tue, 29 Mar 2022 07:42:14 GMT  
		Size: 6.8 MB (6782789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; s390x

```console
$ docker pull irssi@sha256:8aa6207ef3bc8833bb6a35d3870a604c6e90fc607bf1bbebab6688fb11f2d4ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49068950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9b140f48665cda5494c089acdb6eae60f96d15c3fb4dd0ba4b19d99953db655`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:52:27 GMT
ADD file:dbf01085079906b34f3ec9db0b9ce31aa1466b935a47e8e30772a5488f76fec0 in / 
# Tue, 29 Mar 2022 00:52:29 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 15:57:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 15:57:55 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 15:57:56 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 15:57:56 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 15:57:56 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 15:58:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 29 Mar 2022 15:58:46 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 15:58:46 GMT
USER user
# Tue, 29 Mar 2022 15:58:46 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:66ccc81b275f683f44a0f40ddce6992117eefe92dca84fadf6d2e51c22d11a64`  
		Last Modified: Tue, 29 Mar 2022 01:10:22 GMT  
		Size: 25.8 MB (25765916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f745ab618468906119bb54aef0c97df6677ebed5694c4d839b8103c60531d8`  
		Last Modified: Tue, 29 Mar 2022 16:00:54 GMT  
		Size: 16.9 MB (16914174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e65abef5df82c79a408eb80534564b0361dc35744b6aa982b493c4f0e59e55d4`  
		Last Modified: Tue, 29 Mar 2022 16:00:54 GMT  
		Size: 4.2 KB (4216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a6b20318811928ca8b7d3a3a3229cab3b5ac4bd24212ec30916433aef99d73`  
		Last Modified: Tue, 29 Mar 2022 16:00:54 GMT  
		Size: 6.4 MB (6384644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
