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
