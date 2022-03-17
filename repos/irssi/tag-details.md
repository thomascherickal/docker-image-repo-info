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
$ docker pull irssi@sha256:4cf3922f3d3b1291213df558ff37994ccb444dfb82fe52c77e32745859de3dc3
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
$ docker pull irssi@sha256:f7fbe756507d2f554079dc2fa72b755ea95e4704b658a88744bcef74fe34cb4e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50615106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf4c02131292a1e862292b323babd939f1776a6a4dc2bd3a74b62a23ee32611f`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:56 GMT
ADD file:702017714ad3e1567b4f60b688750f8b631d91088e4dcf41351c4bb07749c579 in / 
# Tue, 01 Mar 2022 02:13:56 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 13:22:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 13:22:06 GMT
ENV HOME=/home/user
# Tue, 01 Mar 2022 13:22:07 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 01 Mar 2022 13:22:07 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 13:22:07 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 01 Mar 2022 13:24:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 01 Mar 2022 13:24:04 GMT
WORKDIR /home/user
# Tue, 01 Mar 2022 13:24:04 GMT
USER user
# Tue, 01 Mar 2022 13:24:04 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:15115158dd02a1bf2fd28724e3c1024394033fb0e9a5d3e451ed2715b6ae312d`  
		Last Modified: Tue, 01 Mar 2022 02:20:08 GMT  
		Size: 27.2 MB (27153737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8700bed9c2318ddf3095e460ab4319bfc16f6aa57ef33cb8d9b23cec47e466e5`  
		Last Modified: Tue, 01 Mar 2022 13:24:34 GMT  
		Size: 17.0 MB (17023729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d367b585ce183067e4c669de040f569d8ae360ee487aad70f804bb9c482688b6`  
		Last Modified: Tue, 01 Mar 2022 13:24:29 GMT  
		Size: 4.2 KB (4206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0573347742f32ca00d17c18d7df270a960bfff93aefabdd083f50043169f0a`  
		Last Modified: Tue, 01 Mar 2022 13:24:31 GMT  
		Size: 6.4 MB (6433434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm variant v5

```console
$ docker pull irssi@sha256:705f8349cbef27f5bfec1e6a615ce371629eda97ffbaeb77cc8ab233df645202
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46877530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68942e15850cffade567e213f49f99710a48f64c4f220ba0198d104a67aa8630`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 17 Mar 2022 05:20:46 GMT
ADD file:4b7bce60b3e3455ba9b14c881ffa61187b9e56365fe4f275ee871e7c7e930fb9 in / 
# Thu, 17 Mar 2022 05:20:46 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 10:03:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 10:03:08 GMT
ENV HOME=/home/user
# Thu, 17 Mar 2022 10:03:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Mar 2022 10:03:11 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 10:03:11 GMT
ENV IRSSI_VERSION=1.2.3
# Thu, 17 Mar 2022 10:05:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 17 Mar 2022 10:05:22 GMT
WORKDIR /home/user
# Thu, 17 Mar 2022 10:05:22 GMT
USER user
# Thu, 17 Mar 2022 10:05:23 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f193682138b0c37054cb843ef2155a75706f248a369d454bf6444833f120aefc`  
		Last Modified: Thu, 17 Mar 2022 05:36:29 GMT  
		Size: 24.9 MB (24886195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8afac93444b98f19bbf672aab4b0b358eaf47b0e952385ab7d4ad839380315f`  
		Last Modified: Thu, 17 Mar 2022 10:06:11 GMT  
		Size: 15.9 MB (15922671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3389c88e912002d546288257f98a7208ca19f801c85b55949571bc65dfb3be95`  
		Last Modified: Thu, 17 Mar 2022 10:05:55 GMT  
		Size: 4.2 KB (4194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b655b41133cb19826b4d711323336615269f792f53c1affd769ac1d0bd026e`  
		Last Modified: Thu, 17 Mar 2022 10:05:59 GMT  
		Size: 6.1 MB (6064470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm variant v7

```console
$ docker pull irssi@sha256:a04ab92ea03c301760bfcb9a9ddc09b38c10e732e563c7f83417e653a57def8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44273440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de2c18377805a7d11fd2cac579e7e5a42acb66e2d843b1565b34479eca7ee4ce`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 01 Mar 2022 02:04:06 GMT
ADD file:d73a3eaf767825b31d0c0189624b35193e5ad7c5907f839edf6f7917036c2d0b in / 
# Tue, 01 Mar 2022 02:04:07 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 03:09:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 03:09:59 GMT
ENV HOME=/home/user
# Wed, 02 Mar 2022 03:10:01 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 02 Mar 2022 03:10:01 GMT
ENV LANG=C.UTF-8
# Wed, 02 Mar 2022 03:10:02 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 02 Mar 2022 03:11:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 02 Mar 2022 03:11:53 GMT
WORKDIR /home/user
# Wed, 02 Mar 2022 03:11:53 GMT
USER user
# Wed, 02 Mar 2022 03:11:53 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1acfd43b1a25aefe6117ba65bf2b46a19e3cf8e72b76f522a9fe299412e1c5f2`  
		Last Modified: Tue, 01 Mar 2022 02:20:32 GMT  
		Size: 22.8 MB (22754370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ed1c914999ce09a5850058fd4296c038ca35c13723a147f50f4ea54030ce56`  
		Last Modified: Wed, 02 Mar 2022 03:13:17 GMT  
		Size: 15.6 MB (15582331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c242f6ecab39401dfa1b4a8a1e2b62f2d7b4b39d6078dc30923f804bccc8682e`  
		Last Modified: Wed, 02 Mar 2022 03:13:01 GMT  
		Size: 4.2 KB (4198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf212b512b9ef8774b21073f37a32c29b65e1ce1e2cd268ec57cc24307c5de7`  
		Last Modified: Wed, 02 Mar 2022 03:13:05 GMT  
		Size: 5.9 MB (5932541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:cfbea9d7f15b725e78d979c1bf7d87474787f2187fa1810dc5655ab4c428ea6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48899457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7c7d9962e5408ee8ae38eed4b82aece41486bf9d7accd086a3f49fead974c85`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 17 Mar 2022 03:22:22 GMT
ADD file:1c7d8cedf5dc79c676acebde5252ecd3005088a9f29e5e6be547f659f41efb1f in / 
# Thu, 17 Mar 2022 03:22:22 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 11:33:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 11:33:14 GMT
ENV HOME=/home/user
# Thu, 17 Mar 2022 11:33:15 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Mar 2022 11:33:16 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 11:33:17 GMT
ENV IRSSI_VERSION=1.2.3
# Thu, 17 Mar 2022 11:34:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 17 Mar 2022 11:34:48 GMT
WORKDIR /home/user
# Thu, 17 Mar 2022 11:34:49 GMT
USER user
# Thu, 17 Mar 2022 11:34:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c9277cac12165646c33f028489f2a5be3f70745382f4385cd9ed12fcc8cec183`  
		Last Modified: Thu, 17 Mar 2022 03:29:27 GMT  
		Size: 25.9 MB (25923233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68765394fa26a3242947ab026ed84ac73743ba6ea3e9a2a9d5737690f740fffc`  
		Last Modified: Thu, 17 Mar 2022 11:35:22 GMT  
		Size: 16.8 MB (16796123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21216d974d85d8cec172d4aaa29778089c01fdc9243095fb6f361b271192c2e7`  
		Last Modified: Thu, 17 Mar 2022 11:35:19 GMT  
		Size: 4.1 KB (4070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250f896ea3e4765f7fa9882e890c8e909365aa358c3f991edd0342196cc1d800`  
		Last Modified: Thu, 17 Mar 2022 11:35:20 GMT  
		Size: 6.2 MB (6176031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; 386

```console
$ docker pull irssi@sha256:c0a62d463fb49bf3a69db179c0b60cbf4ff7b833d2a60152845a9f8a59e4ddf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50461133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89610068bce58bafeb0e193d0af06b4814dd55faf0b65f98bb7bbd4ff24dbaee`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:04 GMT
ADD file:d9d384f0402bc696e46e7529f52d64859a66aa7a60bca9c7beee7433a5f7af6e in / 
# Tue, 01 Mar 2022 02:08:04 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 04:25:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 04:25:16 GMT
ENV HOME=/home/user
# Wed, 02 Mar 2022 04:25:16 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 02 Mar 2022 04:25:16 GMT
ENV LANG=C.UTF-8
# Wed, 02 Mar 2022 04:25:17 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 02 Mar 2022 04:27:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 02 Mar 2022 04:27:06 GMT
WORKDIR /home/user
# Wed, 02 Mar 2022 04:27:06 GMT
USER user
# Wed, 02 Mar 2022 04:27:06 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c761ce6f2bf0aed07e1198c6f827444969d6e76dda0e55dbb45900920e551d27`  
		Last Modified: Tue, 01 Mar 2022 02:16:51 GMT  
		Size: 27.8 MB (27804590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139be6db820715ec1020fa6d907904a005ff26671f494921c2506cd6bf6a1fc7`  
		Last Modified: Wed, 02 Mar 2022 04:27:55 GMT  
		Size: 16.5 MB (16546984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9b7833f654b31e47588af045ee76e67df88bda2bf2566244c615c18c20edcd`  
		Last Modified: Wed, 02 Mar 2022 04:27:49 GMT  
		Size: 4.2 KB (4193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18696806ef255bda2c34fb5e2b87634943be45ec61cd03501c556d28f210be32`  
		Last Modified: Wed, 02 Mar 2022 04:27:50 GMT  
		Size: 6.1 MB (6105366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; mips64le

```console
$ docker pull irssi@sha256:389489d914e16b932ada3ede3ab90571cf0b8ed0dc925c24217ebdf6d49e5958
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47815154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d367c047358f8297275e01ed32a0837b3dd6387204bd751b52b57afeaefd124`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 01 Mar 2022 02:03:50 GMT
ADD file:f681a18b03e8f8590fb85a806e2c18b3ee2e69fb1a4db7eb933bafb8e7784672 in / 
# Tue, 01 Mar 2022 02:03:50 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:39:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:39:39 GMT
ENV HOME=/home/user
# Tue, 01 Mar 2022 03:39:41 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 01 Mar 2022 03:39:41 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 03:39:41 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 01 Mar 2022 03:42:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 01 Mar 2022 03:42:15 GMT
WORKDIR /home/user
# Tue, 01 Mar 2022 03:42:15 GMT
USER user
# Tue, 01 Mar 2022 03:42:16 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:678634e0b2f87341687ab30235502da4100c2eeafae836b9a671b39e8f7a6da6`  
		Last Modified: Tue, 01 Mar 2022 02:13:43 GMT  
		Size: 25.8 MB (25820204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dcd5e55972035085c7b445e82036cb268e79ab06125f32846c6d7d09dfc7818`  
		Last Modified: Tue, 01 Mar 2022 03:42:52 GMT  
		Size: 15.7 MB (15698106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87570cd46d25689999bce4c019946c4dbe28e5bcb98cf662b8e71b9a2b703b9e`  
		Last Modified: Tue, 01 Mar 2022 03:42:37 GMT  
		Size: 4.2 KB (4179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9096bd6071c77f200e81cca853f3d5d487fc19c0b2048be069c310463d328a5f`  
		Last Modified: Tue, 01 Mar 2022 03:42:42 GMT  
		Size: 6.3 MB (6292665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; ppc64le

```console
$ docker pull irssi@sha256:ca0cbe669ac6398f2eb51fcf038bdce16b96b525083a168612970d1a98f03f08
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54780862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dcdb27db5db000dcf123fce18d1ec14d9f9d5e97f409bb00ada7d5af06ce702`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:48 GMT
ADD file:d87bdffbd9392364fecbbd4148c710bc4948073e773a47c7b9ac1440ebb81c1e in / 
# Wed, 26 Jan 2022 01:47:52 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 22:56:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 22:56:44 GMT
ENV HOME=/home/user
# Wed, 26 Jan 2022 22:56:52 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 26 Jan 2022 22:56:55 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 22:56:59 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 26 Feb 2022 07:38:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 26 Feb 2022 07:38:45 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 07:38:48 GMT
USER user
# Sat, 26 Feb 2022 07:38:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:249357001395b3de58d51723447880f3205d37ea7b902930b5c19f475d4ac8f9`  
		Last Modified: Wed, 26 Jan 2022 01:58:50 GMT  
		Size: 30.6 MB (30562293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76bc6146d874e1a9052b35c297c2dff10eaee69237da9378b2bfa882979e0bb3`  
		Last Modified: Wed, 26 Jan 2022 23:02:16 GMT  
		Size: 17.4 MB (17431167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e871dca1ce277370e3982e11fe9c1cba8e00453eb8e8811efb3a94263a14f0`  
		Last Modified: Wed, 26 Jan 2022 23:02:11 GMT  
		Size: 4.2 KB (4209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253429c0ce6eb715394ea364326563971970bd616f44d6ca025f6fe6ab53ece9`  
		Last Modified: Sat, 26 Feb 2022 07:42:02 GMT  
		Size: 6.8 MB (6783193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; s390x

```console
$ docker pull irssi@sha256:78392a13b131218daad3553dede975d5b4b89c7251462f032c4b3c68653d9a54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49057865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74d95e118adfe6bdb8df2dc4bb9c9a71cb9fcf6773cad51f0ccb2285a27ec8e1`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 17 Mar 2022 03:07:30 GMT
ADD file:4342e1d9db757e91953273ac7120c9d6004d38281f9cea830898b4f35ca43517 in / 
# Thu, 17 Mar 2022 03:07:32 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:45:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 08:45:20 GMT
ENV HOME=/home/user
# Thu, 17 Mar 2022 08:45:21 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Mar 2022 08:45:21 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 08:45:21 GMT
ENV IRSSI_VERSION=1.2.3
# Thu, 17 Mar 2022 08:46:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 17 Mar 2022 08:46:26 GMT
WORKDIR /home/user
# Thu, 17 Mar 2022 08:46:26 GMT
USER user
# Thu, 17 Mar 2022 08:46:26 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6f8a08956872b0f67802da3a67e007322eb963a60e0dadd736077f3ece414e1f`  
		Last Modified: Thu, 17 Mar 2022 03:13:18 GMT  
		Size: 25.8 MB (25769076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af379668e3c95c8de70aaa50b0ea29fe79a526bab60441728ccef56d47a62994`  
		Last Modified: Thu, 17 Mar 2022 08:47:09 GMT  
		Size: 16.9 MB (16899875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8388b5dcf6fd417cdc18b27d3ffa8e19adfeed5396e63f48c4637b130fac0ffe`  
		Last Modified: Thu, 17 Mar 2022 08:47:07 GMT  
		Size: 4.2 KB (4209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508a5e3ccb88964d11fab7a1eea4d169bba20fffe9fab44bccd320d559b443da`  
		Last Modified: Thu, 17 Mar 2022 08:47:07 GMT  
		Size: 6.4 MB (6384705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1-alpine`

```console
$ docker pull irssi@sha256:bc6f96bc4d36d1fc63af4e6b07d68cbe12f15cc806aa3fc90d8c14cbc2aee398
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
$ docker pull irssi@sha256:e81de68bf0b471e0b77ad913541a1f32206fcb8c80fac98a0d9d1350478ac605
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18658093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dead0fe2265236caa74a87944b897072c3db257ea60dcd26ad0f8c8a0a57695`
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
# Sat, 26 Feb 2022 02:42:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 26 Feb 2022 02:42:56 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 02:42:56 GMT
USER user
# Sat, 26 Feb 2022 02:42:56 GMT
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
	-	`sha256:c805e6f5481d38ada6303ac8752840cc587fd0cb676315c10e5c3b97f6dda3e0`  
		Last Modified: Sat, 26 Feb 2022 02:43:33 GMT  
		Size: 6.3 MB (6287505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:f47d5355f67178d363007d5ceb085dc5c31a7474d8dd3717e7a49d016b60d623
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17399747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4440bf00c51e7e1118c662cdcc138a9fc2eb71c6412c3e599195855da1833f5`
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
# Sat, 26 Feb 2022 00:50:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 26 Feb 2022 00:50:54 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 00:50:55 GMT
USER user
# Sat, 26 Feb 2022 00:50:55 GMT
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
	-	`sha256:02c9f2e6dd64e4cf27098cee126ac7e8d3fd7da82e492cd105a0855f350e1d5e`  
		Last Modified: Sat, 26 Feb 2022 00:51:30 GMT  
		Size: 6.0 MB (5987187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:b5190f02bed9f5deb8cd5b609a1e2fcdaf81964aed345fdbaad7b03022356184
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16852378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0211dae8af4e7ddf998d09cb63324461a5d1253fe8997b8d9f2f53a652176f6a`
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
# Sun, 27 Feb 2022 17:01:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sun, 27 Feb 2022 17:01:30 GMT
WORKDIR /home/user
# Sun, 27 Feb 2022 17:01:30 GMT
USER user
# Sun, 27 Feb 2022 17:01:31 GMT
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
	-	`sha256:e03549227edb8b9530872c983ea5e12a413ab939a91e2dcfa926e688ab1dfe1b`  
		Last Modified: Sun, 27 Feb 2022 17:02:52 GMT  
		Size: 5.8 MB (5783760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:15723ad078da19b6695e1c007f755845c6eebd425c8996fc5a2fa161c2080827
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18511732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de0cea899c59de043e14df141069f11d0af7786ca6767a0ca831e95cd7d5bb54`
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
# Sat, 26 Feb 2022 16:42:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 26 Feb 2022 16:42:55 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 16:42:56 GMT
USER user
# Sat, 26 Feb 2022 16:42:57 GMT
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
	-	`sha256:6301442fae9080fb1e5e73ffa49744ab8e62d3dd0af210c3b69a0452c404369c`  
		Last Modified: Sat, 26 Feb 2022 16:43:43 GMT  
		Size: 6.2 MB (6247302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; 386

```console
$ docker pull irssi@sha256:a6c042d635bd7236909e92fb986ea4e9491d19bc3a3d8c8d7f811dee24654b15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17723361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c56ee7059678cc766ade98d596931e5b43d0ddf53e5796344669386e5da7379`
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
# Sat, 26 Feb 2022 16:42:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 26 Feb 2022 16:42:02 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 16:42:02 GMT
USER user
# Sat, 26 Feb 2022 16:42:02 GMT
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
	-	`sha256:ed7782fd3151038808a645b6f78522a79eb588e18ff6d72ffe3a99be2ce38ad3`  
		Last Modified: Sat, 26 Feb 2022 16:42:52 GMT  
		Size: 6.0 MB (5978954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:256febb4e88caa7803e51f3bc7bc6d08a2ee593d903986b0048bb9f2a3adf1dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.0 MB (18956324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c7163a5875310136dafbc963f6cd5ff2f3e2a661335157c1122fab4bbd8b961`
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
# Sat, 26 Feb 2022 07:41:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 26 Feb 2022 07:41:20 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 07:41:23 GMT
USER user
# Sat, 26 Feb 2022 07:41:29 GMT
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
	-	`sha256:b020c19f58e52afc93f0a890fe6012615a585c053cb4cf0da4571f3eb92ac642`  
		Last Modified: Sat, 26 Feb 2022 07:42:26 GMT  
		Size: 6.5 MB (6492301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:50bdb230f1994347e42ae29828177ee13eaaecb603ee60b6a9d294ea0b7d7aa7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18872134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e2a07a0958db17c3a111679879c59fd06187e002b2f6b0fa605868f44f821b9`
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
# Sat, 26 Feb 2022 00:44:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 26 Feb 2022 00:44:16 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 00:44:16 GMT
USER user
# Sat, 26 Feb 2022 00:44:16 GMT
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
	-	`sha256:647b0b24f0a4c27c905b049227cf6d0f7f4c0626fee67a796e2a2a5f234a9632`  
		Last Modified: Sat, 26 Feb 2022 00:44:58 GMT  
		Size: 6.3 MB (6276948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2`

```console
$ docker pull irssi@sha256:4cf3922f3d3b1291213df558ff37994ccb444dfb82fe52c77e32745859de3dc3
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
$ docker pull irssi@sha256:f7fbe756507d2f554079dc2fa72b755ea95e4704b658a88744bcef74fe34cb4e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50615106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf4c02131292a1e862292b323babd939f1776a6a4dc2bd3a74b62a23ee32611f`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:56 GMT
ADD file:702017714ad3e1567b4f60b688750f8b631d91088e4dcf41351c4bb07749c579 in / 
# Tue, 01 Mar 2022 02:13:56 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 13:22:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 13:22:06 GMT
ENV HOME=/home/user
# Tue, 01 Mar 2022 13:22:07 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 01 Mar 2022 13:22:07 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 13:22:07 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 01 Mar 2022 13:24:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 01 Mar 2022 13:24:04 GMT
WORKDIR /home/user
# Tue, 01 Mar 2022 13:24:04 GMT
USER user
# Tue, 01 Mar 2022 13:24:04 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:15115158dd02a1bf2fd28724e3c1024394033fb0e9a5d3e451ed2715b6ae312d`  
		Last Modified: Tue, 01 Mar 2022 02:20:08 GMT  
		Size: 27.2 MB (27153737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8700bed9c2318ddf3095e460ab4319bfc16f6aa57ef33cb8d9b23cec47e466e5`  
		Last Modified: Tue, 01 Mar 2022 13:24:34 GMT  
		Size: 17.0 MB (17023729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d367b585ce183067e4c669de040f569d8ae360ee487aad70f804bb9c482688b6`  
		Last Modified: Tue, 01 Mar 2022 13:24:29 GMT  
		Size: 4.2 KB (4206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0573347742f32ca00d17c18d7df270a960bfff93aefabdd083f50043169f0a`  
		Last Modified: Tue, 01 Mar 2022 13:24:31 GMT  
		Size: 6.4 MB (6433434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; arm variant v5

```console
$ docker pull irssi@sha256:705f8349cbef27f5bfec1e6a615ce371629eda97ffbaeb77cc8ab233df645202
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46877530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68942e15850cffade567e213f49f99710a48f64c4f220ba0198d104a67aa8630`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 17 Mar 2022 05:20:46 GMT
ADD file:4b7bce60b3e3455ba9b14c881ffa61187b9e56365fe4f275ee871e7c7e930fb9 in / 
# Thu, 17 Mar 2022 05:20:46 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 10:03:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 10:03:08 GMT
ENV HOME=/home/user
# Thu, 17 Mar 2022 10:03:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Mar 2022 10:03:11 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 10:03:11 GMT
ENV IRSSI_VERSION=1.2.3
# Thu, 17 Mar 2022 10:05:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 17 Mar 2022 10:05:22 GMT
WORKDIR /home/user
# Thu, 17 Mar 2022 10:05:22 GMT
USER user
# Thu, 17 Mar 2022 10:05:23 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f193682138b0c37054cb843ef2155a75706f248a369d454bf6444833f120aefc`  
		Last Modified: Thu, 17 Mar 2022 05:36:29 GMT  
		Size: 24.9 MB (24886195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8afac93444b98f19bbf672aab4b0b358eaf47b0e952385ab7d4ad839380315f`  
		Last Modified: Thu, 17 Mar 2022 10:06:11 GMT  
		Size: 15.9 MB (15922671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3389c88e912002d546288257f98a7208ca19f801c85b55949571bc65dfb3be95`  
		Last Modified: Thu, 17 Mar 2022 10:05:55 GMT  
		Size: 4.2 KB (4194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b655b41133cb19826b4d711323336615269f792f53c1affd769ac1d0bd026e`  
		Last Modified: Thu, 17 Mar 2022 10:05:59 GMT  
		Size: 6.1 MB (6064470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; arm variant v7

```console
$ docker pull irssi@sha256:a04ab92ea03c301760bfcb9a9ddc09b38c10e732e563c7f83417e653a57def8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44273440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de2c18377805a7d11fd2cac579e7e5a42acb66e2d843b1565b34479eca7ee4ce`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 01 Mar 2022 02:04:06 GMT
ADD file:d73a3eaf767825b31d0c0189624b35193e5ad7c5907f839edf6f7917036c2d0b in / 
# Tue, 01 Mar 2022 02:04:07 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 03:09:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 03:09:59 GMT
ENV HOME=/home/user
# Wed, 02 Mar 2022 03:10:01 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 02 Mar 2022 03:10:01 GMT
ENV LANG=C.UTF-8
# Wed, 02 Mar 2022 03:10:02 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 02 Mar 2022 03:11:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 02 Mar 2022 03:11:53 GMT
WORKDIR /home/user
# Wed, 02 Mar 2022 03:11:53 GMT
USER user
# Wed, 02 Mar 2022 03:11:53 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1acfd43b1a25aefe6117ba65bf2b46a19e3cf8e72b76f522a9fe299412e1c5f2`  
		Last Modified: Tue, 01 Mar 2022 02:20:32 GMT  
		Size: 22.8 MB (22754370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ed1c914999ce09a5850058fd4296c038ca35c13723a147f50f4ea54030ce56`  
		Last Modified: Wed, 02 Mar 2022 03:13:17 GMT  
		Size: 15.6 MB (15582331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c242f6ecab39401dfa1b4a8a1e2b62f2d7b4b39d6078dc30923f804bccc8682e`  
		Last Modified: Wed, 02 Mar 2022 03:13:01 GMT  
		Size: 4.2 KB (4198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf212b512b9ef8774b21073f37a32c29b65e1ce1e2cd268ec57cc24307c5de7`  
		Last Modified: Wed, 02 Mar 2022 03:13:05 GMT  
		Size: 5.9 MB (5932541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:cfbea9d7f15b725e78d979c1bf7d87474787f2187fa1810dc5655ab4c428ea6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48899457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7c7d9962e5408ee8ae38eed4b82aece41486bf9d7accd086a3f49fead974c85`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 17 Mar 2022 03:22:22 GMT
ADD file:1c7d8cedf5dc79c676acebde5252ecd3005088a9f29e5e6be547f659f41efb1f in / 
# Thu, 17 Mar 2022 03:22:22 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 11:33:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 11:33:14 GMT
ENV HOME=/home/user
# Thu, 17 Mar 2022 11:33:15 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Mar 2022 11:33:16 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 11:33:17 GMT
ENV IRSSI_VERSION=1.2.3
# Thu, 17 Mar 2022 11:34:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 17 Mar 2022 11:34:48 GMT
WORKDIR /home/user
# Thu, 17 Mar 2022 11:34:49 GMT
USER user
# Thu, 17 Mar 2022 11:34:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c9277cac12165646c33f028489f2a5be3f70745382f4385cd9ed12fcc8cec183`  
		Last Modified: Thu, 17 Mar 2022 03:29:27 GMT  
		Size: 25.9 MB (25923233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68765394fa26a3242947ab026ed84ac73743ba6ea3e9a2a9d5737690f740fffc`  
		Last Modified: Thu, 17 Mar 2022 11:35:22 GMT  
		Size: 16.8 MB (16796123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21216d974d85d8cec172d4aaa29778089c01fdc9243095fb6f361b271192c2e7`  
		Last Modified: Thu, 17 Mar 2022 11:35:19 GMT  
		Size: 4.1 KB (4070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250f896ea3e4765f7fa9882e890c8e909365aa358c3f991edd0342196cc1d800`  
		Last Modified: Thu, 17 Mar 2022 11:35:20 GMT  
		Size: 6.2 MB (6176031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; 386

```console
$ docker pull irssi@sha256:c0a62d463fb49bf3a69db179c0b60cbf4ff7b833d2a60152845a9f8a59e4ddf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50461133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89610068bce58bafeb0e193d0af06b4814dd55faf0b65f98bb7bbd4ff24dbaee`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:04 GMT
ADD file:d9d384f0402bc696e46e7529f52d64859a66aa7a60bca9c7beee7433a5f7af6e in / 
# Tue, 01 Mar 2022 02:08:04 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 04:25:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 04:25:16 GMT
ENV HOME=/home/user
# Wed, 02 Mar 2022 04:25:16 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 02 Mar 2022 04:25:16 GMT
ENV LANG=C.UTF-8
# Wed, 02 Mar 2022 04:25:17 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 02 Mar 2022 04:27:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 02 Mar 2022 04:27:06 GMT
WORKDIR /home/user
# Wed, 02 Mar 2022 04:27:06 GMT
USER user
# Wed, 02 Mar 2022 04:27:06 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c761ce6f2bf0aed07e1198c6f827444969d6e76dda0e55dbb45900920e551d27`  
		Last Modified: Tue, 01 Mar 2022 02:16:51 GMT  
		Size: 27.8 MB (27804590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139be6db820715ec1020fa6d907904a005ff26671f494921c2506cd6bf6a1fc7`  
		Last Modified: Wed, 02 Mar 2022 04:27:55 GMT  
		Size: 16.5 MB (16546984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9b7833f654b31e47588af045ee76e67df88bda2bf2566244c615c18c20edcd`  
		Last Modified: Wed, 02 Mar 2022 04:27:49 GMT  
		Size: 4.2 KB (4193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18696806ef255bda2c34fb5e2b87634943be45ec61cd03501c556d28f210be32`  
		Last Modified: Wed, 02 Mar 2022 04:27:50 GMT  
		Size: 6.1 MB (6105366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; mips64le

```console
$ docker pull irssi@sha256:389489d914e16b932ada3ede3ab90571cf0b8ed0dc925c24217ebdf6d49e5958
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47815154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d367c047358f8297275e01ed32a0837b3dd6387204bd751b52b57afeaefd124`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 01 Mar 2022 02:03:50 GMT
ADD file:f681a18b03e8f8590fb85a806e2c18b3ee2e69fb1a4db7eb933bafb8e7784672 in / 
# Tue, 01 Mar 2022 02:03:50 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:39:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:39:39 GMT
ENV HOME=/home/user
# Tue, 01 Mar 2022 03:39:41 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 01 Mar 2022 03:39:41 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 03:39:41 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 01 Mar 2022 03:42:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 01 Mar 2022 03:42:15 GMT
WORKDIR /home/user
# Tue, 01 Mar 2022 03:42:15 GMT
USER user
# Tue, 01 Mar 2022 03:42:16 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:678634e0b2f87341687ab30235502da4100c2eeafae836b9a671b39e8f7a6da6`  
		Last Modified: Tue, 01 Mar 2022 02:13:43 GMT  
		Size: 25.8 MB (25820204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dcd5e55972035085c7b445e82036cb268e79ab06125f32846c6d7d09dfc7818`  
		Last Modified: Tue, 01 Mar 2022 03:42:52 GMT  
		Size: 15.7 MB (15698106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87570cd46d25689999bce4c019946c4dbe28e5bcb98cf662b8e71b9a2b703b9e`  
		Last Modified: Tue, 01 Mar 2022 03:42:37 GMT  
		Size: 4.2 KB (4179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9096bd6071c77f200e81cca853f3d5d487fc19c0b2048be069c310463d328a5f`  
		Last Modified: Tue, 01 Mar 2022 03:42:42 GMT  
		Size: 6.3 MB (6292665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; ppc64le

```console
$ docker pull irssi@sha256:ca0cbe669ac6398f2eb51fcf038bdce16b96b525083a168612970d1a98f03f08
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54780862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dcdb27db5db000dcf123fce18d1ec14d9f9d5e97f409bb00ada7d5af06ce702`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:48 GMT
ADD file:d87bdffbd9392364fecbbd4148c710bc4948073e773a47c7b9ac1440ebb81c1e in / 
# Wed, 26 Jan 2022 01:47:52 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 22:56:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 22:56:44 GMT
ENV HOME=/home/user
# Wed, 26 Jan 2022 22:56:52 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 26 Jan 2022 22:56:55 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 22:56:59 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 26 Feb 2022 07:38:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 26 Feb 2022 07:38:45 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 07:38:48 GMT
USER user
# Sat, 26 Feb 2022 07:38:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:249357001395b3de58d51723447880f3205d37ea7b902930b5c19f475d4ac8f9`  
		Last Modified: Wed, 26 Jan 2022 01:58:50 GMT  
		Size: 30.6 MB (30562293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76bc6146d874e1a9052b35c297c2dff10eaee69237da9378b2bfa882979e0bb3`  
		Last Modified: Wed, 26 Jan 2022 23:02:16 GMT  
		Size: 17.4 MB (17431167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e871dca1ce277370e3982e11fe9c1cba8e00453eb8e8811efb3a94263a14f0`  
		Last Modified: Wed, 26 Jan 2022 23:02:11 GMT  
		Size: 4.2 KB (4209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253429c0ce6eb715394ea364326563971970bd616f44d6ca025f6fe6ab53ece9`  
		Last Modified: Sat, 26 Feb 2022 07:42:02 GMT  
		Size: 6.8 MB (6783193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; s390x

```console
$ docker pull irssi@sha256:78392a13b131218daad3553dede975d5b4b89c7251462f032c4b3c68653d9a54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49057865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74d95e118adfe6bdb8df2dc4bb9c9a71cb9fcf6773cad51f0ccb2285a27ec8e1`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 17 Mar 2022 03:07:30 GMT
ADD file:4342e1d9db757e91953273ac7120c9d6004d38281f9cea830898b4f35ca43517 in / 
# Thu, 17 Mar 2022 03:07:32 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:45:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 08:45:20 GMT
ENV HOME=/home/user
# Thu, 17 Mar 2022 08:45:21 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Mar 2022 08:45:21 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 08:45:21 GMT
ENV IRSSI_VERSION=1.2.3
# Thu, 17 Mar 2022 08:46:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 17 Mar 2022 08:46:26 GMT
WORKDIR /home/user
# Thu, 17 Mar 2022 08:46:26 GMT
USER user
# Thu, 17 Mar 2022 08:46:26 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6f8a08956872b0f67802da3a67e007322eb963a60e0dadd736077f3ece414e1f`  
		Last Modified: Thu, 17 Mar 2022 03:13:18 GMT  
		Size: 25.8 MB (25769076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af379668e3c95c8de70aaa50b0ea29fe79a526bab60441728ccef56d47a62994`  
		Last Modified: Thu, 17 Mar 2022 08:47:09 GMT  
		Size: 16.9 MB (16899875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8388b5dcf6fd417cdc18b27d3ffa8e19adfeed5396e63f48c4637b130fac0ffe`  
		Last Modified: Thu, 17 Mar 2022 08:47:07 GMT  
		Size: 4.2 KB (4209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508a5e3ccb88964d11fab7a1eea4d169bba20fffe9fab44bccd320d559b443da`  
		Last Modified: Thu, 17 Mar 2022 08:47:07 GMT  
		Size: 6.4 MB (6384705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2-alpine`

```console
$ docker pull irssi@sha256:bc6f96bc4d36d1fc63af4e6b07d68cbe12f15cc806aa3fc90d8c14cbc2aee398
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
$ docker pull irssi@sha256:e81de68bf0b471e0b77ad913541a1f32206fcb8c80fac98a0d9d1350478ac605
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18658093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dead0fe2265236caa74a87944b897072c3db257ea60dcd26ad0f8c8a0a57695`
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
# Sat, 26 Feb 2022 02:42:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 26 Feb 2022 02:42:56 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 02:42:56 GMT
USER user
# Sat, 26 Feb 2022 02:42:56 GMT
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
	-	`sha256:c805e6f5481d38ada6303ac8752840cc587fd0cb676315c10e5c3b97f6dda3e0`  
		Last Modified: Sat, 26 Feb 2022 02:43:33 GMT  
		Size: 6.3 MB (6287505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:f47d5355f67178d363007d5ceb085dc5c31a7474d8dd3717e7a49d016b60d623
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17399747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4440bf00c51e7e1118c662cdcc138a9fc2eb71c6412c3e599195855da1833f5`
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
# Sat, 26 Feb 2022 00:50:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 26 Feb 2022 00:50:54 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 00:50:55 GMT
USER user
# Sat, 26 Feb 2022 00:50:55 GMT
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
	-	`sha256:02c9f2e6dd64e4cf27098cee126ac7e8d3fd7da82e492cd105a0855f350e1d5e`  
		Last Modified: Sat, 26 Feb 2022 00:51:30 GMT  
		Size: 6.0 MB (5987187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:b5190f02bed9f5deb8cd5b609a1e2fcdaf81964aed345fdbaad7b03022356184
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16852378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0211dae8af4e7ddf998d09cb63324461a5d1253fe8997b8d9f2f53a652176f6a`
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
# Sun, 27 Feb 2022 17:01:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sun, 27 Feb 2022 17:01:30 GMT
WORKDIR /home/user
# Sun, 27 Feb 2022 17:01:30 GMT
USER user
# Sun, 27 Feb 2022 17:01:31 GMT
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
	-	`sha256:e03549227edb8b9530872c983ea5e12a413ab939a91e2dcfa926e688ab1dfe1b`  
		Last Modified: Sun, 27 Feb 2022 17:02:52 GMT  
		Size: 5.8 MB (5783760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:15723ad078da19b6695e1c007f755845c6eebd425c8996fc5a2fa161c2080827
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18511732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de0cea899c59de043e14df141069f11d0af7786ca6767a0ca831e95cd7d5bb54`
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
# Sat, 26 Feb 2022 16:42:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 26 Feb 2022 16:42:55 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 16:42:56 GMT
USER user
# Sat, 26 Feb 2022 16:42:57 GMT
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
	-	`sha256:6301442fae9080fb1e5e73ffa49744ab8e62d3dd0af210c3b69a0452c404369c`  
		Last Modified: Sat, 26 Feb 2022 16:43:43 GMT  
		Size: 6.2 MB (6247302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; 386

```console
$ docker pull irssi@sha256:a6c042d635bd7236909e92fb986ea4e9491d19bc3a3d8c8d7f811dee24654b15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17723361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c56ee7059678cc766ade98d596931e5b43d0ddf53e5796344669386e5da7379`
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
# Sat, 26 Feb 2022 16:42:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 26 Feb 2022 16:42:02 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 16:42:02 GMT
USER user
# Sat, 26 Feb 2022 16:42:02 GMT
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
	-	`sha256:ed7782fd3151038808a645b6f78522a79eb588e18ff6d72ffe3a99be2ce38ad3`  
		Last Modified: Sat, 26 Feb 2022 16:42:52 GMT  
		Size: 6.0 MB (5978954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:256febb4e88caa7803e51f3bc7bc6d08a2ee593d903986b0048bb9f2a3adf1dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.0 MB (18956324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c7163a5875310136dafbc963f6cd5ff2f3e2a661335157c1122fab4bbd8b961`
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
# Sat, 26 Feb 2022 07:41:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 26 Feb 2022 07:41:20 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 07:41:23 GMT
USER user
# Sat, 26 Feb 2022 07:41:29 GMT
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
	-	`sha256:b020c19f58e52afc93f0a890fe6012615a585c053cb4cf0da4571f3eb92ac642`  
		Last Modified: Sat, 26 Feb 2022 07:42:26 GMT  
		Size: 6.5 MB (6492301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:50bdb230f1994347e42ae29828177ee13eaaecb603ee60b6a9d294ea0b7d7aa7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18872134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e2a07a0958db17c3a111679879c59fd06187e002b2f6b0fa605868f44f821b9`
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
# Sat, 26 Feb 2022 00:44:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 26 Feb 2022 00:44:16 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 00:44:16 GMT
USER user
# Sat, 26 Feb 2022 00:44:16 GMT
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
	-	`sha256:647b0b24f0a4c27c905b049227cf6d0f7f4c0626fee67a796e2a2a5f234a9632`  
		Last Modified: Sat, 26 Feb 2022 00:44:58 GMT  
		Size: 6.3 MB (6276948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2.3`

```console
$ docker pull irssi@sha256:4cf3922f3d3b1291213df558ff37994ccb444dfb82fe52c77e32745859de3dc3
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
$ docker pull irssi@sha256:f7fbe756507d2f554079dc2fa72b755ea95e4704b658a88744bcef74fe34cb4e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50615106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf4c02131292a1e862292b323babd939f1776a6a4dc2bd3a74b62a23ee32611f`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:56 GMT
ADD file:702017714ad3e1567b4f60b688750f8b631d91088e4dcf41351c4bb07749c579 in / 
# Tue, 01 Mar 2022 02:13:56 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 13:22:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 13:22:06 GMT
ENV HOME=/home/user
# Tue, 01 Mar 2022 13:22:07 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 01 Mar 2022 13:22:07 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 13:22:07 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 01 Mar 2022 13:24:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 01 Mar 2022 13:24:04 GMT
WORKDIR /home/user
# Tue, 01 Mar 2022 13:24:04 GMT
USER user
# Tue, 01 Mar 2022 13:24:04 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:15115158dd02a1bf2fd28724e3c1024394033fb0e9a5d3e451ed2715b6ae312d`  
		Last Modified: Tue, 01 Mar 2022 02:20:08 GMT  
		Size: 27.2 MB (27153737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8700bed9c2318ddf3095e460ab4319bfc16f6aa57ef33cb8d9b23cec47e466e5`  
		Last Modified: Tue, 01 Mar 2022 13:24:34 GMT  
		Size: 17.0 MB (17023729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d367b585ce183067e4c669de040f569d8ae360ee487aad70f804bb9c482688b6`  
		Last Modified: Tue, 01 Mar 2022 13:24:29 GMT  
		Size: 4.2 KB (4206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0573347742f32ca00d17c18d7df270a960bfff93aefabdd083f50043169f0a`  
		Last Modified: Tue, 01 Mar 2022 13:24:31 GMT  
		Size: 6.4 MB (6433434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; arm variant v5

```console
$ docker pull irssi@sha256:705f8349cbef27f5bfec1e6a615ce371629eda97ffbaeb77cc8ab233df645202
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46877530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68942e15850cffade567e213f49f99710a48f64c4f220ba0198d104a67aa8630`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 17 Mar 2022 05:20:46 GMT
ADD file:4b7bce60b3e3455ba9b14c881ffa61187b9e56365fe4f275ee871e7c7e930fb9 in / 
# Thu, 17 Mar 2022 05:20:46 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 10:03:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 10:03:08 GMT
ENV HOME=/home/user
# Thu, 17 Mar 2022 10:03:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Mar 2022 10:03:11 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 10:03:11 GMT
ENV IRSSI_VERSION=1.2.3
# Thu, 17 Mar 2022 10:05:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 17 Mar 2022 10:05:22 GMT
WORKDIR /home/user
# Thu, 17 Mar 2022 10:05:22 GMT
USER user
# Thu, 17 Mar 2022 10:05:23 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f193682138b0c37054cb843ef2155a75706f248a369d454bf6444833f120aefc`  
		Last Modified: Thu, 17 Mar 2022 05:36:29 GMT  
		Size: 24.9 MB (24886195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8afac93444b98f19bbf672aab4b0b358eaf47b0e952385ab7d4ad839380315f`  
		Last Modified: Thu, 17 Mar 2022 10:06:11 GMT  
		Size: 15.9 MB (15922671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3389c88e912002d546288257f98a7208ca19f801c85b55949571bc65dfb3be95`  
		Last Modified: Thu, 17 Mar 2022 10:05:55 GMT  
		Size: 4.2 KB (4194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b655b41133cb19826b4d711323336615269f792f53c1affd769ac1d0bd026e`  
		Last Modified: Thu, 17 Mar 2022 10:05:59 GMT  
		Size: 6.1 MB (6064470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; arm variant v7

```console
$ docker pull irssi@sha256:a04ab92ea03c301760bfcb9a9ddc09b38c10e732e563c7f83417e653a57def8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44273440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de2c18377805a7d11fd2cac579e7e5a42acb66e2d843b1565b34479eca7ee4ce`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 01 Mar 2022 02:04:06 GMT
ADD file:d73a3eaf767825b31d0c0189624b35193e5ad7c5907f839edf6f7917036c2d0b in / 
# Tue, 01 Mar 2022 02:04:07 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 03:09:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 03:09:59 GMT
ENV HOME=/home/user
# Wed, 02 Mar 2022 03:10:01 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 02 Mar 2022 03:10:01 GMT
ENV LANG=C.UTF-8
# Wed, 02 Mar 2022 03:10:02 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 02 Mar 2022 03:11:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 02 Mar 2022 03:11:53 GMT
WORKDIR /home/user
# Wed, 02 Mar 2022 03:11:53 GMT
USER user
# Wed, 02 Mar 2022 03:11:53 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1acfd43b1a25aefe6117ba65bf2b46a19e3cf8e72b76f522a9fe299412e1c5f2`  
		Last Modified: Tue, 01 Mar 2022 02:20:32 GMT  
		Size: 22.8 MB (22754370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ed1c914999ce09a5850058fd4296c038ca35c13723a147f50f4ea54030ce56`  
		Last Modified: Wed, 02 Mar 2022 03:13:17 GMT  
		Size: 15.6 MB (15582331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c242f6ecab39401dfa1b4a8a1e2b62f2d7b4b39d6078dc30923f804bccc8682e`  
		Last Modified: Wed, 02 Mar 2022 03:13:01 GMT  
		Size: 4.2 KB (4198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf212b512b9ef8774b21073f37a32c29b65e1ce1e2cd268ec57cc24307c5de7`  
		Last Modified: Wed, 02 Mar 2022 03:13:05 GMT  
		Size: 5.9 MB (5932541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:cfbea9d7f15b725e78d979c1bf7d87474787f2187fa1810dc5655ab4c428ea6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48899457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7c7d9962e5408ee8ae38eed4b82aece41486bf9d7accd086a3f49fead974c85`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 17 Mar 2022 03:22:22 GMT
ADD file:1c7d8cedf5dc79c676acebde5252ecd3005088a9f29e5e6be547f659f41efb1f in / 
# Thu, 17 Mar 2022 03:22:22 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 11:33:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 11:33:14 GMT
ENV HOME=/home/user
# Thu, 17 Mar 2022 11:33:15 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Mar 2022 11:33:16 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 11:33:17 GMT
ENV IRSSI_VERSION=1.2.3
# Thu, 17 Mar 2022 11:34:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 17 Mar 2022 11:34:48 GMT
WORKDIR /home/user
# Thu, 17 Mar 2022 11:34:49 GMT
USER user
# Thu, 17 Mar 2022 11:34:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c9277cac12165646c33f028489f2a5be3f70745382f4385cd9ed12fcc8cec183`  
		Last Modified: Thu, 17 Mar 2022 03:29:27 GMT  
		Size: 25.9 MB (25923233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68765394fa26a3242947ab026ed84ac73743ba6ea3e9a2a9d5737690f740fffc`  
		Last Modified: Thu, 17 Mar 2022 11:35:22 GMT  
		Size: 16.8 MB (16796123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21216d974d85d8cec172d4aaa29778089c01fdc9243095fb6f361b271192c2e7`  
		Last Modified: Thu, 17 Mar 2022 11:35:19 GMT  
		Size: 4.1 KB (4070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250f896ea3e4765f7fa9882e890c8e909365aa358c3f991edd0342196cc1d800`  
		Last Modified: Thu, 17 Mar 2022 11:35:20 GMT  
		Size: 6.2 MB (6176031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; 386

```console
$ docker pull irssi@sha256:c0a62d463fb49bf3a69db179c0b60cbf4ff7b833d2a60152845a9f8a59e4ddf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50461133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89610068bce58bafeb0e193d0af06b4814dd55faf0b65f98bb7bbd4ff24dbaee`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:04 GMT
ADD file:d9d384f0402bc696e46e7529f52d64859a66aa7a60bca9c7beee7433a5f7af6e in / 
# Tue, 01 Mar 2022 02:08:04 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 04:25:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 04:25:16 GMT
ENV HOME=/home/user
# Wed, 02 Mar 2022 04:25:16 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 02 Mar 2022 04:25:16 GMT
ENV LANG=C.UTF-8
# Wed, 02 Mar 2022 04:25:17 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 02 Mar 2022 04:27:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 02 Mar 2022 04:27:06 GMT
WORKDIR /home/user
# Wed, 02 Mar 2022 04:27:06 GMT
USER user
# Wed, 02 Mar 2022 04:27:06 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c761ce6f2bf0aed07e1198c6f827444969d6e76dda0e55dbb45900920e551d27`  
		Last Modified: Tue, 01 Mar 2022 02:16:51 GMT  
		Size: 27.8 MB (27804590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139be6db820715ec1020fa6d907904a005ff26671f494921c2506cd6bf6a1fc7`  
		Last Modified: Wed, 02 Mar 2022 04:27:55 GMT  
		Size: 16.5 MB (16546984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9b7833f654b31e47588af045ee76e67df88bda2bf2566244c615c18c20edcd`  
		Last Modified: Wed, 02 Mar 2022 04:27:49 GMT  
		Size: 4.2 KB (4193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18696806ef255bda2c34fb5e2b87634943be45ec61cd03501c556d28f210be32`  
		Last Modified: Wed, 02 Mar 2022 04:27:50 GMT  
		Size: 6.1 MB (6105366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; mips64le

```console
$ docker pull irssi@sha256:389489d914e16b932ada3ede3ab90571cf0b8ed0dc925c24217ebdf6d49e5958
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47815154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d367c047358f8297275e01ed32a0837b3dd6387204bd751b52b57afeaefd124`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 01 Mar 2022 02:03:50 GMT
ADD file:f681a18b03e8f8590fb85a806e2c18b3ee2e69fb1a4db7eb933bafb8e7784672 in / 
# Tue, 01 Mar 2022 02:03:50 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:39:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:39:39 GMT
ENV HOME=/home/user
# Tue, 01 Mar 2022 03:39:41 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 01 Mar 2022 03:39:41 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 03:39:41 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 01 Mar 2022 03:42:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 01 Mar 2022 03:42:15 GMT
WORKDIR /home/user
# Tue, 01 Mar 2022 03:42:15 GMT
USER user
# Tue, 01 Mar 2022 03:42:16 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:678634e0b2f87341687ab30235502da4100c2eeafae836b9a671b39e8f7a6da6`  
		Last Modified: Tue, 01 Mar 2022 02:13:43 GMT  
		Size: 25.8 MB (25820204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dcd5e55972035085c7b445e82036cb268e79ab06125f32846c6d7d09dfc7818`  
		Last Modified: Tue, 01 Mar 2022 03:42:52 GMT  
		Size: 15.7 MB (15698106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87570cd46d25689999bce4c019946c4dbe28e5bcb98cf662b8e71b9a2b703b9e`  
		Last Modified: Tue, 01 Mar 2022 03:42:37 GMT  
		Size: 4.2 KB (4179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9096bd6071c77f200e81cca853f3d5d487fc19c0b2048be069c310463d328a5f`  
		Last Modified: Tue, 01 Mar 2022 03:42:42 GMT  
		Size: 6.3 MB (6292665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; ppc64le

```console
$ docker pull irssi@sha256:ca0cbe669ac6398f2eb51fcf038bdce16b96b525083a168612970d1a98f03f08
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54780862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dcdb27db5db000dcf123fce18d1ec14d9f9d5e97f409bb00ada7d5af06ce702`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:48 GMT
ADD file:d87bdffbd9392364fecbbd4148c710bc4948073e773a47c7b9ac1440ebb81c1e in / 
# Wed, 26 Jan 2022 01:47:52 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 22:56:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 22:56:44 GMT
ENV HOME=/home/user
# Wed, 26 Jan 2022 22:56:52 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 26 Jan 2022 22:56:55 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 22:56:59 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 26 Feb 2022 07:38:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 26 Feb 2022 07:38:45 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 07:38:48 GMT
USER user
# Sat, 26 Feb 2022 07:38:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:249357001395b3de58d51723447880f3205d37ea7b902930b5c19f475d4ac8f9`  
		Last Modified: Wed, 26 Jan 2022 01:58:50 GMT  
		Size: 30.6 MB (30562293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76bc6146d874e1a9052b35c297c2dff10eaee69237da9378b2bfa882979e0bb3`  
		Last Modified: Wed, 26 Jan 2022 23:02:16 GMT  
		Size: 17.4 MB (17431167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e871dca1ce277370e3982e11fe9c1cba8e00453eb8e8811efb3a94263a14f0`  
		Last Modified: Wed, 26 Jan 2022 23:02:11 GMT  
		Size: 4.2 KB (4209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253429c0ce6eb715394ea364326563971970bd616f44d6ca025f6fe6ab53ece9`  
		Last Modified: Sat, 26 Feb 2022 07:42:02 GMT  
		Size: 6.8 MB (6783193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; s390x

```console
$ docker pull irssi@sha256:78392a13b131218daad3553dede975d5b4b89c7251462f032c4b3c68653d9a54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49057865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74d95e118adfe6bdb8df2dc4bb9c9a71cb9fcf6773cad51f0ccb2285a27ec8e1`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 17 Mar 2022 03:07:30 GMT
ADD file:4342e1d9db757e91953273ac7120c9d6004d38281f9cea830898b4f35ca43517 in / 
# Thu, 17 Mar 2022 03:07:32 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:45:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 08:45:20 GMT
ENV HOME=/home/user
# Thu, 17 Mar 2022 08:45:21 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Mar 2022 08:45:21 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 08:45:21 GMT
ENV IRSSI_VERSION=1.2.3
# Thu, 17 Mar 2022 08:46:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 17 Mar 2022 08:46:26 GMT
WORKDIR /home/user
# Thu, 17 Mar 2022 08:46:26 GMT
USER user
# Thu, 17 Mar 2022 08:46:26 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6f8a08956872b0f67802da3a67e007322eb963a60e0dadd736077f3ece414e1f`  
		Last Modified: Thu, 17 Mar 2022 03:13:18 GMT  
		Size: 25.8 MB (25769076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af379668e3c95c8de70aaa50b0ea29fe79a526bab60441728ccef56d47a62994`  
		Last Modified: Thu, 17 Mar 2022 08:47:09 GMT  
		Size: 16.9 MB (16899875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8388b5dcf6fd417cdc18b27d3ffa8e19adfeed5396e63f48c4637b130fac0ffe`  
		Last Modified: Thu, 17 Mar 2022 08:47:07 GMT  
		Size: 4.2 KB (4209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508a5e3ccb88964d11fab7a1eea4d169bba20fffe9fab44bccd320d559b443da`  
		Last Modified: Thu, 17 Mar 2022 08:47:07 GMT  
		Size: 6.4 MB (6384705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2.3-alpine`

```console
$ docker pull irssi@sha256:bc6f96bc4d36d1fc63af4e6b07d68cbe12f15cc806aa3fc90d8c14cbc2aee398
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
$ docker pull irssi@sha256:e81de68bf0b471e0b77ad913541a1f32206fcb8c80fac98a0d9d1350478ac605
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18658093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dead0fe2265236caa74a87944b897072c3db257ea60dcd26ad0f8c8a0a57695`
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
# Sat, 26 Feb 2022 02:42:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 26 Feb 2022 02:42:56 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 02:42:56 GMT
USER user
# Sat, 26 Feb 2022 02:42:56 GMT
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
	-	`sha256:c805e6f5481d38ada6303ac8752840cc587fd0cb676315c10e5c3b97f6dda3e0`  
		Last Modified: Sat, 26 Feb 2022 02:43:33 GMT  
		Size: 6.3 MB (6287505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:f47d5355f67178d363007d5ceb085dc5c31a7474d8dd3717e7a49d016b60d623
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17399747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4440bf00c51e7e1118c662cdcc138a9fc2eb71c6412c3e599195855da1833f5`
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
# Sat, 26 Feb 2022 00:50:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 26 Feb 2022 00:50:54 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 00:50:55 GMT
USER user
# Sat, 26 Feb 2022 00:50:55 GMT
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
	-	`sha256:02c9f2e6dd64e4cf27098cee126ac7e8d3fd7da82e492cd105a0855f350e1d5e`  
		Last Modified: Sat, 26 Feb 2022 00:51:30 GMT  
		Size: 6.0 MB (5987187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:b5190f02bed9f5deb8cd5b609a1e2fcdaf81964aed345fdbaad7b03022356184
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16852378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0211dae8af4e7ddf998d09cb63324461a5d1253fe8997b8d9f2f53a652176f6a`
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
# Sun, 27 Feb 2022 17:01:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sun, 27 Feb 2022 17:01:30 GMT
WORKDIR /home/user
# Sun, 27 Feb 2022 17:01:30 GMT
USER user
# Sun, 27 Feb 2022 17:01:31 GMT
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
	-	`sha256:e03549227edb8b9530872c983ea5e12a413ab939a91e2dcfa926e688ab1dfe1b`  
		Last Modified: Sun, 27 Feb 2022 17:02:52 GMT  
		Size: 5.8 MB (5783760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:15723ad078da19b6695e1c007f755845c6eebd425c8996fc5a2fa161c2080827
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18511732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de0cea899c59de043e14df141069f11d0af7786ca6767a0ca831e95cd7d5bb54`
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
# Sat, 26 Feb 2022 16:42:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 26 Feb 2022 16:42:55 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 16:42:56 GMT
USER user
# Sat, 26 Feb 2022 16:42:57 GMT
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
	-	`sha256:6301442fae9080fb1e5e73ffa49744ab8e62d3dd0af210c3b69a0452c404369c`  
		Last Modified: Sat, 26 Feb 2022 16:43:43 GMT  
		Size: 6.2 MB (6247302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; 386

```console
$ docker pull irssi@sha256:a6c042d635bd7236909e92fb986ea4e9491d19bc3a3d8c8d7f811dee24654b15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17723361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c56ee7059678cc766ade98d596931e5b43d0ddf53e5796344669386e5da7379`
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
# Sat, 26 Feb 2022 16:42:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 26 Feb 2022 16:42:02 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 16:42:02 GMT
USER user
# Sat, 26 Feb 2022 16:42:02 GMT
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
	-	`sha256:ed7782fd3151038808a645b6f78522a79eb588e18ff6d72ffe3a99be2ce38ad3`  
		Last Modified: Sat, 26 Feb 2022 16:42:52 GMT  
		Size: 6.0 MB (5978954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:256febb4e88caa7803e51f3bc7bc6d08a2ee593d903986b0048bb9f2a3adf1dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.0 MB (18956324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c7163a5875310136dafbc963f6cd5ff2f3e2a661335157c1122fab4bbd8b961`
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
# Sat, 26 Feb 2022 07:41:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 26 Feb 2022 07:41:20 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 07:41:23 GMT
USER user
# Sat, 26 Feb 2022 07:41:29 GMT
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
	-	`sha256:b020c19f58e52afc93f0a890fe6012615a585c053cb4cf0da4571f3eb92ac642`  
		Last Modified: Sat, 26 Feb 2022 07:42:26 GMT  
		Size: 6.5 MB (6492301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:50bdb230f1994347e42ae29828177ee13eaaecb603ee60b6a9d294ea0b7d7aa7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18872134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e2a07a0958db17c3a111679879c59fd06187e002b2f6b0fa605868f44f821b9`
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
# Sat, 26 Feb 2022 00:44:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 26 Feb 2022 00:44:16 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 00:44:16 GMT
USER user
# Sat, 26 Feb 2022 00:44:16 GMT
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
	-	`sha256:647b0b24f0a4c27c905b049227cf6d0f7f4c0626fee67a796e2a2a5f234a9632`  
		Last Modified: Sat, 26 Feb 2022 00:44:58 GMT  
		Size: 6.3 MB (6276948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:alpine`

```console
$ docker pull irssi@sha256:bc6f96bc4d36d1fc63af4e6b07d68cbe12f15cc806aa3fc90d8c14cbc2aee398
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
$ docker pull irssi@sha256:e81de68bf0b471e0b77ad913541a1f32206fcb8c80fac98a0d9d1350478ac605
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18658093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dead0fe2265236caa74a87944b897072c3db257ea60dcd26ad0f8c8a0a57695`
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
# Sat, 26 Feb 2022 02:42:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 26 Feb 2022 02:42:56 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 02:42:56 GMT
USER user
# Sat, 26 Feb 2022 02:42:56 GMT
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
	-	`sha256:c805e6f5481d38ada6303ac8752840cc587fd0cb676315c10e5c3b97f6dda3e0`  
		Last Modified: Sat, 26 Feb 2022 02:43:33 GMT  
		Size: 6.3 MB (6287505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:f47d5355f67178d363007d5ceb085dc5c31a7474d8dd3717e7a49d016b60d623
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17399747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4440bf00c51e7e1118c662cdcc138a9fc2eb71c6412c3e599195855da1833f5`
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
# Sat, 26 Feb 2022 00:50:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 26 Feb 2022 00:50:54 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 00:50:55 GMT
USER user
# Sat, 26 Feb 2022 00:50:55 GMT
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
	-	`sha256:02c9f2e6dd64e4cf27098cee126ac7e8d3fd7da82e492cd105a0855f350e1d5e`  
		Last Modified: Sat, 26 Feb 2022 00:51:30 GMT  
		Size: 6.0 MB (5987187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:b5190f02bed9f5deb8cd5b609a1e2fcdaf81964aed345fdbaad7b03022356184
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16852378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0211dae8af4e7ddf998d09cb63324461a5d1253fe8997b8d9f2f53a652176f6a`
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
# Sun, 27 Feb 2022 17:01:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sun, 27 Feb 2022 17:01:30 GMT
WORKDIR /home/user
# Sun, 27 Feb 2022 17:01:30 GMT
USER user
# Sun, 27 Feb 2022 17:01:31 GMT
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
	-	`sha256:e03549227edb8b9530872c983ea5e12a413ab939a91e2dcfa926e688ab1dfe1b`  
		Last Modified: Sun, 27 Feb 2022 17:02:52 GMT  
		Size: 5.8 MB (5783760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:15723ad078da19b6695e1c007f755845c6eebd425c8996fc5a2fa161c2080827
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18511732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de0cea899c59de043e14df141069f11d0af7786ca6767a0ca831e95cd7d5bb54`
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
# Sat, 26 Feb 2022 16:42:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 26 Feb 2022 16:42:55 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 16:42:56 GMT
USER user
# Sat, 26 Feb 2022 16:42:57 GMT
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
	-	`sha256:6301442fae9080fb1e5e73ffa49744ab8e62d3dd0af210c3b69a0452c404369c`  
		Last Modified: Sat, 26 Feb 2022 16:43:43 GMT  
		Size: 6.2 MB (6247302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; 386

```console
$ docker pull irssi@sha256:a6c042d635bd7236909e92fb986ea4e9491d19bc3a3d8c8d7f811dee24654b15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17723361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c56ee7059678cc766ade98d596931e5b43d0ddf53e5796344669386e5da7379`
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
# Sat, 26 Feb 2022 16:42:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 26 Feb 2022 16:42:02 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 16:42:02 GMT
USER user
# Sat, 26 Feb 2022 16:42:02 GMT
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
	-	`sha256:ed7782fd3151038808a645b6f78522a79eb588e18ff6d72ffe3a99be2ce38ad3`  
		Last Modified: Sat, 26 Feb 2022 16:42:52 GMT  
		Size: 6.0 MB (5978954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:256febb4e88caa7803e51f3bc7bc6d08a2ee593d903986b0048bb9f2a3adf1dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.0 MB (18956324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c7163a5875310136dafbc963f6cd5ff2f3e2a661335157c1122fab4bbd8b961`
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
# Sat, 26 Feb 2022 07:41:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 26 Feb 2022 07:41:20 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 07:41:23 GMT
USER user
# Sat, 26 Feb 2022 07:41:29 GMT
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
	-	`sha256:b020c19f58e52afc93f0a890fe6012615a585c053cb4cf0da4571f3eb92ac642`  
		Last Modified: Sat, 26 Feb 2022 07:42:26 GMT  
		Size: 6.5 MB (6492301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; s390x

```console
$ docker pull irssi@sha256:50bdb230f1994347e42ae29828177ee13eaaecb603ee60b6a9d294ea0b7d7aa7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18872134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e2a07a0958db17c3a111679879c59fd06187e002b2f6b0fa605868f44f821b9`
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
# Sat, 26 Feb 2022 00:44:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 26 Feb 2022 00:44:16 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 00:44:16 GMT
USER user
# Sat, 26 Feb 2022 00:44:16 GMT
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
	-	`sha256:647b0b24f0a4c27c905b049227cf6d0f7f4c0626fee67a796e2a2a5f234a9632`  
		Last Modified: Sat, 26 Feb 2022 00:44:58 GMT  
		Size: 6.3 MB (6276948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:latest`

```console
$ docker pull irssi@sha256:4cf3922f3d3b1291213df558ff37994ccb444dfb82fe52c77e32745859de3dc3
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
$ docker pull irssi@sha256:f7fbe756507d2f554079dc2fa72b755ea95e4704b658a88744bcef74fe34cb4e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50615106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf4c02131292a1e862292b323babd939f1776a6a4dc2bd3a74b62a23ee32611f`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:56 GMT
ADD file:702017714ad3e1567b4f60b688750f8b631d91088e4dcf41351c4bb07749c579 in / 
# Tue, 01 Mar 2022 02:13:56 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 13:22:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 13:22:06 GMT
ENV HOME=/home/user
# Tue, 01 Mar 2022 13:22:07 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 01 Mar 2022 13:22:07 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 13:22:07 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 01 Mar 2022 13:24:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 01 Mar 2022 13:24:04 GMT
WORKDIR /home/user
# Tue, 01 Mar 2022 13:24:04 GMT
USER user
# Tue, 01 Mar 2022 13:24:04 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:15115158dd02a1bf2fd28724e3c1024394033fb0e9a5d3e451ed2715b6ae312d`  
		Last Modified: Tue, 01 Mar 2022 02:20:08 GMT  
		Size: 27.2 MB (27153737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8700bed9c2318ddf3095e460ab4319bfc16f6aa57ef33cb8d9b23cec47e466e5`  
		Last Modified: Tue, 01 Mar 2022 13:24:34 GMT  
		Size: 17.0 MB (17023729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d367b585ce183067e4c669de040f569d8ae360ee487aad70f804bb9c482688b6`  
		Last Modified: Tue, 01 Mar 2022 13:24:29 GMT  
		Size: 4.2 KB (4206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0573347742f32ca00d17c18d7df270a960bfff93aefabdd083f50043169f0a`  
		Last Modified: Tue, 01 Mar 2022 13:24:31 GMT  
		Size: 6.4 MB (6433434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm variant v5

```console
$ docker pull irssi@sha256:705f8349cbef27f5bfec1e6a615ce371629eda97ffbaeb77cc8ab233df645202
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46877530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68942e15850cffade567e213f49f99710a48f64c4f220ba0198d104a67aa8630`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 17 Mar 2022 05:20:46 GMT
ADD file:4b7bce60b3e3455ba9b14c881ffa61187b9e56365fe4f275ee871e7c7e930fb9 in / 
# Thu, 17 Mar 2022 05:20:46 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 10:03:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 10:03:08 GMT
ENV HOME=/home/user
# Thu, 17 Mar 2022 10:03:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Mar 2022 10:03:11 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 10:03:11 GMT
ENV IRSSI_VERSION=1.2.3
# Thu, 17 Mar 2022 10:05:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 17 Mar 2022 10:05:22 GMT
WORKDIR /home/user
# Thu, 17 Mar 2022 10:05:22 GMT
USER user
# Thu, 17 Mar 2022 10:05:23 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f193682138b0c37054cb843ef2155a75706f248a369d454bf6444833f120aefc`  
		Last Modified: Thu, 17 Mar 2022 05:36:29 GMT  
		Size: 24.9 MB (24886195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8afac93444b98f19bbf672aab4b0b358eaf47b0e952385ab7d4ad839380315f`  
		Last Modified: Thu, 17 Mar 2022 10:06:11 GMT  
		Size: 15.9 MB (15922671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3389c88e912002d546288257f98a7208ca19f801c85b55949571bc65dfb3be95`  
		Last Modified: Thu, 17 Mar 2022 10:05:55 GMT  
		Size: 4.2 KB (4194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b655b41133cb19826b4d711323336615269f792f53c1affd769ac1d0bd026e`  
		Last Modified: Thu, 17 Mar 2022 10:05:59 GMT  
		Size: 6.1 MB (6064470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm variant v7

```console
$ docker pull irssi@sha256:a04ab92ea03c301760bfcb9a9ddc09b38c10e732e563c7f83417e653a57def8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44273440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de2c18377805a7d11fd2cac579e7e5a42acb66e2d843b1565b34479eca7ee4ce`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 01 Mar 2022 02:04:06 GMT
ADD file:d73a3eaf767825b31d0c0189624b35193e5ad7c5907f839edf6f7917036c2d0b in / 
# Tue, 01 Mar 2022 02:04:07 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 03:09:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 03:09:59 GMT
ENV HOME=/home/user
# Wed, 02 Mar 2022 03:10:01 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 02 Mar 2022 03:10:01 GMT
ENV LANG=C.UTF-8
# Wed, 02 Mar 2022 03:10:02 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 02 Mar 2022 03:11:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 02 Mar 2022 03:11:53 GMT
WORKDIR /home/user
# Wed, 02 Mar 2022 03:11:53 GMT
USER user
# Wed, 02 Mar 2022 03:11:53 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1acfd43b1a25aefe6117ba65bf2b46a19e3cf8e72b76f522a9fe299412e1c5f2`  
		Last Modified: Tue, 01 Mar 2022 02:20:32 GMT  
		Size: 22.8 MB (22754370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ed1c914999ce09a5850058fd4296c038ca35c13723a147f50f4ea54030ce56`  
		Last Modified: Wed, 02 Mar 2022 03:13:17 GMT  
		Size: 15.6 MB (15582331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c242f6ecab39401dfa1b4a8a1e2b62f2d7b4b39d6078dc30923f804bccc8682e`  
		Last Modified: Wed, 02 Mar 2022 03:13:01 GMT  
		Size: 4.2 KB (4198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf212b512b9ef8774b21073f37a32c29b65e1ce1e2cd268ec57cc24307c5de7`  
		Last Modified: Wed, 02 Mar 2022 03:13:05 GMT  
		Size: 5.9 MB (5932541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:cfbea9d7f15b725e78d979c1bf7d87474787f2187fa1810dc5655ab4c428ea6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48899457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7c7d9962e5408ee8ae38eed4b82aece41486bf9d7accd086a3f49fead974c85`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 17 Mar 2022 03:22:22 GMT
ADD file:1c7d8cedf5dc79c676acebde5252ecd3005088a9f29e5e6be547f659f41efb1f in / 
# Thu, 17 Mar 2022 03:22:22 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 11:33:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 11:33:14 GMT
ENV HOME=/home/user
# Thu, 17 Mar 2022 11:33:15 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Mar 2022 11:33:16 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 11:33:17 GMT
ENV IRSSI_VERSION=1.2.3
# Thu, 17 Mar 2022 11:34:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 17 Mar 2022 11:34:48 GMT
WORKDIR /home/user
# Thu, 17 Mar 2022 11:34:49 GMT
USER user
# Thu, 17 Mar 2022 11:34:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c9277cac12165646c33f028489f2a5be3f70745382f4385cd9ed12fcc8cec183`  
		Last Modified: Thu, 17 Mar 2022 03:29:27 GMT  
		Size: 25.9 MB (25923233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68765394fa26a3242947ab026ed84ac73743ba6ea3e9a2a9d5737690f740fffc`  
		Last Modified: Thu, 17 Mar 2022 11:35:22 GMT  
		Size: 16.8 MB (16796123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21216d974d85d8cec172d4aaa29778089c01fdc9243095fb6f361b271192c2e7`  
		Last Modified: Thu, 17 Mar 2022 11:35:19 GMT  
		Size: 4.1 KB (4070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250f896ea3e4765f7fa9882e890c8e909365aa358c3f991edd0342196cc1d800`  
		Last Modified: Thu, 17 Mar 2022 11:35:20 GMT  
		Size: 6.2 MB (6176031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; 386

```console
$ docker pull irssi@sha256:c0a62d463fb49bf3a69db179c0b60cbf4ff7b833d2a60152845a9f8a59e4ddf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50461133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89610068bce58bafeb0e193d0af06b4814dd55faf0b65f98bb7bbd4ff24dbaee`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:04 GMT
ADD file:d9d384f0402bc696e46e7529f52d64859a66aa7a60bca9c7beee7433a5f7af6e in / 
# Tue, 01 Mar 2022 02:08:04 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 04:25:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 04:25:16 GMT
ENV HOME=/home/user
# Wed, 02 Mar 2022 04:25:16 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 02 Mar 2022 04:25:16 GMT
ENV LANG=C.UTF-8
# Wed, 02 Mar 2022 04:25:17 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 02 Mar 2022 04:27:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 02 Mar 2022 04:27:06 GMT
WORKDIR /home/user
# Wed, 02 Mar 2022 04:27:06 GMT
USER user
# Wed, 02 Mar 2022 04:27:06 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c761ce6f2bf0aed07e1198c6f827444969d6e76dda0e55dbb45900920e551d27`  
		Last Modified: Tue, 01 Mar 2022 02:16:51 GMT  
		Size: 27.8 MB (27804590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139be6db820715ec1020fa6d907904a005ff26671f494921c2506cd6bf6a1fc7`  
		Last Modified: Wed, 02 Mar 2022 04:27:55 GMT  
		Size: 16.5 MB (16546984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9b7833f654b31e47588af045ee76e67df88bda2bf2566244c615c18c20edcd`  
		Last Modified: Wed, 02 Mar 2022 04:27:49 GMT  
		Size: 4.2 KB (4193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18696806ef255bda2c34fb5e2b87634943be45ec61cd03501c556d28f210be32`  
		Last Modified: Wed, 02 Mar 2022 04:27:50 GMT  
		Size: 6.1 MB (6105366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; mips64le

```console
$ docker pull irssi@sha256:389489d914e16b932ada3ede3ab90571cf0b8ed0dc925c24217ebdf6d49e5958
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47815154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d367c047358f8297275e01ed32a0837b3dd6387204bd751b52b57afeaefd124`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 01 Mar 2022 02:03:50 GMT
ADD file:f681a18b03e8f8590fb85a806e2c18b3ee2e69fb1a4db7eb933bafb8e7784672 in / 
# Tue, 01 Mar 2022 02:03:50 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:39:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:39:39 GMT
ENV HOME=/home/user
# Tue, 01 Mar 2022 03:39:41 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 01 Mar 2022 03:39:41 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 03:39:41 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 01 Mar 2022 03:42:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 01 Mar 2022 03:42:15 GMT
WORKDIR /home/user
# Tue, 01 Mar 2022 03:42:15 GMT
USER user
# Tue, 01 Mar 2022 03:42:16 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:678634e0b2f87341687ab30235502da4100c2eeafae836b9a671b39e8f7a6da6`  
		Last Modified: Tue, 01 Mar 2022 02:13:43 GMT  
		Size: 25.8 MB (25820204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dcd5e55972035085c7b445e82036cb268e79ab06125f32846c6d7d09dfc7818`  
		Last Modified: Tue, 01 Mar 2022 03:42:52 GMT  
		Size: 15.7 MB (15698106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87570cd46d25689999bce4c019946c4dbe28e5bcb98cf662b8e71b9a2b703b9e`  
		Last Modified: Tue, 01 Mar 2022 03:42:37 GMT  
		Size: 4.2 KB (4179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9096bd6071c77f200e81cca853f3d5d487fc19c0b2048be069c310463d328a5f`  
		Last Modified: Tue, 01 Mar 2022 03:42:42 GMT  
		Size: 6.3 MB (6292665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; ppc64le

```console
$ docker pull irssi@sha256:ca0cbe669ac6398f2eb51fcf038bdce16b96b525083a168612970d1a98f03f08
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54780862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dcdb27db5db000dcf123fce18d1ec14d9f9d5e97f409bb00ada7d5af06ce702`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:48 GMT
ADD file:d87bdffbd9392364fecbbd4148c710bc4948073e773a47c7b9ac1440ebb81c1e in / 
# Wed, 26 Jan 2022 01:47:52 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 22:56:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 22:56:44 GMT
ENV HOME=/home/user
# Wed, 26 Jan 2022 22:56:52 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 26 Jan 2022 22:56:55 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 22:56:59 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 26 Feb 2022 07:38:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 26 Feb 2022 07:38:45 GMT
WORKDIR /home/user
# Sat, 26 Feb 2022 07:38:48 GMT
USER user
# Sat, 26 Feb 2022 07:38:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:249357001395b3de58d51723447880f3205d37ea7b902930b5c19f475d4ac8f9`  
		Last Modified: Wed, 26 Jan 2022 01:58:50 GMT  
		Size: 30.6 MB (30562293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76bc6146d874e1a9052b35c297c2dff10eaee69237da9378b2bfa882979e0bb3`  
		Last Modified: Wed, 26 Jan 2022 23:02:16 GMT  
		Size: 17.4 MB (17431167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e871dca1ce277370e3982e11fe9c1cba8e00453eb8e8811efb3a94263a14f0`  
		Last Modified: Wed, 26 Jan 2022 23:02:11 GMT  
		Size: 4.2 KB (4209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253429c0ce6eb715394ea364326563971970bd616f44d6ca025f6fe6ab53ece9`  
		Last Modified: Sat, 26 Feb 2022 07:42:02 GMT  
		Size: 6.8 MB (6783193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; s390x

```console
$ docker pull irssi@sha256:78392a13b131218daad3553dede975d5b4b89c7251462f032c4b3c68653d9a54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49057865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74d95e118adfe6bdb8df2dc4bb9c9a71cb9fcf6773cad51f0ccb2285a27ec8e1`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 17 Mar 2022 03:07:30 GMT
ADD file:4342e1d9db757e91953273ac7120c9d6004d38281f9cea830898b4f35ca43517 in / 
# Thu, 17 Mar 2022 03:07:32 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:45:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 08:45:20 GMT
ENV HOME=/home/user
# Thu, 17 Mar 2022 08:45:21 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Mar 2022 08:45:21 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 08:45:21 GMT
ENV IRSSI_VERSION=1.2.3
# Thu, 17 Mar 2022 08:46:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Thu, 17 Mar 2022 08:46:26 GMT
WORKDIR /home/user
# Thu, 17 Mar 2022 08:46:26 GMT
USER user
# Thu, 17 Mar 2022 08:46:26 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6f8a08956872b0f67802da3a67e007322eb963a60e0dadd736077f3ece414e1f`  
		Last Modified: Thu, 17 Mar 2022 03:13:18 GMT  
		Size: 25.8 MB (25769076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af379668e3c95c8de70aaa50b0ea29fe79a526bab60441728ccef56d47a62994`  
		Last Modified: Thu, 17 Mar 2022 08:47:09 GMT  
		Size: 16.9 MB (16899875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8388b5dcf6fd417cdc18b27d3ffa8e19adfeed5396e63f48c4637b130fac0ffe`  
		Last Modified: Thu, 17 Mar 2022 08:47:07 GMT  
		Size: 4.2 KB (4209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508a5e3ccb88964d11fab7a1eea4d169bba20fffe9fab44bccd320d559b443da`  
		Last Modified: Thu, 17 Mar 2022 08:47:07 GMT  
		Size: 6.4 MB (6384705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
