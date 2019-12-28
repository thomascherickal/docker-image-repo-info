## `irssi:latest`

```console
$ docker pull irssi@sha256:12d8b760fe84a08bbf0939158f9750c760255e10a7e1eac8710f0a9d01cb9053
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
$ docker pull irssi@sha256:fceaa1c24ae9b2bcea8f7b4646030d22f94a3751225cb749ed8e735069358749
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51551616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ba00a45689070653199efcc7646b5fddf24ab47a59e87a818a5b0689c9bb135`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 00:37:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libglib2.0-0 		libwww-perl 		perl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:37:43 GMT
ENV HOME=/home/user
# Sat, 23 Nov 2019 00:37:44 GMT
RUN useradd --create-home --home-dir $HOME user 	&& mkdir -p $HOME/.irssi 	&& chown -R user:user $HOME
# Sat, 23 Nov 2019 00:37:44 GMT
ENV LANG=C.UTF-8
# Sat, 23 Nov 2019 00:37:44 GMT
ENV IRSSI_VERSION=1.2.2
# Sat, 23 Nov 2019 00:38:45 GMT
RUN buildDeps=' 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	' 	&& set -x 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 	&& rm -rf /var/lib/apt/lists/* 	&& wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz 	&& wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1 	&& gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz 	&& gpgconf --kill all 	&& rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc 	&& mkdir -p /usr/src/irssi 	&& tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1 	&& rm /tmp/irssi.tar.xz 	&& cd /usr/src/irssi 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/irssi 	&& apt-get purge -y --auto-remove $buildDeps
# Sat, 23 Nov 2019 00:38:46 GMT
WORKDIR /home/user
# Sat, 23 Nov 2019 00:38:46 GMT
USER user
# Sat, 23 Nov 2019 00:38:46 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5063b42097898ad79993342546e0817c6a5a32f8fc431cc800223b1db2cedcd0`  
		Last Modified: Sat, 23 Nov 2019 00:39:03 GMT  
		Size: 18.7 MB (18741794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2448d4490610658a0c6171c9135c61e182f06380849d9407af447601f624f53`  
		Last Modified: Sat, 23 Nov 2019 00:38:58 GMT  
		Size: 4.2 KB (4172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d68c08ce70bf49ca774f55df45d371ea6a8d7a8d5079d794648a54be77931c8c`  
		Last Modified: Sat, 23 Nov 2019 00:39:00 GMT  
		Size: 10.3 MB (10281078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm variant v5

```console
$ docker pull irssi@sha256:b95d702b961abae34c8a789b7d443c8a1ecfbf0e48f4806f6d4cd65682c6473a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47865117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99b837d7ce89ff440d561070aa2b48ace599c4086bbc586eab5ba60c3a140017`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:53:16 GMT
ADD file:7d6af454b55cb354e31c096e935358dd5914688ded04ebc76243a4ff598c4495 in / 
# Sat, 28 Dec 2019 04:53:18 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:23:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libglib2.0-0 		libwww-perl 		perl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 07:23:17 GMT
ENV HOME=/home/user
# Sat, 28 Dec 2019 07:23:22 GMT
RUN useradd --create-home --home-dir $HOME user 	&& mkdir -p $HOME/.irssi 	&& chown -R user:user $HOME
# Sat, 28 Dec 2019 07:23:23 GMT
ENV LANG=C.UTF-8
# Sat, 28 Dec 2019 07:23:23 GMT
ENV IRSSI_VERSION=1.2.2
# Sat, 28 Dec 2019 07:25:11 GMT
RUN buildDeps=' 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	' 	&& set -x 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 	&& rm -rf /var/lib/apt/lists/* 	&& wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz 	&& wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1 	&& gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz 	&& gpgconf --kill all 	&& rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc 	&& mkdir -p /usr/src/irssi 	&& tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1 	&& rm /tmp/irssi.tar.xz 	&& cd /usr/src/irssi 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/irssi 	&& apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 07:25:13 GMT
WORKDIR /home/user
# Sat, 28 Dec 2019 07:25:14 GMT
USER user
# Sat, 28 Dec 2019 07:25:15 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:af28f499fd964f4506ea46c2ac342bc52328a8c30cd633661b69f383a5144e9b`  
		Last Modified: Sat, 28 Dec 2019 05:00:23 GMT  
		Size: 21.2 MB (21202822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c01f040c41ab659447df558bac450d5ed5fdbf7791faa7713b5fb3cd30fecb`  
		Last Modified: Sat, 28 Dec 2019 07:25:41 GMT  
		Size: 17.5 MB (17515901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505157c39fc96fefcb2f712c1f0ebbd7bcb3a792876913d20308f67d1f9c71d0`  
		Last Modified: Sat, 28 Dec 2019 07:25:31 GMT  
		Size: 4.2 KB (4185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e7d9570eb87e3639c662dbeef52c6eefb6f59217f577c2065a0ee7d126edda`  
		Last Modified: Sat, 28 Dec 2019 07:25:35 GMT  
		Size: 9.1 MB (9142209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm variant v7

```console
$ docker pull irssi@sha256:322a7046ce8123140f26534065241996c8cb0ceae2b260b8e96abe844ae09ebc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45112271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b35e4c0802696baf0328fd44223061663b855c0995d3b5e7fd24c9458f78ef1`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:13:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libglib2.0-0 		libwww-perl 		perl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 07:13:48 GMT
ENV HOME=/home/user
# Sat, 28 Dec 2019 07:13:50 GMT
RUN useradd --create-home --home-dir $HOME user 	&& mkdir -p $HOME/.irssi 	&& chown -R user:user $HOME
# Sat, 28 Dec 2019 07:13:51 GMT
ENV LANG=C.UTF-8
# Sat, 28 Dec 2019 07:13:52 GMT
ENV IRSSI_VERSION=1.2.2
# Sat, 28 Dec 2019 07:15:48 GMT
RUN buildDeps=' 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	' 	&& set -x 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 	&& rm -rf /var/lib/apt/lists/* 	&& wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz 	&& wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1 	&& gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz 	&& gpgconf --kill all 	&& rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc 	&& mkdir -p /usr/src/irssi 	&& tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1 	&& rm /tmp/irssi.tar.xz 	&& cd /usr/src/irssi 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/irssi 	&& apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 07:15:52 GMT
WORKDIR /home/user
# Sat, 28 Dec 2019 07:15:54 GMT
USER user
# Sat, 28 Dec 2019 07:15:55 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f96fcac748b2592caf99942ae0799237ab5f022bceab39f1f3accb91a3d7141`  
		Last Modified: Sat, 28 Dec 2019 07:16:27 GMT  
		Size: 17.0 MB (17010048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086e9e3818781609ef57fea1fd08208d947ea3fcdd4afc7bffd4399bd7cda5ac`  
		Last Modified: Sat, 28 Dec 2019 07:16:19 GMT  
		Size: 4.2 KB (4193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3065b76bfe928fb26a64db03b1bb645430d16f56eece249345a81a9c73c19b37`  
		Last Modified: Sat, 28 Dec 2019 07:16:23 GMT  
		Size: 8.8 MB (8786443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:9879e98aec2ea4fcc2a4229cf9aca83573b96eab5a505ff60c312f92cb5aeef1
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47823730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8fb65ddf906788b4d6800238faf5292ff33f277ccf2e996617379c9143eeab4`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:43:36 GMT
ADD file:ba40f5080cbd89c576c350bfe5acfe16f2ec59636fdb082efc3a8cef66ae7cb7 in / 
# Sat, 28 Dec 2019 04:43:39 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 08:29:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libglib2.0-0 		libwww-perl 		perl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:29:29 GMT
ENV HOME=/home/user
# Sat, 28 Dec 2019 08:29:31 GMT
RUN useradd --create-home --home-dir $HOME user 	&& mkdir -p $HOME/.irssi 	&& chown -R user:user $HOME
# Sat, 28 Dec 2019 08:29:31 GMT
ENV LANG=C.UTF-8
# Sat, 28 Dec 2019 08:29:32 GMT
ENV IRSSI_VERSION=1.2.2
# Sat, 28 Dec 2019 08:31:42 GMT
RUN buildDeps=' 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	' 	&& set -x 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 	&& rm -rf /var/lib/apt/lists/* 	&& wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz 	&& wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1 	&& gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz 	&& gpgconf --kill all 	&& rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc 	&& mkdir -p /usr/src/irssi 	&& tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1 	&& rm /tmp/irssi.tar.xz 	&& cd /usr/src/irssi 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/irssi 	&& apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 08:31:44 GMT
WORKDIR /home/user
# Sat, 28 Dec 2019 08:31:45 GMT
USER user
# Sat, 28 Dec 2019 08:31:46 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:588374d57fdb5120d024340eef3d8927af23a5b806d41b4f049ee430a153c0b4`  
		Last Modified: Sat, 28 Dec 2019 04:49:14 GMT  
		Size: 20.4 MB (20385801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c6dd34c63bf4b76dc826fb9d471f1eaea283415a41d056060258d34bd46394`  
		Last Modified: Sat, 28 Dec 2019 08:32:21 GMT  
		Size: 17.9 MB (17856036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a226c8cd92dafcb2cd4d2c1b3160a83eae752c029ff441da3b56298d91addf`  
		Last Modified: Sat, 28 Dec 2019 08:32:14 GMT  
		Size: 4.2 KB (4200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca90a5652293eac903417c2896bd8d44152ba18a4d98e77dfb149145b7d013f`  
		Last Modified: Sat, 28 Dec 2019 08:32:18 GMT  
		Size: 9.6 MB (9577693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; 386

```console
$ docker pull irssi@sha256:4356307224be3309a3b9e973871be8073f0e53b9af8e6168b6c4d44dda5fa4b2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54900129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32df0f4a0812f79492c7c76c626d5cf8af00575453e4351d38e4fce5740e9861`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:42:05 GMT
ADD file:d43798bcf0e72b342c261b8585dde072d9363d19fab4b8d9f08f15db189f287b in / 
# Sat, 28 Dec 2019 04:42:05 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:49:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libglib2.0-0 		libwww-perl 		perl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:49:09 GMT
ENV HOME=/home/user
# Sat, 28 Dec 2019 05:49:10 GMT
RUN useradd --create-home --home-dir $HOME user 	&& mkdir -p $HOME/.irssi 	&& chown -R user:user $HOME
# Sat, 28 Dec 2019 05:49:10 GMT
ENV LANG=C.UTF-8
# Sat, 28 Dec 2019 05:49:10 GMT
ENV IRSSI_VERSION=1.2.2
# Sat, 28 Dec 2019 05:50:43 GMT
RUN buildDeps=' 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	' 	&& set -x 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 	&& rm -rf /var/lib/apt/lists/* 	&& wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz 	&& wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1 	&& gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz 	&& gpgconf --kill all 	&& rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc 	&& mkdir -p /usr/src/irssi 	&& tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1 	&& rm /tmp/irssi.tar.xz 	&& cd /usr/src/irssi 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/irssi 	&& apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 05:50:44 GMT
WORKDIR /home/user
# Sat, 28 Dec 2019 05:50:44 GMT
USER user
# Sat, 28 Dec 2019 05:50:44 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2cb401c016d2f9802d5ef9cf6c6dc07251e9f87757a0de0a8df318fb7f00385c`  
		Last Modified: Sat, 28 Dec 2019 04:47:36 GMT  
		Size: 23.2 MB (23152142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2cab5d941f7b7b821fd657d73363f098eb38a2090dbee3667f063907776da55`  
		Last Modified: Sat, 28 Dec 2019 05:51:05 GMT  
		Size: 18.4 MB (18429305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c776858f645be861ae7f4fb2519d20db7a7b134fe920274cbe7c8d31c591f15`  
		Last Modified: Sat, 28 Dec 2019 05:50:57 GMT  
		Size: 4.2 KB (4160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d81352acd980a1c01f5571c34cc71c9b41600c8dba95077d00ca94010ed2091`  
		Last Modified: Sat, 28 Dec 2019 05:51:02 GMT  
		Size: 13.3 MB (13314522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; ppc64le

```console
$ docker pull irssi@sha256:c335ec5fbd6f15ebf7bafa583b4ba8ab6415f687e1f9f8dfda26d86960a31b6c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51282154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec2fd2882955eafcdb65d1da3725f0b05f401f504ac15b49b90b3feff4f49331`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:21 GMT
ADD file:a1ee5955ff3ede8df9558f4bec0c7962d54c43374f857e1da7e2639ddf82a9f1 in / 
# Sat, 28 Dec 2019 04:23:24 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 08:42:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libglib2.0-0 		libwww-perl 		perl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:42:44 GMT
ENV HOME=/home/user
# Sat, 28 Dec 2019 08:42:52 GMT
RUN useradd --create-home --home-dir $HOME user 	&& mkdir -p $HOME/.irssi 	&& chown -R user:user $HOME
# Sat, 28 Dec 2019 08:42:54 GMT
ENV LANG=C.UTF-8
# Sat, 28 Dec 2019 08:42:56 GMT
ENV IRSSI_VERSION=1.2.2
# Sat, 28 Dec 2019 08:45:37 GMT
RUN buildDeps=' 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	' 	&& set -x 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 	&& rm -rf /var/lib/apt/lists/* 	&& wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz 	&& wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1 	&& gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz 	&& gpgconf --kill all 	&& rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc 	&& mkdir -p /usr/src/irssi 	&& tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1 	&& rm /tmp/irssi.tar.xz 	&& cd /usr/src/irssi 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/irssi 	&& apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 08:45:40 GMT
WORKDIR /home/user
# Sat, 28 Dec 2019 08:45:43 GMT
USER user
# Sat, 28 Dec 2019 08:45:45 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:af52e7ef6e83efadeae17be91daa6ecf61b7dfb39709c29be9b24876e60c0e36`  
		Last Modified: Sat, 28 Dec 2019 04:33:19 GMT  
		Size: 22.8 MB (22800791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:429b34b33a101026b231eb4a0bac99a8cbe7465d249248cd8801d53881cbb564`  
		Last Modified: Sat, 28 Dec 2019 08:46:23 GMT  
		Size: 18.2 MB (18180739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df81bd98b73bb164dac838c9cbffaf09b287ea8359c71c43a78d4d78ad56b6c`  
		Last Modified: Sat, 28 Dec 2019 08:46:16 GMT  
		Size: 4.2 KB (4198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8478a7061b53f33072600977a759460905447818585e9322eafb21ad1e8408`  
		Last Modified: Sat, 28 Dec 2019 08:46:20 GMT  
		Size: 10.3 MB (10296426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; s390x

```console
$ docker pull irssi@sha256:4575594d26c237cf4ee2129f1cfbad37724ae5fa147fb23be759e1ed1d3aa9a5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52494005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:866eda2042c2eec2b746fa3fc5123171753337517168301c4f940ac479551c89`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 Dec 2019 04:43:21 GMT
ADD file:f5d0e8fb7b76fc65fc5a0951e7d647f26d110f5c92d4effe2ada348f661c87af in / 
# Sat, 28 Dec 2019 04:43:21 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:58:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libglib2.0-0 		libwww-perl 		perl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:58:49 GMT
ENV HOME=/home/user
# Sat, 28 Dec 2019 05:58:50 GMT
RUN useradd --create-home --home-dir $HOME user 	&& mkdir -p $HOME/.irssi 	&& chown -R user:user $HOME
# Sat, 28 Dec 2019 05:58:50 GMT
ENV LANG=C.UTF-8
# Sat, 28 Dec 2019 05:58:50 GMT
ENV IRSSI_VERSION=1.2.2
# Sat, 28 Dec 2019 05:59:34 GMT
RUN buildDeps=' 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	' 	&& set -x 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 	&& rm -rf /var/lib/apt/lists/* 	&& wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz 	&& wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1 	&& gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz 	&& gpgconf --kill all 	&& rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc 	&& mkdir -p /usr/src/irssi 	&& tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1 	&& rm /tmp/irssi.tar.xz 	&& cd /usr/src/irssi 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	&& make -j "$(nproc)" 	&& make install 	&& rm -rf /usr/src/irssi 	&& apt-get purge -y --auto-remove $buildDeps
# Sat, 28 Dec 2019 05:59:34 GMT
WORKDIR /home/user
# Sat, 28 Dec 2019 05:59:34 GMT
USER user
# Sat, 28 Dec 2019 05:59:35 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:9498763e47873a85a1a6b3ba1f12b6936fcd769bb6b0d094c36c0dd6435bb902`  
		Last Modified: Sat, 28 Dec 2019 04:46:38 GMT  
		Size: 22.4 MB (22380154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8556c0656691ac4def0fbdc2f62b54a304b1e979699dff3266259fb6d2ccda59`  
		Last Modified: Sat, 28 Dec 2019 06:00:02 GMT  
		Size: 18.8 MB (18820370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04406de3e7518bfdbfef78de8612f9e5e94d8995fda997c35ee90c80963798b0`  
		Last Modified: Sat, 28 Dec 2019 05:59:58 GMT  
		Size: 4.2 KB (4180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe7db9c217468756b6d36f8262c7e2fa70d5ab498c1e1cdf6d62a72897d2ddb`  
		Last Modified: Sat, 28 Dec 2019 06:00:00 GMT  
		Size: 11.3 MB (11289301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
