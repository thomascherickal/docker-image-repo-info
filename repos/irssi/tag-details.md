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
$ docker pull irssi@sha256:eabe9a654c437d1055782b8fd8a2ff73fd3f2254a9549914cba6215fa321dc67
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
$ docker pull irssi@sha256:e959721514032b8e73f930e42ef95a7b1908148e563aee4eda55c80e3113f236
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50615098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28696f30fb5f7f5f5582364cae89ac875de7c473e676dfc8f80df20886029e2a`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:28:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:28:56 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 02:28:57 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 02:28:57 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 02:28:57 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 02:30:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 02:30:02 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 02:30:03 GMT
USER user
# Tue, 21 Dec 2021 02:30:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59be89c444cb2d9ace3b84fc5c5762d43da553450735ff834500ef787752fe6`  
		Last Modified: Tue, 21 Dec 2021 02:30:24 GMT  
		Size: 17.0 MB (17023696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416b353fa94267ed4404524f3572e09a455d86006dd420743d6b4ff16c94cdcd`  
		Last Modified: Tue, 21 Dec 2021 02:30:20 GMT  
		Size: 4.2 KB (4206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd3a6792e918c8d1e966ac97d2b00cd8b94b23ded6762536c890d459079ac9b`  
		Last Modified: Tue, 21 Dec 2021 02:30:21 GMT  
		Size: 6.4 MB (6433473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm variant v5

```console
$ docker pull irssi@sha256:27ad09505b4c6d369dfff267a263c9644582ddb3300e2b92d99b3d881ee91dc2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46877720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b2f7fd8bcc1ff3dc6bc7b848d4158846f575718a4314a85a49cce74f8b9bf2d`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 01:51:32 GMT
ADD file:f757929225218280f26d0eca53387788343e93cc9658f5baeb58957776114579 in / 
# Tue, 21 Dec 2021 01:51:33 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:32:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:32:04 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 03:32:06 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 03:32:07 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:32:07 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 03:34:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 03:34:08 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 03:34:09 GMT
USER user
# Tue, 21 Dec 2021 03:34:09 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:7d69cd3acec6d9e5ca88bdd718b069a7272b722048f49b6d21fbe85fc6c82560`  
		Last Modified: Tue, 21 Dec 2021 02:07:21 GMT  
		Size: 24.9 MB (24886253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9972abbb34ae72d3b0070f65b0ce5d55ab8380dd8a5b296110f26f4c1e4c8739`  
		Last Modified: Tue, 21 Dec 2021 03:34:59 GMT  
		Size: 15.9 MB (15922774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11e8b11f795a11c52cb86064bfcf17c440413738a87072860c0459aa457734e`  
		Last Modified: Tue, 21 Dec 2021 03:34:42 GMT  
		Size: 4.2 KB (4198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70f23a6e04f65c37ab26f520582f612442f447852daeb23349c80ec42b30552`  
		Last Modified: Tue, 21 Dec 2021 03:34:46 GMT  
		Size: 6.1 MB (6064495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm variant v7

```console
$ docker pull irssi@sha256:4a19c10049a9e3a6a6f2a6b48f17ed5cf6a9eeffdac2084f2a1e3bb2454b14ba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44274081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05f35d7af06a94f17bb1a15631d0a2cf2b7b2470c13c789d5cc4318e4ce4afd1`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:52 GMT
ADD file:1381e18e2847f24ebd16d8e83ad940adeff45aca2c327d4e07d7451816f29420 in / 
# Tue, 21 Dec 2021 02:00:52 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:21:25 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 07:21:27 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 07:21:28 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 07:21:28 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 07:23:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 07:23:17 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 07:23:17 GMT
USER user
# Tue, 21 Dec 2021 07:23:18 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b597e1a6bc27aa2a24a587cb687c9551dfbcfa730a11d48c5a44ff77ff6fdd75`  
		Last Modified: Tue, 21 Dec 2021 02:16:50 GMT  
		Size: 22.8 MB (22754324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338c7f0212075503206eaa4c6bcfae4b0b7c9c0aae5b57377ed3148c5e84491d`  
		Last Modified: Tue, 21 Dec 2021 07:24:41 GMT  
		Size: 15.6 MB (15583032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf715040fb97757cdd867af3ca6d76d851b0745b5e558aa78a93c8bd45e9892`  
		Last Modified: Tue, 21 Dec 2021 07:24:25 GMT  
		Size: 4.2 KB (4192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0dae9b7e84b9a5d9aacb48828f3eed3a1e422e5d7b3ba85cd0c83b1f8fcec70`  
		Last Modified: Tue, 21 Dec 2021 07:24:29 GMT  
		Size: 5.9 MB (5932533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:60457f603545fcd1f5dec369b7188e9fdf72344e5ae315294459bd17f5deb454
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48899497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfa76b323be41cbaca5865013d170ba2315088f61d4fa21f9ce40c9580d29828`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 10:18:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 10:18:09 GMT
ENV HOME=/home/user
# Thu, 02 Dec 2021 10:18:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 02 Dec 2021 10:18:11 GMT
ENV LANG=C.UTF-8
# Thu, 02 Dec 2021 10:18:12 GMT
ENV IRSSI_VERSION=1.2.3
# Thu, 02 Dec 2021 10:18:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 02 Dec 2021 10:18:53 GMT
WORKDIR /home/user
# Thu, 02 Dec 2021 10:18:54 GMT
USER user
# Thu, 02 Dec 2021 10:18:55 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd767de3273672ff5b8b0dbc5e7946d73f8a48def2a475e0aeba3663abd64f51`  
		Last Modified: Thu, 02 Dec 2021 10:19:36 GMT  
		Size: 16.8 MB (16796286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7292819705b5179aa616a780be2baa620f3ee6875935bf179183753616b6f349`  
		Last Modified: Thu, 02 Dec 2021 10:19:33 GMT  
		Size: 4.1 KB (4071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d72ba2e26eefead289f206dc9f257d1a52db264eb062b40fb6303214a47df`  
		Last Modified: Thu, 02 Dec 2021 10:19:34 GMT  
		Size: 6.2 MB (6175996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; 386

```console
$ docker pull irssi@sha256:d3ca7f90d7175158499ce79b153f9e6491202d0350e781fffff0cdb3b4323ccc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50461376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27404c72d886d49efaab162f5322fdd7bab66e3e2639d274745a61ecce8258ea`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:45 GMT
ADD file:78342a77df22ca22804ea5aec6415ce10c1fdc35687f1b25c5f86850f41d3905 in / 
# Tue, 21 Dec 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:41:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:41:06 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 07:41:07 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 07:41:08 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 07:41:08 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 07:42:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 07:42:35 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 07:42:35 GMT
USER user
# Tue, 21 Dec 2021 07:42:35 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:16e3a221bce3a5f7f4a71f72926f381ff9c6141ccb5918b7ea924ff7f7f09d06`  
		Last Modified: Tue, 21 Dec 2021 01:49:46 GMT  
		Size: 27.8 MB (27804573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdb20cfd72adfabb1343532d94fa58046b2e715c114de2bb2d495ebeece2682`  
		Last Modified: Tue, 21 Dec 2021 07:43:36 GMT  
		Size: 16.5 MB (16547064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b5781734632e07624e3572ae1a80fd1bdacd055a3bd11c4ce849401446c677`  
		Last Modified: Tue, 21 Dec 2021 07:43:29 GMT  
		Size: 4.2 KB (4198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b8a3e21b6c0511f13ead53720a5597649f9f96d918e32816c7c7674ba4972b`  
		Last Modified: Tue, 21 Dec 2021 07:43:32 GMT  
		Size: 6.1 MB (6105541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; mips64le

```console
$ docker pull irssi@sha256:afed46d618a02883850d985cfc57351066756ac4be967e25c0c2b45b93307c71
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47815170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d18fc013099ba02ad5eef9adde31927330aa957623529cf16ede04b3ea37087`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 02:09:59 GMT
ADD file:1e736cd218a1aa1d9d52dfb824407b84a8d10720ee840b3d81cdf74df62b74b8 in / 
# Tue, 21 Dec 2021 02:10:00 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:51:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:51:49 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 03:51:51 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 03:51:51 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:51:51 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 03:54:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 03:54:23 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 03:54:24 GMT
USER user
# Tue, 21 Dec 2021 03:54:24 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4425ebd1b1a185b87251c0eb43ab9b16b24ec96090a67323f44e2365b8f9bc19`  
		Last Modified: Tue, 21 Dec 2021 02:19:49 GMT  
		Size: 25.8 MB (25820202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85cbf48de6d54494842b75c145a74d8f799e352a563f58a8b164546fd9815dd`  
		Last Modified: Tue, 21 Dec 2021 03:55:05 GMT  
		Size: 15.7 MB (15698102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e524d04d8239c5b2e5bf926abdd70e466e556364301e359b5667f14b961b63`  
		Last Modified: Tue, 21 Dec 2021 03:54:50 GMT  
		Size: 4.2 KB (4179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7359d2585748ca1c9bc41d663fe7a39c7c91976a72362c271b7459f3177b1b07`  
		Last Modified: Tue, 21 Dec 2021 03:54:54 GMT  
		Size: 6.3 MB (6292687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; ppc64le

```console
$ docker pull irssi@sha256:ababf449214d8594cf18a462f9a08d25102f9aa24c06f45cc230056441d48550
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54779424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a153eea02c8c045e1f776a30ce44b81a10652c78d8144e18e07fba9d364e92d`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 02:21:09 GMT
ADD file:85a8af105e3fa794598824266068cbb3c0dc66067e10e3263dab26a230458a82 in / 
# Tue, 21 Dec 2021 02:21:13 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 05:20:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 05:20:04 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 05:20:09 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 05:20:11 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 05:20:12 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 05:23:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 05:23:06 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 05:23:07 GMT
USER user
# Tue, 21 Dec 2021 05:23:08 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:e2c79f8e0929abda2022fed71e090d3c34c8c3fdfb2a513ede1d117020a46821`  
		Last Modified: Tue, 21 Dec 2021 02:30:19 GMT  
		Size: 30.6 MB (30562311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec64c0808b37b40ecbae401a09f525b3599c4933104d9f91c1b02f531261f4e4`  
		Last Modified: Tue, 21 Dec 2021 05:23:52 GMT  
		Size: 17.4 MB (17430519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271fe3dcc65a9b19c4341ced9310438adb824c08206ea6944e756081de79e466`  
		Last Modified: Tue, 21 Dec 2021 05:23:47 GMT  
		Size: 4.2 KB (4219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304933c35b9311c11cc8edccb32e806769ecfb2944b2388f8a07da23ffeca40b`  
		Last Modified: Tue, 21 Dec 2021 05:23:49 GMT  
		Size: 6.8 MB (6782375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; s390x

```console
$ docker pull irssi@sha256:bb09bd5c28f1f789db24dfa8fd41a1d6e641e66e04a3596381232aecbd1f3e91
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49057908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcb7eecb8644b9881365cf635f37d162033bff573786804e8b703f3ce8846c69`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:57 GMT
ADD file:33e37861eefa46f6e5f7f4967ce8ae3167e28bc817c3c71ff90a3d51e2376a0f in / 
# Tue, 21 Dec 2021 01:42:59 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:09:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:09:35 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 03:09:36 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 03:09:36 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:09:36 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 03:10:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 03:10:11 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 03:10:11 GMT
USER user
# Tue, 21 Dec 2021 03:10:12 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:10979941d091693f28e3dc033cc6ca88996acf42a0aace27ad85fbd894945e20`  
		Last Modified: Tue, 21 Dec 2021 01:48:51 GMT  
		Size: 25.8 MB (25769051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b63d4cfd4aa344eea05406bab43c94faa838c6ead77d009d598529af4daa60a`  
		Last Modified: Tue, 21 Dec 2021 03:10:50 GMT  
		Size: 16.9 MB (16899907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a0decb3e6de2f0b3f7995b35b377ce3394134e98d44f3f8038a6db18883faf`  
		Last Modified: Tue, 21 Dec 2021 03:10:45 GMT  
		Size: 4.2 KB (4211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875d816cdaed07c7b756014dc420c87bd1991d3b3c8d3380d90c2bf738d50e88`  
		Last Modified: Tue, 21 Dec 2021 03:10:46 GMT  
		Size: 6.4 MB (6384739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1-alpine`

```console
$ docker pull irssi@sha256:b6199cce4bbccd62cdf2ab15c4e36f381babd27c1f693bb96ea99c20a6c9a9ef
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
$ docker pull irssi@sha256:a7f12f792fd4bf788c131dfa714df982d08d040cb5f0cc002e43e6e2b6675fb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18651944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:064295e6180eddccae4c53bfa3ccc4198baf64035be43d045aea0053df5b5ab2`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:21:09 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 13 Nov 2021 06:21:09 GMT
ENV HOME=/home/user
# Sat, 13 Nov 2021 06:21:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 13 Nov 2021 06:21:10 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 06:21:10 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 13 Nov 2021 06:22:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 13 Nov 2021 06:22:07 GMT
WORKDIR /home/user
# Sat, 13 Nov 2021 06:22:07 GMT
USER user
# Sat, 13 Nov 2021 06:22:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce5baac574d8b4271c82fa64dcdd49fa857685442591bb2a9088f4a17aa326d`  
		Last Modified: Sat, 13 Nov 2021 06:22:31 GMT  
		Size: 9.5 MB (9546893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6a10ef4b17c6ffd971ee996f3f9f1f835f466b8f8bf05e5f6d7b8e11bdf3e0`  
		Last Modified: Sat, 13 Nov 2021 06:22:28 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd14ec244a7d85641c549e5c3e926f9619beb3ef04c2de1296ef5d278268ef54`  
		Last Modified: Sat, 13 Nov 2021 06:22:30 GMT  
		Size: 6.3 MB (6281356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:411622af3811853615c7098dfa1b54089cbfd39ee2b84ad609555f5667f92b82
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17394658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da6d2fa6232e825db829628177a338984e9d93065e36f18f273ddbbbf1230bba`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 03:07:25 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 13 Nov 2021 03:07:26 GMT
ENV HOME=/home/user
# Sat, 13 Nov 2021 03:07:27 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 13 Nov 2021 03:07:28 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 03:07:28 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 13 Nov 2021 03:08:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 13 Nov 2021 03:08:38 GMT
WORKDIR /home/user
# Sat, 13 Nov 2021 03:08:38 GMT
USER user
# Sat, 13 Nov 2021 03:08:38 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e18644b7db2c0521d7b46f9a0ad2bbef1e78c4441a4eb4edd2e471d076617e`  
		Last Modified: Sat, 13 Nov 2021 03:09:18 GMT  
		Size: 8.8 MB (8777945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47719028b3d12f241ef81a872a66d640d50374d5c7b7ada4dea7a5d4f8d628b9`  
		Last Modified: Sat, 13 Nov 2021 03:09:12 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71524eae839c07718e925705fc282eabdc5f7bdf00917807520a46cd4952a20`  
		Last Modified: Sat, 13 Nov 2021 03:09:16 GMT  
		Size: 6.0 MB (5982098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:39fd318eba9bfe402c70dbb1658cc83d2008473a2bf7c6640ffcbf0f4cab5410
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16843546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80cf593f5cd7256f7f600c886f639c64a7fef945a7476ac8f235f315f2834f7f`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:54 GMT
ADD file:a13993855beba2267575c54a0c6707ddda85d238e697a81046a8b1c1a34df054 in / 
# Fri, 12 Nov 2021 16:57:54 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 10:53:57 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 13 Nov 2021 10:53:58 GMT
ENV HOME=/home/user
# Sat, 13 Nov 2021 10:54:01 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 13 Nov 2021 10:54:02 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 10:54:02 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 13 Nov 2021 10:55:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 13 Nov 2021 10:55:27 GMT
WORKDIR /home/user
# Sat, 13 Nov 2021 10:55:27 GMT
USER user
# Sat, 13 Nov 2021 10:55:28 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:767c1b67bc22761376676021ea5a310e7a7d1344b7a017bb8ede1a202340dbaf`  
		Last Modified: Fri, 12 Nov 2021 16:59:54 GMT  
		Size: 2.4 MB (2436506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf65fbf3cfd284ebb1b6bcbb3f5aeb9c90f25a8ef76be7e8626b4de4cbc9d12f`  
		Last Modified: Sat, 13 Nov 2021 10:56:37 GMT  
		Size: 8.6 MB (8630841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb323d0bda53eaa67141782bb2c816d1ee006b00a1834b70ab92d64c7bf823ed`  
		Last Modified: Sat, 13 Nov 2021 10:56:32 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d23d9d27bff57b2dbc2a08da74408f29dc954f150b5886a7e982dbfa160800`  
		Last Modified: Sat, 13 Nov 2021 10:56:35 GMT  
		Size: 5.8 MB (5774928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:237a3fb28d0d750071b6920a2ccc32afab7b574fc1a31deb71006cc8820b50de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18493717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43e7f354df530cf5903915bf52cff862c5931681cd9d85b24b826e77a9a3998f`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:27:36 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 13 Nov 2021 06:27:37 GMT
ENV HOME=/home/user
# Sat, 13 Nov 2021 06:27:38 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 13 Nov 2021 06:27:39 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 06:27:40 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 13 Nov 2021 06:28:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 13 Nov 2021 06:28:27 GMT
WORKDIR /home/user
# Sat, 13 Nov 2021 06:28:28 GMT
USER user
# Sat, 13 Nov 2021 06:28:29 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e152f8af96423f066d9e00e70b1fbbc96e94dbf4c98f075c6b7117135d97be4b`  
		Last Modified: Sat, 13 Nov 2021 06:29:25 GMT  
		Size: 9.5 MB (9543545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6065fe2276d0eabc118421590a0496be4176b2ecb15421a8798cfd55ea4ff0eb`  
		Last Modified: Sat, 13 Nov 2021 06:29:23 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39cb7b7de97a12a3eb299292e27a79d7e76bb96fd8eef37dc3d046620f92fb67`  
		Last Modified: Sat, 13 Nov 2021 06:29:24 GMT  
		Size: 6.2 MB (6229287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; 386

```console
$ docker pull irssi@sha256:e1533792e9821046cba4fd97ad160b36c6943d86078fde47a356e79b1184755a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17711979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1216a4299c56d5ac15112c6e1df985afef515bf2dbaeaa74ac5b8479b4080fbf`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 04:44:05 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 13 Nov 2021 04:44:06 GMT
ENV HOME=/home/user
# Sat, 13 Nov 2021 04:44:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 13 Nov 2021 04:44:07 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 04:44:07 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 13 Nov 2021 04:45:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 13 Nov 2021 04:45:13 GMT
WORKDIR /home/user
# Sat, 13 Nov 2021 04:45:13 GMT
USER user
# Sat, 13 Nov 2021 04:45:13 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fb5374975ca920199ffda46b9a54fba11dd5eda1e231d1586fd28b00bfab55`  
		Last Modified: Sat, 13 Nov 2021 04:45:58 GMT  
		Size: 8.9 MB (8914326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bda351aa4adae26d595a83d58109f6b9e63f43b0ef135c5c65ae3d27207425`  
		Last Modified: Sat, 13 Nov 2021 04:45:53 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19698f734fdb7985e49d87a08629d95fecae4a127bcb935a6cb36b5e2f1eed82`  
		Last Modified: Sat, 13 Nov 2021 04:45:56 GMT  
		Size: 6.0 MB (5967572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:e563662cc89c1019d39f0eda3f4457bdc094c27f61a77384ef8358537bda818c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18946306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66dc37eef2bb5aa0607437ea97b4d616b4956415415daf2ed8dc11105d08efb9`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:25 GMT
ADD file:f7216323de17450e653f77c86d2c1e2e8ec01e1133e93f29c515761b3e9d8f7d in / 
# Fri, 12 Nov 2021 21:18:28 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:17:21 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 13 Nov 2021 15:17:25 GMT
ENV HOME=/home/user
# Sat, 13 Nov 2021 15:17:37 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 13 Nov 2021 15:17:39 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 15:17:41 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 13 Nov 2021 15:18:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 13 Nov 2021 15:18:45 GMT
WORKDIR /home/user
# Sat, 13 Nov 2021 15:18:49 GMT
USER user
# Sat, 13 Nov 2021 15:19:01 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6729720a3e6b58511df148134bb67d786ad90f9fce1c02ba5bbfd31f33055fbe`  
		Last Modified: Fri, 12 Nov 2021 21:19:49 GMT  
		Size: 2.8 MB (2820517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5c3bca0019540f7fc24b101be6d560cac83a81f1b6cda2b2fd1dcb4400c6e7`  
		Last Modified: Sat, 13 Nov 2021 15:19:52 GMT  
		Size: 9.6 MB (9642236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2dbb74b4ba4c2dc34b3813acf99e0b991bcdb045c4404168d74feb0a7d550f8`  
		Last Modified: Sat, 13 Nov 2021 15:19:50 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa5a61caf2a0e156b37a62805b3fdcfab0ec5484229e4df282556b21c89b49e`  
		Last Modified: Sat, 13 Nov 2021 15:19:51 GMT  
		Size: 6.5 MB (6482283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:4508d5ff1fb06c6ca41ad14725242a83a585019ba2c7523518098e9662766edf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18862132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aed48119bc23818d5a430a4e15912061316a5a404add032ef2b41ae01f4c0b7d`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:44 GMT
ADD file:637f327c9b07758709ef7dbc42eb472c888d221acde89b1c3775553864334d5c in / 
# Fri, 12 Nov 2021 16:41:44 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:46:37 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 12 Nov 2021 21:46:38 GMT
ENV HOME=/home/user
# Fri, 12 Nov 2021 21:46:38 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Nov 2021 21:46:39 GMT
ENV LANG=C.UTF-8
# Fri, 12 Nov 2021 21:46:39 GMT
ENV IRSSI_VERSION=1.2.3
# Fri, 12 Nov 2021 21:47:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 12 Nov 2021 21:47:14 GMT
WORKDIR /home/user
# Fri, 12 Nov 2021 21:47:14 GMT
USER user
# Fri, 12 Nov 2021 21:47:14 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b872f056719bde6e6722091afb2a3376d720c69c142b91ac352050080dd79615`  
		Last Modified: Fri, 12 Nov 2021 16:42:54 GMT  
		Size: 2.6 MB (2611155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbee0262fb10c6ee826cdf9ad391574e205886b3ecbe48df9d7faefc8631395`  
		Last Modified: Fri, 12 Nov 2021 21:47:46 GMT  
		Size: 10.0 MB (9982759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d313f2224226336843ad5b4eed2dc03c80a76d54cb049248fa3ce29f7b17f6fe`  
		Last Modified: Fri, 12 Nov 2021 21:47:44 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e0e764314fb955762494927c095f9cc4118e7b8a19b75971a7202a131ebdc4`  
		Last Modified: Fri, 12 Nov 2021 21:47:45 GMT  
		Size: 6.3 MB (6266946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2`

```console
$ docker pull irssi@sha256:eabe9a654c437d1055782b8fd8a2ff73fd3f2254a9549914cba6215fa321dc67
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
$ docker pull irssi@sha256:e959721514032b8e73f930e42ef95a7b1908148e563aee4eda55c80e3113f236
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50615098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28696f30fb5f7f5f5582364cae89ac875de7c473e676dfc8f80df20886029e2a`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:28:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:28:56 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 02:28:57 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 02:28:57 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 02:28:57 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 02:30:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 02:30:02 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 02:30:03 GMT
USER user
# Tue, 21 Dec 2021 02:30:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59be89c444cb2d9ace3b84fc5c5762d43da553450735ff834500ef787752fe6`  
		Last Modified: Tue, 21 Dec 2021 02:30:24 GMT  
		Size: 17.0 MB (17023696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416b353fa94267ed4404524f3572e09a455d86006dd420743d6b4ff16c94cdcd`  
		Last Modified: Tue, 21 Dec 2021 02:30:20 GMT  
		Size: 4.2 KB (4206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd3a6792e918c8d1e966ac97d2b00cd8b94b23ded6762536c890d459079ac9b`  
		Last Modified: Tue, 21 Dec 2021 02:30:21 GMT  
		Size: 6.4 MB (6433473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; arm variant v5

```console
$ docker pull irssi@sha256:27ad09505b4c6d369dfff267a263c9644582ddb3300e2b92d99b3d881ee91dc2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46877720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b2f7fd8bcc1ff3dc6bc7b848d4158846f575718a4314a85a49cce74f8b9bf2d`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 01:51:32 GMT
ADD file:f757929225218280f26d0eca53387788343e93cc9658f5baeb58957776114579 in / 
# Tue, 21 Dec 2021 01:51:33 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:32:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:32:04 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 03:32:06 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 03:32:07 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:32:07 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 03:34:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 03:34:08 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 03:34:09 GMT
USER user
# Tue, 21 Dec 2021 03:34:09 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:7d69cd3acec6d9e5ca88bdd718b069a7272b722048f49b6d21fbe85fc6c82560`  
		Last Modified: Tue, 21 Dec 2021 02:07:21 GMT  
		Size: 24.9 MB (24886253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9972abbb34ae72d3b0070f65b0ce5d55ab8380dd8a5b296110f26f4c1e4c8739`  
		Last Modified: Tue, 21 Dec 2021 03:34:59 GMT  
		Size: 15.9 MB (15922774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11e8b11f795a11c52cb86064bfcf17c440413738a87072860c0459aa457734e`  
		Last Modified: Tue, 21 Dec 2021 03:34:42 GMT  
		Size: 4.2 KB (4198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70f23a6e04f65c37ab26f520582f612442f447852daeb23349c80ec42b30552`  
		Last Modified: Tue, 21 Dec 2021 03:34:46 GMT  
		Size: 6.1 MB (6064495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; arm variant v7

```console
$ docker pull irssi@sha256:4a19c10049a9e3a6a6f2a6b48f17ed5cf6a9eeffdac2084f2a1e3bb2454b14ba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44274081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05f35d7af06a94f17bb1a15631d0a2cf2b7b2470c13c789d5cc4318e4ce4afd1`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:52 GMT
ADD file:1381e18e2847f24ebd16d8e83ad940adeff45aca2c327d4e07d7451816f29420 in / 
# Tue, 21 Dec 2021 02:00:52 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:21:25 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 07:21:27 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 07:21:28 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 07:21:28 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 07:23:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 07:23:17 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 07:23:17 GMT
USER user
# Tue, 21 Dec 2021 07:23:18 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b597e1a6bc27aa2a24a587cb687c9551dfbcfa730a11d48c5a44ff77ff6fdd75`  
		Last Modified: Tue, 21 Dec 2021 02:16:50 GMT  
		Size: 22.8 MB (22754324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338c7f0212075503206eaa4c6bcfae4b0b7c9c0aae5b57377ed3148c5e84491d`  
		Last Modified: Tue, 21 Dec 2021 07:24:41 GMT  
		Size: 15.6 MB (15583032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf715040fb97757cdd867af3ca6d76d851b0745b5e558aa78a93c8bd45e9892`  
		Last Modified: Tue, 21 Dec 2021 07:24:25 GMT  
		Size: 4.2 KB (4192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0dae9b7e84b9a5d9aacb48828f3eed3a1e422e5d7b3ba85cd0c83b1f8fcec70`  
		Last Modified: Tue, 21 Dec 2021 07:24:29 GMT  
		Size: 5.9 MB (5932533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:60457f603545fcd1f5dec369b7188e9fdf72344e5ae315294459bd17f5deb454
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48899497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfa76b323be41cbaca5865013d170ba2315088f61d4fa21f9ce40c9580d29828`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 10:18:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 10:18:09 GMT
ENV HOME=/home/user
# Thu, 02 Dec 2021 10:18:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 02 Dec 2021 10:18:11 GMT
ENV LANG=C.UTF-8
# Thu, 02 Dec 2021 10:18:12 GMT
ENV IRSSI_VERSION=1.2.3
# Thu, 02 Dec 2021 10:18:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 02 Dec 2021 10:18:53 GMT
WORKDIR /home/user
# Thu, 02 Dec 2021 10:18:54 GMT
USER user
# Thu, 02 Dec 2021 10:18:55 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd767de3273672ff5b8b0dbc5e7946d73f8a48def2a475e0aeba3663abd64f51`  
		Last Modified: Thu, 02 Dec 2021 10:19:36 GMT  
		Size: 16.8 MB (16796286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7292819705b5179aa616a780be2baa620f3ee6875935bf179183753616b6f349`  
		Last Modified: Thu, 02 Dec 2021 10:19:33 GMT  
		Size: 4.1 KB (4071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d72ba2e26eefead289f206dc9f257d1a52db264eb062b40fb6303214a47df`  
		Last Modified: Thu, 02 Dec 2021 10:19:34 GMT  
		Size: 6.2 MB (6175996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; 386

```console
$ docker pull irssi@sha256:d3ca7f90d7175158499ce79b153f9e6491202d0350e781fffff0cdb3b4323ccc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50461376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27404c72d886d49efaab162f5322fdd7bab66e3e2639d274745a61ecce8258ea`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:45 GMT
ADD file:78342a77df22ca22804ea5aec6415ce10c1fdc35687f1b25c5f86850f41d3905 in / 
# Tue, 21 Dec 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:41:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:41:06 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 07:41:07 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 07:41:08 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 07:41:08 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 07:42:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 07:42:35 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 07:42:35 GMT
USER user
# Tue, 21 Dec 2021 07:42:35 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:16e3a221bce3a5f7f4a71f72926f381ff9c6141ccb5918b7ea924ff7f7f09d06`  
		Last Modified: Tue, 21 Dec 2021 01:49:46 GMT  
		Size: 27.8 MB (27804573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdb20cfd72adfabb1343532d94fa58046b2e715c114de2bb2d495ebeece2682`  
		Last Modified: Tue, 21 Dec 2021 07:43:36 GMT  
		Size: 16.5 MB (16547064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b5781734632e07624e3572ae1a80fd1bdacd055a3bd11c4ce849401446c677`  
		Last Modified: Tue, 21 Dec 2021 07:43:29 GMT  
		Size: 4.2 KB (4198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b8a3e21b6c0511f13ead53720a5597649f9f96d918e32816c7c7674ba4972b`  
		Last Modified: Tue, 21 Dec 2021 07:43:32 GMT  
		Size: 6.1 MB (6105541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; mips64le

```console
$ docker pull irssi@sha256:afed46d618a02883850d985cfc57351066756ac4be967e25c0c2b45b93307c71
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47815170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d18fc013099ba02ad5eef9adde31927330aa957623529cf16ede04b3ea37087`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 02:09:59 GMT
ADD file:1e736cd218a1aa1d9d52dfb824407b84a8d10720ee840b3d81cdf74df62b74b8 in / 
# Tue, 21 Dec 2021 02:10:00 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:51:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:51:49 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 03:51:51 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 03:51:51 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:51:51 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 03:54:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 03:54:23 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 03:54:24 GMT
USER user
# Tue, 21 Dec 2021 03:54:24 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4425ebd1b1a185b87251c0eb43ab9b16b24ec96090a67323f44e2365b8f9bc19`  
		Last Modified: Tue, 21 Dec 2021 02:19:49 GMT  
		Size: 25.8 MB (25820202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85cbf48de6d54494842b75c145a74d8f799e352a563f58a8b164546fd9815dd`  
		Last Modified: Tue, 21 Dec 2021 03:55:05 GMT  
		Size: 15.7 MB (15698102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e524d04d8239c5b2e5bf926abdd70e466e556364301e359b5667f14b961b63`  
		Last Modified: Tue, 21 Dec 2021 03:54:50 GMT  
		Size: 4.2 KB (4179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7359d2585748ca1c9bc41d663fe7a39c7c91976a72362c271b7459f3177b1b07`  
		Last Modified: Tue, 21 Dec 2021 03:54:54 GMT  
		Size: 6.3 MB (6292687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; ppc64le

```console
$ docker pull irssi@sha256:ababf449214d8594cf18a462f9a08d25102f9aa24c06f45cc230056441d48550
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54779424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a153eea02c8c045e1f776a30ce44b81a10652c78d8144e18e07fba9d364e92d`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 02:21:09 GMT
ADD file:85a8af105e3fa794598824266068cbb3c0dc66067e10e3263dab26a230458a82 in / 
# Tue, 21 Dec 2021 02:21:13 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 05:20:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 05:20:04 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 05:20:09 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 05:20:11 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 05:20:12 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 05:23:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 05:23:06 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 05:23:07 GMT
USER user
# Tue, 21 Dec 2021 05:23:08 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:e2c79f8e0929abda2022fed71e090d3c34c8c3fdfb2a513ede1d117020a46821`  
		Last Modified: Tue, 21 Dec 2021 02:30:19 GMT  
		Size: 30.6 MB (30562311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec64c0808b37b40ecbae401a09f525b3599c4933104d9f91c1b02f531261f4e4`  
		Last Modified: Tue, 21 Dec 2021 05:23:52 GMT  
		Size: 17.4 MB (17430519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271fe3dcc65a9b19c4341ced9310438adb824c08206ea6944e756081de79e466`  
		Last Modified: Tue, 21 Dec 2021 05:23:47 GMT  
		Size: 4.2 KB (4219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304933c35b9311c11cc8edccb32e806769ecfb2944b2388f8a07da23ffeca40b`  
		Last Modified: Tue, 21 Dec 2021 05:23:49 GMT  
		Size: 6.8 MB (6782375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; s390x

```console
$ docker pull irssi@sha256:bb09bd5c28f1f789db24dfa8fd41a1d6e641e66e04a3596381232aecbd1f3e91
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49057908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcb7eecb8644b9881365cf635f37d162033bff573786804e8b703f3ce8846c69`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:57 GMT
ADD file:33e37861eefa46f6e5f7f4967ce8ae3167e28bc817c3c71ff90a3d51e2376a0f in / 
# Tue, 21 Dec 2021 01:42:59 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:09:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:09:35 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 03:09:36 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 03:09:36 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:09:36 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 03:10:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 03:10:11 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 03:10:11 GMT
USER user
# Tue, 21 Dec 2021 03:10:12 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:10979941d091693f28e3dc033cc6ca88996acf42a0aace27ad85fbd894945e20`  
		Last Modified: Tue, 21 Dec 2021 01:48:51 GMT  
		Size: 25.8 MB (25769051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b63d4cfd4aa344eea05406bab43c94faa838c6ead77d009d598529af4daa60a`  
		Last Modified: Tue, 21 Dec 2021 03:10:50 GMT  
		Size: 16.9 MB (16899907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a0decb3e6de2f0b3f7995b35b377ce3394134e98d44f3f8038a6db18883faf`  
		Last Modified: Tue, 21 Dec 2021 03:10:45 GMT  
		Size: 4.2 KB (4211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875d816cdaed07c7b756014dc420c87bd1991d3b3c8d3380d90c2bf738d50e88`  
		Last Modified: Tue, 21 Dec 2021 03:10:46 GMT  
		Size: 6.4 MB (6384739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2-alpine`

```console
$ docker pull irssi@sha256:b6199cce4bbccd62cdf2ab15c4e36f381babd27c1f693bb96ea99c20a6c9a9ef
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
$ docker pull irssi@sha256:a7f12f792fd4bf788c131dfa714df982d08d040cb5f0cc002e43e6e2b6675fb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18651944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:064295e6180eddccae4c53bfa3ccc4198baf64035be43d045aea0053df5b5ab2`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:21:09 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 13 Nov 2021 06:21:09 GMT
ENV HOME=/home/user
# Sat, 13 Nov 2021 06:21:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 13 Nov 2021 06:21:10 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 06:21:10 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 13 Nov 2021 06:22:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 13 Nov 2021 06:22:07 GMT
WORKDIR /home/user
# Sat, 13 Nov 2021 06:22:07 GMT
USER user
# Sat, 13 Nov 2021 06:22:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce5baac574d8b4271c82fa64dcdd49fa857685442591bb2a9088f4a17aa326d`  
		Last Modified: Sat, 13 Nov 2021 06:22:31 GMT  
		Size: 9.5 MB (9546893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6a10ef4b17c6ffd971ee996f3f9f1f835f466b8f8bf05e5f6d7b8e11bdf3e0`  
		Last Modified: Sat, 13 Nov 2021 06:22:28 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd14ec244a7d85641c549e5c3e926f9619beb3ef04c2de1296ef5d278268ef54`  
		Last Modified: Sat, 13 Nov 2021 06:22:30 GMT  
		Size: 6.3 MB (6281356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:411622af3811853615c7098dfa1b54089cbfd39ee2b84ad609555f5667f92b82
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17394658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da6d2fa6232e825db829628177a338984e9d93065e36f18f273ddbbbf1230bba`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 03:07:25 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 13 Nov 2021 03:07:26 GMT
ENV HOME=/home/user
# Sat, 13 Nov 2021 03:07:27 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 13 Nov 2021 03:07:28 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 03:07:28 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 13 Nov 2021 03:08:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 13 Nov 2021 03:08:38 GMT
WORKDIR /home/user
# Sat, 13 Nov 2021 03:08:38 GMT
USER user
# Sat, 13 Nov 2021 03:08:38 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e18644b7db2c0521d7b46f9a0ad2bbef1e78c4441a4eb4edd2e471d076617e`  
		Last Modified: Sat, 13 Nov 2021 03:09:18 GMT  
		Size: 8.8 MB (8777945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47719028b3d12f241ef81a872a66d640d50374d5c7b7ada4dea7a5d4f8d628b9`  
		Last Modified: Sat, 13 Nov 2021 03:09:12 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71524eae839c07718e925705fc282eabdc5f7bdf00917807520a46cd4952a20`  
		Last Modified: Sat, 13 Nov 2021 03:09:16 GMT  
		Size: 6.0 MB (5982098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:39fd318eba9bfe402c70dbb1658cc83d2008473a2bf7c6640ffcbf0f4cab5410
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16843546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80cf593f5cd7256f7f600c886f639c64a7fef945a7476ac8f235f315f2834f7f`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:54 GMT
ADD file:a13993855beba2267575c54a0c6707ddda85d238e697a81046a8b1c1a34df054 in / 
# Fri, 12 Nov 2021 16:57:54 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 10:53:57 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 13 Nov 2021 10:53:58 GMT
ENV HOME=/home/user
# Sat, 13 Nov 2021 10:54:01 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 13 Nov 2021 10:54:02 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 10:54:02 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 13 Nov 2021 10:55:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 13 Nov 2021 10:55:27 GMT
WORKDIR /home/user
# Sat, 13 Nov 2021 10:55:27 GMT
USER user
# Sat, 13 Nov 2021 10:55:28 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:767c1b67bc22761376676021ea5a310e7a7d1344b7a017bb8ede1a202340dbaf`  
		Last Modified: Fri, 12 Nov 2021 16:59:54 GMT  
		Size: 2.4 MB (2436506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf65fbf3cfd284ebb1b6bcbb3f5aeb9c90f25a8ef76be7e8626b4de4cbc9d12f`  
		Last Modified: Sat, 13 Nov 2021 10:56:37 GMT  
		Size: 8.6 MB (8630841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb323d0bda53eaa67141782bb2c816d1ee006b00a1834b70ab92d64c7bf823ed`  
		Last Modified: Sat, 13 Nov 2021 10:56:32 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d23d9d27bff57b2dbc2a08da74408f29dc954f150b5886a7e982dbfa160800`  
		Last Modified: Sat, 13 Nov 2021 10:56:35 GMT  
		Size: 5.8 MB (5774928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:237a3fb28d0d750071b6920a2ccc32afab7b574fc1a31deb71006cc8820b50de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18493717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43e7f354df530cf5903915bf52cff862c5931681cd9d85b24b826e77a9a3998f`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:27:36 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 13 Nov 2021 06:27:37 GMT
ENV HOME=/home/user
# Sat, 13 Nov 2021 06:27:38 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 13 Nov 2021 06:27:39 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 06:27:40 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 13 Nov 2021 06:28:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 13 Nov 2021 06:28:27 GMT
WORKDIR /home/user
# Sat, 13 Nov 2021 06:28:28 GMT
USER user
# Sat, 13 Nov 2021 06:28:29 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e152f8af96423f066d9e00e70b1fbbc96e94dbf4c98f075c6b7117135d97be4b`  
		Last Modified: Sat, 13 Nov 2021 06:29:25 GMT  
		Size: 9.5 MB (9543545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6065fe2276d0eabc118421590a0496be4176b2ecb15421a8798cfd55ea4ff0eb`  
		Last Modified: Sat, 13 Nov 2021 06:29:23 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39cb7b7de97a12a3eb299292e27a79d7e76bb96fd8eef37dc3d046620f92fb67`  
		Last Modified: Sat, 13 Nov 2021 06:29:24 GMT  
		Size: 6.2 MB (6229287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; 386

```console
$ docker pull irssi@sha256:e1533792e9821046cba4fd97ad160b36c6943d86078fde47a356e79b1184755a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17711979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1216a4299c56d5ac15112c6e1df985afef515bf2dbaeaa74ac5b8479b4080fbf`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 04:44:05 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 13 Nov 2021 04:44:06 GMT
ENV HOME=/home/user
# Sat, 13 Nov 2021 04:44:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 13 Nov 2021 04:44:07 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 04:44:07 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 13 Nov 2021 04:45:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 13 Nov 2021 04:45:13 GMT
WORKDIR /home/user
# Sat, 13 Nov 2021 04:45:13 GMT
USER user
# Sat, 13 Nov 2021 04:45:13 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fb5374975ca920199ffda46b9a54fba11dd5eda1e231d1586fd28b00bfab55`  
		Last Modified: Sat, 13 Nov 2021 04:45:58 GMT  
		Size: 8.9 MB (8914326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bda351aa4adae26d595a83d58109f6b9e63f43b0ef135c5c65ae3d27207425`  
		Last Modified: Sat, 13 Nov 2021 04:45:53 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19698f734fdb7985e49d87a08629d95fecae4a127bcb935a6cb36b5e2f1eed82`  
		Last Modified: Sat, 13 Nov 2021 04:45:56 GMT  
		Size: 6.0 MB (5967572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:e563662cc89c1019d39f0eda3f4457bdc094c27f61a77384ef8358537bda818c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18946306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66dc37eef2bb5aa0607437ea97b4d616b4956415415daf2ed8dc11105d08efb9`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:25 GMT
ADD file:f7216323de17450e653f77c86d2c1e2e8ec01e1133e93f29c515761b3e9d8f7d in / 
# Fri, 12 Nov 2021 21:18:28 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:17:21 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 13 Nov 2021 15:17:25 GMT
ENV HOME=/home/user
# Sat, 13 Nov 2021 15:17:37 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 13 Nov 2021 15:17:39 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 15:17:41 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 13 Nov 2021 15:18:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 13 Nov 2021 15:18:45 GMT
WORKDIR /home/user
# Sat, 13 Nov 2021 15:18:49 GMT
USER user
# Sat, 13 Nov 2021 15:19:01 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6729720a3e6b58511df148134bb67d786ad90f9fce1c02ba5bbfd31f33055fbe`  
		Last Modified: Fri, 12 Nov 2021 21:19:49 GMT  
		Size: 2.8 MB (2820517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5c3bca0019540f7fc24b101be6d560cac83a81f1b6cda2b2fd1dcb4400c6e7`  
		Last Modified: Sat, 13 Nov 2021 15:19:52 GMT  
		Size: 9.6 MB (9642236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2dbb74b4ba4c2dc34b3813acf99e0b991bcdb045c4404168d74feb0a7d550f8`  
		Last Modified: Sat, 13 Nov 2021 15:19:50 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa5a61caf2a0e156b37a62805b3fdcfab0ec5484229e4df282556b21c89b49e`  
		Last Modified: Sat, 13 Nov 2021 15:19:51 GMT  
		Size: 6.5 MB (6482283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:4508d5ff1fb06c6ca41ad14725242a83a585019ba2c7523518098e9662766edf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18862132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aed48119bc23818d5a430a4e15912061316a5a404add032ef2b41ae01f4c0b7d`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:44 GMT
ADD file:637f327c9b07758709ef7dbc42eb472c888d221acde89b1c3775553864334d5c in / 
# Fri, 12 Nov 2021 16:41:44 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:46:37 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 12 Nov 2021 21:46:38 GMT
ENV HOME=/home/user
# Fri, 12 Nov 2021 21:46:38 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Nov 2021 21:46:39 GMT
ENV LANG=C.UTF-8
# Fri, 12 Nov 2021 21:46:39 GMT
ENV IRSSI_VERSION=1.2.3
# Fri, 12 Nov 2021 21:47:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 12 Nov 2021 21:47:14 GMT
WORKDIR /home/user
# Fri, 12 Nov 2021 21:47:14 GMT
USER user
# Fri, 12 Nov 2021 21:47:14 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b872f056719bde6e6722091afb2a3376d720c69c142b91ac352050080dd79615`  
		Last Modified: Fri, 12 Nov 2021 16:42:54 GMT  
		Size: 2.6 MB (2611155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbee0262fb10c6ee826cdf9ad391574e205886b3ecbe48df9d7faefc8631395`  
		Last Modified: Fri, 12 Nov 2021 21:47:46 GMT  
		Size: 10.0 MB (9982759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d313f2224226336843ad5b4eed2dc03c80a76d54cb049248fa3ce29f7b17f6fe`  
		Last Modified: Fri, 12 Nov 2021 21:47:44 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e0e764314fb955762494927c095f9cc4118e7b8a19b75971a7202a131ebdc4`  
		Last Modified: Fri, 12 Nov 2021 21:47:45 GMT  
		Size: 6.3 MB (6266946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2.3`

```console
$ docker pull irssi@sha256:eabe9a654c437d1055782b8fd8a2ff73fd3f2254a9549914cba6215fa321dc67
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
$ docker pull irssi@sha256:e959721514032b8e73f930e42ef95a7b1908148e563aee4eda55c80e3113f236
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50615098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28696f30fb5f7f5f5582364cae89ac875de7c473e676dfc8f80df20886029e2a`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:28:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:28:56 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 02:28:57 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 02:28:57 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 02:28:57 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 02:30:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 02:30:02 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 02:30:03 GMT
USER user
# Tue, 21 Dec 2021 02:30:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59be89c444cb2d9ace3b84fc5c5762d43da553450735ff834500ef787752fe6`  
		Last Modified: Tue, 21 Dec 2021 02:30:24 GMT  
		Size: 17.0 MB (17023696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416b353fa94267ed4404524f3572e09a455d86006dd420743d6b4ff16c94cdcd`  
		Last Modified: Tue, 21 Dec 2021 02:30:20 GMT  
		Size: 4.2 KB (4206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd3a6792e918c8d1e966ac97d2b00cd8b94b23ded6762536c890d459079ac9b`  
		Last Modified: Tue, 21 Dec 2021 02:30:21 GMT  
		Size: 6.4 MB (6433473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; arm variant v5

```console
$ docker pull irssi@sha256:27ad09505b4c6d369dfff267a263c9644582ddb3300e2b92d99b3d881ee91dc2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46877720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b2f7fd8bcc1ff3dc6bc7b848d4158846f575718a4314a85a49cce74f8b9bf2d`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 01:51:32 GMT
ADD file:f757929225218280f26d0eca53387788343e93cc9658f5baeb58957776114579 in / 
# Tue, 21 Dec 2021 01:51:33 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:32:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:32:04 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 03:32:06 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 03:32:07 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:32:07 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 03:34:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 03:34:08 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 03:34:09 GMT
USER user
# Tue, 21 Dec 2021 03:34:09 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:7d69cd3acec6d9e5ca88bdd718b069a7272b722048f49b6d21fbe85fc6c82560`  
		Last Modified: Tue, 21 Dec 2021 02:07:21 GMT  
		Size: 24.9 MB (24886253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9972abbb34ae72d3b0070f65b0ce5d55ab8380dd8a5b296110f26f4c1e4c8739`  
		Last Modified: Tue, 21 Dec 2021 03:34:59 GMT  
		Size: 15.9 MB (15922774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11e8b11f795a11c52cb86064bfcf17c440413738a87072860c0459aa457734e`  
		Last Modified: Tue, 21 Dec 2021 03:34:42 GMT  
		Size: 4.2 KB (4198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70f23a6e04f65c37ab26f520582f612442f447852daeb23349c80ec42b30552`  
		Last Modified: Tue, 21 Dec 2021 03:34:46 GMT  
		Size: 6.1 MB (6064495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; arm variant v7

```console
$ docker pull irssi@sha256:4a19c10049a9e3a6a6f2a6b48f17ed5cf6a9eeffdac2084f2a1e3bb2454b14ba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44274081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05f35d7af06a94f17bb1a15631d0a2cf2b7b2470c13c789d5cc4318e4ce4afd1`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:52 GMT
ADD file:1381e18e2847f24ebd16d8e83ad940adeff45aca2c327d4e07d7451816f29420 in / 
# Tue, 21 Dec 2021 02:00:52 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:21:25 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 07:21:27 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 07:21:28 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 07:21:28 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 07:23:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 07:23:17 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 07:23:17 GMT
USER user
# Tue, 21 Dec 2021 07:23:18 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b597e1a6bc27aa2a24a587cb687c9551dfbcfa730a11d48c5a44ff77ff6fdd75`  
		Last Modified: Tue, 21 Dec 2021 02:16:50 GMT  
		Size: 22.8 MB (22754324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338c7f0212075503206eaa4c6bcfae4b0b7c9c0aae5b57377ed3148c5e84491d`  
		Last Modified: Tue, 21 Dec 2021 07:24:41 GMT  
		Size: 15.6 MB (15583032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf715040fb97757cdd867af3ca6d76d851b0745b5e558aa78a93c8bd45e9892`  
		Last Modified: Tue, 21 Dec 2021 07:24:25 GMT  
		Size: 4.2 KB (4192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0dae9b7e84b9a5d9aacb48828f3eed3a1e422e5d7b3ba85cd0c83b1f8fcec70`  
		Last Modified: Tue, 21 Dec 2021 07:24:29 GMT  
		Size: 5.9 MB (5932533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:60457f603545fcd1f5dec369b7188e9fdf72344e5ae315294459bd17f5deb454
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48899497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfa76b323be41cbaca5865013d170ba2315088f61d4fa21f9ce40c9580d29828`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 10:18:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 10:18:09 GMT
ENV HOME=/home/user
# Thu, 02 Dec 2021 10:18:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 02 Dec 2021 10:18:11 GMT
ENV LANG=C.UTF-8
# Thu, 02 Dec 2021 10:18:12 GMT
ENV IRSSI_VERSION=1.2.3
# Thu, 02 Dec 2021 10:18:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 02 Dec 2021 10:18:53 GMT
WORKDIR /home/user
# Thu, 02 Dec 2021 10:18:54 GMT
USER user
# Thu, 02 Dec 2021 10:18:55 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd767de3273672ff5b8b0dbc5e7946d73f8a48def2a475e0aeba3663abd64f51`  
		Last Modified: Thu, 02 Dec 2021 10:19:36 GMT  
		Size: 16.8 MB (16796286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7292819705b5179aa616a780be2baa620f3ee6875935bf179183753616b6f349`  
		Last Modified: Thu, 02 Dec 2021 10:19:33 GMT  
		Size: 4.1 KB (4071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d72ba2e26eefead289f206dc9f257d1a52db264eb062b40fb6303214a47df`  
		Last Modified: Thu, 02 Dec 2021 10:19:34 GMT  
		Size: 6.2 MB (6175996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; 386

```console
$ docker pull irssi@sha256:d3ca7f90d7175158499ce79b153f9e6491202d0350e781fffff0cdb3b4323ccc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50461376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27404c72d886d49efaab162f5322fdd7bab66e3e2639d274745a61ecce8258ea`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:45 GMT
ADD file:78342a77df22ca22804ea5aec6415ce10c1fdc35687f1b25c5f86850f41d3905 in / 
# Tue, 21 Dec 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:41:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:41:06 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 07:41:07 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 07:41:08 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 07:41:08 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 07:42:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 07:42:35 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 07:42:35 GMT
USER user
# Tue, 21 Dec 2021 07:42:35 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:16e3a221bce3a5f7f4a71f72926f381ff9c6141ccb5918b7ea924ff7f7f09d06`  
		Last Modified: Tue, 21 Dec 2021 01:49:46 GMT  
		Size: 27.8 MB (27804573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdb20cfd72adfabb1343532d94fa58046b2e715c114de2bb2d495ebeece2682`  
		Last Modified: Tue, 21 Dec 2021 07:43:36 GMT  
		Size: 16.5 MB (16547064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b5781734632e07624e3572ae1a80fd1bdacd055a3bd11c4ce849401446c677`  
		Last Modified: Tue, 21 Dec 2021 07:43:29 GMT  
		Size: 4.2 KB (4198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b8a3e21b6c0511f13ead53720a5597649f9f96d918e32816c7c7674ba4972b`  
		Last Modified: Tue, 21 Dec 2021 07:43:32 GMT  
		Size: 6.1 MB (6105541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; mips64le

```console
$ docker pull irssi@sha256:afed46d618a02883850d985cfc57351066756ac4be967e25c0c2b45b93307c71
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47815170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d18fc013099ba02ad5eef9adde31927330aa957623529cf16ede04b3ea37087`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 02:09:59 GMT
ADD file:1e736cd218a1aa1d9d52dfb824407b84a8d10720ee840b3d81cdf74df62b74b8 in / 
# Tue, 21 Dec 2021 02:10:00 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:51:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:51:49 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 03:51:51 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 03:51:51 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:51:51 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 03:54:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 03:54:23 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 03:54:24 GMT
USER user
# Tue, 21 Dec 2021 03:54:24 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4425ebd1b1a185b87251c0eb43ab9b16b24ec96090a67323f44e2365b8f9bc19`  
		Last Modified: Tue, 21 Dec 2021 02:19:49 GMT  
		Size: 25.8 MB (25820202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85cbf48de6d54494842b75c145a74d8f799e352a563f58a8b164546fd9815dd`  
		Last Modified: Tue, 21 Dec 2021 03:55:05 GMT  
		Size: 15.7 MB (15698102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e524d04d8239c5b2e5bf926abdd70e466e556364301e359b5667f14b961b63`  
		Last Modified: Tue, 21 Dec 2021 03:54:50 GMT  
		Size: 4.2 KB (4179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7359d2585748ca1c9bc41d663fe7a39c7c91976a72362c271b7459f3177b1b07`  
		Last Modified: Tue, 21 Dec 2021 03:54:54 GMT  
		Size: 6.3 MB (6292687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; ppc64le

```console
$ docker pull irssi@sha256:ababf449214d8594cf18a462f9a08d25102f9aa24c06f45cc230056441d48550
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54779424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a153eea02c8c045e1f776a30ce44b81a10652c78d8144e18e07fba9d364e92d`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 02:21:09 GMT
ADD file:85a8af105e3fa794598824266068cbb3c0dc66067e10e3263dab26a230458a82 in / 
# Tue, 21 Dec 2021 02:21:13 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 05:20:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 05:20:04 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 05:20:09 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 05:20:11 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 05:20:12 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 05:23:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 05:23:06 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 05:23:07 GMT
USER user
# Tue, 21 Dec 2021 05:23:08 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:e2c79f8e0929abda2022fed71e090d3c34c8c3fdfb2a513ede1d117020a46821`  
		Last Modified: Tue, 21 Dec 2021 02:30:19 GMT  
		Size: 30.6 MB (30562311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec64c0808b37b40ecbae401a09f525b3599c4933104d9f91c1b02f531261f4e4`  
		Last Modified: Tue, 21 Dec 2021 05:23:52 GMT  
		Size: 17.4 MB (17430519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271fe3dcc65a9b19c4341ced9310438adb824c08206ea6944e756081de79e466`  
		Last Modified: Tue, 21 Dec 2021 05:23:47 GMT  
		Size: 4.2 KB (4219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304933c35b9311c11cc8edccb32e806769ecfb2944b2388f8a07da23ffeca40b`  
		Last Modified: Tue, 21 Dec 2021 05:23:49 GMT  
		Size: 6.8 MB (6782375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; s390x

```console
$ docker pull irssi@sha256:bb09bd5c28f1f789db24dfa8fd41a1d6e641e66e04a3596381232aecbd1f3e91
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49057908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcb7eecb8644b9881365cf635f37d162033bff573786804e8b703f3ce8846c69`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:57 GMT
ADD file:33e37861eefa46f6e5f7f4967ce8ae3167e28bc817c3c71ff90a3d51e2376a0f in / 
# Tue, 21 Dec 2021 01:42:59 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:09:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:09:35 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 03:09:36 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 03:09:36 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:09:36 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 03:10:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 03:10:11 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 03:10:11 GMT
USER user
# Tue, 21 Dec 2021 03:10:12 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:10979941d091693f28e3dc033cc6ca88996acf42a0aace27ad85fbd894945e20`  
		Last Modified: Tue, 21 Dec 2021 01:48:51 GMT  
		Size: 25.8 MB (25769051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b63d4cfd4aa344eea05406bab43c94faa838c6ead77d009d598529af4daa60a`  
		Last Modified: Tue, 21 Dec 2021 03:10:50 GMT  
		Size: 16.9 MB (16899907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a0decb3e6de2f0b3f7995b35b377ce3394134e98d44f3f8038a6db18883faf`  
		Last Modified: Tue, 21 Dec 2021 03:10:45 GMT  
		Size: 4.2 KB (4211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875d816cdaed07c7b756014dc420c87bd1991d3b3c8d3380d90c2bf738d50e88`  
		Last Modified: Tue, 21 Dec 2021 03:10:46 GMT  
		Size: 6.4 MB (6384739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2.3-alpine`

```console
$ docker pull irssi@sha256:b6199cce4bbccd62cdf2ab15c4e36f381babd27c1f693bb96ea99c20a6c9a9ef
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
$ docker pull irssi@sha256:a7f12f792fd4bf788c131dfa714df982d08d040cb5f0cc002e43e6e2b6675fb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18651944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:064295e6180eddccae4c53bfa3ccc4198baf64035be43d045aea0053df5b5ab2`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:21:09 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 13 Nov 2021 06:21:09 GMT
ENV HOME=/home/user
# Sat, 13 Nov 2021 06:21:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 13 Nov 2021 06:21:10 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 06:21:10 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 13 Nov 2021 06:22:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 13 Nov 2021 06:22:07 GMT
WORKDIR /home/user
# Sat, 13 Nov 2021 06:22:07 GMT
USER user
# Sat, 13 Nov 2021 06:22:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce5baac574d8b4271c82fa64dcdd49fa857685442591bb2a9088f4a17aa326d`  
		Last Modified: Sat, 13 Nov 2021 06:22:31 GMT  
		Size: 9.5 MB (9546893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6a10ef4b17c6ffd971ee996f3f9f1f835f466b8f8bf05e5f6d7b8e11bdf3e0`  
		Last Modified: Sat, 13 Nov 2021 06:22:28 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd14ec244a7d85641c549e5c3e926f9619beb3ef04c2de1296ef5d278268ef54`  
		Last Modified: Sat, 13 Nov 2021 06:22:30 GMT  
		Size: 6.3 MB (6281356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:411622af3811853615c7098dfa1b54089cbfd39ee2b84ad609555f5667f92b82
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17394658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da6d2fa6232e825db829628177a338984e9d93065e36f18f273ddbbbf1230bba`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 03:07:25 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 13 Nov 2021 03:07:26 GMT
ENV HOME=/home/user
# Sat, 13 Nov 2021 03:07:27 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 13 Nov 2021 03:07:28 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 03:07:28 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 13 Nov 2021 03:08:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 13 Nov 2021 03:08:38 GMT
WORKDIR /home/user
# Sat, 13 Nov 2021 03:08:38 GMT
USER user
# Sat, 13 Nov 2021 03:08:38 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e18644b7db2c0521d7b46f9a0ad2bbef1e78c4441a4eb4edd2e471d076617e`  
		Last Modified: Sat, 13 Nov 2021 03:09:18 GMT  
		Size: 8.8 MB (8777945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47719028b3d12f241ef81a872a66d640d50374d5c7b7ada4dea7a5d4f8d628b9`  
		Last Modified: Sat, 13 Nov 2021 03:09:12 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71524eae839c07718e925705fc282eabdc5f7bdf00917807520a46cd4952a20`  
		Last Modified: Sat, 13 Nov 2021 03:09:16 GMT  
		Size: 6.0 MB (5982098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:39fd318eba9bfe402c70dbb1658cc83d2008473a2bf7c6640ffcbf0f4cab5410
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16843546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80cf593f5cd7256f7f600c886f639c64a7fef945a7476ac8f235f315f2834f7f`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:54 GMT
ADD file:a13993855beba2267575c54a0c6707ddda85d238e697a81046a8b1c1a34df054 in / 
# Fri, 12 Nov 2021 16:57:54 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 10:53:57 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 13 Nov 2021 10:53:58 GMT
ENV HOME=/home/user
# Sat, 13 Nov 2021 10:54:01 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 13 Nov 2021 10:54:02 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 10:54:02 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 13 Nov 2021 10:55:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 13 Nov 2021 10:55:27 GMT
WORKDIR /home/user
# Sat, 13 Nov 2021 10:55:27 GMT
USER user
# Sat, 13 Nov 2021 10:55:28 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:767c1b67bc22761376676021ea5a310e7a7d1344b7a017bb8ede1a202340dbaf`  
		Last Modified: Fri, 12 Nov 2021 16:59:54 GMT  
		Size: 2.4 MB (2436506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf65fbf3cfd284ebb1b6bcbb3f5aeb9c90f25a8ef76be7e8626b4de4cbc9d12f`  
		Last Modified: Sat, 13 Nov 2021 10:56:37 GMT  
		Size: 8.6 MB (8630841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb323d0bda53eaa67141782bb2c816d1ee006b00a1834b70ab92d64c7bf823ed`  
		Last Modified: Sat, 13 Nov 2021 10:56:32 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d23d9d27bff57b2dbc2a08da74408f29dc954f150b5886a7e982dbfa160800`  
		Last Modified: Sat, 13 Nov 2021 10:56:35 GMT  
		Size: 5.8 MB (5774928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:237a3fb28d0d750071b6920a2ccc32afab7b574fc1a31deb71006cc8820b50de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18493717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43e7f354df530cf5903915bf52cff862c5931681cd9d85b24b826e77a9a3998f`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:27:36 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 13 Nov 2021 06:27:37 GMT
ENV HOME=/home/user
# Sat, 13 Nov 2021 06:27:38 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 13 Nov 2021 06:27:39 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 06:27:40 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 13 Nov 2021 06:28:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 13 Nov 2021 06:28:27 GMT
WORKDIR /home/user
# Sat, 13 Nov 2021 06:28:28 GMT
USER user
# Sat, 13 Nov 2021 06:28:29 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e152f8af96423f066d9e00e70b1fbbc96e94dbf4c98f075c6b7117135d97be4b`  
		Last Modified: Sat, 13 Nov 2021 06:29:25 GMT  
		Size: 9.5 MB (9543545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6065fe2276d0eabc118421590a0496be4176b2ecb15421a8798cfd55ea4ff0eb`  
		Last Modified: Sat, 13 Nov 2021 06:29:23 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39cb7b7de97a12a3eb299292e27a79d7e76bb96fd8eef37dc3d046620f92fb67`  
		Last Modified: Sat, 13 Nov 2021 06:29:24 GMT  
		Size: 6.2 MB (6229287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; 386

```console
$ docker pull irssi@sha256:e1533792e9821046cba4fd97ad160b36c6943d86078fde47a356e79b1184755a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17711979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1216a4299c56d5ac15112c6e1df985afef515bf2dbaeaa74ac5b8479b4080fbf`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 04:44:05 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 13 Nov 2021 04:44:06 GMT
ENV HOME=/home/user
# Sat, 13 Nov 2021 04:44:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 13 Nov 2021 04:44:07 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 04:44:07 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 13 Nov 2021 04:45:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 13 Nov 2021 04:45:13 GMT
WORKDIR /home/user
# Sat, 13 Nov 2021 04:45:13 GMT
USER user
# Sat, 13 Nov 2021 04:45:13 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fb5374975ca920199ffda46b9a54fba11dd5eda1e231d1586fd28b00bfab55`  
		Last Modified: Sat, 13 Nov 2021 04:45:58 GMT  
		Size: 8.9 MB (8914326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bda351aa4adae26d595a83d58109f6b9e63f43b0ef135c5c65ae3d27207425`  
		Last Modified: Sat, 13 Nov 2021 04:45:53 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19698f734fdb7985e49d87a08629d95fecae4a127bcb935a6cb36b5e2f1eed82`  
		Last Modified: Sat, 13 Nov 2021 04:45:56 GMT  
		Size: 6.0 MB (5967572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:e563662cc89c1019d39f0eda3f4457bdc094c27f61a77384ef8358537bda818c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18946306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66dc37eef2bb5aa0607437ea97b4d616b4956415415daf2ed8dc11105d08efb9`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:25 GMT
ADD file:f7216323de17450e653f77c86d2c1e2e8ec01e1133e93f29c515761b3e9d8f7d in / 
# Fri, 12 Nov 2021 21:18:28 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:17:21 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 13 Nov 2021 15:17:25 GMT
ENV HOME=/home/user
# Sat, 13 Nov 2021 15:17:37 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 13 Nov 2021 15:17:39 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 15:17:41 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 13 Nov 2021 15:18:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 13 Nov 2021 15:18:45 GMT
WORKDIR /home/user
# Sat, 13 Nov 2021 15:18:49 GMT
USER user
# Sat, 13 Nov 2021 15:19:01 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6729720a3e6b58511df148134bb67d786ad90f9fce1c02ba5bbfd31f33055fbe`  
		Last Modified: Fri, 12 Nov 2021 21:19:49 GMT  
		Size: 2.8 MB (2820517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5c3bca0019540f7fc24b101be6d560cac83a81f1b6cda2b2fd1dcb4400c6e7`  
		Last Modified: Sat, 13 Nov 2021 15:19:52 GMT  
		Size: 9.6 MB (9642236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2dbb74b4ba4c2dc34b3813acf99e0b991bcdb045c4404168d74feb0a7d550f8`  
		Last Modified: Sat, 13 Nov 2021 15:19:50 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa5a61caf2a0e156b37a62805b3fdcfab0ec5484229e4df282556b21c89b49e`  
		Last Modified: Sat, 13 Nov 2021 15:19:51 GMT  
		Size: 6.5 MB (6482283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:4508d5ff1fb06c6ca41ad14725242a83a585019ba2c7523518098e9662766edf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18862132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aed48119bc23818d5a430a4e15912061316a5a404add032ef2b41ae01f4c0b7d`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:44 GMT
ADD file:637f327c9b07758709ef7dbc42eb472c888d221acde89b1c3775553864334d5c in / 
# Fri, 12 Nov 2021 16:41:44 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:46:37 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 12 Nov 2021 21:46:38 GMT
ENV HOME=/home/user
# Fri, 12 Nov 2021 21:46:38 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Nov 2021 21:46:39 GMT
ENV LANG=C.UTF-8
# Fri, 12 Nov 2021 21:46:39 GMT
ENV IRSSI_VERSION=1.2.3
# Fri, 12 Nov 2021 21:47:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 12 Nov 2021 21:47:14 GMT
WORKDIR /home/user
# Fri, 12 Nov 2021 21:47:14 GMT
USER user
# Fri, 12 Nov 2021 21:47:14 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b872f056719bde6e6722091afb2a3376d720c69c142b91ac352050080dd79615`  
		Last Modified: Fri, 12 Nov 2021 16:42:54 GMT  
		Size: 2.6 MB (2611155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbee0262fb10c6ee826cdf9ad391574e205886b3ecbe48df9d7faefc8631395`  
		Last Modified: Fri, 12 Nov 2021 21:47:46 GMT  
		Size: 10.0 MB (9982759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d313f2224226336843ad5b4eed2dc03c80a76d54cb049248fa3ce29f7b17f6fe`  
		Last Modified: Fri, 12 Nov 2021 21:47:44 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e0e764314fb955762494927c095f9cc4118e7b8a19b75971a7202a131ebdc4`  
		Last Modified: Fri, 12 Nov 2021 21:47:45 GMT  
		Size: 6.3 MB (6266946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:alpine`

```console
$ docker pull irssi@sha256:b6199cce4bbccd62cdf2ab15c4e36f381babd27c1f693bb96ea99c20a6c9a9ef
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
$ docker pull irssi@sha256:a7f12f792fd4bf788c131dfa714df982d08d040cb5f0cc002e43e6e2b6675fb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18651944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:064295e6180eddccae4c53bfa3ccc4198baf64035be43d045aea0053df5b5ab2`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:21:09 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 13 Nov 2021 06:21:09 GMT
ENV HOME=/home/user
# Sat, 13 Nov 2021 06:21:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 13 Nov 2021 06:21:10 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 06:21:10 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 13 Nov 2021 06:22:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 13 Nov 2021 06:22:07 GMT
WORKDIR /home/user
# Sat, 13 Nov 2021 06:22:07 GMT
USER user
# Sat, 13 Nov 2021 06:22:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce5baac574d8b4271c82fa64dcdd49fa857685442591bb2a9088f4a17aa326d`  
		Last Modified: Sat, 13 Nov 2021 06:22:31 GMT  
		Size: 9.5 MB (9546893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6a10ef4b17c6ffd971ee996f3f9f1f835f466b8f8bf05e5f6d7b8e11bdf3e0`  
		Last Modified: Sat, 13 Nov 2021 06:22:28 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd14ec244a7d85641c549e5c3e926f9619beb3ef04c2de1296ef5d278268ef54`  
		Last Modified: Sat, 13 Nov 2021 06:22:30 GMT  
		Size: 6.3 MB (6281356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:411622af3811853615c7098dfa1b54089cbfd39ee2b84ad609555f5667f92b82
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17394658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da6d2fa6232e825db829628177a338984e9d93065e36f18f273ddbbbf1230bba`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 03:07:25 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 13 Nov 2021 03:07:26 GMT
ENV HOME=/home/user
# Sat, 13 Nov 2021 03:07:27 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 13 Nov 2021 03:07:28 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 03:07:28 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 13 Nov 2021 03:08:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 13 Nov 2021 03:08:38 GMT
WORKDIR /home/user
# Sat, 13 Nov 2021 03:08:38 GMT
USER user
# Sat, 13 Nov 2021 03:08:38 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e18644b7db2c0521d7b46f9a0ad2bbef1e78c4441a4eb4edd2e471d076617e`  
		Last Modified: Sat, 13 Nov 2021 03:09:18 GMT  
		Size: 8.8 MB (8777945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47719028b3d12f241ef81a872a66d640d50374d5c7b7ada4dea7a5d4f8d628b9`  
		Last Modified: Sat, 13 Nov 2021 03:09:12 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71524eae839c07718e925705fc282eabdc5f7bdf00917807520a46cd4952a20`  
		Last Modified: Sat, 13 Nov 2021 03:09:16 GMT  
		Size: 6.0 MB (5982098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:39fd318eba9bfe402c70dbb1658cc83d2008473a2bf7c6640ffcbf0f4cab5410
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16843546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80cf593f5cd7256f7f600c886f639c64a7fef945a7476ac8f235f315f2834f7f`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:54 GMT
ADD file:a13993855beba2267575c54a0c6707ddda85d238e697a81046a8b1c1a34df054 in / 
# Fri, 12 Nov 2021 16:57:54 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 10:53:57 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 13 Nov 2021 10:53:58 GMT
ENV HOME=/home/user
# Sat, 13 Nov 2021 10:54:01 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 13 Nov 2021 10:54:02 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 10:54:02 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 13 Nov 2021 10:55:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 13 Nov 2021 10:55:27 GMT
WORKDIR /home/user
# Sat, 13 Nov 2021 10:55:27 GMT
USER user
# Sat, 13 Nov 2021 10:55:28 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:767c1b67bc22761376676021ea5a310e7a7d1344b7a017bb8ede1a202340dbaf`  
		Last Modified: Fri, 12 Nov 2021 16:59:54 GMT  
		Size: 2.4 MB (2436506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf65fbf3cfd284ebb1b6bcbb3f5aeb9c90f25a8ef76be7e8626b4de4cbc9d12f`  
		Last Modified: Sat, 13 Nov 2021 10:56:37 GMT  
		Size: 8.6 MB (8630841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb323d0bda53eaa67141782bb2c816d1ee006b00a1834b70ab92d64c7bf823ed`  
		Last Modified: Sat, 13 Nov 2021 10:56:32 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d23d9d27bff57b2dbc2a08da74408f29dc954f150b5886a7e982dbfa160800`  
		Last Modified: Sat, 13 Nov 2021 10:56:35 GMT  
		Size: 5.8 MB (5774928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:237a3fb28d0d750071b6920a2ccc32afab7b574fc1a31deb71006cc8820b50de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18493717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43e7f354df530cf5903915bf52cff862c5931681cd9d85b24b826e77a9a3998f`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:27:36 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 13 Nov 2021 06:27:37 GMT
ENV HOME=/home/user
# Sat, 13 Nov 2021 06:27:38 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 13 Nov 2021 06:27:39 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 06:27:40 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 13 Nov 2021 06:28:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 13 Nov 2021 06:28:27 GMT
WORKDIR /home/user
# Sat, 13 Nov 2021 06:28:28 GMT
USER user
# Sat, 13 Nov 2021 06:28:29 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e152f8af96423f066d9e00e70b1fbbc96e94dbf4c98f075c6b7117135d97be4b`  
		Last Modified: Sat, 13 Nov 2021 06:29:25 GMT  
		Size: 9.5 MB (9543545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6065fe2276d0eabc118421590a0496be4176b2ecb15421a8798cfd55ea4ff0eb`  
		Last Modified: Sat, 13 Nov 2021 06:29:23 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39cb7b7de97a12a3eb299292e27a79d7e76bb96fd8eef37dc3d046620f92fb67`  
		Last Modified: Sat, 13 Nov 2021 06:29:24 GMT  
		Size: 6.2 MB (6229287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; 386

```console
$ docker pull irssi@sha256:e1533792e9821046cba4fd97ad160b36c6943d86078fde47a356e79b1184755a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17711979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1216a4299c56d5ac15112c6e1df985afef515bf2dbaeaa74ac5b8479b4080fbf`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 04:44:05 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 13 Nov 2021 04:44:06 GMT
ENV HOME=/home/user
# Sat, 13 Nov 2021 04:44:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 13 Nov 2021 04:44:07 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 04:44:07 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 13 Nov 2021 04:45:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 13 Nov 2021 04:45:13 GMT
WORKDIR /home/user
# Sat, 13 Nov 2021 04:45:13 GMT
USER user
# Sat, 13 Nov 2021 04:45:13 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fb5374975ca920199ffda46b9a54fba11dd5eda1e231d1586fd28b00bfab55`  
		Last Modified: Sat, 13 Nov 2021 04:45:58 GMT  
		Size: 8.9 MB (8914326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bda351aa4adae26d595a83d58109f6b9e63f43b0ef135c5c65ae3d27207425`  
		Last Modified: Sat, 13 Nov 2021 04:45:53 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19698f734fdb7985e49d87a08629d95fecae4a127bcb935a6cb36b5e2f1eed82`  
		Last Modified: Sat, 13 Nov 2021 04:45:56 GMT  
		Size: 6.0 MB (5967572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:e563662cc89c1019d39f0eda3f4457bdc094c27f61a77384ef8358537bda818c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18946306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66dc37eef2bb5aa0607437ea97b4d616b4956415415daf2ed8dc11105d08efb9`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:25 GMT
ADD file:f7216323de17450e653f77c86d2c1e2e8ec01e1133e93f29c515761b3e9d8f7d in / 
# Fri, 12 Nov 2021 21:18:28 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:17:21 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 13 Nov 2021 15:17:25 GMT
ENV HOME=/home/user
# Sat, 13 Nov 2021 15:17:37 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 13 Nov 2021 15:17:39 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 15:17:41 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 13 Nov 2021 15:18:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 13 Nov 2021 15:18:45 GMT
WORKDIR /home/user
# Sat, 13 Nov 2021 15:18:49 GMT
USER user
# Sat, 13 Nov 2021 15:19:01 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6729720a3e6b58511df148134bb67d786ad90f9fce1c02ba5bbfd31f33055fbe`  
		Last Modified: Fri, 12 Nov 2021 21:19:49 GMT  
		Size: 2.8 MB (2820517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5c3bca0019540f7fc24b101be6d560cac83a81f1b6cda2b2fd1dcb4400c6e7`  
		Last Modified: Sat, 13 Nov 2021 15:19:52 GMT  
		Size: 9.6 MB (9642236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2dbb74b4ba4c2dc34b3813acf99e0b991bcdb045c4404168d74feb0a7d550f8`  
		Last Modified: Sat, 13 Nov 2021 15:19:50 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa5a61caf2a0e156b37a62805b3fdcfab0ec5484229e4df282556b21c89b49e`  
		Last Modified: Sat, 13 Nov 2021 15:19:51 GMT  
		Size: 6.5 MB (6482283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; s390x

```console
$ docker pull irssi@sha256:4508d5ff1fb06c6ca41ad14725242a83a585019ba2c7523518098e9662766edf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18862132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aed48119bc23818d5a430a4e15912061316a5a404add032ef2b41ae01f4c0b7d`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:44 GMT
ADD file:637f327c9b07758709ef7dbc42eb472c888d221acde89b1c3775553864334d5c in / 
# Fri, 12 Nov 2021 16:41:44 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:46:37 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 12 Nov 2021 21:46:38 GMT
ENV HOME=/home/user
# Fri, 12 Nov 2021 21:46:38 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Nov 2021 21:46:39 GMT
ENV LANG=C.UTF-8
# Fri, 12 Nov 2021 21:46:39 GMT
ENV IRSSI_VERSION=1.2.3
# Fri, 12 Nov 2021 21:47:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 12 Nov 2021 21:47:14 GMT
WORKDIR /home/user
# Fri, 12 Nov 2021 21:47:14 GMT
USER user
# Fri, 12 Nov 2021 21:47:14 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b872f056719bde6e6722091afb2a3376d720c69c142b91ac352050080dd79615`  
		Last Modified: Fri, 12 Nov 2021 16:42:54 GMT  
		Size: 2.6 MB (2611155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbee0262fb10c6ee826cdf9ad391574e205886b3ecbe48df9d7faefc8631395`  
		Last Modified: Fri, 12 Nov 2021 21:47:46 GMT  
		Size: 10.0 MB (9982759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d313f2224226336843ad5b4eed2dc03c80a76d54cb049248fa3ce29f7b17f6fe`  
		Last Modified: Fri, 12 Nov 2021 21:47:44 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e0e764314fb955762494927c095f9cc4118e7b8a19b75971a7202a131ebdc4`  
		Last Modified: Fri, 12 Nov 2021 21:47:45 GMT  
		Size: 6.3 MB (6266946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:latest`

```console
$ docker pull irssi@sha256:eabe9a654c437d1055782b8fd8a2ff73fd3f2254a9549914cba6215fa321dc67
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
$ docker pull irssi@sha256:e959721514032b8e73f930e42ef95a7b1908148e563aee4eda55c80e3113f236
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50615098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28696f30fb5f7f5f5582364cae89ac875de7c473e676dfc8f80df20886029e2a`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:28:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:28:56 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 02:28:57 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 02:28:57 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 02:28:57 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 02:30:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 02:30:02 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 02:30:03 GMT
USER user
# Tue, 21 Dec 2021 02:30:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59be89c444cb2d9ace3b84fc5c5762d43da553450735ff834500ef787752fe6`  
		Last Modified: Tue, 21 Dec 2021 02:30:24 GMT  
		Size: 17.0 MB (17023696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416b353fa94267ed4404524f3572e09a455d86006dd420743d6b4ff16c94cdcd`  
		Last Modified: Tue, 21 Dec 2021 02:30:20 GMT  
		Size: 4.2 KB (4206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd3a6792e918c8d1e966ac97d2b00cd8b94b23ded6762536c890d459079ac9b`  
		Last Modified: Tue, 21 Dec 2021 02:30:21 GMT  
		Size: 6.4 MB (6433473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm variant v5

```console
$ docker pull irssi@sha256:27ad09505b4c6d369dfff267a263c9644582ddb3300e2b92d99b3d881ee91dc2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46877720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b2f7fd8bcc1ff3dc6bc7b848d4158846f575718a4314a85a49cce74f8b9bf2d`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 01:51:32 GMT
ADD file:f757929225218280f26d0eca53387788343e93cc9658f5baeb58957776114579 in / 
# Tue, 21 Dec 2021 01:51:33 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:32:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:32:04 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 03:32:06 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 03:32:07 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:32:07 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 03:34:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 03:34:08 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 03:34:09 GMT
USER user
# Tue, 21 Dec 2021 03:34:09 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:7d69cd3acec6d9e5ca88bdd718b069a7272b722048f49b6d21fbe85fc6c82560`  
		Last Modified: Tue, 21 Dec 2021 02:07:21 GMT  
		Size: 24.9 MB (24886253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9972abbb34ae72d3b0070f65b0ce5d55ab8380dd8a5b296110f26f4c1e4c8739`  
		Last Modified: Tue, 21 Dec 2021 03:34:59 GMT  
		Size: 15.9 MB (15922774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11e8b11f795a11c52cb86064bfcf17c440413738a87072860c0459aa457734e`  
		Last Modified: Tue, 21 Dec 2021 03:34:42 GMT  
		Size: 4.2 KB (4198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70f23a6e04f65c37ab26f520582f612442f447852daeb23349c80ec42b30552`  
		Last Modified: Tue, 21 Dec 2021 03:34:46 GMT  
		Size: 6.1 MB (6064495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm variant v7

```console
$ docker pull irssi@sha256:4a19c10049a9e3a6a6f2a6b48f17ed5cf6a9eeffdac2084f2a1e3bb2454b14ba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44274081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05f35d7af06a94f17bb1a15631d0a2cf2b7b2470c13c789d5cc4318e4ce4afd1`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:52 GMT
ADD file:1381e18e2847f24ebd16d8e83ad940adeff45aca2c327d4e07d7451816f29420 in / 
# Tue, 21 Dec 2021 02:00:52 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:21:25 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 07:21:27 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 07:21:28 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 07:21:28 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 07:23:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 07:23:17 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 07:23:17 GMT
USER user
# Tue, 21 Dec 2021 07:23:18 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b597e1a6bc27aa2a24a587cb687c9551dfbcfa730a11d48c5a44ff77ff6fdd75`  
		Last Modified: Tue, 21 Dec 2021 02:16:50 GMT  
		Size: 22.8 MB (22754324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338c7f0212075503206eaa4c6bcfae4b0b7c9c0aae5b57377ed3148c5e84491d`  
		Last Modified: Tue, 21 Dec 2021 07:24:41 GMT  
		Size: 15.6 MB (15583032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf715040fb97757cdd867af3ca6d76d851b0745b5e558aa78a93c8bd45e9892`  
		Last Modified: Tue, 21 Dec 2021 07:24:25 GMT  
		Size: 4.2 KB (4192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0dae9b7e84b9a5d9aacb48828f3eed3a1e422e5d7b3ba85cd0c83b1f8fcec70`  
		Last Modified: Tue, 21 Dec 2021 07:24:29 GMT  
		Size: 5.9 MB (5932533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:60457f603545fcd1f5dec369b7188e9fdf72344e5ae315294459bd17f5deb454
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48899497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfa76b323be41cbaca5865013d170ba2315088f61d4fa21f9ce40c9580d29828`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 10:18:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 10:18:09 GMT
ENV HOME=/home/user
# Thu, 02 Dec 2021 10:18:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 02 Dec 2021 10:18:11 GMT
ENV LANG=C.UTF-8
# Thu, 02 Dec 2021 10:18:12 GMT
ENV IRSSI_VERSION=1.2.3
# Thu, 02 Dec 2021 10:18:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 02 Dec 2021 10:18:53 GMT
WORKDIR /home/user
# Thu, 02 Dec 2021 10:18:54 GMT
USER user
# Thu, 02 Dec 2021 10:18:55 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd767de3273672ff5b8b0dbc5e7946d73f8a48def2a475e0aeba3663abd64f51`  
		Last Modified: Thu, 02 Dec 2021 10:19:36 GMT  
		Size: 16.8 MB (16796286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7292819705b5179aa616a780be2baa620f3ee6875935bf179183753616b6f349`  
		Last Modified: Thu, 02 Dec 2021 10:19:33 GMT  
		Size: 4.1 KB (4071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d72ba2e26eefead289f206dc9f257d1a52db264eb062b40fb6303214a47df`  
		Last Modified: Thu, 02 Dec 2021 10:19:34 GMT  
		Size: 6.2 MB (6175996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; 386

```console
$ docker pull irssi@sha256:d3ca7f90d7175158499ce79b153f9e6491202d0350e781fffff0cdb3b4323ccc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50461376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27404c72d886d49efaab162f5322fdd7bab66e3e2639d274745a61ecce8258ea`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:45 GMT
ADD file:78342a77df22ca22804ea5aec6415ce10c1fdc35687f1b25c5f86850f41d3905 in / 
# Tue, 21 Dec 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:41:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:41:06 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 07:41:07 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 07:41:08 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 07:41:08 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 07:42:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 07:42:35 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 07:42:35 GMT
USER user
# Tue, 21 Dec 2021 07:42:35 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:16e3a221bce3a5f7f4a71f72926f381ff9c6141ccb5918b7ea924ff7f7f09d06`  
		Last Modified: Tue, 21 Dec 2021 01:49:46 GMT  
		Size: 27.8 MB (27804573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdb20cfd72adfabb1343532d94fa58046b2e715c114de2bb2d495ebeece2682`  
		Last Modified: Tue, 21 Dec 2021 07:43:36 GMT  
		Size: 16.5 MB (16547064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b5781734632e07624e3572ae1a80fd1bdacd055a3bd11c4ce849401446c677`  
		Last Modified: Tue, 21 Dec 2021 07:43:29 GMT  
		Size: 4.2 KB (4198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b8a3e21b6c0511f13ead53720a5597649f9f96d918e32816c7c7674ba4972b`  
		Last Modified: Tue, 21 Dec 2021 07:43:32 GMT  
		Size: 6.1 MB (6105541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; mips64le

```console
$ docker pull irssi@sha256:afed46d618a02883850d985cfc57351066756ac4be967e25c0c2b45b93307c71
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47815170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d18fc013099ba02ad5eef9adde31927330aa957623529cf16ede04b3ea37087`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 02:09:59 GMT
ADD file:1e736cd218a1aa1d9d52dfb824407b84a8d10720ee840b3d81cdf74df62b74b8 in / 
# Tue, 21 Dec 2021 02:10:00 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:51:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:51:49 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 03:51:51 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 03:51:51 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:51:51 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 03:54:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 03:54:23 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 03:54:24 GMT
USER user
# Tue, 21 Dec 2021 03:54:24 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4425ebd1b1a185b87251c0eb43ab9b16b24ec96090a67323f44e2365b8f9bc19`  
		Last Modified: Tue, 21 Dec 2021 02:19:49 GMT  
		Size: 25.8 MB (25820202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85cbf48de6d54494842b75c145a74d8f799e352a563f58a8b164546fd9815dd`  
		Last Modified: Tue, 21 Dec 2021 03:55:05 GMT  
		Size: 15.7 MB (15698102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e524d04d8239c5b2e5bf926abdd70e466e556364301e359b5667f14b961b63`  
		Last Modified: Tue, 21 Dec 2021 03:54:50 GMT  
		Size: 4.2 KB (4179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7359d2585748ca1c9bc41d663fe7a39c7c91976a72362c271b7459f3177b1b07`  
		Last Modified: Tue, 21 Dec 2021 03:54:54 GMT  
		Size: 6.3 MB (6292687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; ppc64le

```console
$ docker pull irssi@sha256:ababf449214d8594cf18a462f9a08d25102f9aa24c06f45cc230056441d48550
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54779424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a153eea02c8c045e1f776a30ce44b81a10652c78d8144e18e07fba9d364e92d`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 02:21:09 GMT
ADD file:85a8af105e3fa794598824266068cbb3c0dc66067e10e3263dab26a230458a82 in / 
# Tue, 21 Dec 2021 02:21:13 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 05:20:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 05:20:04 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 05:20:09 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 05:20:11 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 05:20:12 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 05:23:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 05:23:06 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 05:23:07 GMT
USER user
# Tue, 21 Dec 2021 05:23:08 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:e2c79f8e0929abda2022fed71e090d3c34c8c3fdfb2a513ede1d117020a46821`  
		Last Modified: Tue, 21 Dec 2021 02:30:19 GMT  
		Size: 30.6 MB (30562311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec64c0808b37b40ecbae401a09f525b3599c4933104d9f91c1b02f531261f4e4`  
		Last Modified: Tue, 21 Dec 2021 05:23:52 GMT  
		Size: 17.4 MB (17430519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271fe3dcc65a9b19c4341ced9310438adb824c08206ea6944e756081de79e466`  
		Last Modified: Tue, 21 Dec 2021 05:23:47 GMT  
		Size: 4.2 KB (4219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304933c35b9311c11cc8edccb32e806769ecfb2944b2388f8a07da23ffeca40b`  
		Last Modified: Tue, 21 Dec 2021 05:23:49 GMT  
		Size: 6.8 MB (6782375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; s390x

```console
$ docker pull irssi@sha256:bb09bd5c28f1f789db24dfa8fd41a1d6e641e66e04a3596381232aecbd1f3e91
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49057908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcb7eecb8644b9881365cf635f37d162033bff573786804e8b703f3ce8846c69`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:57 GMT
ADD file:33e37861eefa46f6e5f7f4967ce8ae3167e28bc817c3c71ff90a3d51e2376a0f in / 
# Tue, 21 Dec 2021 01:42:59 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:09:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:09:35 GMT
ENV HOME=/home/user
# Tue, 21 Dec 2021 03:09:36 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 21 Dec 2021 03:09:36 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:09:36 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 21 Dec 2021 03:10:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 21 Dec 2021 03:10:11 GMT
WORKDIR /home/user
# Tue, 21 Dec 2021 03:10:11 GMT
USER user
# Tue, 21 Dec 2021 03:10:12 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:10979941d091693f28e3dc033cc6ca88996acf42a0aace27ad85fbd894945e20`  
		Last Modified: Tue, 21 Dec 2021 01:48:51 GMT  
		Size: 25.8 MB (25769051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b63d4cfd4aa344eea05406bab43c94faa838c6ead77d009d598529af4daa60a`  
		Last Modified: Tue, 21 Dec 2021 03:10:50 GMT  
		Size: 16.9 MB (16899907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a0decb3e6de2f0b3f7995b35b377ce3394134e98d44f3f8038a6db18883faf`  
		Last Modified: Tue, 21 Dec 2021 03:10:45 GMT  
		Size: 4.2 KB (4211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875d816cdaed07c7b756014dc420c87bd1991d3b3c8d3380d90c2bf738d50e88`  
		Last Modified: Tue, 21 Dec 2021 03:10:46 GMT  
		Size: 6.4 MB (6384739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
