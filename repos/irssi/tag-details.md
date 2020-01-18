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
$ docker pull irssi@sha256:10d70bb9912ee6af38e32c68e5147774527371b837d2e96c38496cbd89c460af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `irssi:1` - linux; amd64

```console
$ docker pull irssi@sha256:94ade928c56069ab24e07a671d461627157bfc4b4c75cddc7e0eef74dc429668
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50512777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:071f6fdb9d31c1fdb38e00b3f4aa5f35f0488bf3f0be7ec47c8609d9b77f7d82`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 22:19:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 22:19:55 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:19:55 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:19:56 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:19:56 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:20:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 22:20:56 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:20:56 GMT
USER user
# Mon, 30 Dec 2019 22:20:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155ffa1aba8607e36ef345d54c69e06dff0957646eb0a3ff4ea1f247f2d6f834`  
		Last Modified: Mon, 30 Dec 2019 22:22:11 GMT  
		Size: 17.0 MB (16987485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c035b099bd2ec74cb6afce844b250fd133eb9632293848ada2628bdbc84f1db`  
		Last Modified: Mon, 30 Dec 2019 22:22:06 GMT  
		Size: 4.2 KB (4181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32794dd5d2b6704bd7908f83a0bc9c91af102b15cb616927fc7c5aa4e1917f2`  
		Last Modified: Mon, 30 Dec 2019 22:22:08 GMT  
		Size: 6.4 MB (6428837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm variant v5

```console
$ docker pull irssi@sha256:0e2ffdb40c1813fcd5d664cd43f803e9fae16d23158c37a0a3a77ee6f9c6ea30
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46786540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2429596187b3420620bfa930a489829d17b7ae16f68a5e12f468600ead30f6b0`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:49:50 GMT
ADD file:5d34c769f80c3fdbb04048f4336cf212164934607a642144ef557faef5896192 in / 
# Sat, 28 Dec 2019 04:49:51 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 22:49:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 22:49:11 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:49:13 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:49:14 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:49:14 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:51:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 22:51:50 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:51:51 GMT
USER user
# Mon, 30 Dec 2019 22:51:53 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:153ccec980772b5fc4c786af0b26bba09f0a2d95d9755400febf9a79aa4220c8`  
		Last Modified: Sat, 28 Dec 2019 04:56:28 GMT  
		Size: 24.8 MB (24829618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa69714a630c9112cb8ed12a6a0c9ae434a0a7195c6e4f68933886f7fd1983f`  
		Last Modified: Mon, 30 Dec 2019 22:52:22 GMT  
		Size: 15.9 MB (15890061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab31781254acfc5b427e96a9157a02a9ba33029a2005b185eb5269c4163787d`  
		Last Modified: Mon, 30 Dec 2019 22:52:11 GMT  
		Size: 4.2 KB (4205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6924de57ca5fe0466f8a204c8e8f92726d55e29433871e0a91aba15f983c8c`  
		Last Modified: Mon, 30 Dec 2019 22:52:14 GMT  
		Size: 6.1 MB (6062656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm variant v7

```console
$ docker pull irssi@sha256:4ac9143ebda80df861793e06c1ab529a0c82cbc5fbb1467ad6f905a717d1242f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44188477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebc901e04efd19e1b84420fee3ddabfa2c5e0f65bf74941175283da2815154aa`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 23:02:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 23:02:55 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 23:02:57 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 23:02:58 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 23:02:58 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 23:04:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 23:04:30 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 23:04:31 GMT
USER user
# Mon, 30 Dec 2019 23:04:32 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09075676a7576165b8ed1990b233d29b4a112b50d5957c1a1c8cbf0c1853dc76`  
		Last Modified: Mon, 30 Dec 2019 23:06:11 GMT  
		Size: 15.6 MB (15554857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373ec572d9c27ba5c4b59943b257138a84a107907c938b6300b34503f7f2e602`  
		Last Modified: Mon, 30 Dec 2019 23:06:03 GMT  
		Size: 4.2 KB (4197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec006cec70b4f55bcb3b95111258702e778f90ad5362b4c08bc1b87f10b405e2`  
		Last Modified: Mon, 30 Dec 2019 23:06:05 GMT  
		Size: 5.9 MB (5930294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:52d0ead408e844bba3ea08864d9ee1ce400727f99711658a332c8ab953b41ae7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49005367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13e82aa16b7576863ef36d2b9ffce9df153f1aa8177e97e220143821458a55a7`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 22:41:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 22:41:08 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:41:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:41:10 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:41:11 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:42:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 22:42:54 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:42:56 GMT
USER user
# Mon, 30 Dec 2019 22:42:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc97913e2d0d8cb44f6fd5a47a49974057573a753cf66d3212046b6c376fd9f0`  
		Last Modified: Mon, 30 Dec 2019 22:44:30 GMT  
		Size: 16.8 MB (16762627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0709e009ad51ad0a0ec48f8c3c0b0de4fd412ad5b3b42e53757cec282180e87`  
		Last Modified: Mon, 30 Dec 2019 22:44:23 GMT  
		Size: 4.2 KB (4215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c555b242ddbe0e9335602cbdca56f5c307d560b4635c31338861407810b9945`  
		Last Modified: Mon, 30 Dec 2019 22:44:25 GMT  
		Size: 6.4 MB (6387823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; 386

```console
$ docker pull irssi@sha256:c5e4274b633a2d299ec9af52d580010154758ada9929bb758022334ac968820e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50367637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdbe22cc632c3d69ce50527e20598a64ea33d2dbffff7cdd42ccff0be736b6ac`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 22:38:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 22:38:37 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:38:38 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:38:38 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:38:38 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:39:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 22:39:57 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:39:57 GMT
USER user
# Mon, 30 Dec 2019 22:39:57 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72221f577a2f5220d3b7671a23bbf707e559dc20fd260e9e321a3bca8bf4e7fc`  
		Last Modified: Mon, 30 Dec 2019 22:41:20 GMT  
		Size: 16.5 MB (16515220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e488155fc2527b4ab798931fac3fa6f7521f5e687e0c82ea1cf007b495ea88`  
		Last Modified: Mon, 30 Dec 2019 22:41:14 GMT  
		Size: 4.2 KB (4170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07b243b29fe05690820a603d2c31463dbe08ca974efc99b033aca2703d9ac65`  
		Last Modified: Mon, 30 Dec 2019 22:41:16 GMT  
		Size: 6.1 MB (6101227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; ppc64le

```console
$ docker pull irssi@sha256:aabbe2ff8e02fa9376da9c3d21d0f747aee3e97fcf372951d07e85252732b28a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.7 MB (54698717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8c59fc543020e65db22f51fb7a5f22a0bdb0284f7a68619e2daeac2a6d27567`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 22:18:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 22:18:43 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:18:51 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:18:53 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:18:55 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:23:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 22:23:22 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:23:24 GMT
USER user
# Mon, 30 Dec 2019 22:23:26 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4a48662b243e889598e0a1b8e2a224407e08aa8c152a7b96352dc261c2b903`  
		Last Modified: Mon, 30 Dec 2019 22:25:36 GMT  
		Size: 17.4 MB (17396769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bd95038cb0e8d80e4cb33f7dbe1b0ae5c5b33f2f63955c2eafabeacead3d95`  
		Last Modified: Mon, 30 Dec 2019 22:25:30 GMT  
		Size: 4.2 KB (4219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d27ae35ac7ced8f7f75a99531f03b1e8e174a10f78c8c77acfc606ef3a1c40`  
		Last Modified: Mon, 30 Dec 2019 22:25:31 GMT  
		Size: 6.8 MB (6780200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; s390x

```console
$ docker pull irssi@sha256:b265d21e8baf744ec4ed0e1a75b3bb821b3b7cdc75cad870581f37a461d734a5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48951117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10fb4e99edc6f16e535536593259d9363aa1b59890a278a793360a6a601b02a9`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:42:03 GMT
ADD file:eec6c56f8680753860198c3af0d94aabb87018ca30f6f6e346621a6bffe0e4b8 in / 
# Sat, 28 Dec 2019 04:42:04 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 22:41:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 22:41:41 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:41:42 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:41:42 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:41:43 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:42:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 22:42:36 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:42:36 GMT
USER user
# Mon, 30 Dec 2019 22:42:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f7542f43e95fb32a870ee38d7f0e7bb23267ac8dcf709e3944311b0a30d7a479`  
		Last Modified: Sat, 28 Dec 2019 04:45:08 GMT  
		Size: 25.7 MB (25705315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3021cd15a7c1a65d381978e66c420a23e06b0714cb8038e6937152fbd77e6740`  
		Last Modified: Mon, 30 Dec 2019 22:43:35 GMT  
		Size: 16.9 MB (16858905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8176e43a5836b18e5ec920d3c606074b54d1ba1dfe4552fd0d71e0e419c56113`  
		Last Modified: Mon, 30 Dec 2019 22:43:31 GMT  
		Size: 4.2 KB (4189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3213bdc14a62074eb7cbd9519f9599043778dd6c5bbe78299eb33914f2eaddc2`  
		Last Modified: Mon, 30 Dec 2019 22:43:32 GMT  
		Size: 6.4 MB (6382708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2`

```console
$ docker pull irssi@sha256:10d70bb9912ee6af38e32c68e5147774527371b837d2e96c38496cbd89c460af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `irssi:1.2` - linux; amd64

```console
$ docker pull irssi@sha256:94ade928c56069ab24e07a671d461627157bfc4b4c75cddc7e0eef74dc429668
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50512777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:071f6fdb9d31c1fdb38e00b3f4aa5f35f0488bf3f0be7ec47c8609d9b77f7d82`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 22:19:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 22:19:55 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:19:55 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:19:56 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:19:56 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:20:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 22:20:56 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:20:56 GMT
USER user
# Mon, 30 Dec 2019 22:20:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155ffa1aba8607e36ef345d54c69e06dff0957646eb0a3ff4ea1f247f2d6f834`  
		Last Modified: Mon, 30 Dec 2019 22:22:11 GMT  
		Size: 17.0 MB (16987485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c035b099bd2ec74cb6afce844b250fd133eb9632293848ada2628bdbc84f1db`  
		Last Modified: Mon, 30 Dec 2019 22:22:06 GMT  
		Size: 4.2 KB (4181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32794dd5d2b6704bd7908f83a0bc9c91af102b15cb616927fc7c5aa4e1917f2`  
		Last Modified: Mon, 30 Dec 2019 22:22:08 GMT  
		Size: 6.4 MB (6428837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; arm variant v5

```console
$ docker pull irssi@sha256:0e2ffdb40c1813fcd5d664cd43f803e9fae16d23158c37a0a3a77ee6f9c6ea30
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46786540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2429596187b3420620bfa930a489829d17b7ae16f68a5e12f468600ead30f6b0`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:49:50 GMT
ADD file:5d34c769f80c3fdbb04048f4336cf212164934607a642144ef557faef5896192 in / 
# Sat, 28 Dec 2019 04:49:51 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 22:49:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 22:49:11 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:49:13 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:49:14 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:49:14 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:51:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 22:51:50 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:51:51 GMT
USER user
# Mon, 30 Dec 2019 22:51:53 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:153ccec980772b5fc4c786af0b26bba09f0a2d95d9755400febf9a79aa4220c8`  
		Last Modified: Sat, 28 Dec 2019 04:56:28 GMT  
		Size: 24.8 MB (24829618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa69714a630c9112cb8ed12a6a0c9ae434a0a7195c6e4f68933886f7fd1983f`  
		Last Modified: Mon, 30 Dec 2019 22:52:22 GMT  
		Size: 15.9 MB (15890061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab31781254acfc5b427e96a9157a02a9ba33029a2005b185eb5269c4163787d`  
		Last Modified: Mon, 30 Dec 2019 22:52:11 GMT  
		Size: 4.2 KB (4205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6924de57ca5fe0466f8a204c8e8f92726d55e29433871e0a91aba15f983c8c`  
		Last Modified: Mon, 30 Dec 2019 22:52:14 GMT  
		Size: 6.1 MB (6062656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; arm variant v7

```console
$ docker pull irssi@sha256:4ac9143ebda80df861793e06c1ab529a0c82cbc5fbb1467ad6f905a717d1242f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44188477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebc901e04efd19e1b84420fee3ddabfa2c5e0f65bf74941175283da2815154aa`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 23:02:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 23:02:55 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 23:02:57 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 23:02:58 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 23:02:58 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 23:04:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 23:04:30 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 23:04:31 GMT
USER user
# Mon, 30 Dec 2019 23:04:32 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09075676a7576165b8ed1990b233d29b4a112b50d5957c1a1c8cbf0c1853dc76`  
		Last Modified: Mon, 30 Dec 2019 23:06:11 GMT  
		Size: 15.6 MB (15554857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373ec572d9c27ba5c4b59943b257138a84a107907c938b6300b34503f7f2e602`  
		Last Modified: Mon, 30 Dec 2019 23:06:03 GMT  
		Size: 4.2 KB (4197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec006cec70b4f55bcb3b95111258702e778f90ad5362b4c08bc1b87f10b405e2`  
		Last Modified: Mon, 30 Dec 2019 23:06:05 GMT  
		Size: 5.9 MB (5930294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:52d0ead408e844bba3ea08864d9ee1ce400727f99711658a332c8ab953b41ae7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49005367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13e82aa16b7576863ef36d2b9ffce9df153f1aa8177e97e220143821458a55a7`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 22:41:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 22:41:08 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:41:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:41:10 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:41:11 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:42:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 22:42:54 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:42:56 GMT
USER user
# Mon, 30 Dec 2019 22:42:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc97913e2d0d8cb44f6fd5a47a49974057573a753cf66d3212046b6c376fd9f0`  
		Last Modified: Mon, 30 Dec 2019 22:44:30 GMT  
		Size: 16.8 MB (16762627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0709e009ad51ad0a0ec48f8c3c0b0de4fd412ad5b3b42e53757cec282180e87`  
		Last Modified: Mon, 30 Dec 2019 22:44:23 GMT  
		Size: 4.2 KB (4215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c555b242ddbe0e9335602cbdca56f5c307d560b4635c31338861407810b9945`  
		Last Modified: Mon, 30 Dec 2019 22:44:25 GMT  
		Size: 6.4 MB (6387823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; 386

```console
$ docker pull irssi@sha256:c5e4274b633a2d299ec9af52d580010154758ada9929bb758022334ac968820e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50367637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdbe22cc632c3d69ce50527e20598a64ea33d2dbffff7cdd42ccff0be736b6ac`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 22:38:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 22:38:37 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:38:38 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:38:38 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:38:38 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:39:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 22:39:57 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:39:57 GMT
USER user
# Mon, 30 Dec 2019 22:39:57 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72221f577a2f5220d3b7671a23bbf707e559dc20fd260e9e321a3bca8bf4e7fc`  
		Last Modified: Mon, 30 Dec 2019 22:41:20 GMT  
		Size: 16.5 MB (16515220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e488155fc2527b4ab798931fac3fa6f7521f5e687e0c82ea1cf007b495ea88`  
		Last Modified: Mon, 30 Dec 2019 22:41:14 GMT  
		Size: 4.2 KB (4170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07b243b29fe05690820a603d2c31463dbe08ca974efc99b033aca2703d9ac65`  
		Last Modified: Mon, 30 Dec 2019 22:41:16 GMT  
		Size: 6.1 MB (6101227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; ppc64le

```console
$ docker pull irssi@sha256:aabbe2ff8e02fa9376da9c3d21d0f747aee3e97fcf372951d07e85252732b28a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.7 MB (54698717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8c59fc543020e65db22f51fb7a5f22a0bdb0284f7a68619e2daeac2a6d27567`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 22:18:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 22:18:43 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:18:51 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:18:53 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:18:55 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:23:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 22:23:22 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:23:24 GMT
USER user
# Mon, 30 Dec 2019 22:23:26 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4a48662b243e889598e0a1b8e2a224407e08aa8c152a7b96352dc261c2b903`  
		Last Modified: Mon, 30 Dec 2019 22:25:36 GMT  
		Size: 17.4 MB (17396769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bd95038cb0e8d80e4cb33f7dbe1b0ae5c5b33f2f63955c2eafabeacead3d95`  
		Last Modified: Mon, 30 Dec 2019 22:25:30 GMT  
		Size: 4.2 KB (4219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d27ae35ac7ced8f7f75a99531f03b1e8e174a10f78c8c77acfc606ef3a1c40`  
		Last Modified: Mon, 30 Dec 2019 22:25:31 GMT  
		Size: 6.8 MB (6780200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; s390x

```console
$ docker pull irssi@sha256:b265d21e8baf744ec4ed0e1a75b3bb821b3b7cdc75cad870581f37a461d734a5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48951117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10fb4e99edc6f16e535536593259d9363aa1b59890a278a793360a6a601b02a9`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:42:03 GMT
ADD file:eec6c56f8680753860198c3af0d94aabb87018ca30f6f6e346621a6bffe0e4b8 in / 
# Sat, 28 Dec 2019 04:42:04 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 22:41:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 22:41:41 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:41:42 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:41:42 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:41:43 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:42:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 22:42:36 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:42:36 GMT
USER user
# Mon, 30 Dec 2019 22:42:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f7542f43e95fb32a870ee38d7f0e7bb23267ac8dcf709e3944311b0a30d7a479`  
		Last Modified: Sat, 28 Dec 2019 04:45:08 GMT  
		Size: 25.7 MB (25705315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3021cd15a7c1a65d381978e66c420a23e06b0714cb8038e6937152fbd77e6740`  
		Last Modified: Mon, 30 Dec 2019 22:43:35 GMT  
		Size: 16.9 MB (16858905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8176e43a5836b18e5ec920d3c606074b54d1ba1dfe4552fd0d71e0e419c56113`  
		Last Modified: Mon, 30 Dec 2019 22:43:31 GMT  
		Size: 4.2 KB (4189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3213bdc14a62074eb7cbd9519f9599043778dd6c5bbe78299eb33914f2eaddc2`  
		Last Modified: Mon, 30 Dec 2019 22:43:32 GMT  
		Size: 6.4 MB (6382708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2.2`

```console
$ docker pull irssi@sha256:10d70bb9912ee6af38e32c68e5147774527371b837d2e96c38496cbd89c460af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `irssi:1.2.2` - linux; amd64

```console
$ docker pull irssi@sha256:94ade928c56069ab24e07a671d461627157bfc4b4c75cddc7e0eef74dc429668
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50512777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:071f6fdb9d31c1fdb38e00b3f4aa5f35f0488bf3f0be7ec47c8609d9b77f7d82`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 22:19:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 22:19:55 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:19:55 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:19:56 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:19:56 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:20:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 22:20:56 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:20:56 GMT
USER user
# Mon, 30 Dec 2019 22:20:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155ffa1aba8607e36ef345d54c69e06dff0957646eb0a3ff4ea1f247f2d6f834`  
		Last Modified: Mon, 30 Dec 2019 22:22:11 GMT  
		Size: 17.0 MB (16987485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c035b099bd2ec74cb6afce844b250fd133eb9632293848ada2628bdbc84f1db`  
		Last Modified: Mon, 30 Dec 2019 22:22:06 GMT  
		Size: 4.2 KB (4181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32794dd5d2b6704bd7908f83a0bc9c91af102b15cb616927fc7c5aa4e1917f2`  
		Last Modified: Mon, 30 Dec 2019 22:22:08 GMT  
		Size: 6.4 MB (6428837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2` - linux; arm variant v5

```console
$ docker pull irssi@sha256:0e2ffdb40c1813fcd5d664cd43f803e9fae16d23158c37a0a3a77ee6f9c6ea30
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46786540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2429596187b3420620bfa930a489829d17b7ae16f68a5e12f468600ead30f6b0`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:49:50 GMT
ADD file:5d34c769f80c3fdbb04048f4336cf212164934607a642144ef557faef5896192 in / 
# Sat, 28 Dec 2019 04:49:51 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 22:49:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 22:49:11 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:49:13 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:49:14 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:49:14 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:51:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 22:51:50 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:51:51 GMT
USER user
# Mon, 30 Dec 2019 22:51:53 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:153ccec980772b5fc4c786af0b26bba09f0a2d95d9755400febf9a79aa4220c8`  
		Last Modified: Sat, 28 Dec 2019 04:56:28 GMT  
		Size: 24.8 MB (24829618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa69714a630c9112cb8ed12a6a0c9ae434a0a7195c6e4f68933886f7fd1983f`  
		Last Modified: Mon, 30 Dec 2019 22:52:22 GMT  
		Size: 15.9 MB (15890061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab31781254acfc5b427e96a9157a02a9ba33029a2005b185eb5269c4163787d`  
		Last Modified: Mon, 30 Dec 2019 22:52:11 GMT  
		Size: 4.2 KB (4205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6924de57ca5fe0466f8a204c8e8f92726d55e29433871e0a91aba15f983c8c`  
		Last Modified: Mon, 30 Dec 2019 22:52:14 GMT  
		Size: 6.1 MB (6062656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2` - linux; arm variant v7

```console
$ docker pull irssi@sha256:4ac9143ebda80df861793e06c1ab529a0c82cbc5fbb1467ad6f905a717d1242f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44188477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebc901e04efd19e1b84420fee3ddabfa2c5e0f65bf74941175283da2815154aa`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 23:02:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 23:02:55 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 23:02:57 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 23:02:58 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 23:02:58 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 23:04:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 23:04:30 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 23:04:31 GMT
USER user
# Mon, 30 Dec 2019 23:04:32 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09075676a7576165b8ed1990b233d29b4a112b50d5957c1a1c8cbf0c1853dc76`  
		Last Modified: Mon, 30 Dec 2019 23:06:11 GMT  
		Size: 15.6 MB (15554857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373ec572d9c27ba5c4b59943b257138a84a107907c938b6300b34503f7f2e602`  
		Last Modified: Mon, 30 Dec 2019 23:06:03 GMT  
		Size: 4.2 KB (4197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec006cec70b4f55bcb3b95111258702e778f90ad5362b4c08bc1b87f10b405e2`  
		Last Modified: Mon, 30 Dec 2019 23:06:05 GMT  
		Size: 5.9 MB (5930294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:52d0ead408e844bba3ea08864d9ee1ce400727f99711658a332c8ab953b41ae7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49005367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13e82aa16b7576863ef36d2b9ffce9df153f1aa8177e97e220143821458a55a7`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 22:41:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 22:41:08 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:41:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:41:10 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:41:11 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:42:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 22:42:54 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:42:56 GMT
USER user
# Mon, 30 Dec 2019 22:42:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc97913e2d0d8cb44f6fd5a47a49974057573a753cf66d3212046b6c376fd9f0`  
		Last Modified: Mon, 30 Dec 2019 22:44:30 GMT  
		Size: 16.8 MB (16762627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0709e009ad51ad0a0ec48f8c3c0b0de4fd412ad5b3b42e53757cec282180e87`  
		Last Modified: Mon, 30 Dec 2019 22:44:23 GMT  
		Size: 4.2 KB (4215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c555b242ddbe0e9335602cbdca56f5c307d560b4635c31338861407810b9945`  
		Last Modified: Mon, 30 Dec 2019 22:44:25 GMT  
		Size: 6.4 MB (6387823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2` - linux; 386

```console
$ docker pull irssi@sha256:c5e4274b633a2d299ec9af52d580010154758ada9929bb758022334ac968820e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50367637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdbe22cc632c3d69ce50527e20598a64ea33d2dbffff7cdd42ccff0be736b6ac`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 22:38:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 22:38:37 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:38:38 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:38:38 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:38:38 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:39:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 22:39:57 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:39:57 GMT
USER user
# Mon, 30 Dec 2019 22:39:57 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72221f577a2f5220d3b7671a23bbf707e559dc20fd260e9e321a3bca8bf4e7fc`  
		Last Modified: Mon, 30 Dec 2019 22:41:20 GMT  
		Size: 16.5 MB (16515220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e488155fc2527b4ab798931fac3fa6f7521f5e687e0c82ea1cf007b495ea88`  
		Last Modified: Mon, 30 Dec 2019 22:41:14 GMT  
		Size: 4.2 KB (4170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07b243b29fe05690820a603d2c31463dbe08ca974efc99b033aca2703d9ac65`  
		Last Modified: Mon, 30 Dec 2019 22:41:16 GMT  
		Size: 6.1 MB (6101227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2` - linux; ppc64le

```console
$ docker pull irssi@sha256:aabbe2ff8e02fa9376da9c3d21d0f747aee3e97fcf372951d07e85252732b28a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.7 MB (54698717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8c59fc543020e65db22f51fb7a5f22a0bdb0284f7a68619e2daeac2a6d27567`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 22:18:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 22:18:43 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:18:51 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:18:53 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:18:55 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:23:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 22:23:22 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:23:24 GMT
USER user
# Mon, 30 Dec 2019 22:23:26 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4a48662b243e889598e0a1b8e2a224407e08aa8c152a7b96352dc261c2b903`  
		Last Modified: Mon, 30 Dec 2019 22:25:36 GMT  
		Size: 17.4 MB (17396769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bd95038cb0e8d80e4cb33f7dbe1b0ae5c5b33f2f63955c2eafabeacead3d95`  
		Last Modified: Mon, 30 Dec 2019 22:25:30 GMT  
		Size: 4.2 KB (4219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d27ae35ac7ced8f7f75a99531f03b1e8e174a10f78c8c77acfc606ef3a1c40`  
		Last Modified: Mon, 30 Dec 2019 22:25:31 GMT  
		Size: 6.8 MB (6780200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2` - linux; s390x

```console
$ docker pull irssi@sha256:b265d21e8baf744ec4ed0e1a75b3bb821b3b7cdc75cad870581f37a461d734a5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48951117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10fb4e99edc6f16e535536593259d9363aa1b59890a278a793360a6a601b02a9`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:42:03 GMT
ADD file:eec6c56f8680753860198c3af0d94aabb87018ca30f6f6e346621a6bffe0e4b8 in / 
# Sat, 28 Dec 2019 04:42:04 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 22:41:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 22:41:41 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:41:42 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:41:42 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:41:43 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:42:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 22:42:36 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:42:36 GMT
USER user
# Mon, 30 Dec 2019 22:42:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f7542f43e95fb32a870ee38d7f0e7bb23267ac8dcf709e3944311b0a30d7a479`  
		Last Modified: Sat, 28 Dec 2019 04:45:08 GMT  
		Size: 25.7 MB (25705315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3021cd15a7c1a65d381978e66c420a23e06b0714cb8038e6937152fbd77e6740`  
		Last Modified: Mon, 30 Dec 2019 22:43:35 GMT  
		Size: 16.9 MB (16858905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8176e43a5836b18e5ec920d3c606074b54d1ba1dfe4552fd0d71e0e419c56113`  
		Last Modified: Mon, 30 Dec 2019 22:43:31 GMT  
		Size: 4.2 KB (4189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3213bdc14a62074eb7cbd9519f9599043778dd6c5bbe78299eb33914f2eaddc2`  
		Last Modified: Mon, 30 Dec 2019 22:43:32 GMT  
		Size: 6.4 MB (6382708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2.2-alpine`

```console
$ docker pull irssi@sha256:53b6347f3c707a75a374b41b571d0bcbcce97d2a69c4130ef2901476ac751bab
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
$ docker pull irssi@sha256:e83aeb2a7084a795b1284c2516cf6ec658ffc6b1e9f1aa692391f75d88ed466a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.2 MB (19241142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3c5cc461cc163d5ec6d54832d0926a96cb206eafa515b3945aee2f605e516fa`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:13:07 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 18 Jan 2020 03:13:07 GMT
ENV HOME=/home/user
# Sat, 18 Jan 2020 03:13:08 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 18 Jan 2020 03:13:08 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 03:13:08 GMT
ENV IRSSI_VERSION=1.2.2
# Sat, 18 Jan 2020 03:13:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 18 Jan 2020 03:13:50 GMT
WORKDIR /home/user
# Sat, 18 Jan 2020 03:13:50 GMT
USER user
# Sat, 18 Jan 2020 03:13:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f318a8e84ae847d821a731ba55cd1a45783802db04e560d11e1e3c7538e5397`  
		Last Modified: Sat, 18 Jan 2020 03:14:05 GMT  
		Size: 9.4 MB (9422666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78354d333eb114a03dfe861868b5485c89a1356eaff9f656546233af1926b4fb`  
		Last Modified: Sat, 18 Jan 2020 03:14:02 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14774cc8271a38ba75ed5ce296e0330929d69d58a12218a597e64d9de32e6aa8`  
		Last Modified: Sat, 18 Jan 2020 03:14:04 GMT  
		Size: 7.0 MB (7014276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:342b2c19ea74b251a8c406ff065393a1826ac54052946813237158beea60ddfb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.4 MB (19363564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9260d7ed17bd0aa35c4da740d6f224880fcc65b175e242e816b586e973b33db0`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 24 Dec 2019 18:49:41 GMT
ADD file:c4f944e24d0f2e758363506e8b98b3b53973ec18dd4dd23da3f09520ef22c65c in / 
# Tue, 24 Dec 2019 18:49:42 GMT
CMD ["/bin/sh"]
# Mon, 30 Dec 2019 22:50:56 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Mon, 30 Dec 2019 22:51:02 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:51:08 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:51:10 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:51:13 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:52:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Mon, 30 Dec 2019 22:52:18 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:52:19 GMT
USER user
# Mon, 30 Dec 2019 22:52:19 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:546eec1e02ac5f4494868d8b22e8ced00773a2fba8e25b3edd30002889874299`  
		Last Modified: Tue, 24 Dec 2019 18:50:07 GMT  
		Size: 2.6 MB (2612021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e096f7e647acbccc301b850346b30db145dbc810757f233bbd4b9203c86d77a1`  
		Last Modified: Mon, 30 Dec 2019 22:52:36 GMT  
		Size: 8.7 MB (8665185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e252d91ac1eeb24eda441bc7025af739933267533fccbb1f5aca50534a8536`  
		Last Modified: Mon, 30 Dec 2019 22:52:32 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a7f820d727394e1780cfbc82d9c6cbb3b358c303cc6374fdf02405a913329b`  
		Last Modified: Mon, 30 Dec 2019 22:52:35 GMT  
		Size: 8.1 MB (8085085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:0ae5303301eb71e8a0ae6950e7a5444c1f4915d4cb995a345402a28d7594b6dc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17447893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93e2dfe3c6929bec1e86463bd93b9c895af9f7fead7afbd7a940c014c4f294b1`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:18:12 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 18 Jan 2020 05:18:23 GMT
ENV HOME=/home/user
# Sat, 18 Jan 2020 05:18:34 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 18 Jan 2020 05:18:41 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 05:18:47 GMT
ENV IRSSI_VERSION=1.2.2
# Sat, 18 Jan 2020 05:19:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 18 Jan 2020 05:20:01 GMT
WORKDIR /home/user
# Sat, 18 Jan 2020 05:20:03 GMT
USER user
# Sat, 18 Jan 2020 05:20:05 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94079a590d0a41243d2c73a7f80d095fed025f2bc91ecba53a6fa01a602d54f2`  
		Last Modified: Sat, 18 Jan 2020 05:20:33 GMT  
		Size: 8.5 MB (8516143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2389694069ce07ceb540b166dbacd58df5db01de5b53a7b7eb70e03b010046`  
		Last Modified: Sat, 18 Jan 2020 05:20:29 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c930171b23884f8216e769bd4a98a38794efe4fe9b14be9d630a886dafc272b`  
		Last Modified: Sat, 18 Jan 2020 05:20:32 GMT  
		Size: 6.5 MB (6510922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:207c264f04e366c5bd1fb958a98a72b995af1ef534d9f0023bc03eaac2f84346
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19140791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d45b6d8eff3e11e1532c225b72d6e2948edcff1a40672f0f16c62f72c1014ae`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:15:17 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 18 Jan 2020 02:15:20 GMT
ENV HOME=/home/user
# Sat, 18 Jan 2020 02:15:26 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 18 Jan 2020 02:15:28 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 02:15:30 GMT
ENV IRSSI_VERSION=1.2.2
# Sat, 18 Jan 2020 02:16:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 18 Jan 2020 02:16:42 GMT
WORKDIR /home/user
# Sat, 18 Jan 2020 02:16:44 GMT
USER user
# Sat, 18 Jan 2020 02:16:45 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69e852f652474e05d47f735b6cd5f72da8c34afad334b50738688b19b0a4db4`  
		Last Modified: Sat, 18 Jan 2020 02:17:06 GMT  
		Size: 9.4 MB (9425621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6def3b6ee199ce1adf97bb4eeaa035b672219b0ee8b530d9d64d8cbade20bdd3`  
		Last Modified: Sat, 18 Jan 2020 02:17:02 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73860e239366f5942b9248b359261d13cc9f5f3bcfdf519862444ed2311678f1`  
		Last Modified: Sat, 18 Jan 2020 02:17:05 GMT  
		Size: 7.0 MB (6990825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2-alpine` - linux; 386

```console
$ docker pull irssi@sha256:06ceaa49272143bc576a7ba5152770993749081dcf137f1fb1eb2013782a9651
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.9 MB (19947359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efd9498f6332d6dd2090dfa8ea6ebd973aae9d1ed9ae4c972432518e7e04603b`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 24 Dec 2019 19:38:57 GMT
ADD file:d0127a9692e8445993a88163cb741dbb23fa25436dd65289e76b08484264b397 in / 
# Tue, 24 Dec 2019 19:38:57 GMT
CMD ["/bin/sh"]
# Mon, 30 Dec 2019 22:40:08 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Mon, 30 Dec 2019 22:40:09 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:40:09 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:40:10 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:40:10 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:40:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Mon, 30 Dec 2019 22:40:58 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:40:58 GMT
USER user
# Mon, 30 Dec 2019 22:40:59 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:57bbc6f150623b3e4f01930af4ab2efa6ed5df02319341a08b1ce0bbd7e4afdf`  
		Last Modified: Tue, 24 Dec 2019 19:39:19 GMT  
		Size: 2.8 MB (2805146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff76006f62081ce832038868fe5b0b60ceed2187a08ed77ee36104006fbba791`  
		Last Modified: Mon, 30 Dec 2019 22:41:28 GMT  
		Size: 8.8 MB (8795524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db6f9ad44fed6961e6e5583a2858d76ed51e909d36e5f56257c2c3f01ec9aa3`  
		Last Modified: Mon, 30 Dec 2019 22:41:25 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbbf684b8369fac0090667874a96aa8959617cdf6f3e2efd898b900ee2271f00`  
		Last Modified: Mon, 30 Dec 2019 22:41:28 GMT  
		Size: 8.3 MB (8345445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:a4ee2c5582db1a8e3172e6b52c07a9d50751899e91c6fe9daf19a2db1fa377b8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.6 MB (19585238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1708846a38a9f626fbcde811f250e21368ce7d11f1a02dc0f62668375efaebcd`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:17:53 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 18 Jan 2020 04:17:59 GMT
ENV HOME=/home/user
# Sat, 18 Jan 2020 04:18:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 18 Jan 2020 04:18:09 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 04:18:12 GMT
ENV IRSSI_VERSION=1.2.2
# Sat, 18 Jan 2020 04:18:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 18 Jan 2020 04:19:00 GMT
WORKDIR /home/user
# Sat, 18 Jan 2020 04:19:03 GMT
USER user
# Sat, 18 Jan 2020 04:19:05 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cee495aeeccb8a9ca2b5b61da748591694470663de0f02e137bdb40886e1b1a`  
		Last Modified: Sat, 18 Jan 2020 04:19:40 GMT  
		Size: 9.5 MB (9521127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9dff5f290556e9df6faaefe25d1df97863e26a25255105adb22223ac042277`  
		Last Modified: Sat, 18 Jan 2020 04:19:36 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb398dcd302a5d86beba50e971e877dfc1df78f1dd0ba3be19395b75714c53d`  
		Last Modified: Sat, 18 Jan 2020 04:19:45 GMT  
		Size: 7.2 MB (7240714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.2-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:743262e0cf05ee5125863b88cda7b7377c3062926189f5e02a2b42df784f2cb2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.4 MB (19412058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ccf5f5bf85e76d9796ebb1c43c0e0bdf44eda4060d07dcb03f2ad6d9c96c1e5`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 18 Jan 2020 01:41:33 GMT
ADD file:a6f8b7d4ba199527053ef1ac710b5e318135cb6903cb9ad6fae4fe42e6ad0bf7 in / 
# Sat, 18 Jan 2020 01:41:33 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:18:41 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 18 Jan 2020 02:18:42 GMT
ENV HOME=/home/user
# Sat, 18 Jan 2020 02:18:42 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 18 Jan 2020 02:18:43 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 02:18:43 GMT
ENV IRSSI_VERSION=1.2.2
# Sat, 18 Jan 2020 02:19:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 18 Jan 2020 02:19:07 GMT
WORKDIR /home/user
# Sat, 18 Jan 2020 02:19:07 GMT
USER user
# Sat, 18 Jan 2020 02:19:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:176bad61a3a435da03ec603d2bd8f7a69286d92f21f447b17f21f0bc4e085bde`  
		Last Modified: Sat, 18 Jan 2020 01:41:59 GMT  
		Size: 2.6 MB (2582031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e137b1edc1565268f2019b28a1283c2b36e957c2009bb8ae076a030a13cb509`  
		Last Modified: Sat, 18 Jan 2020 02:19:21 GMT  
		Size: 9.8 MB (9834358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b03d27ba39922c28999efffd37fba89df9b0a24245f1a6512c36d8addc6d77`  
		Last Modified: Sat, 18 Jan 2020 02:19:20 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4f0c62b30ce5b338a1a15eae2c2181316c105dd21264175c162f3ae6c511f3`  
		Last Modified: Sat, 18 Jan 2020 02:19:21 GMT  
		Size: 7.0 MB (6994424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2-alpine`

```console
$ docker pull irssi@sha256:53b6347f3c707a75a374b41b571d0bcbcce97d2a69c4130ef2901476ac751bab
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
$ docker pull irssi@sha256:e83aeb2a7084a795b1284c2516cf6ec658ffc6b1e9f1aa692391f75d88ed466a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.2 MB (19241142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3c5cc461cc163d5ec6d54832d0926a96cb206eafa515b3945aee2f605e516fa`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:13:07 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 18 Jan 2020 03:13:07 GMT
ENV HOME=/home/user
# Sat, 18 Jan 2020 03:13:08 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 18 Jan 2020 03:13:08 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 03:13:08 GMT
ENV IRSSI_VERSION=1.2.2
# Sat, 18 Jan 2020 03:13:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 18 Jan 2020 03:13:50 GMT
WORKDIR /home/user
# Sat, 18 Jan 2020 03:13:50 GMT
USER user
# Sat, 18 Jan 2020 03:13:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f318a8e84ae847d821a731ba55cd1a45783802db04e560d11e1e3c7538e5397`  
		Last Modified: Sat, 18 Jan 2020 03:14:05 GMT  
		Size: 9.4 MB (9422666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78354d333eb114a03dfe861868b5485c89a1356eaff9f656546233af1926b4fb`  
		Last Modified: Sat, 18 Jan 2020 03:14:02 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14774cc8271a38ba75ed5ce296e0330929d69d58a12218a597e64d9de32e6aa8`  
		Last Modified: Sat, 18 Jan 2020 03:14:04 GMT  
		Size: 7.0 MB (7014276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:342b2c19ea74b251a8c406ff065393a1826ac54052946813237158beea60ddfb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.4 MB (19363564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9260d7ed17bd0aa35c4da740d6f224880fcc65b175e242e816b586e973b33db0`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 24 Dec 2019 18:49:41 GMT
ADD file:c4f944e24d0f2e758363506e8b98b3b53973ec18dd4dd23da3f09520ef22c65c in / 
# Tue, 24 Dec 2019 18:49:42 GMT
CMD ["/bin/sh"]
# Mon, 30 Dec 2019 22:50:56 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Mon, 30 Dec 2019 22:51:02 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:51:08 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:51:10 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:51:13 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:52:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Mon, 30 Dec 2019 22:52:18 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:52:19 GMT
USER user
# Mon, 30 Dec 2019 22:52:19 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:546eec1e02ac5f4494868d8b22e8ced00773a2fba8e25b3edd30002889874299`  
		Last Modified: Tue, 24 Dec 2019 18:50:07 GMT  
		Size: 2.6 MB (2612021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e096f7e647acbccc301b850346b30db145dbc810757f233bbd4b9203c86d77a1`  
		Last Modified: Mon, 30 Dec 2019 22:52:36 GMT  
		Size: 8.7 MB (8665185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e252d91ac1eeb24eda441bc7025af739933267533fccbb1f5aca50534a8536`  
		Last Modified: Mon, 30 Dec 2019 22:52:32 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a7f820d727394e1780cfbc82d9c6cbb3b358c303cc6374fdf02405a913329b`  
		Last Modified: Mon, 30 Dec 2019 22:52:35 GMT  
		Size: 8.1 MB (8085085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:0ae5303301eb71e8a0ae6950e7a5444c1f4915d4cb995a345402a28d7594b6dc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17447893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93e2dfe3c6929bec1e86463bd93b9c895af9f7fead7afbd7a940c014c4f294b1`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:18:12 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 18 Jan 2020 05:18:23 GMT
ENV HOME=/home/user
# Sat, 18 Jan 2020 05:18:34 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 18 Jan 2020 05:18:41 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 05:18:47 GMT
ENV IRSSI_VERSION=1.2.2
# Sat, 18 Jan 2020 05:19:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 18 Jan 2020 05:20:01 GMT
WORKDIR /home/user
# Sat, 18 Jan 2020 05:20:03 GMT
USER user
# Sat, 18 Jan 2020 05:20:05 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94079a590d0a41243d2c73a7f80d095fed025f2bc91ecba53a6fa01a602d54f2`  
		Last Modified: Sat, 18 Jan 2020 05:20:33 GMT  
		Size: 8.5 MB (8516143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2389694069ce07ceb540b166dbacd58df5db01de5b53a7b7eb70e03b010046`  
		Last Modified: Sat, 18 Jan 2020 05:20:29 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c930171b23884f8216e769bd4a98a38794efe4fe9b14be9d630a886dafc272b`  
		Last Modified: Sat, 18 Jan 2020 05:20:32 GMT  
		Size: 6.5 MB (6510922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:207c264f04e366c5bd1fb958a98a72b995af1ef534d9f0023bc03eaac2f84346
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19140791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d45b6d8eff3e11e1532c225b72d6e2948edcff1a40672f0f16c62f72c1014ae`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:15:17 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 18 Jan 2020 02:15:20 GMT
ENV HOME=/home/user
# Sat, 18 Jan 2020 02:15:26 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 18 Jan 2020 02:15:28 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 02:15:30 GMT
ENV IRSSI_VERSION=1.2.2
# Sat, 18 Jan 2020 02:16:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 18 Jan 2020 02:16:42 GMT
WORKDIR /home/user
# Sat, 18 Jan 2020 02:16:44 GMT
USER user
# Sat, 18 Jan 2020 02:16:45 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69e852f652474e05d47f735b6cd5f72da8c34afad334b50738688b19b0a4db4`  
		Last Modified: Sat, 18 Jan 2020 02:17:06 GMT  
		Size: 9.4 MB (9425621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6def3b6ee199ce1adf97bb4eeaa035b672219b0ee8b530d9d64d8cbade20bdd3`  
		Last Modified: Sat, 18 Jan 2020 02:17:02 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73860e239366f5942b9248b359261d13cc9f5f3bcfdf519862444ed2311678f1`  
		Last Modified: Sat, 18 Jan 2020 02:17:05 GMT  
		Size: 7.0 MB (6990825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; 386

```console
$ docker pull irssi@sha256:06ceaa49272143bc576a7ba5152770993749081dcf137f1fb1eb2013782a9651
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.9 MB (19947359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efd9498f6332d6dd2090dfa8ea6ebd973aae9d1ed9ae4c972432518e7e04603b`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 24 Dec 2019 19:38:57 GMT
ADD file:d0127a9692e8445993a88163cb741dbb23fa25436dd65289e76b08484264b397 in / 
# Tue, 24 Dec 2019 19:38:57 GMT
CMD ["/bin/sh"]
# Mon, 30 Dec 2019 22:40:08 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Mon, 30 Dec 2019 22:40:09 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:40:09 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:40:10 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:40:10 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:40:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Mon, 30 Dec 2019 22:40:58 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:40:58 GMT
USER user
# Mon, 30 Dec 2019 22:40:59 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:57bbc6f150623b3e4f01930af4ab2efa6ed5df02319341a08b1ce0bbd7e4afdf`  
		Last Modified: Tue, 24 Dec 2019 19:39:19 GMT  
		Size: 2.8 MB (2805146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff76006f62081ce832038868fe5b0b60ceed2187a08ed77ee36104006fbba791`  
		Last Modified: Mon, 30 Dec 2019 22:41:28 GMT  
		Size: 8.8 MB (8795524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db6f9ad44fed6961e6e5583a2858d76ed51e909d36e5f56257c2c3f01ec9aa3`  
		Last Modified: Mon, 30 Dec 2019 22:41:25 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbbf684b8369fac0090667874a96aa8959617cdf6f3e2efd898b900ee2271f00`  
		Last Modified: Mon, 30 Dec 2019 22:41:28 GMT  
		Size: 8.3 MB (8345445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:a4ee2c5582db1a8e3172e6b52c07a9d50751899e91c6fe9daf19a2db1fa377b8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.6 MB (19585238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1708846a38a9f626fbcde811f250e21368ce7d11f1a02dc0f62668375efaebcd`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:17:53 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 18 Jan 2020 04:17:59 GMT
ENV HOME=/home/user
# Sat, 18 Jan 2020 04:18:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 18 Jan 2020 04:18:09 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 04:18:12 GMT
ENV IRSSI_VERSION=1.2.2
# Sat, 18 Jan 2020 04:18:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 18 Jan 2020 04:19:00 GMT
WORKDIR /home/user
# Sat, 18 Jan 2020 04:19:03 GMT
USER user
# Sat, 18 Jan 2020 04:19:05 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cee495aeeccb8a9ca2b5b61da748591694470663de0f02e137bdb40886e1b1a`  
		Last Modified: Sat, 18 Jan 2020 04:19:40 GMT  
		Size: 9.5 MB (9521127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9dff5f290556e9df6faaefe25d1df97863e26a25255105adb22223ac042277`  
		Last Modified: Sat, 18 Jan 2020 04:19:36 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb398dcd302a5d86beba50e971e877dfc1df78f1dd0ba3be19395b75714c53d`  
		Last Modified: Sat, 18 Jan 2020 04:19:45 GMT  
		Size: 7.2 MB (7240714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:743262e0cf05ee5125863b88cda7b7377c3062926189f5e02a2b42df784f2cb2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.4 MB (19412058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ccf5f5bf85e76d9796ebb1c43c0e0bdf44eda4060d07dcb03f2ad6d9c96c1e5`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 18 Jan 2020 01:41:33 GMT
ADD file:a6f8b7d4ba199527053ef1ac710b5e318135cb6903cb9ad6fae4fe42e6ad0bf7 in / 
# Sat, 18 Jan 2020 01:41:33 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:18:41 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 18 Jan 2020 02:18:42 GMT
ENV HOME=/home/user
# Sat, 18 Jan 2020 02:18:42 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 18 Jan 2020 02:18:43 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 02:18:43 GMT
ENV IRSSI_VERSION=1.2.2
# Sat, 18 Jan 2020 02:19:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 18 Jan 2020 02:19:07 GMT
WORKDIR /home/user
# Sat, 18 Jan 2020 02:19:07 GMT
USER user
# Sat, 18 Jan 2020 02:19:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:176bad61a3a435da03ec603d2bd8f7a69286d92f21f447b17f21f0bc4e085bde`  
		Last Modified: Sat, 18 Jan 2020 01:41:59 GMT  
		Size: 2.6 MB (2582031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e137b1edc1565268f2019b28a1283c2b36e957c2009bb8ae076a030a13cb509`  
		Last Modified: Sat, 18 Jan 2020 02:19:21 GMT  
		Size: 9.8 MB (9834358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b03d27ba39922c28999efffd37fba89df9b0a24245f1a6512c36d8addc6d77`  
		Last Modified: Sat, 18 Jan 2020 02:19:20 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4f0c62b30ce5b338a1a15eae2c2181316c105dd21264175c162f3ae6c511f3`  
		Last Modified: Sat, 18 Jan 2020 02:19:21 GMT  
		Size: 7.0 MB (6994424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1-alpine`

```console
$ docker pull irssi@sha256:53b6347f3c707a75a374b41b571d0bcbcce97d2a69c4130ef2901476ac751bab
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
$ docker pull irssi@sha256:e83aeb2a7084a795b1284c2516cf6ec658ffc6b1e9f1aa692391f75d88ed466a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.2 MB (19241142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3c5cc461cc163d5ec6d54832d0926a96cb206eafa515b3945aee2f605e516fa`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:13:07 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 18 Jan 2020 03:13:07 GMT
ENV HOME=/home/user
# Sat, 18 Jan 2020 03:13:08 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 18 Jan 2020 03:13:08 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 03:13:08 GMT
ENV IRSSI_VERSION=1.2.2
# Sat, 18 Jan 2020 03:13:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 18 Jan 2020 03:13:50 GMT
WORKDIR /home/user
# Sat, 18 Jan 2020 03:13:50 GMT
USER user
# Sat, 18 Jan 2020 03:13:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f318a8e84ae847d821a731ba55cd1a45783802db04e560d11e1e3c7538e5397`  
		Last Modified: Sat, 18 Jan 2020 03:14:05 GMT  
		Size: 9.4 MB (9422666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78354d333eb114a03dfe861868b5485c89a1356eaff9f656546233af1926b4fb`  
		Last Modified: Sat, 18 Jan 2020 03:14:02 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14774cc8271a38ba75ed5ce296e0330929d69d58a12218a597e64d9de32e6aa8`  
		Last Modified: Sat, 18 Jan 2020 03:14:04 GMT  
		Size: 7.0 MB (7014276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:342b2c19ea74b251a8c406ff065393a1826ac54052946813237158beea60ddfb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.4 MB (19363564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9260d7ed17bd0aa35c4da740d6f224880fcc65b175e242e816b586e973b33db0`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 24 Dec 2019 18:49:41 GMT
ADD file:c4f944e24d0f2e758363506e8b98b3b53973ec18dd4dd23da3f09520ef22c65c in / 
# Tue, 24 Dec 2019 18:49:42 GMT
CMD ["/bin/sh"]
# Mon, 30 Dec 2019 22:50:56 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Mon, 30 Dec 2019 22:51:02 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:51:08 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:51:10 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:51:13 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:52:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Mon, 30 Dec 2019 22:52:18 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:52:19 GMT
USER user
# Mon, 30 Dec 2019 22:52:19 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:546eec1e02ac5f4494868d8b22e8ced00773a2fba8e25b3edd30002889874299`  
		Last Modified: Tue, 24 Dec 2019 18:50:07 GMT  
		Size: 2.6 MB (2612021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e096f7e647acbccc301b850346b30db145dbc810757f233bbd4b9203c86d77a1`  
		Last Modified: Mon, 30 Dec 2019 22:52:36 GMT  
		Size: 8.7 MB (8665185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e252d91ac1eeb24eda441bc7025af739933267533fccbb1f5aca50534a8536`  
		Last Modified: Mon, 30 Dec 2019 22:52:32 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a7f820d727394e1780cfbc82d9c6cbb3b358c303cc6374fdf02405a913329b`  
		Last Modified: Mon, 30 Dec 2019 22:52:35 GMT  
		Size: 8.1 MB (8085085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:0ae5303301eb71e8a0ae6950e7a5444c1f4915d4cb995a345402a28d7594b6dc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17447893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93e2dfe3c6929bec1e86463bd93b9c895af9f7fead7afbd7a940c014c4f294b1`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:18:12 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 18 Jan 2020 05:18:23 GMT
ENV HOME=/home/user
# Sat, 18 Jan 2020 05:18:34 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 18 Jan 2020 05:18:41 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 05:18:47 GMT
ENV IRSSI_VERSION=1.2.2
# Sat, 18 Jan 2020 05:19:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 18 Jan 2020 05:20:01 GMT
WORKDIR /home/user
# Sat, 18 Jan 2020 05:20:03 GMT
USER user
# Sat, 18 Jan 2020 05:20:05 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94079a590d0a41243d2c73a7f80d095fed025f2bc91ecba53a6fa01a602d54f2`  
		Last Modified: Sat, 18 Jan 2020 05:20:33 GMT  
		Size: 8.5 MB (8516143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2389694069ce07ceb540b166dbacd58df5db01de5b53a7b7eb70e03b010046`  
		Last Modified: Sat, 18 Jan 2020 05:20:29 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c930171b23884f8216e769bd4a98a38794efe4fe9b14be9d630a886dafc272b`  
		Last Modified: Sat, 18 Jan 2020 05:20:32 GMT  
		Size: 6.5 MB (6510922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:207c264f04e366c5bd1fb958a98a72b995af1ef534d9f0023bc03eaac2f84346
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19140791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d45b6d8eff3e11e1532c225b72d6e2948edcff1a40672f0f16c62f72c1014ae`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:15:17 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 18 Jan 2020 02:15:20 GMT
ENV HOME=/home/user
# Sat, 18 Jan 2020 02:15:26 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 18 Jan 2020 02:15:28 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 02:15:30 GMT
ENV IRSSI_VERSION=1.2.2
# Sat, 18 Jan 2020 02:16:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 18 Jan 2020 02:16:42 GMT
WORKDIR /home/user
# Sat, 18 Jan 2020 02:16:44 GMT
USER user
# Sat, 18 Jan 2020 02:16:45 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69e852f652474e05d47f735b6cd5f72da8c34afad334b50738688b19b0a4db4`  
		Last Modified: Sat, 18 Jan 2020 02:17:06 GMT  
		Size: 9.4 MB (9425621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6def3b6ee199ce1adf97bb4eeaa035b672219b0ee8b530d9d64d8cbade20bdd3`  
		Last Modified: Sat, 18 Jan 2020 02:17:02 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73860e239366f5942b9248b359261d13cc9f5f3bcfdf519862444ed2311678f1`  
		Last Modified: Sat, 18 Jan 2020 02:17:05 GMT  
		Size: 7.0 MB (6990825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; 386

```console
$ docker pull irssi@sha256:06ceaa49272143bc576a7ba5152770993749081dcf137f1fb1eb2013782a9651
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.9 MB (19947359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efd9498f6332d6dd2090dfa8ea6ebd973aae9d1ed9ae4c972432518e7e04603b`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 24 Dec 2019 19:38:57 GMT
ADD file:d0127a9692e8445993a88163cb741dbb23fa25436dd65289e76b08484264b397 in / 
# Tue, 24 Dec 2019 19:38:57 GMT
CMD ["/bin/sh"]
# Mon, 30 Dec 2019 22:40:08 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Mon, 30 Dec 2019 22:40:09 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:40:09 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:40:10 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:40:10 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:40:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Mon, 30 Dec 2019 22:40:58 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:40:58 GMT
USER user
# Mon, 30 Dec 2019 22:40:59 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:57bbc6f150623b3e4f01930af4ab2efa6ed5df02319341a08b1ce0bbd7e4afdf`  
		Last Modified: Tue, 24 Dec 2019 19:39:19 GMT  
		Size: 2.8 MB (2805146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff76006f62081ce832038868fe5b0b60ceed2187a08ed77ee36104006fbba791`  
		Last Modified: Mon, 30 Dec 2019 22:41:28 GMT  
		Size: 8.8 MB (8795524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db6f9ad44fed6961e6e5583a2858d76ed51e909d36e5f56257c2c3f01ec9aa3`  
		Last Modified: Mon, 30 Dec 2019 22:41:25 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbbf684b8369fac0090667874a96aa8959617cdf6f3e2efd898b900ee2271f00`  
		Last Modified: Mon, 30 Dec 2019 22:41:28 GMT  
		Size: 8.3 MB (8345445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:a4ee2c5582db1a8e3172e6b52c07a9d50751899e91c6fe9daf19a2db1fa377b8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.6 MB (19585238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1708846a38a9f626fbcde811f250e21368ce7d11f1a02dc0f62668375efaebcd`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:17:53 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 18 Jan 2020 04:17:59 GMT
ENV HOME=/home/user
# Sat, 18 Jan 2020 04:18:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 18 Jan 2020 04:18:09 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 04:18:12 GMT
ENV IRSSI_VERSION=1.2.2
# Sat, 18 Jan 2020 04:18:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 18 Jan 2020 04:19:00 GMT
WORKDIR /home/user
# Sat, 18 Jan 2020 04:19:03 GMT
USER user
# Sat, 18 Jan 2020 04:19:05 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cee495aeeccb8a9ca2b5b61da748591694470663de0f02e137bdb40886e1b1a`  
		Last Modified: Sat, 18 Jan 2020 04:19:40 GMT  
		Size: 9.5 MB (9521127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9dff5f290556e9df6faaefe25d1df97863e26a25255105adb22223ac042277`  
		Last Modified: Sat, 18 Jan 2020 04:19:36 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb398dcd302a5d86beba50e971e877dfc1df78f1dd0ba3be19395b75714c53d`  
		Last Modified: Sat, 18 Jan 2020 04:19:45 GMT  
		Size: 7.2 MB (7240714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:743262e0cf05ee5125863b88cda7b7377c3062926189f5e02a2b42df784f2cb2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.4 MB (19412058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ccf5f5bf85e76d9796ebb1c43c0e0bdf44eda4060d07dcb03f2ad6d9c96c1e5`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 18 Jan 2020 01:41:33 GMT
ADD file:a6f8b7d4ba199527053ef1ac710b5e318135cb6903cb9ad6fae4fe42e6ad0bf7 in / 
# Sat, 18 Jan 2020 01:41:33 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:18:41 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 18 Jan 2020 02:18:42 GMT
ENV HOME=/home/user
# Sat, 18 Jan 2020 02:18:42 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 18 Jan 2020 02:18:43 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 02:18:43 GMT
ENV IRSSI_VERSION=1.2.2
# Sat, 18 Jan 2020 02:19:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 18 Jan 2020 02:19:07 GMT
WORKDIR /home/user
# Sat, 18 Jan 2020 02:19:07 GMT
USER user
# Sat, 18 Jan 2020 02:19:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:176bad61a3a435da03ec603d2bd8f7a69286d92f21f447b17f21f0bc4e085bde`  
		Last Modified: Sat, 18 Jan 2020 01:41:59 GMT  
		Size: 2.6 MB (2582031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e137b1edc1565268f2019b28a1283c2b36e957c2009bb8ae076a030a13cb509`  
		Last Modified: Sat, 18 Jan 2020 02:19:21 GMT  
		Size: 9.8 MB (9834358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b03d27ba39922c28999efffd37fba89df9b0a24245f1a6512c36d8addc6d77`  
		Last Modified: Sat, 18 Jan 2020 02:19:20 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4f0c62b30ce5b338a1a15eae2c2181316c105dd21264175c162f3ae6c511f3`  
		Last Modified: Sat, 18 Jan 2020 02:19:21 GMT  
		Size: 7.0 MB (6994424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:alpine`

```console
$ docker pull irssi@sha256:53b6347f3c707a75a374b41b571d0bcbcce97d2a69c4130ef2901476ac751bab
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
$ docker pull irssi@sha256:e83aeb2a7084a795b1284c2516cf6ec658ffc6b1e9f1aa692391f75d88ed466a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.2 MB (19241142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3c5cc461cc163d5ec6d54832d0926a96cb206eafa515b3945aee2f605e516fa`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:13:07 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 18 Jan 2020 03:13:07 GMT
ENV HOME=/home/user
# Sat, 18 Jan 2020 03:13:08 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 18 Jan 2020 03:13:08 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 03:13:08 GMT
ENV IRSSI_VERSION=1.2.2
# Sat, 18 Jan 2020 03:13:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 18 Jan 2020 03:13:50 GMT
WORKDIR /home/user
# Sat, 18 Jan 2020 03:13:50 GMT
USER user
# Sat, 18 Jan 2020 03:13:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f318a8e84ae847d821a731ba55cd1a45783802db04e560d11e1e3c7538e5397`  
		Last Modified: Sat, 18 Jan 2020 03:14:05 GMT  
		Size: 9.4 MB (9422666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78354d333eb114a03dfe861868b5485c89a1356eaff9f656546233af1926b4fb`  
		Last Modified: Sat, 18 Jan 2020 03:14:02 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14774cc8271a38ba75ed5ce296e0330929d69d58a12218a597e64d9de32e6aa8`  
		Last Modified: Sat, 18 Jan 2020 03:14:04 GMT  
		Size: 7.0 MB (7014276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:342b2c19ea74b251a8c406ff065393a1826ac54052946813237158beea60ddfb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.4 MB (19363564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9260d7ed17bd0aa35c4da740d6f224880fcc65b175e242e816b586e973b33db0`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 24 Dec 2019 18:49:41 GMT
ADD file:c4f944e24d0f2e758363506e8b98b3b53973ec18dd4dd23da3f09520ef22c65c in / 
# Tue, 24 Dec 2019 18:49:42 GMT
CMD ["/bin/sh"]
# Mon, 30 Dec 2019 22:50:56 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Mon, 30 Dec 2019 22:51:02 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:51:08 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:51:10 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:51:13 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:52:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Mon, 30 Dec 2019 22:52:18 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:52:19 GMT
USER user
# Mon, 30 Dec 2019 22:52:19 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:546eec1e02ac5f4494868d8b22e8ced00773a2fba8e25b3edd30002889874299`  
		Last Modified: Tue, 24 Dec 2019 18:50:07 GMT  
		Size: 2.6 MB (2612021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e096f7e647acbccc301b850346b30db145dbc810757f233bbd4b9203c86d77a1`  
		Last Modified: Mon, 30 Dec 2019 22:52:36 GMT  
		Size: 8.7 MB (8665185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e252d91ac1eeb24eda441bc7025af739933267533fccbb1f5aca50534a8536`  
		Last Modified: Mon, 30 Dec 2019 22:52:32 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a7f820d727394e1780cfbc82d9c6cbb3b358c303cc6374fdf02405a913329b`  
		Last Modified: Mon, 30 Dec 2019 22:52:35 GMT  
		Size: 8.1 MB (8085085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:0ae5303301eb71e8a0ae6950e7a5444c1f4915d4cb995a345402a28d7594b6dc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17447893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93e2dfe3c6929bec1e86463bd93b9c895af9f7fead7afbd7a940c014c4f294b1`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:18:12 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 18 Jan 2020 05:18:23 GMT
ENV HOME=/home/user
# Sat, 18 Jan 2020 05:18:34 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 18 Jan 2020 05:18:41 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 05:18:47 GMT
ENV IRSSI_VERSION=1.2.2
# Sat, 18 Jan 2020 05:19:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 18 Jan 2020 05:20:01 GMT
WORKDIR /home/user
# Sat, 18 Jan 2020 05:20:03 GMT
USER user
# Sat, 18 Jan 2020 05:20:05 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94079a590d0a41243d2c73a7f80d095fed025f2bc91ecba53a6fa01a602d54f2`  
		Last Modified: Sat, 18 Jan 2020 05:20:33 GMT  
		Size: 8.5 MB (8516143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2389694069ce07ceb540b166dbacd58df5db01de5b53a7b7eb70e03b010046`  
		Last Modified: Sat, 18 Jan 2020 05:20:29 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c930171b23884f8216e769bd4a98a38794efe4fe9b14be9d630a886dafc272b`  
		Last Modified: Sat, 18 Jan 2020 05:20:32 GMT  
		Size: 6.5 MB (6510922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:207c264f04e366c5bd1fb958a98a72b995af1ef534d9f0023bc03eaac2f84346
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19140791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d45b6d8eff3e11e1532c225b72d6e2948edcff1a40672f0f16c62f72c1014ae`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:15:17 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 18 Jan 2020 02:15:20 GMT
ENV HOME=/home/user
# Sat, 18 Jan 2020 02:15:26 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 18 Jan 2020 02:15:28 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 02:15:30 GMT
ENV IRSSI_VERSION=1.2.2
# Sat, 18 Jan 2020 02:16:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 18 Jan 2020 02:16:42 GMT
WORKDIR /home/user
# Sat, 18 Jan 2020 02:16:44 GMT
USER user
# Sat, 18 Jan 2020 02:16:45 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69e852f652474e05d47f735b6cd5f72da8c34afad334b50738688b19b0a4db4`  
		Last Modified: Sat, 18 Jan 2020 02:17:06 GMT  
		Size: 9.4 MB (9425621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6def3b6ee199ce1adf97bb4eeaa035b672219b0ee8b530d9d64d8cbade20bdd3`  
		Last Modified: Sat, 18 Jan 2020 02:17:02 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73860e239366f5942b9248b359261d13cc9f5f3bcfdf519862444ed2311678f1`  
		Last Modified: Sat, 18 Jan 2020 02:17:05 GMT  
		Size: 7.0 MB (6990825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; 386

```console
$ docker pull irssi@sha256:06ceaa49272143bc576a7ba5152770993749081dcf137f1fb1eb2013782a9651
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.9 MB (19947359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efd9498f6332d6dd2090dfa8ea6ebd973aae9d1ed9ae4c972432518e7e04603b`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 24 Dec 2019 19:38:57 GMT
ADD file:d0127a9692e8445993a88163cb741dbb23fa25436dd65289e76b08484264b397 in / 
# Tue, 24 Dec 2019 19:38:57 GMT
CMD ["/bin/sh"]
# Mon, 30 Dec 2019 22:40:08 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Mon, 30 Dec 2019 22:40:09 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:40:09 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:40:10 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:40:10 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:40:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Mon, 30 Dec 2019 22:40:58 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:40:58 GMT
USER user
# Mon, 30 Dec 2019 22:40:59 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:57bbc6f150623b3e4f01930af4ab2efa6ed5df02319341a08b1ce0bbd7e4afdf`  
		Last Modified: Tue, 24 Dec 2019 19:39:19 GMT  
		Size: 2.8 MB (2805146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff76006f62081ce832038868fe5b0b60ceed2187a08ed77ee36104006fbba791`  
		Last Modified: Mon, 30 Dec 2019 22:41:28 GMT  
		Size: 8.8 MB (8795524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db6f9ad44fed6961e6e5583a2858d76ed51e909d36e5f56257c2c3f01ec9aa3`  
		Last Modified: Mon, 30 Dec 2019 22:41:25 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbbf684b8369fac0090667874a96aa8959617cdf6f3e2efd898b900ee2271f00`  
		Last Modified: Mon, 30 Dec 2019 22:41:28 GMT  
		Size: 8.3 MB (8345445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:a4ee2c5582db1a8e3172e6b52c07a9d50751899e91c6fe9daf19a2db1fa377b8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.6 MB (19585238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1708846a38a9f626fbcde811f250e21368ce7d11f1a02dc0f62668375efaebcd`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:17:53 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 18 Jan 2020 04:17:59 GMT
ENV HOME=/home/user
# Sat, 18 Jan 2020 04:18:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 18 Jan 2020 04:18:09 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 04:18:12 GMT
ENV IRSSI_VERSION=1.2.2
# Sat, 18 Jan 2020 04:18:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 18 Jan 2020 04:19:00 GMT
WORKDIR /home/user
# Sat, 18 Jan 2020 04:19:03 GMT
USER user
# Sat, 18 Jan 2020 04:19:05 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cee495aeeccb8a9ca2b5b61da748591694470663de0f02e137bdb40886e1b1a`  
		Last Modified: Sat, 18 Jan 2020 04:19:40 GMT  
		Size: 9.5 MB (9521127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9dff5f290556e9df6faaefe25d1df97863e26a25255105adb22223ac042277`  
		Last Modified: Sat, 18 Jan 2020 04:19:36 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb398dcd302a5d86beba50e971e877dfc1df78f1dd0ba3be19395b75714c53d`  
		Last Modified: Sat, 18 Jan 2020 04:19:45 GMT  
		Size: 7.2 MB (7240714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; s390x

```console
$ docker pull irssi@sha256:743262e0cf05ee5125863b88cda7b7377c3062926189f5e02a2b42df784f2cb2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.4 MB (19412058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ccf5f5bf85e76d9796ebb1c43c0e0bdf44eda4060d07dcb03f2ad6d9c96c1e5`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 18 Jan 2020 01:41:33 GMT
ADD file:a6f8b7d4ba199527053ef1ac710b5e318135cb6903cb9ad6fae4fe42e6ad0bf7 in / 
# Sat, 18 Jan 2020 01:41:33 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:18:41 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 18 Jan 2020 02:18:42 GMT
ENV HOME=/home/user
# Sat, 18 Jan 2020 02:18:42 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 18 Jan 2020 02:18:43 GMT
ENV LANG=C.UTF-8
# Sat, 18 Jan 2020 02:18:43 GMT
ENV IRSSI_VERSION=1.2.2
# Sat, 18 Jan 2020 02:19:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 18 Jan 2020 02:19:07 GMT
WORKDIR /home/user
# Sat, 18 Jan 2020 02:19:07 GMT
USER user
# Sat, 18 Jan 2020 02:19:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:176bad61a3a435da03ec603d2bd8f7a69286d92f21f447b17f21f0bc4e085bde`  
		Last Modified: Sat, 18 Jan 2020 01:41:59 GMT  
		Size: 2.6 MB (2582031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e137b1edc1565268f2019b28a1283c2b36e957c2009bb8ae076a030a13cb509`  
		Last Modified: Sat, 18 Jan 2020 02:19:21 GMT  
		Size: 9.8 MB (9834358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b03d27ba39922c28999efffd37fba89df9b0a24245f1a6512c36d8addc6d77`  
		Last Modified: Sat, 18 Jan 2020 02:19:20 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4f0c62b30ce5b338a1a15eae2c2181316c105dd21264175c162f3ae6c511f3`  
		Last Modified: Sat, 18 Jan 2020 02:19:21 GMT  
		Size: 7.0 MB (6994424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:latest`

```console
$ docker pull irssi@sha256:10d70bb9912ee6af38e32c68e5147774527371b837d2e96c38496cbd89c460af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `irssi:latest` - linux; amd64

```console
$ docker pull irssi@sha256:94ade928c56069ab24e07a671d461627157bfc4b4c75cddc7e0eef74dc429668
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50512777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:071f6fdb9d31c1fdb38e00b3f4aa5f35f0488bf3f0be7ec47c8609d9b77f7d82`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 22:19:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 22:19:55 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:19:55 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:19:56 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:19:56 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:20:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 22:20:56 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:20:56 GMT
USER user
# Mon, 30 Dec 2019 22:20:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155ffa1aba8607e36ef345d54c69e06dff0957646eb0a3ff4ea1f247f2d6f834`  
		Last Modified: Mon, 30 Dec 2019 22:22:11 GMT  
		Size: 17.0 MB (16987485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c035b099bd2ec74cb6afce844b250fd133eb9632293848ada2628bdbc84f1db`  
		Last Modified: Mon, 30 Dec 2019 22:22:06 GMT  
		Size: 4.2 KB (4181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32794dd5d2b6704bd7908f83a0bc9c91af102b15cb616927fc7c5aa4e1917f2`  
		Last Modified: Mon, 30 Dec 2019 22:22:08 GMT  
		Size: 6.4 MB (6428837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm variant v5

```console
$ docker pull irssi@sha256:0e2ffdb40c1813fcd5d664cd43f803e9fae16d23158c37a0a3a77ee6f9c6ea30
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46786540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2429596187b3420620bfa930a489829d17b7ae16f68a5e12f468600ead30f6b0`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:49:50 GMT
ADD file:5d34c769f80c3fdbb04048f4336cf212164934607a642144ef557faef5896192 in / 
# Sat, 28 Dec 2019 04:49:51 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 22:49:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 22:49:11 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:49:13 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:49:14 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:49:14 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:51:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 22:51:50 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:51:51 GMT
USER user
# Mon, 30 Dec 2019 22:51:53 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:153ccec980772b5fc4c786af0b26bba09f0a2d95d9755400febf9a79aa4220c8`  
		Last Modified: Sat, 28 Dec 2019 04:56:28 GMT  
		Size: 24.8 MB (24829618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa69714a630c9112cb8ed12a6a0c9ae434a0a7195c6e4f68933886f7fd1983f`  
		Last Modified: Mon, 30 Dec 2019 22:52:22 GMT  
		Size: 15.9 MB (15890061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab31781254acfc5b427e96a9157a02a9ba33029a2005b185eb5269c4163787d`  
		Last Modified: Mon, 30 Dec 2019 22:52:11 GMT  
		Size: 4.2 KB (4205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6924de57ca5fe0466f8a204c8e8f92726d55e29433871e0a91aba15f983c8c`  
		Last Modified: Mon, 30 Dec 2019 22:52:14 GMT  
		Size: 6.1 MB (6062656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm variant v7

```console
$ docker pull irssi@sha256:4ac9143ebda80df861793e06c1ab529a0c82cbc5fbb1467ad6f905a717d1242f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44188477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebc901e04efd19e1b84420fee3ddabfa2c5e0f65bf74941175283da2815154aa`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 23:02:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 23:02:55 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 23:02:57 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 23:02:58 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 23:02:58 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 23:04:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 23:04:30 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 23:04:31 GMT
USER user
# Mon, 30 Dec 2019 23:04:32 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09075676a7576165b8ed1990b233d29b4a112b50d5957c1a1c8cbf0c1853dc76`  
		Last Modified: Mon, 30 Dec 2019 23:06:11 GMT  
		Size: 15.6 MB (15554857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373ec572d9c27ba5c4b59943b257138a84a107907c938b6300b34503f7f2e602`  
		Last Modified: Mon, 30 Dec 2019 23:06:03 GMT  
		Size: 4.2 KB (4197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec006cec70b4f55bcb3b95111258702e778f90ad5362b4c08bc1b87f10b405e2`  
		Last Modified: Mon, 30 Dec 2019 23:06:05 GMT  
		Size: 5.9 MB (5930294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:52d0ead408e844bba3ea08864d9ee1ce400727f99711658a332c8ab953b41ae7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49005367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13e82aa16b7576863ef36d2b9ffce9df153f1aa8177e97e220143821458a55a7`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 22:41:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 22:41:08 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:41:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:41:10 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:41:11 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:42:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 22:42:54 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:42:56 GMT
USER user
# Mon, 30 Dec 2019 22:42:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc97913e2d0d8cb44f6fd5a47a49974057573a753cf66d3212046b6c376fd9f0`  
		Last Modified: Mon, 30 Dec 2019 22:44:30 GMT  
		Size: 16.8 MB (16762627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0709e009ad51ad0a0ec48f8c3c0b0de4fd412ad5b3b42e53757cec282180e87`  
		Last Modified: Mon, 30 Dec 2019 22:44:23 GMT  
		Size: 4.2 KB (4215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c555b242ddbe0e9335602cbdca56f5c307d560b4635c31338861407810b9945`  
		Last Modified: Mon, 30 Dec 2019 22:44:25 GMT  
		Size: 6.4 MB (6387823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; 386

```console
$ docker pull irssi@sha256:c5e4274b633a2d299ec9af52d580010154758ada9929bb758022334ac968820e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50367637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdbe22cc632c3d69ce50527e20598a64ea33d2dbffff7cdd42ccff0be736b6ac`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 22:38:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 22:38:37 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:38:38 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:38:38 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:38:38 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:39:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 22:39:57 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:39:57 GMT
USER user
# Mon, 30 Dec 2019 22:39:57 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72221f577a2f5220d3b7671a23bbf707e559dc20fd260e9e321a3bca8bf4e7fc`  
		Last Modified: Mon, 30 Dec 2019 22:41:20 GMT  
		Size: 16.5 MB (16515220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e488155fc2527b4ab798931fac3fa6f7521f5e687e0c82ea1cf007b495ea88`  
		Last Modified: Mon, 30 Dec 2019 22:41:14 GMT  
		Size: 4.2 KB (4170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07b243b29fe05690820a603d2c31463dbe08ca974efc99b033aca2703d9ac65`  
		Last Modified: Mon, 30 Dec 2019 22:41:16 GMT  
		Size: 6.1 MB (6101227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; ppc64le

```console
$ docker pull irssi@sha256:aabbe2ff8e02fa9376da9c3d21d0f747aee3e97fcf372951d07e85252732b28a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.7 MB (54698717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8c59fc543020e65db22f51fb7a5f22a0bdb0284f7a68619e2daeac2a6d27567`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 22:18:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 22:18:43 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:18:51 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:18:53 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:18:55 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:23:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 22:23:22 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:23:24 GMT
USER user
# Mon, 30 Dec 2019 22:23:26 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4a48662b243e889598e0a1b8e2a224407e08aa8c152a7b96352dc261c2b903`  
		Last Modified: Mon, 30 Dec 2019 22:25:36 GMT  
		Size: 17.4 MB (17396769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bd95038cb0e8d80e4cb33f7dbe1b0ae5c5b33f2f63955c2eafabeacead3d95`  
		Last Modified: Mon, 30 Dec 2019 22:25:30 GMT  
		Size: 4.2 KB (4219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d27ae35ac7ced8f7f75a99531f03b1e8e174a10f78c8c77acfc606ef3a1c40`  
		Last Modified: Mon, 30 Dec 2019 22:25:31 GMT  
		Size: 6.8 MB (6780200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; s390x

```console
$ docker pull irssi@sha256:b265d21e8baf744ec4ed0e1a75b3bb821b3b7cdc75cad870581f37a461d734a5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48951117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10fb4e99edc6f16e535536593259d9363aa1b59890a278a793360a6a601b02a9`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:42:03 GMT
ADD file:eec6c56f8680753860198c3af0d94aabb87018ca30f6f6e346621a6bffe0e4b8 in / 
# Sat, 28 Dec 2019 04:42:04 GMT
CMD ["bash"]
# Mon, 30 Dec 2019 22:41:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 Dec 2019 22:41:41 GMT
ENV HOME=/home/user
# Mon, 30 Dec 2019 22:41:42 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 30 Dec 2019 22:41:42 GMT
ENV LANG=C.UTF-8
# Mon, 30 Dec 2019 22:41:43 GMT
ENV IRSSI_VERSION=1.2.2
# Mon, 30 Dec 2019 22:42:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Mon, 30 Dec 2019 22:42:36 GMT
WORKDIR /home/user
# Mon, 30 Dec 2019 22:42:36 GMT
USER user
# Mon, 30 Dec 2019 22:42:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f7542f43e95fb32a870ee38d7f0e7bb23267ac8dcf709e3944311b0a30d7a479`  
		Last Modified: Sat, 28 Dec 2019 04:45:08 GMT  
		Size: 25.7 MB (25705315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3021cd15a7c1a65d381978e66c420a23e06b0714cb8038e6937152fbd77e6740`  
		Last Modified: Mon, 30 Dec 2019 22:43:35 GMT  
		Size: 16.9 MB (16858905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8176e43a5836b18e5ec920d3c606074b54d1ba1dfe4552fd0d71e0e419c56113`  
		Last Modified: Mon, 30 Dec 2019 22:43:31 GMT  
		Size: 4.2 KB (4189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3213bdc14a62074eb7cbd9519f9599043778dd6c5bbe78299eb33914f2eaddc2`  
		Last Modified: Mon, 30 Dec 2019 22:43:32 GMT  
		Size: 6.4 MB (6382708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
