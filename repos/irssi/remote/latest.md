## `irssi:latest`

```console
$ docker pull irssi@sha256:682f32f8a7f163ddb31130094957b1cf95e3ba6b51c46c5e83e8339e93003fa5
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
$ docker pull irssi@sha256:1e32949b8ccefb73568dbf2a4a83f21be8269578bb4745a2bd64b6088478310c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50601059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:062977003ea314e7f36e43858f2d947140c868c9c2c81d87db183d2b8168f016`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 12:29:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:29:07 GMT
ENV HOME=/home/user
# Tue, 12 Oct 2021 12:29:07 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Oct 2021 12:29:08 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 12:29:08 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 12 Oct 2021 12:30:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Oct 2021 12:30:58 GMT
WORKDIR /home/user
# Tue, 12 Oct 2021 12:30:58 GMT
USER user
# Tue, 12 Oct 2021 12:30:59 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b005ed3201fa289b98f8fe9ff68b8fd7ec11fe1a7123c8242a1c850f6fae6f36`  
		Last Modified: Tue, 12 Oct 2021 12:31:39 GMT  
		Size: 17.0 MB (17023772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ecc459893fe8bd1d9f6e921cd68cb8f523b6fd9a9f2fff699baf4ba22ce0fd`  
		Last Modified: Tue, 12 Oct 2021 12:31:33 GMT  
		Size: 4.2 KB (4206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ad90d31c4b9ef63a4c6f608f9fcb697c0edc713395fcf1599d1e6e074fd1c8`  
		Last Modified: Tue, 12 Oct 2021 12:31:36 GMT  
		Size: 6.4 MB (6433571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm variant v5

```console
$ docker pull irssi@sha256:129739526060c81cc4bde28067e78cc58db6e2e618b77aa4ce09721b376bd91c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46864002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbd9c5a8aa55bf049beb205a8dd1112698c6386d80b6c095825255b2f34eedae`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Oct 2021 00:51:32 GMT
ADD file:0d95eee31ffe3f4260263e4fac2a61123a4b98d2e7a67efcc7bfea338c54f41d in / 
# Tue, 12 Oct 2021 00:51:32 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 11:45:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 11:45:05 GMT
ENV HOME=/home/user
# Tue, 12 Oct 2021 11:45:07 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Oct 2021 11:45:07 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 11:45:08 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 12 Oct 2021 11:47:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Oct 2021 11:47:11 GMT
WORKDIR /home/user
# Tue, 12 Oct 2021 11:47:11 GMT
USER user
# Tue, 12 Oct 2021 11:47:12 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:175b083b22fb061f7d1894fe4916a2967ce636d47376da526d90d57c8f7efc60`  
		Last Modified: Tue, 12 Oct 2021 01:07:45 GMT  
		Size: 24.9 MB (24872704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8ba1bf702bf6855070908160c403a7f011fb0b18478b66a37f35ad1db0d4c0`  
		Last Modified: Tue, 12 Oct 2021 11:48:02 GMT  
		Size: 15.9 MB (15922602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35437390eb1642d22184243003945d40b147284a8c70dccd7ab38293581bc78`  
		Last Modified: Tue, 12 Oct 2021 11:47:46 GMT  
		Size: 4.2 KB (4193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c5baee4f6db64503236f380e7c545b402522ea5f64e0329b3ccb87a083544ea`  
		Last Modified: Tue, 12 Oct 2021 11:47:50 GMT  
		Size: 6.1 MB (6064503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm variant v7

```console
$ docker pull irssi@sha256:939ab44e389fb1dcd8539414813d73d17b8b97ab6b803505af8e8e25754ac581
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44259449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82a5209718aea8826d4bab9b751ecb9275774ce8098db93133e32f269ad78bf9`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:45:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:45:16 GMT
ENV HOME=/home/user
# Tue, 12 Oct 2021 05:45:18 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Oct 2021 05:45:18 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 05:45:19 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 12 Oct 2021 05:47:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Oct 2021 05:47:10 GMT
WORKDIR /home/user
# Tue, 12 Oct 2021 05:47:11 GMT
USER user
# Tue, 12 Oct 2021 05:47:11 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c6fb4e9c1ab694039ac7d2060f68aaddd264a9196f0cee640d4d547841815f`  
		Last Modified: Tue, 12 Oct 2021 05:48:33 GMT  
		Size: 15.6 MB (15583024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0f39ead0712be7783f4762f578cf81bff7138ae09d0f6304456ac597e9786d`  
		Last Modified: Tue, 12 Oct 2021 05:48:17 GMT  
		Size: 4.2 KB (4191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95f23eae92cf2c75f4b171e1f38903f6fdb2185ff00e2fb9a2de1766fe7adc1`  
		Last Modified: Tue, 12 Oct 2021 05:48:21 GMT  
		Size: 5.9 MB (5932536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:4543305b7e3d9d996dfb9e284a04894f87ecee5ef6dd9a830fe4456e18e00bb2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48884023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56fb3af9cd5aaed2a52238a7be79f099941651c5adae3a389901af0137aad0f6`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Sat, 13 Nov 2021 06:26:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 13 Nov 2021 06:26:20 GMT
ENV HOME=/home/user
# Sat, 13 Nov 2021 06:26:21 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 13 Nov 2021 06:26:22 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 06:26:23 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 13 Nov 2021 06:27:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 13 Nov 2021 06:27:16 GMT
WORKDIR /home/user
# Sat, 13 Nov 2021 06:27:17 GMT
USER user
# Sat, 13 Nov 2021 06:27:18 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5407b19ec4e69fe0f727336fba762f1f09adacec268bed9947d877476b07f3e3`  
		Last Modified: Sat, 13 Nov 2021 06:29:07 GMT  
		Size: 16.8 MB (16795488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6146d159944c4b740284fb1efb12599e33e3ee9805bd9e63a694895145aa8dc`  
		Last Modified: Sat, 13 Nov 2021 06:29:03 GMT  
		Size: 4.1 KB (4076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124d369634a1881d5bc048e103d34f04f2b7e09c73d48a5c675be8c3a162bd9f`  
		Last Modified: Sat, 13 Nov 2021 06:29:04 GMT  
		Size: 6.2 MB (6175980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; 386

```console
$ docker pull irssi@sha256:32f25796e3fb4ce918afdc3f718db0a460686f24a9ac441d8a9b0d5f782a7186
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50448187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d69d4fc5d0ac00634b670c29f8201bba0568f7c3cb26da768f93c3b0fa732e45`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Oct 2021 01:40:17 GMT
ADD file:1b432d2306b487c59442b30c65ddabd08b45484c6ce09b0c25112c29f4a98f17 in / 
# Tue, 12 Oct 2021 01:40:17 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:09:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:10:00 GMT
ENV HOME=/home/user
# Tue, 12 Oct 2021 02:10:01 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Oct 2021 02:10:01 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 02:10:01 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 12 Oct 2021 02:11:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Oct 2021 02:11:52 GMT
WORKDIR /home/user
# Tue, 12 Oct 2021 02:11:53 GMT
USER user
# Tue, 12 Oct 2021 02:11:53 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:860d012fe46ce39c3737ace24d10d8ad65ae9c78abde6891ca6e97b0d7f271dd`  
		Last Modified: Tue, 12 Oct 2021 01:48:37 GMT  
		Size: 27.8 MB (27791445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22b775a122d57dd802b3fe320f46d00c1014473776db028811421f342d2a018`  
		Last Modified: Tue, 12 Oct 2021 02:12:39 GMT  
		Size: 16.5 MB (16547042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7603d2bea90c7b89384038aaf61333b86fb1de19df490cbf74e72e9edc2350a0`  
		Last Modified: Tue, 12 Oct 2021 02:12:33 GMT  
		Size: 4.2 KB (4197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c81a5a299eaccfc5d80d6ddd48a34eb9f59a1681d6c6414710b00d87e08a9dd`  
		Last Modified: Tue, 12 Oct 2021 02:12:35 GMT  
		Size: 6.1 MB (6105503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; mips64le

```console
$ docker pull irssi@sha256:1ca8a12e6da64d85b875579653d03d87d057ed5bcbe4e5c3cb906828306d07af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47801561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:938932492bc107408f0f09704b1c1c699e68c270ab06c85fae67bdfd1522891a`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Oct 2021 01:12:07 GMT
ADD file:a467fbf2015350da455cad98b5f5f247d88749cf317062ca09c466c27d53f87b in / 
# Tue, 12 Oct 2021 01:12:07 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 01:45:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 01:45:04 GMT
ENV HOME=/home/user
# Tue, 12 Oct 2021 01:45:06 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Oct 2021 01:45:06 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 01:45:07 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 12 Oct 2021 01:47:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Oct 2021 01:47:43 GMT
WORKDIR /home/user
# Tue, 12 Oct 2021 01:47:43 GMT
USER user
# Tue, 12 Oct 2021 01:47:44 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4d8cdee9d607e77b6f8c2203cc9cc02b38004def2b7fe162538c1538da10c870`  
		Last Modified: Tue, 12 Oct 2021 01:21:36 GMT  
		Size: 25.8 MB (25806535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab43f75905844891d3ecee1fa5c42c9efdc9fbf399823869d463ee0ec6fcb417`  
		Last Modified: Tue, 12 Oct 2021 01:48:18 GMT  
		Size: 15.7 MB (15698159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713dd93900bdb355c112537c15064e27f43f4ace85bb00d0af5c1d1ac91314b2`  
		Last Modified: Tue, 12 Oct 2021 01:48:01 GMT  
		Size: 4.2 KB (4178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be476970595ea42de4dd244e19e9d7c08d6e8d16e24e3194084d00ab224496f`  
		Last Modified: Tue, 12 Oct 2021 01:48:07 GMT  
		Size: 6.3 MB (6292689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; ppc64le

```console
$ docker pull irssi@sha256:8dda88ff8ca3aae06d98832f49c377c9895e1b9217e5507869ca7804ece07020
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54765963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3555b72ae4067258ebf60ce1bb623b15536987952bad18d00509e17bab30e8ff`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Oct 2021 01:26:46 GMT
ADD file:5526880c6f19a4b4231a8b2bd7cfc625d116764c4918eff6f0b55f8c1eb38e1a in / 
# Tue, 12 Oct 2021 01:26:50 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 06:59:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 06:59:10 GMT
ENV HOME=/home/user
# Tue, 12 Oct 2021 06:59:35 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Oct 2021 06:59:39 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 06:59:45 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 12 Oct 2021 07:05:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Oct 2021 07:05:54 GMT
WORKDIR /home/user
# Tue, 12 Oct 2021 07:05:56 GMT
USER user
# Tue, 12 Oct 2021 07:05:59 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:d69973af32573c07c8789c0f9c144a5c0b822a1e85b59db3ce9f8ebc489ce85d`  
		Last Modified: Tue, 12 Oct 2021 01:38:40 GMT  
		Size: 30.5 MB (30547197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b801c8c1faeb53e77886b8bd7404df5cc5831a996288879050244a0012431252`  
		Last Modified: Tue, 12 Oct 2021 07:06:42 GMT  
		Size: 17.4 MB (17431416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9eb7059bc445124e2341403f223da5c96ff3b2f3ea32be156454fc909ded299`  
		Last Modified: Tue, 12 Oct 2021 07:06:37 GMT  
		Size: 4.2 KB (4228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c992d416f9a1370f66cc25167921c871fca544e5ab3dbf2d9e855466577a58c5`  
		Last Modified: Tue, 12 Oct 2021 07:06:39 GMT  
		Size: 6.8 MB (6783122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; s390x

```console
$ docker pull irssi@sha256:44160b4b2a7e2658526d5643b5edbb4e8f96d9713f5f1af3fe80ad70ef13a1e7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49043087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7165ef62b0dad2a1f2f58a154efcf596f64d4bdc93e9b4a8774635dcc09e097d`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 12 Oct 2021 00:42:56 GMT
ADD file:39da9acd4d06d69f3ca8d25ef5c097ae741972d6b15a6a057bc7487380157b61 in / 
# Tue, 12 Oct 2021 00:42:57 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 06:56:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 06:56:45 GMT
ENV HOME=/home/user
# Tue, 12 Oct 2021 06:56:45 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 12 Oct 2021 06:56:45 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 06:56:45 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 12 Oct 2021 06:57:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 12 Oct 2021 06:57:31 GMT
WORKDIR /home/user
# Tue, 12 Oct 2021 06:57:31 GMT
USER user
# Tue, 12 Oct 2021 06:57:31 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:78a640c6bb4733e5156ce97c5ec773cf97b357c3a07244348384da5060788a61`  
		Last Modified: Tue, 12 Oct 2021 00:48:41 GMT  
		Size: 25.8 MB (25754252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3765c7afb62a3b4109b0345621f825816741afdb2bf30572c28fab0910e52211`  
		Last Modified: Tue, 12 Oct 2021 06:58:06 GMT  
		Size: 16.9 MB (16899883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f94a74eb15b964a89599921c4d0a02b916ff726bcafe8325d0e9b1b37730961`  
		Last Modified: Tue, 12 Oct 2021 06:58:03 GMT  
		Size: 4.2 KB (4209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674e53d446d987a72c382e279295b75ac8c44e07c5ffac5af0d54b01b3e7e249`  
		Last Modified: Tue, 12 Oct 2021 06:58:04 GMT  
		Size: 6.4 MB (6384743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
