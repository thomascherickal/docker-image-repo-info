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
$ docker pull irssi@sha256:21aebe0f969df877f64465e13ac0b228c7dadf841b3a220b3288a71d9a0db022
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
$ docker pull irssi@sha256:73eeea3fe8864f534c05c5720ef3f08b4a143b8ef3a8d015da100094dad6a835
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50616927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a221922d64e7a5f2ceab14950bc25d7824ed11accd24cb3606aad52bec0afd81`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:51:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 09:51:55 GMT
ENV HOME=/home/user
# Wed, 20 Apr 2022 09:51:56 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Apr 2022 09:51:56 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 09:51:56 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 20 Apr 2022 09:52:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Apr 2022 09:52:41 GMT
WORKDIR /home/user
# Wed, 20 Apr 2022 09:52:41 GMT
USER user
# Wed, 20 Apr 2022 09:52:41 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b90d559f62672d2aaa0b155cc1e81f4c0335f6c6d5992301536b307f6ecfc5f`  
		Last Modified: Wed, 20 Apr 2022 09:53:08 GMT  
		Size: 17.0 MB (17038607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca716a8e2f28387368616a6e17f95b7c147c78e12a279c467e642ef17dcffbc8`  
		Last Modified: Wed, 20 Apr 2022 09:53:04 GMT  
		Size: 4.2 KB (4203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a954de24a56a094455fc42c1d5826fcad65a0a8db6ffbf144f81f9417109d898`  
		Last Modified: Wed, 20 Apr 2022 09:53:05 GMT  
		Size: 6.4 MB (6433453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm variant v5

```console
$ docker pull irssi@sha256:5bda585bef4c01cf35df8f01f9c0f1fd8fb01ca4f18ad62efc210468febf3366
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46895518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a8f29e5ecc0f86367a380847eee70dccc7e50983ffe21a0a10517802e2c3982`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Apr 2022 07:17:47 GMT
ADD file:5b740716d202d2f3494df5e108c0ba999125920ed9c97803fe0ccdfeba5cf518 in / 
# Wed, 20 Apr 2022 07:17:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:36:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 13:36:19 GMT
ENV HOME=/home/user
# Wed, 20 Apr 2022 13:36:21 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Apr 2022 13:36:21 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 13:36:22 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 20 Apr 2022 13:38:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Apr 2022 13:38:14 GMT
WORKDIR /home/user
# Wed, 20 Apr 2022 13:38:14 GMT
USER user
# Wed, 20 Apr 2022 13:38:14 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1fc8704cfa531d4583c5d4d571b836a82c02a812dae88792c4397cf1c1770405`  
		Last Modified: Wed, 20 Apr 2022 07:33:54 GMT  
		Size: 24.9 MB (24889592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d712999a90ba1db6fb4a832bbfda68dc7ab9cd398b5c16e489f0e2f26b27bb62`  
		Last Modified: Wed, 20 Apr 2022 13:39:03 GMT  
		Size: 15.9 MB (15937246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8209faf477433cd094581e5465a0a9f0d917a546715580161097219fa9b9d56`  
		Last Modified: Wed, 20 Apr 2022 13:38:46 GMT  
		Size: 4.2 KB (4196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:102dcf521e04ca2d60a4752626d29b240b0d22690dd5a8831f660b9dd997469c`  
		Last Modified: Wed, 20 Apr 2022 13:38:50 GMT  
		Size: 6.1 MB (6064484 bytes)  
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
$ docker pull irssi@sha256:006b8def53f48a57a1adc76c8bb48271d1c323dff2e46a8a78dd9bec1acfca3a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48903268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6bcfcb3be6ccc226ff30616bc214852c32389d7a7cb1f8efb027ce7f97b28e0`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:25:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 09:25:18 GMT
ENV HOME=/home/user
# Wed, 20 Apr 2022 09:25:19 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Apr 2022 09:25:19 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 09:25:20 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 20 Apr 2022 09:26:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Apr 2022 09:26:04 GMT
WORKDIR /home/user
# Wed, 20 Apr 2022 09:26:05 GMT
USER user
# Wed, 20 Apr 2022 09:26:06 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f0468f2e47c92a374ac255a77884dcad97c6f37a5b458ff6f92188bca6d82c`  
		Last Modified: Wed, 20 Apr 2022 09:26:43 GMT  
		Size: 16.8 MB (16814853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177a8142bec8627b6eb8c372f76448f218e274d1ff21e6d19ec4a11ea1ee059d`  
		Last Modified: Wed, 20 Apr 2022 09:26:39 GMT  
		Size: 4.1 KB (4068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b72a244dd871eb4792d547404ef3800c8df98aed91e81950218bd44f82df1d`  
		Last Modified: Wed, 20 Apr 2022 09:26:40 GMT  
		Size: 6.2 MB (6175998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; 386

```console
$ docker pull irssi@sha256:821ad21b1a160f11558a20323bf0f1479cafd575e0440a655f996e14e7246b41
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50263111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c21a608d1eff21f66971c0fc5646baadb692a8a78541e095ae26befc626e6fee`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Apr 2022 07:38:03 GMT
ADD file:602a25173054242f635a5a299845b7f1b56864ac5d3b8af1ae29dec3a9da119f in / 
# Wed, 20 Apr 2022 07:38:04 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:39:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:39:47 GMT
ENV HOME=/home/user
# Wed, 20 Apr 2022 12:39:48 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Apr 2022 12:39:49 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 12:39:50 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 20 Apr 2022 12:40:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Apr 2022 12:40:40 GMT
WORKDIR /home/user
# Wed, 20 Apr 2022 12:40:41 GMT
USER user
# Wed, 20 Apr 2022 12:40:42 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a13b13d818745c4d2234aab71df26e4a01bfe59f396ab62f20d156b94803650c`  
		Last Modified: Wed, 20 Apr 2022 07:45:46 GMT  
		Size: 27.8 MB (27799825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd1690b27b64a6ece24dd4be73f7615988de276e59d5202b15cf379006d6b4c`  
		Last Modified: Wed, 20 Apr 2022 12:41:16 GMT  
		Size: 16.6 MB (16565741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2093fb439f2ad43eb953b6195e8da3ba5227d26a7a53ce4daf3d435131b42bd1`  
		Last Modified: Wed, 20 Apr 2022 12:41:13 GMT  
		Size: 4.1 KB (4052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fa17d08104200257a36b7d8baf7ac42fe3b14d21847439379ec371347da717`  
		Last Modified: Wed, 20 Apr 2022 12:41:14 GMT  
		Size: 5.9 MB (5893493 bytes)  
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
$ docker pull irssi@sha256:674d6845c5de4d8e243e168fb56a649d7fb8a4c77ea53f46517b68bf5ca072cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49061909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40f0e08be1db449f78356ac19326266df23eced238602b70ea697e10ecde3c1e`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Apr 2022 08:40:41 GMT
ADD file:e9840ab2ce3aeff61b68bf4837f65471a86dcba02c5023863f3e7493098b07ba in / 
# Wed, 20 Apr 2022 08:40:45 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:54:45 GMT
ENV HOME=/home/user
# Wed, 20 Apr 2022 12:54:46 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Apr 2022 12:54:47 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 12:54:47 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 20 Apr 2022 12:55:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Apr 2022 12:55:39 GMT
WORKDIR /home/user
# Wed, 20 Apr 2022 12:55:39 GMT
USER user
# Wed, 20 Apr 2022 12:55:39 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b59fdcf2cb29d2ee4dd08aa08a467372e33525431c4caba9b01e9eb28f76425f`  
		Last Modified: Wed, 20 Apr 2022 08:50:14 GMT  
		Size: 25.8 MB (25758600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84aa94504e16d563a7f953f43b8bb95b13d5156527a49986656ed7e79ecbb456`  
		Last Modified: Wed, 20 Apr 2022 12:56:19 GMT  
		Size: 16.9 MB (16914203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349fa3b5b2db4893cb2724353ac6f146f52e097b86480a4dc1d1831f2b7db8f5`  
		Last Modified: Wed, 20 Apr 2022 12:56:16 GMT  
		Size: 4.2 KB (4210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f92d4d941d09ed135194b56663949c39da03fd1ea1de785a9aac2a7947daf3`  
		Last Modified: Wed, 20 Apr 2022 12:56:17 GMT  
		Size: 6.4 MB (6384896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1-alpine`

```console
$ docker pull irssi@sha256:bfbb6e415dbf4cd1ea2d6bd42bdcc5fcc054d6b053c6d07b983c9b390dac8f9d
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
$ docker pull irssi@sha256:c38f2415219abd42abe51fa4eaf222d8d7c7bdebb86910500d59bb7d0c21b231
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18648499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6c0676773ef4ea9992d62133ac02ba861fde6dd9ba437e8fb36eaf4aae78852`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:18:16 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 11:18:17 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 11:18:17 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 11:18:17 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 11:18:17 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 11:19:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 11:19:01 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 11:19:01 GMT
USER user
# Tue, 05 Apr 2022 11:19:01 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa1dbdb27d63340f8b8fa494a282aeded5f878185e2847d6dfb481b353b8c11`  
		Last Modified: Tue, 05 Apr 2022 11:19:27 GMT  
		Size: 9.5 MB (9540662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30dd245485e0307925fa298d8f511fe481b6600ce336c8ff0a0b5c13ce1435d9`  
		Last Modified: Tue, 05 Apr 2022 11:19:24 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4513426f1a6993290c7fa1e95a9f0bd0309456d69e3c04c0a7e8b17b66c9a079`  
		Last Modified: Tue, 05 Apr 2022 11:19:25 GMT  
		Size: 6.3 MB (6287259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:5262462a3f32457835863ac8b11823de2d926d672219bdff8c5c67bc5e116e2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17385410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab49acd659041f4c479472bb7ed35e0fc93656b968625544d96599e44c57c01`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:50:07 GMT
ADD file:9e96de1fefc4e9efba26e76103eca5f1495f00a66a8d8207d493fa9eabed19c0 in / 
# Mon, 04 Apr 2022 23:50:07 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:01:19 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 04:01:20 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 04:01:21 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 04:01:22 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 04:01:22 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 04:02:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 04:02:32 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 04:02:32 GMT
USER user
# Tue, 05 Apr 2022 04:02:33 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:83a39d5693a8029bb5246b7d72205357bcd5d8306489b586abf44bc8659dfc1e`  
		Last Modified: Mon, 04 Apr 2022 23:51:58 GMT  
		Size: 2.6 MB (2625144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b589ee3c7baf4a3043d5c498c04269109c4a45e58c44ab98b5a969b7ba2f8a`  
		Last Modified: Tue, 05 Apr 2022 04:03:13 GMT  
		Size: 8.8 MB (8771955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82acf7c178275d848adf6769cd6193b1f701750ef2bf058c507c10c4af90080d`  
		Last Modified: Tue, 05 Apr 2022 04:03:05 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391da21a1ce4611cc08325dc363346ea9ae04e1724386ad9b1a8801e1843e835`  
		Last Modified: Tue, 05 Apr 2022 04:03:09 GMT  
		Size: 6.0 MB (5987042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:85b6871234efe5afa8aee356cecfc27abb04e6a99f43a969eedce41a3230299b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16839452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f387771b9c45b2879b4d36faf8f6326c4b27afacac146e4d774c52b2d0f103cb`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:58:06 GMT
ADD file:0834e20e80add8b1c6bd545ebe0729239e00a4dff08b025cb5555cd3ce58e4c6 in / 
# Mon, 04 Apr 2022 23:58:07 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 16:02:01 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 16:02:01 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 16:02:03 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 16:02:03 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 16:02:04 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 16:03:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 16:03:10 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 16:03:10 GMT
USER user
# Tue, 05 Apr 2022 16:03:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a8b8a1c7a552f6893757dd6327a5a430981d78aa06a59298076603526186829e`  
		Last Modified: Mon, 04 Apr 2022 23:59:56 GMT  
		Size: 2.4 MB (2427836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0c71a12aa1dc1147bd41cf6458906772bf77be69de2e8fc3d9242f641fc445`  
		Last Modified: Tue, 05 Apr 2022 16:04:19 GMT  
		Size: 8.6 MB (8626381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf67fa3e83093b4230c7f24388cfb9f6f9aa8bd3c5d76434f7b058a66d7ab80`  
		Last Modified: Tue, 05 Apr 2022 16:04:11 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95a6a97274960e7695eb8d37b680b0fe6bc45a12b2b550e310504260e923285`  
		Last Modified: Tue, 05 Apr 2022 16:04:15 GMT  
		Size: 5.8 MB (5783964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:d49fa5e7d3a8cd10c7bfad3e9bec2fa37e6a44c2911c1958c7014a121f4eef59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18505792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e98cf9f811eb592e3b8c251eb41f7f7dfdadc8c7b6dc2e9fae2c2d835173d8ac`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:14:15 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 04:14:16 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 04:14:17 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 04:14:18 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 04:14:19 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 04:14:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 04:14:54 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 04:14:55 GMT
USER user
# Tue, 05 Apr 2022 04:14:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f125d0f2f3de8f4307e1218e71620016554b5120c8ce30e8786904dc74366d0b`  
		Last Modified: Tue, 05 Apr 2022 04:15:25 GMT  
		Size: 9.5 MB (9536419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c48a8193426a12a478ffa39f46aa61977b41d48a60d252930c3c2a4708fd0b7`  
		Last Modified: Tue, 05 Apr 2022 04:15:23 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7a5707b30c726d92bca84220a2cb23b4ff000e7119f0a696975a866269d135`  
		Last Modified: Tue, 05 Apr 2022 04:15:24 GMT  
		Size: 6.2 MB (6247234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; 386

```console
$ docker pull irssi@sha256:f4044a89fe2a5119671314da6e8cbfed9929c215d20d677e6b84a7e5b713611f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17704054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aea095e2938971334ab2464fcf39c254bd75a69e3b56999f7fab374fb813c92`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:38 GMT
ADD file:caa278dc5cc6257518d542227fef491a89b0b4a7fc4dcb87632c2b786b65752a in / 
# Mon, 04 Apr 2022 23:38:38 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:47:49 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 06:47:49 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 06:47:50 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 06:47:51 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 06:47:52 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 06:48:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 06:48:28 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 06:48:29 GMT
USER user
# Tue, 05 Apr 2022 06:48:30 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:54c95c2f58283907ca735a3fe8d3ac4a49a63dc20092eb6fddd7bad2429e3f67`  
		Last Modified: Mon, 04 Apr 2022 23:39:46 GMT  
		Size: 2.8 MB (2820530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90d17b6eaf713c06aeabfe2feac029d7c880865cf49ab0c148c784791c31779`  
		Last Modified: Tue, 05 Apr 2022 06:49:01 GMT  
		Size: 8.9 MB (8904271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a831ba5a4f1fc534f7dec6b2cf96d9935df1d6b00524538974d10799fd6f4c53`  
		Last Modified: Tue, 05 Apr 2022 06:48:59 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd3dd29c50ebba7606220a2a714a5fdb3059694e3f39c9b707f4c43086cf958`  
		Last Modified: Tue, 05 Apr 2022 06:49:00 GMT  
		Size: 6.0 MB (5978011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:beba11d08d6df10a4fe4518b49c2e3d8b54f2cb9f15feb8bce4bfba5d97c6674
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18941010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37da7ed44ea84c9ebfb079e981447b44fccab806fd3be499c492a079908bf21d`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:56 GMT
ADD file:a9d5347a58c095f620406d9afc12b5ae4fd6c3994ea7e88e6415db7b09725289 in / 
# Tue, 05 Apr 2022 00:24:00 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 19:10:05 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 19:10:11 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 19:10:20 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 19:10:25 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 19:10:29 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 19:11:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 19:11:33 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 19:11:36 GMT
USER user
# Tue, 05 Apr 2022 19:11:39 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:afbded953e7f469508815262f0ff60fc06823cc1701e4b7aa211eb10bca545bd`  
		Last Modified: Tue, 05 Apr 2022 00:25:18 GMT  
		Size: 2.8 MB (2814791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d73fa56481e3f5fd84b721b288e4628ef18d832025ab22c2cb0601f85d9025b`  
		Last Modified: Tue, 05 Apr 2022 19:12:17 GMT  
		Size: 9.6 MB (9632765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2998f1c0df5727d61352cf5bbb86f17a2b07e8d0feef2892ad0c1a13693ed8`  
		Last Modified: Tue, 05 Apr 2022 19:12:15 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0ce73fb7b2975452460737c989e296843d87ad3f26c26f5c7df696df51a1ea`  
		Last Modified: Tue, 05 Apr 2022 19:12:16 GMT  
		Size: 6.5 MB (6492183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:07e9626c05472af1fce5448f4310a04d7bc5e3a7e6a4384227d5aaec02d65705
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18855197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc5ea35b9201821c8168c1b19f5a926438127784e392a0465b5a49bc2b7f98e1`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:55 GMT
ADD file:0f7653032bb9c65a5643cc31ad93fca7bd018ca0466a2d1c4ccadc5db00ad0f0 in / 
# Mon, 04 Apr 2022 23:41:55 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:58:34 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 03:58:35 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 03:58:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 03:58:36 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 03:58:36 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 03:59:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 03:59:07 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 03:59:07 GMT
USER user
# Tue, 05 Apr 2022 03:59:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:22b3eb8fdd3cabd13718400a1a4d1e75330e6e512d556cdd902359adeb0b014a`  
		Last Modified: Mon, 04 Apr 2022 23:42:54 GMT  
		Size: 2.6 MB (2605058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2a655edb7398e76b909cbb12baf208d875c598793a42546c8f2b906ab8e2c7`  
		Last Modified: Tue, 05 Apr 2022 03:59:36 GMT  
		Size: 10.0 MB (9972200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16218c4743041a59790e9a6b9388344940cd9dbf0e8c3cff8ea17486b32b553`  
		Last Modified: Tue, 05 Apr 2022 03:59:34 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc92e5f35e6bfccd90acff05f4db673effe1dce4f736f0d128d6e878f5524767`  
		Last Modified: Tue, 05 Apr 2022 03:59:35 GMT  
		Size: 6.3 MB (6276668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2`

```console
$ docker pull irssi@sha256:21aebe0f969df877f64465e13ac0b228c7dadf841b3a220b3288a71d9a0db022
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
$ docker pull irssi@sha256:73eeea3fe8864f534c05c5720ef3f08b4a143b8ef3a8d015da100094dad6a835
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50616927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a221922d64e7a5f2ceab14950bc25d7824ed11accd24cb3606aad52bec0afd81`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:51:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 09:51:55 GMT
ENV HOME=/home/user
# Wed, 20 Apr 2022 09:51:56 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Apr 2022 09:51:56 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 09:51:56 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 20 Apr 2022 09:52:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Apr 2022 09:52:41 GMT
WORKDIR /home/user
# Wed, 20 Apr 2022 09:52:41 GMT
USER user
# Wed, 20 Apr 2022 09:52:41 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b90d559f62672d2aaa0b155cc1e81f4c0335f6c6d5992301536b307f6ecfc5f`  
		Last Modified: Wed, 20 Apr 2022 09:53:08 GMT  
		Size: 17.0 MB (17038607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca716a8e2f28387368616a6e17f95b7c147c78e12a279c467e642ef17dcffbc8`  
		Last Modified: Wed, 20 Apr 2022 09:53:04 GMT  
		Size: 4.2 KB (4203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a954de24a56a094455fc42c1d5826fcad65a0a8db6ffbf144f81f9417109d898`  
		Last Modified: Wed, 20 Apr 2022 09:53:05 GMT  
		Size: 6.4 MB (6433453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; arm variant v5

```console
$ docker pull irssi@sha256:5bda585bef4c01cf35df8f01f9c0f1fd8fb01ca4f18ad62efc210468febf3366
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46895518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a8f29e5ecc0f86367a380847eee70dccc7e50983ffe21a0a10517802e2c3982`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Apr 2022 07:17:47 GMT
ADD file:5b740716d202d2f3494df5e108c0ba999125920ed9c97803fe0ccdfeba5cf518 in / 
# Wed, 20 Apr 2022 07:17:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:36:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 13:36:19 GMT
ENV HOME=/home/user
# Wed, 20 Apr 2022 13:36:21 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Apr 2022 13:36:21 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 13:36:22 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 20 Apr 2022 13:38:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Apr 2022 13:38:14 GMT
WORKDIR /home/user
# Wed, 20 Apr 2022 13:38:14 GMT
USER user
# Wed, 20 Apr 2022 13:38:14 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1fc8704cfa531d4583c5d4d571b836a82c02a812dae88792c4397cf1c1770405`  
		Last Modified: Wed, 20 Apr 2022 07:33:54 GMT  
		Size: 24.9 MB (24889592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d712999a90ba1db6fb4a832bbfda68dc7ab9cd398b5c16e489f0e2f26b27bb62`  
		Last Modified: Wed, 20 Apr 2022 13:39:03 GMT  
		Size: 15.9 MB (15937246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8209faf477433cd094581e5465a0a9f0d917a546715580161097219fa9b9d56`  
		Last Modified: Wed, 20 Apr 2022 13:38:46 GMT  
		Size: 4.2 KB (4196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:102dcf521e04ca2d60a4752626d29b240b0d22690dd5a8831f660b9dd997469c`  
		Last Modified: Wed, 20 Apr 2022 13:38:50 GMT  
		Size: 6.1 MB (6064484 bytes)  
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
$ docker pull irssi@sha256:006b8def53f48a57a1adc76c8bb48271d1c323dff2e46a8a78dd9bec1acfca3a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48903268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6bcfcb3be6ccc226ff30616bc214852c32389d7a7cb1f8efb027ce7f97b28e0`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:25:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 09:25:18 GMT
ENV HOME=/home/user
# Wed, 20 Apr 2022 09:25:19 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Apr 2022 09:25:19 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 09:25:20 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 20 Apr 2022 09:26:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Apr 2022 09:26:04 GMT
WORKDIR /home/user
# Wed, 20 Apr 2022 09:26:05 GMT
USER user
# Wed, 20 Apr 2022 09:26:06 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f0468f2e47c92a374ac255a77884dcad97c6f37a5b458ff6f92188bca6d82c`  
		Last Modified: Wed, 20 Apr 2022 09:26:43 GMT  
		Size: 16.8 MB (16814853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177a8142bec8627b6eb8c372f76448f218e274d1ff21e6d19ec4a11ea1ee059d`  
		Last Modified: Wed, 20 Apr 2022 09:26:39 GMT  
		Size: 4.1 KB (4068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b72a244dd871eb4792d547404ef3800c8df98aed91e81950218bd44f82df1d`  
		Last Modified: Wed, 20 Apr 2022 09:26:40 GMT  
		Size: 6.2 MB (6175998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; 386

```console
$ docker pull irssi@sha256:821ad21b1a160f11558a20323bf0f1479cafd575e0440a655f996e14e7246b41
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50263111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c21a608d1eff21f66971c0fc5646baadb692a8a78541e095ae26befc626e6fee`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Apr 2022 07:38:03 GMT
ADD file:602a25173054242f635a5a299845b7f1b56864ac5d3b8af1ae29dec3a9da119f in / 
# Wed, 20 Apr 2022 07:38:04 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:39:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:39:47 GMT
ENV HOME=/home/user
# Wed, 20 Apr 2022 12:39:48 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Apr 2022 12:39:49 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 12:39:50 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 20 Apr 2022 12:40:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Apr 2022 12:40:40 GMT
WORKDIR /home/user
# Wed, 20 Apr 2022 12:40:41 GMT
USER user
# Wed, 20 Apr 2022 12:40:42 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a13b13d818745c4d2234aab71df26e4a01bfe59f396ab62f20d156b94803650c`  
		Last Modified: Wed, 20 Apr 2022 07:45:46 GMT  
		Size: 27.8 MB (27799825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd1690b27b64a6ece24dd4be73f7615988de276e59d5202b15cf379006d6b4c`  
		Last Modified: Wed, 20 Apr 2022 12:41:16 GMT  
		Size: 16.6 MB (16565741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2093fb439f2ad43eb953b6195e8da3ba5227d26a7a53ce4daf3d435131b42bd1`  
		Last Modified: Wed, 20 Apr 2022 12:41:13 GMT  
		Size: 4.1 KB (4052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fa17d08104200257a36b7d8baf7ac42fe3b14d21847439379ec371347da717`  
		Last Modified: Wed, 20 Apr 2022 12:41:14 GMT  
		Size: 5.9 MB (5893493 bytes)  
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
$ docker pull irssi@sha256:674d6845c5de4d8e243e168fb56a649d7fb8a4c77ea53f46517b68bf5ca072cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49061909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40f0e08be1db449f78356ac19326266df23eced238602b70ea697e10ecde3c1e`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Apr 2022 08:40:41 GMT
ADD file:e9840ab2ce3aeff61b68bf4837f65471a86dcba02c5023863f3e7493098b07ba in / 
# Wed, 20 Apr 2022 08:40:45 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:54:45 GMT
ENV HOME=/home/user
# Wed, 20 Apr 2022 12:54:46 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Apr 2022 12:54:47 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 12:54:47 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 20 Apr 2022 12:55:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Apr 2022 12:55:39 GMT
WORKDIR /home/user
# Wed, 20 Apr 2022 12:55:39 GMT
USER user
# Wed, 20 Apr 2022 12:55:39 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b59fdcf2cb29d2ee4dd08aa08a467372e33525431c4caba9b01e9eb28f76425f`  
		Last Modified: Wed, 20 Apr 2022 08:50:14 GMT  
		Size: 25.8 MB (25758600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84aa94504e16d563a7f953f43b8bb95b13d5156527a49986656ed7e79ecbb456`  
		Last Modified: Wed, 20 Apr 2022 12:56:19 GMT  
		Size: 16.9 MB (16914203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349fa3b5b2db4893cb2724353ac6f146f52e097b86480a4dc1d1831f2b7db8f5`  
		Last Modified: Wed, 20 Apr 2022 12:56:16 GMT  
		Size: 4.2 KB (4210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f92d4d941d09ed135194b56663949c39da03fd1ea1de785a9aac2a7947daf3`  
		Last Modified: Wed, 20 Apr 2022 12:56:17 GMT  
		Size: 6.4 MB (6384896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2-alpine`

```console
$ docker pull irssi@sha256:bfbb6e415dbf4cd1ea2d6bd42bdcc5fcc054d6b053c6d07b983c9b390dac8f9d
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
$ docker pull irssi@sha256:c38f2415219abd42abe51fa4eaf222d8d7c7bdebb86910500d59bb7d0c21b231
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18648499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6c0676773ef4ea9992d62133ac02ba861fde6dd9ba437e8fb36eaf4aae78852`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:18:16 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 11:18:17 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 11:18:17 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 11:18:17 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 11:18:17 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 11:19:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 11:19:01 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 11:19:01 GMT
USER user
# Tue, 05 Apr 2022 11:19:01 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa1dbdb27d63340f8b8fa494a282aeded5f878185e2847d6dfb481b353b8c11`  
		Last Modified: Tue, 05 Apr 2022 11:19:27 GMT  
		Size: 9.5 MB (9540662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30dd245485e0307925fa298d8f511fe481b6600ce336c8ff0a0b5c13ce1435d9`  
		Last Modified: Tue, 05 Apr 2022 11:19:24 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4513426f1a6993290c7fa1e95a9f0bd0309456d69e3c04c0a7e8b17b66c9a079`  
		Last Modified: Tue, 05 Apr 2022 11:19:25 GMT  
		Size: 6.3 MB (6287259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:5262462a3f32457835863ac8b11823de2d926d672219bdff8c5c67bc5e116e2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17385410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab49acd659041f4c479472bb7ed35e0fc93656b968625544d96599e44c57c01`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:50:07 GMT
ADD file:9e96de1fefc4e9efba26e76103eca5f1495f00a66a8d8207d493fa9eabed19c0 in / 
# Mon, 04 Apr 2022 23:50:07 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:01:19 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 04:01:20 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 04:01:21 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 04:01:22 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 04:01:22 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 04:02:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 04:02:32 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 04:02:32 GMT
USER user
# Tue, 05 Apr 2022 04:02:33 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:83a39d5693a8029bb5246b7d72205357bcd5d8306489b586abf44bc8659dfc1e`  
		Last Modified: Mon, 04 Apr 2022 23:51:58 GMT  
		Size: 2.6 MB (2625144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b589ee3c7baf4a3043d5c498c04269109c4a45e58c44ab98b5a969b7ba2f8a`  
		Last Modified: Tue, 05 Apr 2022 04:03:13 GMT  
		Size: 8.8 MB (8771955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82acf7c178275d848adf6769cd6193b1f701750ef2bf058c507c10c4af90080d`  
		Last Modified: Tue, 05 Apr 2022 04:03:05 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391da21a1ce4611cc08325dc363346ea9ae04e1724386ad9b1a8801e1843e835`  
		Last Modified: Tue, 05 Apr 2022 04:03:09 GMT  
		Size: 6.0 MB (5987042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:85b6871234efe5afa8aee356cecfc27abb04e6a99f43a969eedce41a3230299b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16839452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f387771b9c45b2879b4d36faf8f6326c4b27afacac146e4d774c52b2d0f103cb`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:58:06 GMT
ADD file:0834e20e80add8b1c6bd545ebe0729239e00a4dff08b025cb5555cd3ce58e4c6 in / 
# Mon, 04 Apr 2022 23:58:07 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 16:02:01 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 16:02:01 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 16:02:03 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 16:02:03 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 16:02:04 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 16:03:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 16:03:10 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 16:03:10 GMT
USER user
# Tue, 05 Apr 2022 16:03:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a8b8a1c7a552f6893757dd6327a5a430981d78aa06a59298076603526186829e`  
		Last Modified: Mon, 04 Apr 2022 23:59:56 GMT  
		Size: 2.4 MB (2427836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0c71a12aa1dc1147bd41cf6458906772bf77be69de2e8fc3d9242f641fc445`  
		Last Modified: Tue, 05 Apr 2022 16:04:19 GMT  
		Size: 8.6 MB (8626381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf67fa3e83093b4230c7f24388cfb9f6f9aa8bd3c5d76434f7b058a66d7ab80`  
		Last Modified: Tue, 05 Apr 2022 16:04:11 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95a6a97274960e7695eb8d37b680b0fe6bc45a12b2b550e310504260e923285`  
		Last Modified: Tue, 05 Apr 2022 16:04:15 GMT  
		Size: 5.8 MB (5783964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:d49fa5e7d3a8cd10c7bfad3e9bec2fa37e6a44c2911c1958c7014a121f4eef59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18505792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e98cf9f811eb592e3b8c251eb41f7f7dfdadc8c7b6dc2e9fae2c2d835173d8ac`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:14:15 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 04:14:16 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 04:14:17 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 04:14:18 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 04:14:19 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 04:14:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 04:14:54 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 04:14:55 GMT
USER user
# Tue, 05 Apr 2022 04:14:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f125d0f2f3de8f4307e1218e71620016554b5120c8ce30e8786904dc74366d0b`  
		Last Modified: Tue, 05 Apr 2022 04:15:25 GMT  
		Size: 9.5 MB (9536419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c48a8193426a12a478ffa39f46aa61977b41d48a60d252930c3c2a4708fd0b7`  
		Last Modified: Tue, 05 Apr 2022 04:15:23 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7a5707b30c726d92bca84220a2cb23b4ff000e7119f0a696975a866269d135`  
		Last Modified: Tue, 05 Apr 2022 04:15:24 GMT  
		Size: 6.2 MB (6247234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; 386

```console
$ docker pull irssi@sha256:f4044a89fe2a5119671314da6e8cbfed9929c215d20d677e6b84a7e5b713611f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17704054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aea095e2938971334ab2464fcf39c254bd75a69e3b56999f7fab374fb813c92`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:38 GMT
ADD file:caa278dc5cc6257518d542227fef491a89b0b4a7fc4dcb87632c2b786b65752a in / 
# Mon, 04 Apr 2022 23:38:38 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:47:49 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 06:47:49 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 06:47:50 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 06:47:51 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 06:47:52 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 06:48:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 06:48:28 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 06:48:29 GMT
USER user
# Tue, 05 Apr 2022 06:48:30 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:54c95c2f58283907ca735a3fe8d3ac4a49a63dc20092eb6fddd7bad2429e3f67`  
		Last Modified: Mon, 04 Apr 2022 23:39:46 GMT  
		Size: 2.8 MB (2820530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90d17b6eaf713c06aeabfe2feac029d7c880865cf49ab0c148c784791c31779`  
		Last Modified: Tue, 05 Apr 2022 06:49:01 GMT  
		Size: 8.9 MB (8904271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a831ba5a4f1fc534f7dec6b2cf96d9935df1d6b00524538974d10799fd6f4c53`  
		Last Modified: Tue, 05 Apr 2022 06:48:59 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd3dd29c50ebba7606220a2a714a5fdb3059694e3f39c9b707f4c43086cf958`  
		Last Modified: Tue, 05 Apr 2022 06:49:00 GMT  
		Size: 6.0 MB (5978011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:beba11d08d6df10a4fe4518b49c2e3d8b54f2cb9f15feb8bce4bfba5d97c6674
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18941010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37da7ed44ea84c9ebfb079e981447b44fccab806fd3be499c492a079908bf21d`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:56 GMT
ADD file:a9d5347a58c095f620406d9afc12b5ae4fd6c3994ea7e88e6415db7b09725289 in / 
# Tue, 05 Apr 2022 00:24:00 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 19:10:05 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 19:10:11 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 19:10:20 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 19:10:25 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 19:10:29 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 19:11:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 19:11:33 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 19:11:36 GMT
USER user
# Tue, 05 Apr 2022 19:11:39 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:afbded953e7f469508815262f0ff60fc06823cc1701e4b7aa211eb10bca545bd`  
		Last Modified: Tue, 05 Apr 2022 00:25:18 GMT  
		Size: 2.8 MB (2814791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d73fa56481e3f5fd84b721b288e4628ef18d832025ab22c2cb0601f85d9025b`  
		Last Modified: Tue, 05 Apr 2022 19:12:17 GMT  
		Size: 9.6 MB (9632765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2998f1c0df5727d61352cf5bbb86f17a2b07e8d0feef2892ad0c1a13693ed8`  
		Last Modified: Tue, 05 Apr 2022 19:12:15 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0ce73fb7b2975452460737c989e296843d87ad3f26c26f5c7df696df51a1ea`  
		Last Modified: Tue, 05 Apr 2022 19:12:16 GMT  
		Size: 6.5 MB (6492183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:07e9626c05472af1fce5448f4310a04d7bc5e3a7e6a4384227d5aaec02d65705
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18855197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc5ea35b9201821c8168c1b19f5a926438127784e392a0465b5a49bc2b7f98e1`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:55 GMT
ADD file:0f7653032bb9c65a5643cc31ad93fca7bd018ca0466a2d1c4ccadc5db00ad0f0 in / 
# Mon, 04 Apr 2022 23:41:55 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:58:34 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 03:58:35 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 03:58:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 03:58:36 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 03:58:36 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 03:59:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 03:59:07 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 03:59:07 GMT
USER user
# Tue, 05 Apr 2022 03:59:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:22b3eb8fdd3cabd13718400a1a4d1e75330e6e512d556cdd902359adeb0b014a`  
		Last Modified: Mon, 04 Apr 2022 23:42:54 GMT  
		Size: 2.6 MB (2605058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2a655edb7398e76b909cbb12baf208d875c598793a42546c8f2b906ab8e2c7`  
		Last Modified: Tue, 05 Apr 2022 03:59:36 GMT  
		Size: 10.0 MB (9972200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16218c4743041a59790e9a6b9388344940cd9dbf0e8c3cff8ea17486b32b553`  
		Last Modified: Tue, 05 Apr 2022 03:59:34 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc92e5f35e6bfccd90acff05f4db673effe1dce4f736f0d128d6e878f5524767`  
		Last Modified: Tue, 05 Apr 2022 03:59:35 GMT  
		Size: 6.3 MB (6276668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2.3`

```console
$ docker pull irssi@sha256:21aebe0f969df877f64465e13ac0b228c7dadf841b3a220b3288a71d9a0db022
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
$ docker pull irssi@sha256:73eeea3fe8864f534c05c5720ef3f08b4a143b8ef3a8d015da100094dad6a835
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50616927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a221922d64e7a5f2ceab14950bc25d7824ed11accd24cb3606aad52bec0afd81`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:51:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 09:51:55 GMT
ENV HOME=/home/user
# Wed, 20 Apr 2022 09:51:56 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Apr 2022 09:51:56 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 09:51:56 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 20 Apr 2022 09:52:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Apr 2022 09:52:41 GMT
WORKDIR /home/user
# Wed, 20 Apr 2022 09:52:41 GMT
USER user
# Wed, 20 Apr 2022 09:52:41 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b90d559f62672d2aaa0b155cc1e81f4c0335f6c6d5992301536b307f6ecfc5f`  
		Last Modified: Wed, 20 Apr 2022 09:53:08 GMT  
		Size: 17.0 MB (17038607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca716a8e2f28387368616a6e17f95b7c147c78e12a279c467e642ef17dcffbc8`  
		Last Modified: Wed, 20 Apr 2022 09:53:04 GMT  
		Size: 4.2 KB (4203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a954de24a56a094455fc42c1d5826fcad65a0a8db6ffbf144f81f9417109d898`  
		Last Modified: Wed, 20 Apr 2022 09:53:05 GMT  
		Size: 6.4 MB (6433453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; arm variant v5

```console
$ docker pull irssi@sha256:5bda585bef4c01cf35df8f01f9c0f1fd8fb01ca4f18ad62efc210468febf3366
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46895518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a8f29e5ecc0f86367a380847eee70dccc7e50983ffe21a0a10517802e2c3982`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Apr 2022 07:17:47 GMT
ADD file:5b740716d202d2f3494df5e108c0ba999125920ed9c97803fe0ccdfeba5cf518 in / 
# Wed, 20 Apr 2022 07:17:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:36:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 13:36:19 GMT
ENV HOME=/home/user
# Wed, 20 Apr 2022 13:36:21 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Apr 2022 13:36:21 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 13:36:22 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 20 Apr 2022 13:38:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Apr 2022 13:38:14 GMT
WORKDIR /home/user
# Wed, 20 Apr 2022 13:38:14 GMT
USER user
# Wed, 20 Apr 2022 13:38:14 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1fc8704cfa531d4583c5d4d571b836a82c02a812dae88792c4397cf1c1770405`  
		Last Modified: Wed, 20 Apr 2022 07:33:54 GMT  
		Size: 24.9 MB (24889592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d712999a90ba1db6fb4a832bbfda68dc7ab9cd398b5c16e489f0e2f26b27bb62`  
		Last Modified: Wed, 20 Apr 2022 13:39:03 GMT  
		Size: 15.9 MB (15937246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8209faf477433cd094581e5465a0a9f0d917a546715580161097219fa9b9d56`  
		Last Modified: Wed, 20 Apr 2022 13:38:46 GMT  
		Size: 4.2 KB (4196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:102dcf521e04ca2d60a4752626d29b240b0d22690dd5a8831f660b9dd997469c`  
		Last Modified: Wed, 20 Apr 2022 13:38:50 GMT  
		Size: 6.1 MB (6064484 bytes)  
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
$ docker pull irssi@sha256:006b8def53f48a57a1adc76c8bb48271d1c323dff2e46a8a78dd9bec1acfca3a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48903268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6bcfcb3be6ccc226ff30616bc214852c32389d7a7cb1f8efb027ce7f97b28e0`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:25:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 09:25:18 GMT
ENV HOME=/home/user
# Wed, 20 Apr 2022 09:25:19 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Apr 2022 09:25:19 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 09:25:20 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 20 Apr 2022 09:26:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Apr 2022 09:26:04 GMT
WORKDIR /home/user
# Wed, 20 Apr 2022 09:26:05 GMT
USER user
# Wed, 20 Apr 2022 09:26:06 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f0468f2e47c92a374ac255a77884dcad97c6f37a5b458ff6f92188bca6d82c`  
		Last Modified: Wed, 20 Apr 2022 09:26:43 GMT  
		Size: 16.8 MB (16814853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177a8142bec8627b6eb8c372f76448f218e274d1ff21e6d19ec4a11ea1ee059d`  
		Last Modified: Wed, 20 Apr 2022 09:26:39 GMT  
		Size: 4.1 KB (4068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b72a244dd871eb4792d547404ef3800c8df98aed91e81950218bd44f82df1d`  
		Last Modified: Wed, 20 Apr 2022 09:26:40 GMT  
		Size: 6.2 MB (6175998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; 386

```console
$ docker pull irssi@sha256:821ad21b1a160f11558a20323bf0f1479cafd575e0440a655f996e14e7246b41
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50263111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c21a608d1eff21f66971c0fc5646baadb692a8a78541e095ae26befc626e6fee`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Apr 2022 07:38:03 GMT
ADD file:602a25173054242f635a5a299845b7f1b56864ac5d3b8af1ae29dec3a9da119f in / 
# Wed, 20 Apr 2022 07:38:04 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:39:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:39:47 GMT
ENV HOME=/home/user
# Wed, 20 Apr 2022 12:39:48 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Apr 2022 12:39:49 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 12:39:50 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 20 Apr 2022 12:40:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Apr 2022 12:40:40 GMT
WORKDIR /home/user
# Wed, 20 Apr 2022 12:40:41 GMT
USER user
# Wed, 20 Apr 2022 12:40:42 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a13b13d818745c4d2234aab71df26e4a01bfe59f396ab62f20d156b94803650c`  
		Last Modified: Wed, 20 Apr 2022 07:45:46 GMT  
		Size: 27.8 MB (27799825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd1690b27b64a6ece24dd4be73f7615988de276e59d5202b15cf379006d6b4c`  
		Last Modified: Wed, 20 Apr 2022 12:41:16 GMT  
		Size: 16.6 MB (16565741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2093fb439f2ad43eb953b6195e8da3ba5227d26a7a53ce4daf3d435131b42bd1`  
		Last Modified: Wed, 20 Apr 2022 12:41:13 GMT  
		Size: 4.1 KB (4052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fa17d08104200257a36b7d8baf7ac42fe3b14d21847439379ec371347da717`  
		Last Modified: Wed, 20 Apr 2022 12:41:14 GMT  
		Size: 5.9 MB (5893493 bytes)  
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
$ docker pull irssi@sha256:674d6845c5de4d8e243e168fb56a649d7fb8a4c77ea53f46517b68bf5ca072cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49061909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40f0e08be1db449f78356ac19326266df23eced238602b70ea697e10ecde3c1e`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Apr 2022 08:40:41 GMT
ADD file:e9840ab2ce3aeff61b68bf4837f65471a86dcba02c5023863f3e7493098b07ba in / 
# Wed, 20 Apr 2022 08:40:45 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:54:45 GMT
ENV HOME=/home/user
# Wed, 20 Apr 2022 12:54:46 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Apr 2022 12:54:47 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 12:54:47 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 20 Apr 2022 12:55:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Apr 2022 12:55:39 GMT
WORKDIR /home/user
# Wed, 20 Apr 2022 12:55:39 GMT
USER user
# Wed, 20 Apr 2022 12:55:39 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b59fdcf2cb29d2ee4dd08aa08a467372e33525431c4caba9b01e9eb28f76425f`  
		Last Modified: Wed, 20 Apr 2022 08:50:14 GMT  
		Size: 25.8 MB (25758600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84aa94504e16d563a7f953f43b8bb95b13d5156527a49986656ed7e79ecbb456`  
		Last Modified: Wed, 20 Apr 2022 12:56:19 GMT  
		Size: 16.9 MB (16914203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349fa3b5b2db4893cb2724353ac6f146f52e097b86480a4dc1d1831f2b7db8f5`  
		Last Modified: Wed, 20 Apr 2022 12:56:16 GMT  
		Size: 4.2 KB (4210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f92d4d941d09ed135194b56663949c39da03fd1ea1de785a9aac2a7947daf3`  
		Last Modified: Wed, 20 Apr 2022 12:56:17 GMT  
		Size: 6.4 MB (6384896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2.3-alpine`

```console
$ docker pull irssi@sha256:bfbb6e415dbf4cd1ea2d6bd42bdcc5fcc054d6b053c6d07b983c9b390dac8f9d
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
$ docker pull irssi@sha256:c38f2415219abd42abe51fa4eaf222d8d7c7bdebb86910500d59bb7d0c21b231
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18648499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6c0676773ef4ea9992d62133ac02ba861fde6dd9ba437e8fb36eaf4aae78852`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:18:16 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 11:18:17 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 11:18:17 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 11:18:17 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 11:18:17 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 11:19:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 11:19:01 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 11:19:01 GMT
USER user
# Tue, 05 Apr 2022 11:19:01 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa1dbdb27d63340f8b8fa494a282aeded5f878185e2847d6dfb481b353b8c11`  
		Last Modified: Tue, 05 Apr 2022 11:19:27 GMT  
		Size: 9.5 MB (9540662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30dd245485e0307925fa298d8f511fe481b6600ce336c8ff0a0b5c13ce1435d9`  
		Last Modified: Tue, 05 Apr 2022 11:19:24 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4513426f1a6993290c7fa1e95a9f0bd0309456d69e3c04c0a7e8b17b66c9a079`  
		Last Modified: Tue, 05 Apr 2022 11:19:25 GMT  
		Size: 6.3 MB (6287259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:5262462a3f32457835863ac8b11823de2d926d672219bdff8c5c67bc5e116e2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17385410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab49acd659041f4c479472bb7ed35e0fc93656b968625544d96599e44c57c01`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:50:07 GMT
ADD file:9e96de1fefc4e9efba26e76103eca5f1495f00a66a8d8207d493fa9eabed19c0 in / 
# Mon, 04 Apr 2022 23:50:07 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:01:19 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 04:01:20 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 04:01:21 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 04:01:22 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 04:01:22 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 04:02:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 04:02:32 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 04:02:32 GMT
USER user
# Tue, 05 Apr 2022 04:02:33 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:83a39d5693a8029bb5246b7d72205357bcd5d8306489b586abf44bc8659dfc1e`  
		Last Modified: Mon, 04 Apr 2022 23:51:58 GMT  
		Size: 2.6 MB (2625144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b589ee3c7baf4a3043d5c498c04269109c4a45e58c44ab98b5a969b7ba2f8a`  
		Last Modified: Tue, 05 Apr 2022 04:03:13 GMT  
		Size: 8.8 MB (8771955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82acf7c178275d848adf6769cd6193b1f701750ef2bf058c507c10c4af90080d`  
		Last Modified: Tue, 05 Apr 2022 04:03:05 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391da21a1ce4611cc08325dc363346ea9ae04e1724386ad9b1a8801e1843e835`  
		Last Modified: Tue, 05 Apr 2022 04:03:09 GMT  
		Size: 6.0 MB (5987042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:85b6871234efe5afa8aee356cecfc27abb04e6a99f43a969eedce41a3230299b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16839452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f387771b9c45b2879b4d36faf8f6326c4b27afacac146e4d774c52b2d0f103cb`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:58:06 GMT
ADD file:0834e20e80add8b1c6bd545ebe0729239e00a4dff08b025cb5555cd3ce58e4c6 in / 
# Mon, 04 Apr 2022 23:58:07 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 16:02:01 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 16:02:01 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 16:02:03 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 16:02:03 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 16:02:04 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 16:03:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 16:03:10 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 16:03:10 GMT
USER user
# Tue, 05 Apr 2022 16:03:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a8b8a1c7a552f6893757dd6327a5a430981d78aa06a59298076603526186829e`  
		Last Modified: Mon, 04 Apr 2022 23:59:56 GMT  
		Size: 2.4 MB (2427836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0c71a12aa1dc1147bd41cf6458906772bf77be69de2e8fc3d9242f641fc445`  
		Last Modified: Tue, 05 Apr 2022 16:04:19 GMT  
		Size: 8.6 MB (8626381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf67fa3e83093b4230c7f24388cfb9f6f9aa8bd3c5d76434f7b058a66d7ab80`  
		Last Modified: Tue, 05 Apr 2022 16:04:11 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95a6a97274960e7695eb8d37b680b0fe6bc45a12b2b550e310504260e923285`  
		Last Modified: Tue, 05 Apr 2022 16:04:15 GMT  
		Size: 5.8 MB (5783964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:d49fa5e7d3a8cd10c7bfad3e9bec2fa37e6a44c2911c1958c7014a121f4eef59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18505792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e98cf9f811eb592e3b8c251eb41f7f7dfdadc8c7b6dc2e9fae2c2d835173d8ac`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:14:15 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 04:14:16 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 04:14:17 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 04:14:18 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 04:14:19 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 04:14:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 04:14:54 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 04:14:55 GMT
USER user
# Tue, 05 Apr 2022 04:14:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f125d0f2f3de8f4307e1218e71620016554b5120c8ce30e8786904dc74366d0b`  
		Last Modified: Tue, 05 Apr 2022 04:15:25 GMT  
		Size: 9.5 MB (9536419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c48a8193426a12a478ffa39f46aa61977b41d48a60d252930c3c2a4708fd0b7`  
		Last Modified: Tue, 05 Apr 2022 04:15:23 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7a5707b30c726d92bca84220a2cb23b4ff000e7119f0a696975a866269d135`  
		Last Modified: Tue, 05 Apr 2022 04:15:24 GMT  
		Size: 6.2 MB (6247234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; 386

```console
$ docker pull irssi@sha256:f4044a89fe2a5119671314da6e8cbfed9929c215d20d677e6b84a7e5b713611f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17704054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aea095e2938971334ab2464fcf39c254bd75a69e3b56999f7fab374fb813c92`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:38 GMT
ADD file:caa278dc5cc6257518d542227fef491a89b0b4a7fc4dcb87632c2b786b65752a in / 
# Mon, 04 Apr 2022 23:38:38 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:47:49 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 06:47:49 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 06:47:50 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 06:47:51 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 06:47:52 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 06:48:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 06:48:28 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 06:48:29 GMT
USER user
# Tue, 05 Apr 2022 06:48:30 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:54c95c2f58283907ca735a3fe8d3ac4a49a63dc20092eb6fddd7bad2429e3f67`  
		Last Modified: Mon, 04 Apr 2022 23:39:46 GMT  
		Size: 2.8 MB (2820530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90d17b6eaf713c06aeabfe2feac029d7c880865cf49ab0c148c784791c31779`  
		Last Modified: Tue, 05 Apr 2022 06:49:01 GMT  
		Size: 8.9 MB (8904271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a831ba5a4f1fc534f7dec6b2cf96d9935df1d6b00524538974d10799fd6f4c53`  
		Last Modified: Tue, 05 Apr 2022 06:48:59 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd3dd29c50ebba7606220a2a714a5fdb3059694e3f39c9b707f4c43086cf958`  
		Last Modified: Tue, 05 Apr 2022 06:49:00 GMT  
		Size: 6.0 MB (5978011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:beba11d08d6df10a4fe4518b49c2e3d8b54f2cb9f15feb8bce4bfba5d97c6674
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18941010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37da7ed44ea84c9ebfb079e981447b44fccab806fd3be499c492a079908bf21d`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:56 GMT
ADD file:a9d5347a58c095f620406d9afc12b5ae4fd6c3994ea7e88e6415db7b09725289 in / 
# Tue, 05 Apr 2022 00:24:00 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 19:10:05 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 19:10:11 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 19:10:20 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 19:10:25 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 19:10:29 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 19:11:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 19:11:33 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 19:11:36 GMT
USER user
# Tue, 05 Apr 2022 19:11:39 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:afbded953e7f469508815262f0ff60fc06823cc1701e4b7aa211eb10bca545bd`  
		Last Modified: Tue, 05 Apr 2022 00:25:18 GMT  
		Size: 2.8 MB (2814791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d73fa56481e3f5fd84b721b288e4628ef18d832025ab22c2cb0601f85d9025b`  
		Last Modified: Tue, 05 Apr 2022 19:12:17 GMT  
		Size: 9.6 MB (9632765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2998f1c0df5727d61352cf5bbb86f17a2b07e8d0feef2892ad0c1a13693ed8`  
		Last Modified: Tue, 05 Apr 2022 19:12:15 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0ce73fb7b2975452460737c989e296843d87ad3f26c26f5c7df696df51a1ea`  
		Last Modified: Tue, 05 Apr 2022 19:12:16 GMT  
		Size: 6.5 MB (6492183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:07e9626c05472af1fce5448f4310a04d7bc5e3a7e6a4384227d5aaec02d65705
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18855197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc5ea35b9201821c8168c1b19f5a926438127784e392a0465b5a49bc2b7f98e1`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:55 GMT
ADD file:0f7653032bb9c65a5643cc31ad93fca7bd018ca0466a2d1c4ccadc5db00ad0f0 in / 
# Mon, 04 Apr 2022 23:41:55 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:58:34 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 03:58:35 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 03:58:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 03:58:36 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 03:58:36 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 03:59:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 03:59:07 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 03:59:07 GMT
USER user
# Tue, 05 Apr 2022 03:59:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:22b3eb8fdd3cabd13718400a1a4d1e75330e6e512d556cdd902359adeb0b014a`  
		Last Modified: Mon, 04 Apr 2022 23:42:54 GMT  
		Size: 2.6 MB (2605058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2a655edb7398e76b909cbb12baf208d875c598793a42546c8f2b906ab8e2c7`  
		Last Modified: Tue, 05 Apr 2022 03:59:36 GMT  
		Size: 10.0 MB (9972200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16218c4743041a59790e9a6b9388344940cd9dbf0e8c3cff8ea17486b32b553`  
		Last Modified: Tue, 05 Apr 2022 03:59:34 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc92e5f35e6bfccd90acff05f4db673effe1dce4f736f0d128d6e878f5524767`  
		Last Modified: Tue, 05 Apr 2022 03:59:35 GMT  
		Size: 6.3 MB (6276668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:alpine`

```console
$ docker pull irssi@sha256:bfbb6e415dbf4cd1ea2d6bd42bdcc5fcc054d6b053c6d07b983c9b390dac8f9d
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
$ docker pull irssi@sha256:c38f2415219abd42abe51fa4eaf222d8d7c7bdebb86910500d59bb7d0c21b231
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18648499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6c0676773ef4ea9992d62133ac02ba861fde6dd9ba437e8fb36eaf4aae78852`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:18:16 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 11:18:17 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 11:18:17 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 11:18:17 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 11:18:17 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 11:19:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 11:19:01 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 11:19:01 GMT
USER user
# Tue, 05 Apr 2022 11:19:01 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa1dbdb27d63340f8b8fa494a282aeded5f878185e2847d6dfb481b353b8c11`  
		Last Modified: Tue, 05 Apr 2022 11:19:27 GMT  
		Size: 9.5 MB (9540662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30dd245485e0307925fa298d8f511fe481b6600ce336c8ff0a0b5c13ce1435d9`  
		Last Modified: Tue, 05 Apr 2022 11:19:24 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4513426f1a6993290c7fa1e95a9f0bd0309456d69e3c04c0a7e8b17b66c9a079`  
		Last Modified: Tue, 05 Apr 2022 11:19:25 GMT  
		Size: 6.3 MB (6287259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:5262462a3f32457835863ac8b11823de2d926d672219bdff8c5c67bc5e116e2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17385410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab49acd659041f4c479472bb7ed35e0fc93656b968625544d96599e44c57c01`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:50:07 GMT
ADD file:9e96de1fefc4e9efba26e76103eca5f1495f00a66a8d8207d493fa9eabed19c0 in / 
# Mon, 04 Apr 2022 23:50:07 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:01:19 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 04:01:20 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 04:01:21 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 04:01:22 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 04:01:22 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 04:02:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 04:02:32 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 04:02:32 GMT
USER user
# Tue, 05 Apr 2022 04:02:33 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:83a39d5693a8029bb5246b7d72205357bcd5d8306489b586abf44bc8659dfc1e`  
		Last Modified: Mon, 04 Apr 2022 23:51:58 GMT  
		Size: 2.6 MB (2625144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b589ee3c7baf4a3043d5c498c04269109c4a45e58c44ab98b5a969b7ba2f8a`  
		Last Modified: Tue, 05 Apr 2022 04:03:13 GMT  
		Size: 8.8 MB (8771955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82acf7c178275d848adf6769cd6193b1f701750ef2bf058c507c10c4af90080d`  
		Last Modified: Tue, 05 Apr 2022 04:03:05 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391da21a1ce4611cc08325dc363346ea9ae04e1724386ad9b1a8801e1843e835`  
		Last Modified: Tue, 05 Apr 2022 04:03:09 GMT  
		Size: 6.0 MB (5987042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:85b6871234efe5afa8aee356cecfc27abb04e6a99f43a969eedce41a3230299b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16839452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f387771b9c45b2879b4d36faf8f6326c4b27afacac146e4d774c52b2d0f103cb`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:58:06 GMT
ADD file:0834e20e80add8b1c6bd545ebe0729239e00a4dff08b025cb5555cd3ce58e4c6 in / 
# Mon, 04 Apr 2022 23:58:07 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 16:02:01 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 16:02:01 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 16:02:03 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 16:02:03 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 16:02:04 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 16:03:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 16:03:10 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 16:03:10 GMT
USER user
# Tue, 05 Apr 2022 16:03:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a8b8a1c7a552f6893757dd6327a5a430981d78aa06a59298076603526186829e`  
		Last Modified: Mon, 04 Apr 2022 23:59:56 GMT  
		Size: 2.4 MB (2427836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0c71a12aa1dc1147bd41cf6458906772bf77be69de2e8fc3d9242f641fc445`  
		Last Modified: Tue, 05 Apr 2022 16:04:19 GMT  
		Size: 8.6 MB (8626381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf67fa3e83093b4230c7f24388cfb9f6f9aa8bd3c5d76434f7b058a66d7ab80`  
		Last Modified: Tue, 05 Apr 2022 16:04:11 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95a6a97274960e7695eb8d37b680b0fe6bc45a12b2b550e310504260e923285`  
		Last Modified: Tue, 05 Apr 2022 16:04:15 GMT  
		Size: 5.8 MB (5783964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:d49fa5e7d3a8cd10c7bfad3e9bec2fa37e6a44c2911c1958c7014a121f4eef59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18505792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e98cf9f811eb592e3b8c251eb41f7f7dfdadc8c7b6dc2e9fae2c2d835173d8ac`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:14:15 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 04:14:16 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 04:14:17 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 04:14:18 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 04:14:19 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 04:14:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 04:14:54 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 04:14:55 GMT
USER user
# Tue, 05 Apr 2022 04:14:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f125d0f2f3de8f4307e1218e71620016554b5120c8ce30e8786904dc74366d0b`  
		Last Modified: Tue, 05 Apr 2022 04:15:25 GMT  
		Size: 9.5 MB (9536419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c48a8193426a12a478ffa39f46aa61977b41d48a60d252930c3c2a4708fd0b7`  
		Last Modified: Tue, 05 Apr 2022 04:15:23 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7a5707b30c726d92bca84220a2cb23b4ff000e7119f0a696975a866269d135`  
		Last Modified: Tue, 05 Apr 2022 04:15:24 GMT  
		Size: 6.2 MB (6247234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; 386

```console
$ docker pull irssi@sha256:f4044a89fe2a5119671314da6e8cbfed9929c215d20d677e6b84a7e5b713611f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17704054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aea095e2938971334ab2464fcf39c254bd75a69e3b56999f7fab374fb813c92`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:38 GMT
ADD file:caa278dc5cc6257518d542227fef491a89b0b4a7fc4dcb87632c2b786b65752a in / 
# Mon, 04 Apr 2022 23:38:38 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:47:49 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 06:47:49 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 06:47:50 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 06:47:51 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 06:47:52 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 06:48:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 06:48:28 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 06:48:29 GMT
USER user
# Tue, 05 Apr 2022 06:48:30 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:54c95c2f58283907ca735a3fe8d3ac4a49a63dc20092eb6fddd7bad2429e3f67`  
		Last Modified: Mon, 04 Apr 2022 23:39:46 GMT  
		Size: 2.8 MB (2820530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90d17b6eaf713c06aeabfe2feac029d7c880865cf49ab0c148c784791c31779`  
		Last Modified: Tue, 05 Apr 2022 06:49:01 GMT  
		Size: 8.9 MB (8904271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a831ba5a4f1fc534f7dec6b2cf96d9935df1d6b00524538974d10799fd6f4c53`  
		Last Modified: Tue, 05 Apr 2022 06:48:59 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd3dd29c50ebba7606220a2a714a5fdb3059694e3f39c9b707f4c43086cf958`  
		Last Modified: Tue, 05 Apr 2022 06:49:00 GMT  
		Size: 6.0 MB (5978011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:beba11d08d6df10a4fe4518b49c2e3d8b54f2cb9f15feb8bce4bfba5d97c6674
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18941010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37da7ed44ea84c9ebfb079e981447b44fccab806fd3be499c492a079908bf21d`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:56 GMT
ADD file:a9d5347a58c095f620406d9afc12b5ae4fd6c3994ea7e88e6415db7b09725289 in / 
# Tue, 05 Apr 2022 00:24:00 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 19:10:05 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 19:10:11 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 19:10:20 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 19:10:25 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 19:10:29 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 19:11:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 19:11:33 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 19:11:36 GMT
USER user
# Tue, 05 Apr 2022 19:11:39 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:afbded953e7f469508815262f0ff60fc06823cc1701e4b7aa211eb10bca545bd`  
		Last Modified: Tue, 05 Apr 2022 00:25:18 GMT  
		Size: 2.8 MB (2814791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d73fa56481e3f5fd84b721b288e4628ef18d832025ab22c2cb0601f85d9025b`  
		Last Modified: Tue, 05 Apr 2022 19:12:17 GMT  
		Size: 9.6 MB (9632765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2998f1c0df5727d61352cf5bbb86f17a2b07e8d0feef2892ad0c1a13693ed8`  
		Last Modified: Tue, 05 Apr 2022 19:12:15 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0ce73fb7b2975452460737c989e296843d87ad3f26c26f5c7df696df51a1ea`  
		Last Modified: Tue, 05 Apr 2022 19:12:16 GMT  
		Size: 6.5 MB (6492183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; s390x

```console
$ docker pull irssi@sha256:07e9626c05472af1fce5448f4310a04d7bc5e3a7e6a4384227d5aaec02d65705
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18855197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc5ea35b9201821c8168c1b19f5a926438127784e392a0465b5a49bc2b7f98e1`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:55 GMT
ADD file:0f7653032bb9c65a5643cc31ad93fca7bd018ca0466a2d1c4ccadc5db00ad0f0 in / 
# Mon, 04 Apr 2022 23:41:55 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:58:34 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 03:58:35 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 03:58:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 03:58:36 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 03:58:36 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 03:59:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 03:59:07 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 03:59:07 GMT
USER user
# Tue, 05 Apr 2022 03:59:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:22b3eb8fdd3cabd13718400a1a4d1e75330e6e512d556cdd902359adeb0b014a`  
		Last Modified: Mon, 04 Apr 2022 23:42:54 GMT  
		Size: 2.6 MB (2605058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2a655edb7398e76b909cbb12baf208d875c598793a42546c8f2b906ab8e2c7`  
		Last Modified: Tue, 05 Apr 2022 03:59:36 GMT  
		Size: 10.0 MB (9972200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16218c4743041a59790e9a6b9388344940cd9dbf0e8c3cff8ea17486b32b553`  
		Last Modified: Tue, 05 Apr 2022 03:59:34 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc92e5f35e6bfccd90acff05f4db673effe1dce4f736f0d128d6e878f5524767`  
		Last Modified: Tue, 05 Apr 2022 03:59:35 GMT  
		Size: 6.3 MB (6276668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:latest`

```console
$ docker pull irssi@sha256:21aebe0f969df877f64465e13ac0b228c7dadf841b3a220b3288a71d9a0db022
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
$ docker pull irssi@sha256:73eeea3fe8864f534c05c5720ef3f08b4a143b8ef3a8d015da100094dad6a835
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50616927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a221922d64e7a5f2ceab14950bc25d7824ed11accd24cb3606aad52bec0afd81`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:51:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 09:51:55 GMT
ENV HOME=/home/user
# Wed, 20 Apr 2022 09:51:56 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Apr 2022 09:51:56 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 09:51:56 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 20 Apr 2022 09:52:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Apr 2022 09:52:41 GMT
WORKDIR /home/user
# Wed, 20 Apr 2022 09:52:41 GMT
USER user
# Wed, 20 Apr 2022 09:52:41 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b90d559f62672d2aaa0b155cc1e81f4c0335f6c6d5992301536b307f6ecfc5f`  
		Last Modified: Wed, 20 Apr 2022 09:53:08 GMT  
		Size: 17.0 MB (17038607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca716a8e2f28387368616a6e17f95b7c147c78e12a279c467e642ef17dcffbc8`  
		Last Modified: Wed, 20 Apr 2022 09:53:04 GMT  
		Size: 4.2 KB (4203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a954de24a56a094455fc42c1d5826fcad65a0a8db6ffbf144f81f9417109d898`  
		Last Modified: Wed, 20 Apr 2022 09:53:05 GMT  
		Size: 6.4 MB (6433453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm variant v5

```console
$ docker pull irssi@sha256:5bda585bef4c01cf35df8f01f9c0f1fd8fb01ca4f18ad62efc210468febf3366
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46895518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a8f29e5ecc0f86367a380847eee70dccc7e50983ffe21a0a10517802e2c3982`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Apr 2022 07:17:47 GMT
ADD file:5b740716d202d2f3494df5e108c0ba999125920ed9c97803fe0ccdfeba5cf518 in / 
# Wed, 20 Apr 2022 07:17:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:36:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 13:36:19 GMT
ENV HOME=/home/user
# Wed, 20 Apr 2022 13:36:21 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Apr 2022 13:36:21 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 13:36:22 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 20 Apr 2022 13:38:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Apr 2022 13:38:14 GMT
WORKDIR /home/user
# Wed, 20 Apr 2022 13:38:14 GMT
USER user
# Wed, 20 Apr 2022 13:38:14 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1fc8704cfa531d4583c5d4d571b836a82c02a812dae88792c4397cf1c1770405`  
		Last Modified: Wed, 20 Apr 2022 07:33:54 GMT  
		Size: 24.9 MB (24889592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d712999a90ba1db6fb4a832bbfda68dc7ab9cd398b5c16e489f0e2f26b27bb62`  
		Last Modified: Wed, 20 Apr 2022 13:39:03 GMT  
		Size: 15.9 MB (15937246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8209faf477433cd094581e5465a0a9f0d917a546715580161097219fa9b9d56`  
		Last Modified: Wed, 20 Apr 2022 13:38:46 GMT  
		Size: 4.2 KB (4196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:102dcf521e04ca2d60a4752626d29b240b0d22690dd5a8831f660b9dd997469c`  
		Last Modified: Wed, 20 Apr 2022 13:38:50 GMT  
		Size: 6.1 MB (6064484 bytes)  
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
$ docker pull irssi@sha256:006b8def53f48a57a1adc76c8bb48271d1c323dff2e46a8a78dd9bec1acfca3a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48903268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6bcfcb3be6ccc226ff30616bc214852c32389d7a7cb1f8efb027ce7f97b28e0`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:25:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 09:25:18 GMT
ENV HOME=/home/user
# Wed, 20 Apr 2022 09:25:19 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Apr 2022 09:25:19 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 09:25:20 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 20 Apr 2022 09:26:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Apr 2022 09:26:04 GMT
WORKDIR /home/user
# Wed, 20 Apr 2022 09:26:05 GMT
USER user
# Wed, 20 Apr 2022 09:26:06 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f0468f2e47c92a374ac255a77884dcad97c6f37a5b458ff6f92188bca6d82c`  
		Last Modified: Wed, 20 Apr 2022 09:26:43 GMT  
		Size: 16.8 MB (16814853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177a8142bec8627b6eb8c372f76448f218e274d1ff21e6d19ec4a11ea1ee059d`  
		Last Modified: Wed, 20 Apr 2022 09:26:39 GMT  
		Size: 4.1 KB (4068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b72a244dd871eb4792d547404ef3800c8df98aed91e81950218bd44f82df1d`  
		Last Modified: Wed, 20 Apr 2022 09:26:40 GMT  
		Size: 6.2 MB (6175998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; 386

```console
$ docker pull irssi@sha256:821ad21b1a160f11558a20323bf0f1479cafd575e0440a655f996e14e7246b41
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50263111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c21a608d1eff21f66971c0fc5646baadb692a8a78541e095ae26befc626e6fee`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Apr 2022 07:38:03 GMT
ADD file:602a25173054242f635a5a299845b7f1b56864ac5d3b8af1ae29dec3a9da119f in / 
# Wed, 20 Apr 2022 07:38:04 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:39:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:39:47 GMT
ENV HOME=/home/user
# Wed, 20 Apr 2022 12:39:48 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Apr 2022 12:39:49 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 12:39:50 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 20 Apr 2022 12:40:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Apr 2022 12:40:40 GMT
WORKDIR /home/user
# Wed, 20 Apr 2022 12:40:41 GMT
USER user
# Wed, 20 Apr 2022 12:40:42 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a13b13d818745c4d2234aab71df26e4a01bfe59f396ab62f20d156b94803650c`  
		Last Modified: Wed, 20 Apr 2022 07:45:46 GMT  
		Size: 27.8 MB (27799825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd1690b27b64a6ece24dd4be73f7615988de276e59d5202b15cf379006d6b4c`  
		Last Modified: Wed, 20 Apr 2022 12:41:16 GMT  
		Size: 16.6 MB (16565741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2093fb439f2ad43eb953b6195e8da3ba5227d26a7a53ce4daf3d435131b42bd1`  
		Last Modified: Wed, 20 Apr 2022 12:41:13 GMT  
		Size: 4.1 KB (4052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fa17d08104200257a36b7d8baf7ac42fe3b14d21847439379ec371347da717`  
		Last Modified: Wed, 20 Apr 2022 12:41:14 GMT  
		Size: 5.9 MB (5893493 bytes)  
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
$ docker pull irssi@sha256:674d6845c5de4d8e243e168fb56a649d7fb8a4c77ea53f46517b68bf5ca072cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49061909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40f0e08be1db449f78356ac19326266df23eced238602b70ea697e10ecde3c1e`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 20 Apr 2022 08:40:41 GMT
ADD file:e9840ab2ce3aeff61b68bf4837f65471a86dcba02c5023863f3e7493098b07ba in / 
# Wed, 20 Apr 2022 08:40:45 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:54:45 GMT
ENV HOME=/home/user
# Wed, 20 Apr 2022 12:54:46 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Apr 2022 12:54:47 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 12:54:47 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 20 Apr 2022 12:55:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Apr 2022 12:55:39 GMT
WORKDIR /home/user
# Wed, 20 Apr 2022 12:55:39 GMT
USER user
# Wed, 20 Apr 2022 12:55:39 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b59fdcf2cb29d2ee4dd08aa08a467372e33525431c4caba9b01e9eb28f76425f`  
		Last Modified: Wed, 20 Apr 2022 08:50:14 GMT  
		Size: 25.8 MB (25758600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84aa94504e16d563a7f953f43b8bb95b13d5156527a49986656ed7e79ecbb456`  
		Last Modified: Wed, 20 Apr 2022 12:56:19 GMT  
		Size: 16.9 MB (16914203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349fa3b5b2db4893cb2724353ac6f146f52e097b86480a4dc1d1831f2b7db8f5`  
		Last Modified: Wed, 20 Apr 2022 12:56:16 GMT  
		Size: 4.2 KB (4210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f92d4d941d09ed135194b56663949c39da03fd1ea1de785a9aac2a7947daf3`  
		Last Modified: Wed, 20 Apr 2022 12:56:17 GMT  
		Size: 6.4 MB (6384896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
