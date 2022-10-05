<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `irssi`

-	[`irssi:1`](#irssi1)
-	[`irssi:1-alpine`](#irssi1-alpine)
-	[`irssi:1.4`](#irssi14)
-	[`irssi:1.4-alpine`](#irssi14-alpine)
-	[`irssi:1.4.2`](#irssi142)
-	[`irssi:1.4.2-alpine`](#irssi142-alpine)
-	[`irssi:alpine`](#irssialpine)
-	[`irssi:latest`](#irssilatest)

## `irssi:1`

```console
$ docker pull irssi@sha256:4db96ec9b6933517d7c7ced80d5a431de322d56e3902934e167c031b40839993
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
$ docker pull irssi@sha256:b1bcbdd80b73f4ae87e078dc59ee578c2c34093b1ea355431ab0c1631a3bce23
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51347952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d527f60d93d54762986cae22b527791861f7b1584ab0298a550917a7f29bad58`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:11:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:11:37 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 04:11:38 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 04:11:38 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 04:11:38 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 04:12:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 04:12:17 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 04:12:17 GMT
USER user
# Wed, 05 Oct 2022 04:12:17 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77bdc13b2e9374e6b09e9fd7914a2324820a068a5b6f9e657052f6d7b67dbe95`  
		Last Modified: Wed, 05 Oct 2022 04:12:36 GMT  
		Size: 15.4 MB (15448732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2311da599c35f52f01d838f912b22e3af729ec1c3c5e575755a7094821746e`  
		Last Modified: Wed, 05 Oct 2022 04:12:33 GMT  
		Size: 4.2 KB (4207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2738f49d9720ad13f5ea47e7e1c8b46ef94eeca692abb7f8f0e706df113993eb`  
		Last Modified: Wed, 05 Oct 2022 04:12:34 GMT  
		Size: 4.5 MB (4474911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm variant v5

```console
$ docker pull irssi@sha256:88740de9cca35c2163e8ab77e8f1f166cbfd5d6df038fc4aef033c614706b8c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47873450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5230135f43ca49675070ca5c9aac96ac2bd7312dfa3892a5eaf2a6edaeb7438`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Oct 2022 23:49:11 GMT
ADD file:effb9e2e2f8c7539e1a2200d069a2592e8ba20c9d034b5a73fbf173b6987193c in / 
# Tue, 04 Oct 2022 23:49:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:44:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:44:56 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 01:44:56 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 01:44:57 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 01:44:57 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 01:46:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 01:46:08 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 01:46:08 GMT
USER user
# Wed, 05 Oct 2022 01:46:08 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:7b9558bbfd8050a8e6af6e60560101c49bd53f81df6fa068419b44d028e465eb`  
		Last Modified: Tue, 04 Oct 2022 23:53:54 GMT  
		Size: 28.9 MB (28918381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926bcca95f828ebbc9b9335e97fb7ea77630d58d58cdd57f095c304cbaaa5445`  
		Last Modified: Wed, 05 Oct 2022 01:46:40 GMT  
		Size: 14.6 MB (14625022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38273d8025ef0cf0e39724333850dd022ee9855d34870a753a057c6253a7bae`  
		Last Modified: Wed, 05 Oct 2022 01:46:35 GMT  
		Size: 4.2 KB (4195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5d67be13c2c15c402de10807e4690cc8cd3b47d1039d23c1918ca0077d2864`  
		Last Modified: Wed, 05 Oct 2022 01:46:36 GMT  
		Size: 4.3 MB (4325852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm variant v7

```console
$ docker pull irssi@sha256:fd77837c1e9019a6315e4620169b8ce504ec742b5e319173e3a4f0e1d37ec9ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45142511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff37cf9a11943845b033f0e6918067f1250ce298cff0924b7314e0d9e9cea429`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Sep 2022 03:42:37 GMT
ADD file:04b0c48a2d326e2ac4255df4a6165508f0d29d8a32147fb8df6bf9504b8f6b09 in / 
# Tue, 13 Sep 2022 03:42:37 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 11:39:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 11:39:07 GMT
ENV HOME=/home/user
# Tue, 13 Sep 2022 11:39:07 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 13 Sep 2022 11:39:08 GMT
ENV LANG=C.UTF-8
# Tue, 13 Sep 2022 11:39:08 GMT
ENV IRSSI_VERSION=1.4.2
# Tue, 13 Sep 2022 11:40:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 13 Sep 2022 11:40:23 GMT
WORKDIR /home/user
# Tue, 13 Sep 2022 11:40:23 GMT
USER user
# Tue, 13 Sep 2022 11:40:24 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:43caeee1782255456dd3403ae8e6ba191802c3deb004ca68ce0420b30368995d`  
		Last Modified: Tue, 13 Sep 2022 03:49:46 GMT  
		Size: 26.6 MB (26567059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d805b7c20340610b722146aba672823a39d3687d3816cf2cc01353f06476f569`  
		Last Modified: Tue, 13 Sep 2022 11:41:05 GMT  
		Size: 14.4 MB (14383616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be59b0b8bf1d750a007870d450e9d03125f62ff1f4b7b5c01baa939c6db0171c`  
		Last Modified: Tue, 13 Sep 2022 11:40:59 GMT  
		Size: 4.2 KB (4196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9351cace1f78aa2d855c828a2561e32e92804525197f378640aaba5b21bb2f5f`  
		Last Modified: Tue, 13 Sep 2022 11:41:01 GMT  
		Size: 4.2 MB (4187640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:276cb1d76f06ba8c2e067583632967b86be703d681b616e52772ca4ed9196706
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49359797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a3299bc6183d268d3238f72dc1cca2959c9f48f5f4a4b4ff45db50bd842be98`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:59:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:59:00 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 02:59:01 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 02:59:02 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 02:59:03 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 02:59:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 02:59:35 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 02:59:36 GMT
USER user
# Wed, 05 Oct 2022 02:59:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38058a32b36e9b598982dc9e84bc5b442f0d993d8b8cc35b705de77bd4079c0`  
		Last Modified: Wed, 05 Oct 2022 03:00:20 GMT  
		Size: 15.1 MB (15123612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f685d2ce9caca28651dcef318bf9d1b57f3436ad468d53f90454fb036dabf61`  
		Last Modified: Wed, 05 Oct 2022 03:00:16 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e265c31795984531031fa8f554c13cc2134981d630f4c585ef07c323f7592bf6`  
		Last Modified: Wed, 05 Oct 2022 03:00:17 GMT  
		Size: 4.2 MB (4167716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; 386

```console
$ docker pull irssi@sha256:ede4a5f54acdbac0bbef8dfff2d870f8721f8d7f0f56faf1c30d9cba2b3c1e57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.4 MB (51445349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:401ba8e2caef5aa3ad21791aaaaec357b7ff0c557e981b79ca2cdc752b4202fc`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:40 GMT
ADD file:a66b7a182260a23fdb8b219600a8b48a5079997715006d9a5324dda11f9d0a7f in / 
# Tue, 04 Oct 2022 23:39:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:07:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:07:47 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 02:07:48 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 02:07:49 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 02:07:50 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 02:08:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 02:08:28 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 02:08:29 GMT
USER user
# Wed, 05 Oct 2022 02:08:30 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:711839e532aa3f129f9cfaa5125d0e379ddefd47f3da44d0674372663dfc6a9b`  
		Last Modified: Tue, 04 Oct 2022 23:45:35 GMT  
		Size: 32.4 MB (32396290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3897b78423f5fe2b4ef1b6b44b72cdee85a02656d824e53a9b45fa05119820`  
		Last Modified: Wed, 05 Oct 2022 02:09:03 GMT  
		Size: 14.8 MB (14774804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d026efbb6b96c262146c2ab0678080af5ee43128a48525599459062b19ac933`  
		Last Modified: Wed, 05 Oct 2022 02:08:59 GMT  
		Size: 4.1 KB (4058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec42325882bba3a422ec9d255952eb5b7e7d64a612bc2b7803cc789529fc7af`  
		Last Modified: Wed, 05 Oct 2022 02:09:00 GMT  
		Size: 4.3 MB (4270197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; mips64le

```console
$ docker pull irssi@sha256:5a736737b0db202c5d148c37dfa0d6a9ad1541d1a27b4ed79f7b60ba1bf73303
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.4 MB (48373914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2431db016bb3697fac79163565a239a4ea51fcd6e82ed7582b0d258ff2f1837c`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 05 Oct 2022 00:10:26 GMT
ADD file:48da6b2f4e0315e4f502001a00e4b2abb58d553de11a41901ba859a461052bea in / 
# Wed, 05 Oct 2022 00:10:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:53:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:53:48 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 03:53:54 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 03:53:57 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 03:54:00 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 03:57:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 03:57:51 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 03:57:54 GMT
USER user
# Wed, 05 Oct 2022 03:57:57 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:3288c6e2e7130a1e313203f049bde0e57a05237441a3cab92c27f9ada139315b`  
		Last Modified: Wed, 05 Oct 2022 00:18:36 GMT  
		Size: 29.6 MB (29640851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c68a7b2d0fb0127b410b6897cb6f03d9db6c55bfe969cbd3cb7209008d21508`  
		Last Modified: Wed, 05 Oct 2022 03:58:33 GMT  
		Size: 14.4 MB (14412744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a9833b55885486e8305deeb21f45ab43e0ff76edc4d3007cbab9c95c85bf1b`  
		Last Modified: Wed, 05 Oct 2022 03:58:19 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786c7b4974b80e47439675806e47e06c5f1775807fec5db526c7817fd0c824dc`  
		Last Modified: Wed, 05 Oct 2022 03:58:22 GMT  
		Size: 4.3 MB (4316245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; ppc64le

```console
$ docker pull irssi@sha256:819bfaa2a3c2459299183936a909acc75c4f18b49efa6d236037778662df4d1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55723597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f58016534cac7aab90f0f1ea1595a6a430b875ea3636f3be483941e421de60d5`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:16:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:16:34 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 01:16:36 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 01:16:36 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 01:16:36 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 01:17:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 01:17:50 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 01:17:50 GMT
USER user
# Wed, 05 Oct 2022 01:17:51 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472b4724175e4977a01f80c36525225791a1eb6e26a326b32ae5fab2fdbe536e`  
		Last Modified: Wed, 05 Oct 2022 01:18:33 GMT  
		Size: 15.7 MB (15745778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e97a554db6119c4ed0483c00b8d52962bb5a4896298909894401c8e6d0770e6`  
		Last Modified: Wed, 05 Oct 2022 01:18:26 GMT  
		Size: 4.2 KB (4209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a61e2224e2a4f2b9ff30e2e0cd245a1a57e6eeeb67996f9592408f1caa38b45`  
		Last Modified: Wed, 05 Oct 2022 01:18:28 GMT  
		Size: 4.7 MB (4683026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; s390x

```console
$ docker pull irssi@sha256:821bc91e1f121cea233c4e0535908695024d5ac0c910516e23e55d33f6c951f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50152909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:759c93af933b6ce8cab5a4348f26ee85eea41e4a9bce2d80527f7c0712efdced`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Oct 2022 23:42:42 GMT
ADD file:7acfe92be51da9cffeb5b063cc87926d1ce457729e3080de340603a38216a708 in / 
# Tue, 04 Oct 2022 23:42:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:20:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:20:20 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 01:20:21 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 01:20:21 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 01:20:21 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 01:20:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 01:20:52 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 01:20:52 GMT
USER user
# Wed, 05 Oct 2022 01:20:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:62990b94a520bfcf718ec711f8444f83c536af2c83c8e53fdfe1f89fdcb79826`  
		Last Modified: Tue, 04 Oct 2022 23:47:16 GMT  
		Size: 29.7 MB (29650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd450bf3c86a270a7a33ad03c5257dbce0d0ae0f3cc9fdc2a8626a8105d4376`  
		Last Modified: Wed, 05 Oct 2022 01:21:28 GMT  
		Size: 15.7 MB (15747107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c945f26082a746b0bee6c6e989dd587cef35bcf59f193649426d53cb13e017ea`  
		Last Modified: Wed, 05 Oct 2022 01:21:25 GMT  
		Size: 4.2 KB (4209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60785dc59a371d8e5d3115f1a33a517c7429b86fe85278305999544a2e8c188c`  
		Last Modified: Wed, 05 Oct 2022 01:21:25 GMT  
		Size: 4.8 MB (4750874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1-alpine`

```console
$ docker pull irssi@sha256:f858ce918a2bf1e9a52aa3f8075c66d76539f2e02793d4f845780991fb79305e
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
$ docker pull irssi@sha256:ea6dd4cae5a87901d6561c4ec5905383f0ffd31dc072862ec3bfc9f52be51bdb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.5 MB (17470544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbdbd57b8e8f3d61feff52c3dd0e4a77b86c8ab0a60db7f5dd4f0b499ca1a9a6`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:41:24 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 09 Aug 2022 20:41:24 GMT
ENV HOME=/home/user
# Tue, 09 Aug 2022 20:41:25 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 09 Aug 2022 20:41:25 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 20:41:25 GMT
ENV IRSSI_VERSION=1.4.2
# Tue, 09 Aug 2022 20:41:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 09 Aug 2022 20:41:46 GMT
WORKDIR /home/user
# Tue, 09 Aug 2022 20:41:46 GMT
USER user
# Tue, 09 Aug 2022 20:41:46 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5d9a1c4c1f2ab14d46764ffc31eacb8ad8867425565610eddb4a37b96506dd`  
		Last Modified: Tue, 09 Aug 2022 20:42:05 GMT  
		Size: 9.6 MB (9641367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb63d9e300689b98b6818bc75a9d0f1240542f26918d5f03ee59744ca49b83c1`  
		Last Modified: Tue, 09 Aug 2022 20:42:05 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b9c190fc124c2012dca28f7fc3ac3c5efe9c138a52834b623b8bd71ac1a44a`  
		Last Modified: Tue, 09 Aug 2022 20:42:06 GMT  
		Size: 5.0 MB (5021842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:3da92cc14c4f54ed02a75e97d7ba365ad265097838c36ecc8f6060e32a6a3ac1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16400924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90c6f4fa312a222c721b14a72f090c7351868c8542685a135004eb2d408906ef`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:56:28 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 11 Aug 2022 00:56:28 GMT
ENV HOME=/home/user
# Thu, 11 Aug 2022 00:56:29 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 11 Aug 2022 00:56:29 GMT
ENV LANG=C.UTF-8
# Thu, 11 Aug 2022 00:56:29 GMT
ENV IRSSI_VERSION=1.4.2
# Thu, 11 Aug 2022 00:57:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 11 Aug 2022 00:57:07 GMT
WORKDIR /home/user
# Thu, 11 Aug 2022 00:57:07 GMT
USER user
# Thu, 11 Aug 2022 00:57:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f065e627e6c1c7d3ab86640a59afda980873f8ed6a2d5625bb12bc90f13ca050`  
		Last Modified: Thu, 11 Aug 2022 00:57:30 GMT  
		Size: 8.9 MB (8871533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3001b01987980cec44d47936a4de97a930b97fbe50c31728522beef6d769fe4f`  
		Last Modified: Thu, 11 Aug 2022 00:57:29 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6bab3bbf35689a658c0c3cc820afec8c53e14d41acf8f9ca19daa3065d9ea5`  
		Last Modified: Thu, 11 Aug 2022 00:57:29 GMT  
		Size: 4.9 MB (4914141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:8b159bfe44ef61fe32554d34ea779177ff1e120d3cc57a538bc2d7015bfe861f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.8 MB (15829370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16323f4996b0a0df0c382fea80261be6277dda0c12eb1c60f95c396c296a786d`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:32:59 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 09 Aug 2022 19:32:59 GMT
ENV HOME=/home/user
# Tue, 09 Aug 2022 19:33:00 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 09 Aug 2022 19:33:00 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 19:33:00 GMT
ENV IRSSI_VERSION=1.4.2
# Tue, 09 Aug 2022 19:33:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 09 Aug 2022 19:33:52 GMT
WORKDIR /home/user
# Tue, 09 Aug 2022 19:33:52 GMT
USER user
# Tue, 09 Aug 2022 19:33:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08850f489e1f601ce2f8dccdba25847795fc54b3dcb55ba107f95cc3f0123c36`  
		Last Modified: Tue, 09 Aug 2022 19:34:37 GMT  
		Size: 8.7 MB (8718306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffe35cbcde0da632c5c0fcc26e3b31b10faaa0874d87de116244514f90f8c0e`  
		Last Modified: Tue, 09 Aug 2022 19:34:34 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa13f0efee7ddc81731da64d4d1c922ab8853f146bf3e306e18c059f5a7bfda`  
		Last Modified: Tue, 09 Aug 2022 19:34:36 GMT  
		Size: 4.7 MB (4692715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:5f850f4ffcb0ababe2a456df3f3a27bd2f9cce6c5b76c2c403d1237dfc3c96a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17237743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90ab0c573bef0378b6c1ecd6f732d1e6fc5da398e2a7b83ae38453d43eeb9cb1`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:41:15 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 09 Aug 2022 20:41:16 GMT
ENV HOME=/home/user
# Tue, 09 Aug 2022 20:41:17 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 09 Aug 2022 20:41:18 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 20:41:19 GMT
ENV IRSSI_VERSION=1.4.2
# Tue, 09 Aug 2022 20:41:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 09 Aug 2022 20:41:38 GMT
WORKDIR /home/user
# Tue, 09 Aug 2022 20:41:39 GMT
USER user
# Tue, 09 Aug 2022 20:41:40 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f71300e5989b171ff91b55662b5c6e60fccf216a94e2dc523fb031c0bd2f2d`  
		Last Modified: Tue, 09 Aug 2022 20:42:08 GMT  
		Size: 9.6 MB (9622410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1865821a3671b3a1c2071d9304bb84bd275ae43c8b888fce5b2aa36a468f1686`  
		Last Modified: Tue, 09 Aug 2022 20:42:06 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080c6a619db387601df0d0ecd28d2259a06d26d4c410545736f2f473094e99a6`  
		Last Modified: Tue, 09 Aug 2022 20:42:07 GMT  
		Size: 4.9 MB (4906415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; 386

```console
$ docker pull irssi@sha256:6ed3028eb1909171f0f91a347ae155d04518b668de604dfa934052b72917d244
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16910572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63a782321883e16ef8a4f3c93dce0d7e3f828b0b9fc0b011a31a0baeacc0caae`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 00:22:48 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 10 Aug 2022 00:22:49 GMT
ENV HOME=/home/user
# Wed, 10 Aug 2022 00:22:50 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 10 Aug 2022 00:22:51 GMT
ENV LANG=C.UTF-8
# Wed, 10 Aug 2022 00:22:52 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 10 Aug 2022 00:23:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 10 Aug 2022 00:23:13 GMT
WORKDIR /home/user
# Wed, 10 Aug 2022 00:23:14 GMT
USER user
# Wed, 10 Aug 2022 00:23:15 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978744516fa560e1c271bf8db3148e97ccde460713e502f8833989dfd642d5a1`  
		Last Modified: Wed, 10 Aug 2022 00:23:47 GMT  
		Size: 9.0 MB (9002955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4f72cf94df8e4f8de5d6d3b4997a3082e65894bc4a91137b1579fd4e4f02f2`  
		Last Modified: Wed, 10 Aug 2022 00:23:45 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22750e7e8147aff248d9c1a3b4b387ecaedba31a726ee7f9a1309cf6a34a5081`  
		Last Modified: Wed, 10 Aug 2022 00:23:46 GMT  
		Size: 5.1 MB (5099240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:1a5f3f068371c638326b4b99fee9bcea0d960bfcd57bc9744a00b26c611b6845
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17653661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd9d71d369cea216022e65e47ff44fa8eeea4c3efe3cba5141ccfb8d5c22b483`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:46:40 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 09 Aug 2022 18:46:41 GMT
ENV HOME=/home/user
# Tue, 09 Aug 2022 18:46:42 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 09 Aug 2022 18:46:43 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 18:46:43 GMT
ENV IRSSI_VERSION=1.4.2
# Tue, 09 Aug 2022 18:47:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 09 Aug 2022 18:47:11 GMT
WORKDIR /home/user
# Tue, 09 Aug 2022 18:47:11 GMT
USER user
# Tue, 09 Aug 2022 18:47:11 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c57991f4206038524a4bddff6977cdb787830ff801f4eec780f96cd71882ae2`  
		Last Modified: Tue, 09 Aug 2022 18:47:44 GMT  
		Size: 9.7 MB (9733766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6607afe69f399563a6af6716005e0c00534c535f907afa7ebd0640b067743527`  
		Last Modified: Tue, 09 Aug 2022 18:47:40 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fd143b8ec26961c67226fc801bda07f0f072ec60f57ac2968b6cffeb9e1c4b`  
		Last Modified: Tue, 09 Aug 2022 18:47:42 GMT  
		Size: 5.1 MB (5115292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:7154308b12b2df03369f01f2870ef87cca6c81f07dcd756dfb475df3d405fe4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17700482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:316be5f59a3520b319fac3924c1742e959a5ddc7e1c52e1056ac29beb4f8a7c5`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:09:55 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 09 Aug 2022 19:09:55 GMT
ENV HOME=/home/user
# Tue, 09 Aug 2022 19:09:56 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 09 Aug 2022 19:09:56 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 19:09:56 GMT
ENV IRSSI_VERSION=1.4.2
# Tue, 09 Aug 2022 19:10:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 09 Aug 2022 19:10:16 GMT
WORKDIR /home/user
# Tue, 09 Aug 2022 19:10:16 GMT
USER user
# Tue, 09 Aug 2022 19:10:16 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397bf195fe3fcd3305c8fc52aca185c710447ed85cea20e39fbe44d1bfa29a52`  
		Last Modified: Tue, 09 Aug 2022 19:10:48 GMT  
		Size: 10.1 MB (10078568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0a54068010fe482bca0eaa0c4dcad321f4e2364a0b993da60bb0a7be54ba62`  
		Last Modified: Tue, 09 Aug 2022 19:10:46 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e3c693e69e0ec940fb8c074ef90c5b6a37d65f58970fb54a46322648fe1f8`  
		Last Modified: Tue, 09 Aug 2022 19:10:47 GMT  
		Size: 5.0 MB (5030034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4`

```console
$ docker pull irssi@sha256:4db96ec9b6933517d7c7ced80d5a431de322d56e3902934e167c031b40839993
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
$ docker pull irssi@sha256:b1bcbdd80b73f4ae87e078dc59ee578c2c34093b1ea355431ab0c1631a3bce23
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51347952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d527f60d93d54762986cae22b527791861f7b1584ab0298a550917a7f29bad58`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:11:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:11:37 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 04:11:38 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 04:11:38 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 04:11:38 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 04:12:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 04:12:17 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 04:12:17 GMT
USER user
# Wed, 05 Oct 2022 04:12:17 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77bdc13b2e9374e6b09e9fd7914a2324820a068a5b6f9e657052f6d7b67dbe95`  
		Last Modified: Wed, 05 Oct 2022 04:12:36 GMT  
		Size: 15.4 MB (15448732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2311da599c35f52f01d838f912b22e3af729ec1c3c5e575755a7094821746e`  
		Last Modified: Wed, 05 Oct 2022 04:12:33 GMT  
		Size: 4.2 KB (4207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2738f49d9720ad13f5ea47e7e1c8b46ef94eeca692abb7f8f0e706df113993eb`  
		Last Modified: Wed, 05 Oct 2022 04:12:34 GMT  
		Size: 4.5 MB (4474911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; arm variant v5

```console
$ docker pull irssi@sha256:88740de9cca35c2163e8ab77e8f1f166cbfd5d6df038fc4aef033c614706b8c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47873450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5230135f43ca49675070ca5c9aac96ac2bd7312dfa3892a5eaf2a6edaeb7438`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Oct 2022 23:49:11 GMT
ADD file:effb9e2e2f8c7539e1a2200d069a2592e8ba20c9d034b5a73fbf173b6987193c in / 
# Tue, 04 Oct 2022 23:49:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:44:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:44:56 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 01:44:56 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 01:44:57 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 01:44:57 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 01:46:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 01:46:08 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 01:46:08 GMT
USER user
# Wed, 05 Oct 2022 01:46:08 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:7b9558bbfd8050a8e6af6e60560101c49bd53f81df6fa068419b44d028e465eb`  
		Last Modified: Tue, 04 Oct 2022 23:53:54 GMT  
		Size: 28.9 MB (28918381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926bcca95f828ebbc9b9335e97fb7ea77630d58d58cdd57f095c304cbaaa5445`  
		Last Modified: Wed, 05 Oct 2022 01:46:40 GMT  
		Size: 14.6 MB (14625022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38273d8025ef0cf0e39724333850dd022ee9855d34870a753a057c6253a7bae`  
		Last Modified: Wed, 05 Oct 2022 01:46:35 GMT  
		Size: 4.2 KB (4195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5d67be13c2c15c402de10807e4690cc8cd3b47d1039d23c1918ca0077d2864`  
		Last Modified: Wed, 05 Oct 2022 01:46:36 GMT  
		Size: 4.3 MB (4325852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; arm variant v7

```console
$ docker pull irssi@sha256:fd77837c1e9019a6315e4620169b8ce504ec742b5e319173e3a4f0e1d37ec9ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45142511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff37cf9a11943845b033f0e6918067f1250ce298cff0924b7314e0d9e9cea429`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Sep 2022 03:42:37 GMT
ADD file:04b0c48a2d326e2ac4255df4a6165508f0d29d8a32147fb8df6bf9504b8f6b09 in / 
# Tue, 13 Sep 2022 03:42:37 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 11:39:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 11:39:07 GMT
ENV HOME=/home/user
# Tue, 13 Sep 2022 11:39:07 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 13 Sep 2022 11:39:08 GMT
ENV LANG=C.UTF-8
# Tue, 13 Sep 2022 11:39:08 GMT
ENV IRSSI_VERSION=1.4.2
# Tue, 13 Sep 2022 11:40:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 13 Sep 2022 11:40:23 GMT
WORKDIR /home/user
# Tue, 13 Sep 2022 11:40:23 GMT
USER user
# Tue, 13 Sep 2022 11:40:24 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:43caeee1782255456dd3403ae8e6ba191802c3deb004ca68ce0420b30368995d`  
		Last Modified: Tue, 13 Sep 2022 03:49:46 GMT  
		Size: 26.6 MB (26567059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d805b7c20340610b722146aba672823a39d3687d3816cf2cc01353f06476f569`  
		Last Modified: Tue, 13 Sep 2022 11:41:05 GMT  
		Size: 14.4 MB (14383616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be59b0b8bf1d750a007870d450e9d03125f62ff1f4b7b5c01baa939c6db0171c`  
		Last Modified: Tue, 13 Sep 2022 11:40:59 GMT  
		Size: 4.2 KB (4196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9351cace1f78aa2d855c828a2561e32e92804525197f378640aaba5b21bb2f5f`  
		Last Modified: Tue, 13 Sep 2022 11:41:01 GMT  
		Size: 4.2 MB (4187640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:276cb1d76f06ba8c2e067583632967b86be703d681b616e52772ca4ed9196706
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49359797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a3299bc6183d268d3238f72dc1cca2959c9f48f5f4a4b4ff45db50bd842be98`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:59:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:59:00 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 02:59:01 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 02:59:02 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 02:59:03 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 02:59:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 02:59:35 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 02:59:36 GMT
USER user
# Wed, 05 Oct 2022 02:59:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38058a32b36e9b598982dc9e84bc5b442f0d993d8b8cc35b705de77bd4079c0`  
		Last Modified: Wed, 05 Oct 2022 03:00:20 GMT  
		Size: 15.1 MB (15123612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f685d2ce9caca28651dcef318bf9d1b57f3436ad468d53f90454fb036dabf61`  
		Last Modified: Wed, 05 Oct 2022 03:00:16 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e265c31795984531031fa8f554c13cc2134981d630f4c585ef07c323f7592bf6`  
		Last Modified: Wed, 05 Oct 2022 03:00:17 GMT  
		Size: 4.2 MB (4167716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; 386

```console
$ docker pull irssi@sha256:ede4a5f54acdbac0bbef8dfff2d870f8721f8d7f0f56faf1c30d9cba2b3c1e57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.4 MB (51445349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:401ba8e2caef5aa3ad21791aaaaec357b7ff0c557e981b79ca2cdc752b4202fc`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:40 GMT
ADD file:a66b7a182260a23fdb8b219600a8b48a5079997715006d9a5324dda11f9d0a7f in / 
# Tue, 04 Oct 2022 23:39:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:07:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:07:47 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 02:07:48 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 02:07:49 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 02:07:50 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 02:08:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 02:08:28 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 02:08:29 GMT
USER user
# Wed, 05 Oct 2022 02:08:30 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:711839e532aa3f129f9cfaa5125d0e379ddefd47f3da44d0674372663dfc6a9b`  
		Last Modified: Tue, 04 Oct 2022 23:45:35 GMT  
		Size: 32.4 MB (32396290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3897b78423f5fe2b4ef1b6b44b72cdee85a02656d824e53a9b45fa05119820`  
		Last Modified: Wed, 05 Oct 2022 02:09:03 GMT  
		Size: 14.8 MB (14774804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d026efbb6b96c262146c2ab0678080af5ee43128a48525599459062b19ac933`  
		Last Modified: Wed, 05 Oct 2022 02:08:59 GMT  
		Size: 4.1 KB (4058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec42325882bba3a422ec9d255952eb5b7e7d64a612bc2b7803cc789529fc7af`  
		Last Modified: Wed, 05 Oct 2022 02:09:00 GMT  
		Size: 4.3 MB (4270197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; mips64le

```console
$ docker pull irssi@sha256:5a736737b0db202c5d148c37dfa0d6a9ad1541d1a27b4ed79f7b60ba1bf73303
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.4 MB (48373914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2431db016bb3697fac79163565a239a4ea51fcd6e82ed7582b0d258ff2f1837c`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 05 Oct 2022 00:10:26 GMT
ADD file:48da6b2f4e0315e4f502001a00e4b2abb58d553de11a41901ba859a461052bea in / 
# Wed, 05 Oct 2022 00:10:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:53:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:53:48 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 03:53:54 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 03:53:57 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 03:54:00 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 03:57:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 03:57:51 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 03:57:54 GMT
USER user
# Wed, 05 Oct 2022 03:57:57 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:3288c6e2e7130a1e313203f049bde0e57a05237441a3cab92c27f9ada139315b`  
		Last Modified: Wed, 05 Oct 2022 00:18:36 GMT  
		Size: 29.6 MB (29640851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c68a7b2d0fb0127b410b6897cb6f03d9db6c55bfe969cbd3cb7209008d21508`  
		Last Modified: Wed, 05 Oct 2022 03:58:33 GMT  
		Size: 14.4 MB (14412744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a9833b55885486e8305deeb21f45ab43e0ff76edc4d3007cbab9c95c85bf1b`  
		Last Modified: Wed, 05 Oct 2022 03:58:19 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786c7b4974b80e47439675806e47e06c5f1775807fec5db526c7817fd0c824dc`  
		Last Modified: Wed, 05 Oct 2022 03:58:22 GMT  
		Size: 4.3 MB (4316245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; ppc64le

```console
$ docker pull irssi@sha256:819bfaa2a3c2459299183936a909acc75c4f18b49efa6d236037778662df4d1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55723597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f58016534cac7aab90f0f1ea1595a6a430b875ea3636f3be483941e421de60d5`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:16:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:16:34 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 01:16:36 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 01:16:36 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 01:16:36 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 01:17:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 01:17:50 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 01:17:50 GMT
USER user
# Wed, 05 Oct 2022 01:17:51 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472b4724175e4977a01f80c36525225791a1eb6e26a326b32ae5fab2fdbe536e`  
		Last Modified: Wed, 05 Oct 2022 01:18:33 GMT  
		Size: 15.7 MB (15745778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e97a554db6119c4ed0483c00b8d52962bb5a4896298909894401c8e6d0770e6`  
		Last Modified: Wed, 05 Oct 2022 01:18:26 GMT  
		Size: 4.2 KB (4209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a61e2224e2a4f2b9ff30e2e0cd245a1a57e6eeeb67996f9592408f1caa38b45`  
		Last Modified: Wed, 05 Oct 2022 01:18:28 GMT  
		Size: 4.7 MB (4683026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; s390x

```console
$ docker pull irssi@sha256:821bc91e1f121cea233c4e0535908695024d5ac0c910516e23e55d33f6c951f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50152909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:759c93af933b6ce8cab5a4348f26ee85eea41e4a9bce2d80527f7c0712efdced`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Oct 2022 23:42:42 GMT
ADD file:7acfe92be51da9cffeb5b063cc87926d1ce457729e3080de340603a38216a708 in / 
# Tue, 04 Oct 2022 23:42:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:20:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:20:20 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 01:20:21 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 01:20:21 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 01:20:21 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 01:20:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 01:20:52 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 01:20:52 GMT
USER user
# Wed, 05 Oct 2022 01:20:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:62990b94a520bfcf718ec711f8444f83c536af2c83c8e53fdfe1f89fdcb79826`  
		Last Modified: Tue, 04 Oct 2022 23:47:16 GMT  
		Size: 29.7 MB (29650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd450bf3c86a270a7a33ad03c5257dbce0d0ae0f3cc9fdc2a8626a8105d4376`  
		Last Modified: Wed, 05 Oct 2022 01:21:28 GMT  
		Size: 15.7 MB (15747107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c945f26082a746b0bee6c6e989dd587cef35bcf59f193649426d53cb13e017ea`  
		Last Modified: Wed, 05 Oct 2022 01:21:25 GMT  
		Size: 4.2 KB (4209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60785dc59a371d8e5d3115f1a33a517c7429b86fe85278305999544a2e8c188c`  
		Last Modified: Wed, 05 Oct 2022 01:21:25 GMT  
		Size: 4.8 MB (4750874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4-alpine`

```console
$ docker pull irssi@sha256:f858ce918a2bf1e9a52aa3f8075c66d76539f2e02793d4f845780991fb79305e
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
$ docker pull irssi@sha256:ea6dd4cae5a87901d6561c4ec5905383f0ffd31dc072862ec3bfc9f52be51bdb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.5 MB (17470544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbdbd57b8e8f3d61feff52c3dd0e4a77b86c8ab0a60db7f5dd4f0b499ca1a9a6`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:41:24 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 09 Aug 2022 20:41:24 GMT
ENV HOME=/home/user
# Tue, 09 Aug 2022 20:41:25 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 09 Aug 2022 20:41:25 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 20:41:25 GMT
ENV IRSSI_VERSION=1.4.2
# Tue, 09 Aug 2022 20:41:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 09 Aug 2022 20:41:46 GMT
WORKDIR /home/user
# Tue, 09 Aug 2022 20:41:46 GMT
USER user
# Tue, 09 Aug 2022 20:41:46 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5d9a1c4c1f2ab14d46764ffc31eacb8ad8867425565610eddb4a37b96506dd`  
		Last Modified: Tue, 09 Aug 2022 20:42:05 GMT  
		Size: 9.6 MB (9641367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb63d9e300689b98b6818bc75a9d0f1240542f26918d5f03ee59744ca49b83c1`  
		Last Modified: Tue, 09 Aug 2022 20:42:05 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b9c190fc124c2012dca28f7fc3ac3c5efe9c138a52834b623b8bd71ac1a44a`  
		Last Modified: Tue, 09 Aug 2022 20:42:06 GMT  
		Size: 5.0 MB (5021842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:3da92cc14c4f54ed02a75e97d7ba365ad265097838c36ecc8f6060e32a6a3ac1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16400924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90c6f4fa312a222c721b14a72f090c7351868c8542685a135004eb2d408906ef`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:56:28 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 11 Aug 2022 00:56:28 GMT
ENV HOME=/home/user
# Thu, 11 Aug 2022 00:56:29 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 11 Aug 2022 00:56:29 GMT
ENV LANG=C.UTF-8
# Thu, 11 Aug 2022 00:56:29 GMT
ENV IRSSI_VERSION=1.4.2
# Thu, 11 Aug 2022 00:57:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 11 Aug 2022 00:57:07 GMT
WORKDIR /home/user
# Thu, 11 Aug 2022 00:57:07 GMT
USER user
# Thu, 11 Aug 2022 00:57:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f065e627e6c1c7d3ab86640a59afda980873f8ed6a2d5625bb12bc90f13ca050`  
		Last Modified: Thu, 11 Aug 2022 00:57:30 GMT  
		Size: 8.9 MB (8871533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3001b01987980cec44d47936a4de97a930b97fbe50c31728522beef6d769fe4f`  
		Last Modified: Thu, 11 Aug 2022 00:57:29 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6bab3bbf35689a658c0c3cc820afec8c53e14d41acf8f9ca19daa3065d9ea5`  
		Last Modified: Thu, 11 Aug 2022 00:57:29 GMT  
		Size: 4.9 MB (4914141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:8b159bfe44ef61fe32554d34ea779177ff1e120d3cc57a538bc2d7015bfe861f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.8 MB (15829370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16323f4996b0a0df0c382fea80261be6277dda0c12eb1c60f95c396c296a786d`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:32:59 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 09 Aug 2022 19:32:59 GMT
ENV HOME=/home/user
# Tue, 09 Aug 2022 19:33:00 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 09 Aug 2022 19:33:00 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 19:33:00 GMT
ENV IRSSI_VERSION=1.4.2
# Tue, 09 Aug 2022 19:33:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 09 Aug 2022 19:33:52 GMT
WORKDIR /home/user
# Tue, 09 Aug 2022 19:33:52 GMT
USER user
# Tue, 09 Aug 2022 19:33:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08850f489e1f601ce2f8dccdba25847795fc54b3dcb55ba107f95cc3f0123c36`  
		Last Modified: Tue, 09 Aug 2022 19:34:37 GMT  
		Size: 8.7 MB (8718306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffe35cbcde0da632c5c0fcc26e3b31b10faaa0874d87de116244514f90f8c0e`  
		Last Modified: Tue, 09 Aug 2022 19:34:34 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa13f0efee7ddc81731da64d4d1c922ab8853f146bf3e306e18c059f5a7bfda`  
		Last Modified: Tue, 09 Aug 2022 19:34:36 GMT  
		Size: 4.7 MB (4692715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:5f850f4ffcb0ababe2a456df3f3a27bd2f9cce6c5b76c2c403d1237dfc3c96a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17237743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90ab0c573bef0378b6c1ecd6f732d1e6fc5da398e2a7b83ae38453d43eeb9cb1`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:41:15 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 09 Aug 2022 20:41:16 GMT
ENV HOME=/home/user
# Tue, 09 Aug 2022 20:41:17 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 09 Aug 2022 20:41:18 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 20:41:19 GMT
ENV IRSSI_VERSION=1.4.2
# Tue, 09 Aug 2022 20:41:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 09 Aug 2022 20:41:38 GMT
WORKDIR /home/user
# Tue, 09 Aug 2022 20:41:39 GMT
USER user
# Tue, 09 Aug 2022 20:41:40 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f71300e5989b171ff91b55662b5c6e60fccf216a94e2dc523fb031c0bd2f2d`  
		Last Modified: Tue, 09 Aug 2022 20:42:08 GMT  
		Size: 9.6 MB (9622410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1865821a3671b3a1c2071d9304bb84bd275ae43c8b888fce5b2aa36a468f1686`  
		Last Modified: Tue, 09 Aug 2022 20:42:06 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080c6a619db387601df0d0ecd28d2259a06d26d4c410545736f2f473094e99a6`  
		Last Modified: Tue, 09 Aug 2022 20:42:07 GMT  
		Size: 4.9 MB (4906415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine` - linux; 386

```console
$ docker pull irssi@sha256:6ed3028eb1909171f0f91a347ae155d04518b668de604dfa934052b72917d244
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16910572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63a782321883e16ef8a4f3c93dce0d7e3f828b0b9fc0b011a31a0baeacc0caae`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 00:22:48 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 10 Aug 2022 00:22:49 GMT
ENV HOME=/home/user
# Wed, 10 Aug 2022 00:22:50 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 10 Aug 2022 00:22:51 GMT
ENV LANG=C.UTF-8
# Wed, 10 Aug 2022 00:22:52 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 10 Aug 2022 00:23:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 10 Aug 2022 00:23:13 GMT
WORKDIR /home/user
# Wed, 10 Aug 2022 00:23:14 GMT
USER user
# Wed, 10 Aug 2022 00:23:15 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978744516fa560e1c271bf8db3148e97ccde460713e502f8833989dfd642d5a1`  
		Last Modified: Wed, 10 Aug 2022 00:23:47 GMT  
		Size: 9.0 MB (9002955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4f72cf94df8e4f8de5d6d3b4997a3082e65894bc4a91137b1579fd4e4f02f2`  
		Last Modified: Wed, 10 Aug 2022 00:23:45 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22750e7e8147aff248d9c1a3b4b387ecaedba31a726ee7f9a1309cf6a34a5081`  
		Last Modified: Wed, 10 Aug 2022 00:23:46 GMT  
		Size: 5.1 MB (5099240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:1a5f3f068371c638326b4b99fee9bcea0d960bfcd57bc9744a00b26c611b6845
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17653661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd9d71d369cea216022e65e47ff44fa8eeea4c3efe3cba5141ccfb8d5c22b483`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:46:40 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 09 Aug 2022 18:46:41 GMT
ENV HOME=/home/user
# Tue, 09 Aug 2022 18:46:42 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 09 Aug 2022 18:46:43 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 18:46:43 GMT
ENV IRSSI_VERSION=1.4.2
# Tue, 09 Aug 2022 18:47:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 09 Aug 2022 18:47:11 GMT
WORKDIR /home/user
# Tue, 09 Aug 2022 18:47:11 GMT
USER user
# Tue, 09 Aug 2022 18:47:11 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c57991f4206038524a4bddff6977cdb787830ff801f4eec780f96cd71882ae2`  
		Last Modified: Tue, 09 Aug 2022 18:47:44 GMT  
		Size: 9.7 MB (9733766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6607afe69f399563a6af6716005e0c00534c535f907afa7ebd0640b067743527`  
		Last Modified: Tue, 09 Aug 2022 18:47:40 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fd143b8ec26961c67226fc801bda07f0f072ec60f57ac2968b6cffeb9e1c4b`  
		Last Modified: Tue, 09 Aug 2022 18:47:42 GMT  
		Size: 5.1 MB (5115292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:7154308b12b2df03369f01f2870ef87cca6c81f07dcd756dfb475df3d405fe4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17700482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:316be5f59a3520b319fac3924c1742e959a5ddc7e1c52e1056ac29beb4f8a7c5`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:09:55 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 09 Aug 2022 19:09:55 GMT
ENV HOME=/home/user
# Tue, 09 Aug 2022 19:09:56 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 09 Aug 2022 19:09:56 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 19:09:56 GMT
ENV IRSSI_VERSION=1.4.2
# Tue, 09 Aug 2022 19:10:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 09 Aug 2022 19:10:16 GMT
WORKDIR /home/user
# Tue, 09 Aug 2022 19:10:16 GMT
USER user
# Tue, 09 Aug 2022 19:10:16 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397bf195fe3fcd3305c8fc52aca185c710447ed85cea20e39fbe44d1bfa29a52`  
		Last Modified: Tue, 09 Aug 2022 19:10:48 GMT  
		Size: 10.1 MB (10078568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0a54068010fe482bca0eaa0c4dcad321f4e2364a0b993da60bb0a7be54ba62`  
		Last Modified: Tue, 09 Aug 2022 19:10:46 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e3c693e69e0ec940fb8c074ef90c5b6a37d65f58970fb54a46322648fe1f8`  
		Last Modified: Tue, 09 Aug 2022 19:10:47 GMT  
		Size: 5.0 MB (5030034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4.2`

```console
$ docker pull irssi@sha256:4db96ec9b6933517d7c7ced80d5a431de322d56e3902934e167c031b40839993
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

### `irssi:1.4.2` - linux; amd64

```console
$ docker pull irssi@sha256:b1bcbdd80b73f4ae87e078dc59ee578c2c34093b1ea355431ab0c1631a3bce23
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51347952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d527f60d93d54762986cae22b527791861f7b1584ab0298a550917a7f29bad58`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:11:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:11:37 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 04:11:38 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 04:11:38 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 04:11:38 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 04:12:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 04:12:17 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 04:12:17 GMT
USER user
# Wed, 05 Oct 2022 04:12:17 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77bdc13b2e9374e6b09e9fd7914a2324820a068a5b6f9e657052f6d7b67dbe95`  
		Last Modified: Wed, 05 Oct 2022 04:12:36 GMT  
		Size: 15.4 MB (15448732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2311da599c35f52f01d838f912b22e3af729ec1c3c5e575755a7094821746e`  
		Last Modified: Wed, 05 Oct 2022 04:12:33 GMT  
		Size: 4.2 KB (4207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2738f49d9720ad13f5ea47e7e1c8b46ef94eeca692abb7f8f0e706df113993eb`  
		Last Modified: Wed, 05 Oct 2022 04:12:34 GMT  
		Size: 4.5 MB (4474911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.2` - linux; arm variant v5

```console
$ docker pull irssi@sha256:88740de9cca35c2163e8ab77e8f1f166cbfd5d6df038fc4aef033c614706b8c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47873450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5230135f43ca49675070ca5c9aac96ac2bd7312dfa3892a5eaf2a6edaeb7438`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Oct 2022 23:49:11 GMT
ADD file:effb9e2e2f8c7539e1a2200d069a2592e8ba20c9d034b5a73fbf173b6987193c in / 
# Tue, 04 Oct 2022 23:49:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:44:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:44:56 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 01:44:56 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 01:44:57 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 01:44:57 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 01:46:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 01:46:08 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 01:46:08 GMT
USER user
# Wed, 05 Oct 2022 01:46:08 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:7b9558bbfd8050a8e6af6e60560101c49bd53f81df6fa068419b44d028e465eb`  
		Last Modified: Tue, 04 Oct 2022 23:53:54 GMT  
		Size: 28.9 MB (28918381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926bcca95f828ebbc9b9335e97fb7ea77630d58d58cdd57f095c304cbaaa5445`  
		Last Modified: Wed, 05 Oct 2022 01:46:40 GMT  
		Size: 14.6 MB (14625022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38273d8025ef0cf0e39724333850dd022ee9855d34870a753a057c6253a7bae`  
		Last Modified: Wed, 05 Oct 2022 01:46:35 GMT  
		Size: 4.2 KB (4195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5d67be13c2c15c402de10807e4690cc8cd3b47d1039d23c1918ca0077d2864`  
		Last Modified: Wed, 05 Oct 2022 01:46:36 GMT  
		Size: 4.3 MB (4325852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.2` - linux; arm variant v7

```console
$ docker pull irssi@sha256:fd77837c1e9019a6315e4620169b8ce504ec742b5e319173e3a4f0e1d37ec9ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45142511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff37cf9a11943845b033f0e6918067f1250ce298cff0924b7314e0d9e9cea429`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Sep 2022 03:42:37 GMT
ADD file:04b0c48a2d326e2ac4255df4a6165508f0d29d8a32147fb8df6bf9504b8f6b09 in / 
# Tue, 13 Sep 2022 03:42:37 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 11:39:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 11:39:07 GMT
ENV HOME=/home/user
# Tue, 13 Sep 2022 11:39:07 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 13 Sep 2022 11:39:08 GMT
ENV LANG=C.UTF-8
# Tue, 13 Sep 2022 11:39:08 GMT
ENV IRSSI_VERSION=1.4.2
# Tue, 13 Sep 2022 11:40:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 13 Sep 2022 11:40:23 GMT
WORKDIR /home/user
# Tue, 13 Sep 2022 11:40:23 GMT
USER user
# Tue, 13 Sep 2022 11:40:24 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:43caeee1782255456dd3403ae8e6ba191802c3deb004ca68ce0420b30368995d`  
		Last Modified: Tue, 13 Sep 2022 03:49:46 GMT  
		Size: 26.6 MB (26567059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d805b7c20340610b722146aba672823a39d3687d3816cf2cc01353f06476f569`  
		Last Modified: Tue, 13 Sep 2022 11:41:05 GMT  
		Size: 14.4 MB (14383616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be59b0b8bf1d750a007870d450e9d03125f62ff1f4b7b5c01baa939c6db0171c`  
		Last Modified: Tue, 13 Sep 2022 11:40:59 GMT  
		Size: 4.2 KB (4196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9351cace1f78aa2d855c828a2561e32e92804525197f378640aaba5b21bb2f5f`  
		Last Modified: Tue, 13 Sep 2022 11:41:01 GMT  
		Size: 4.2 MB (4187640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.2` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:276cb1d76f06ba8c2e067583632967b86be703d681b616e52772ca4ed9196706
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49359797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a3299bc6183d268d3238f72dc1cca2959c9f48f5f4a4b4ff45db50bd842be98`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:59:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:59:00 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 02:59:01 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 02:59:02 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 02:59:03 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 02:59:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 02:59:35 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 02:59:36 GMT
USER user
# Wed, 05 Oct 2022 02:59:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38058a32b36e9b598982dc9e84bc5b442f0d993d8b8cc35b705de77bd4079c0`  
		Last Modified: Wed, 05 Oct 2022 03:00:20 GMT  
		Size: 15.1 MB (15123612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f685d2ce9caca28651dcef318bf9d1b57f3436ad468d53f90454fb036dabf61`  
		Last Modified: Wed, 05 Oct 2022 03:00:16 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e265c31795984531031fa8f554c13cc2134981d630f4c585ef07c323f7592bf6`  
		Last Modified: Wed, 05 Oct 2022 03:00:17 GMT  
		Size: 4.2 MB (4167716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.2` - linux; 386

```console
$ docker pull irssi@sha256:ede4a5f54acdbac0bbef8dfff2d870f8721f8d7f0f56faf1c30d9cba2b3c1e57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.4 MB (51445349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:401ba8e2caef5aa3ad21791aaaaec357b7ff0c557e981b79ca2cdc752b4202fc`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:40 GMT
ADD file:a66b7a182260a23fdb8b219600a8b48a5079997715006d9a5324dda11f9d0a7f in / 
# Tue, 04 Oct 2022 23:39:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:07:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:07:47 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 02:07:48 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 02:07:49 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 02:07:50 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 02:08:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 02:08:28 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 02:08:29 GMT
USER user
# Wed, 05 Oct 2022 02:08:30 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:711839e532aa3f129f9cfaa5125d0e379ddefd47f3da44d0674372663dfc6a9b`  
		Last Modified: Tue, 04 Oct 2022 23:45:35 GMT  
		Size: 32.4 MB (32396290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3897b78423f5fe2b4ef1b6b44b72cdee85a02656d824e53a9b45fa05119820`  
		Last Modified: Wed, 05 Oct 2022 02:09:03 GMT  
		Size: 14.8 MB (14774804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d026efbb6b96c262146c2ab0678080af5ee43128a48525599459062b19ac933`  
		Last Modified: Wed, 05 Oct 2022 02:08:59 GMT  
		Size: 4.1 KB (4058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec42325882bba3a422ec9d255952eb5b7e7d64a612bc2b7803cc789529fc7af`  
		Last Modified: Wed, 05 Oct 2022 02:09:00 GMT  
		Size: 4.3 MB (4270197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.2` - linux; mips64le

```console
$ docker pull irssi@sha256:5a736737b0db202c5d148c37dfa0d6a9ad1541d1a27b4ed79f7b60ba1bf73303
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.4 MB (48373914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2431db016bb3697fac79163565a239a4ea51fcd6e82ed7582b0d258ff2f1837c`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 05 Oct 2022 00:10:26 GMT
ADD file:48da6b2f4e0315e4f502001a00e4b2abb58d553de11a41901ba859a461052bea in / 
# Wed, 05 Oct 2022 00:10:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:53:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:53:48 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 03:53:54 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 03:53:57 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 03:54:00 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 03:57:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 03:57:51 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 03:57:54 GMT
USER user
# Wed, 05 Oct 2022 03:57:57 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:3288c6e2e7130a1e313203f049bde0e57a05237441a3cab92c27f9ada139315b`  
		Last Modified: Wed, 05 Oct 2022 00:18:36 GMT  
		Size: 29.6 MB (29640851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c68a7b2d0fb0127b410b6897cb6f03d9db6c55bfe969cbd3cb7209008d21508`  
		Last Modified: Wed, 05 Oct 2022 03:58:33 GMT  
		Size: 14.4 MB (14412744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a9833b55885486e8305deeb21f45ab43e0ff76edc4d3007cbab9c95c85bf1b`  
		Last Modified: Wed, 05 Oct 2022 03:58:19 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786c7b4974b80e47439675806e47e06c5f1775807fec5db526c7817fd0c824dc`  
		Last Modified: Wed, 05 Oct 2022 03:58:22 GMT  
		Size: 4.3 MB (4316245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.2` - linux; ppc64le

```console
$ docker pull irssi@sha256:819bfaa2a3c2459299183936a909acc75c4f18b49efa6d236037778662df4d1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55723597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f58016534cac7aab90f0f1ea1595a6a430b875ea3636f3be483941e421de60d5`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:16:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:16:34 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 01:16:36 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 01:16:36 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 01:16:36 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 01:17:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 01:17:50 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 01:17:50 GMT
USER user
# Wed, 05 Oct 2022 01:17:51 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472b4724175e4977a01f80c36525225791a1eb6e26a326b32ae5fab2fdbe536e`  
		Last Modified: Wed, 05 Oct 2022 01:18:33 GMT  
		Size: 15.7 MB (15745778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e97a554db6119c4ed0483c00b8d52962bb5a4896298909894401c8e6d0770e6`  
		Last Modified: Wed, 05 Oct 2022 01:18:26 GMT  
		Size: 4.2 KB (4209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a61e2224e2a4f2b9ff30e2e0cd245a1a57e6eeeb67996f9592408f1caa38b45`  
		Last Modified: Wed, 05 Oct 2022 01:18:28 GMT  
		Size: 4.7 MB (4683026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.2` - linux; s390x

```console
$ docker pull irssi@sha256:821bc91e1f121cea233c4e0535908695024d5ac0c910516e23e55d33f6c951f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50152909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:759c93af933b6ce8cab5a4348f26ee85eea41e4a9bce2d80527f7c0712efdced`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Oct 2022 23:42:42 GMT
ADD file:7acfe92be51da9cffeb5b063cc87926d1ce457729e3080de340603a38216a708 in / 
# Tue, 04 Oct 2022 23:42:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:20:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:20:20 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 01:20:21 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 01:20:21 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 01:20:21 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 01:20:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 01:20:52 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 01:20:52 GMT
USER user
# Wed, 05 Oct 2022 01:20:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:62990b94a520bfcf718ec711f8444f83c536af2c83c8e53fdfe1f89fdcb79826`  
		Last Modified: Tue, 04 Oct 2022 23:47:16 GMT  
		Size: 29.7 MB (29650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd450bf3c86a270a7a33ad03c5257dbce0d0ae0f3cc9fdc2a8626a8105d4376`  
		Last Modified: Wed, 05 Oct 2022 01:21:28 GMT  
		Size: 15.7 MB (15747107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c945f26082a746b0bee6c6e989dd587cef35bcf59f193649426d53cb13e017ea`  
		Last Modified: Wed, 05 Oct 2022 01:21:25 GMT  
		Size: 4.2 KB (4209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60785dc59a371d8e5d3115f1a33a517c7429b86fe85278305999544a2e8c188c`  
		Last Modified: Wed, 05 Oct 2022 01:21:25 GMT  
		Size: 4.8 MB (4750874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.4.2-alpine`

```console
$ docker pull irssi@sha256:f858ce918a2bf1e9a52aa3f8075c66d76539f2e02793d4f845780991fb79305e
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

### `irssi:1.4.2-alpine` - linux; amd64

```console
$ docker pull irssi@sha256:ea6dd4cae5a87901d6561c4ec5905383f0ffd31dc072862ec3bfc9f52be51bdb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.5 MB (17470544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbdbd57b8e8f3d61feff52c3dd0e4a77b86c8ab0a60db7f5dd4f0b499ca1a9a6`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:41:24 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 09 Aug 2022 20:41:24 GMT
ENV HOME=/home/user
# Tue, 09 Aug 2022 20:41:25 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 09 Aug 2022 20:41:25 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 20:41:25 GMT
ENV IRSSI_VERSION=1.4.2
# Tue, 09 Aug 2022 20:41:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 09 Aug 2022 20:41:46 GMT
WORKDIR /home/user
# Tue, 09 Aug 2022 20:41:46 GMT
USER user
# Tue, 09 Aug 2022 20:41:46 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5d9a1c4c1f2ab14d46764ffc31eacb8ad8867425565610eddb4a37b96506dd`  
		Last Modified: Tue, 09 Aug 2022 20:42:05 GMT  
		Size: 9.6 MB (9641367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb63d9e300689b98b6818bc75a9d0f1240542f26918d5f03ee59744ca49b83c1`  
		Last Modified: Tue, 09 Aug 2022 20:42:05 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b9c190fc124c2012dca28f7fc3ac3c5efe9c138a52834b623b8bd71ac1a44a`  
		Last Modified: Tue, 09 Aug 2022 20:42:06 GMT  
		Size: 5.0 MB (5021842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.2-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:3da92cc14c4f54ed02a75e97d7ba365ad265097838c36ecc8f6060e32a6a3ac1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16400924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90c6f4fa312a222c721b14a72f090c7351868c8542685a135004eb2d408906ef`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:56:28 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 11 Aug 2022 00:56:28 GMT
ENV HOME=/home/user
# Thu, 11 Aug 2022 00:56:29 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 11 Aug 2022 00:56:29 GMT
ENV LANG=C.UTF-8
# Thu, 11 Aug 2022 00:56:29 GMT
ENV IRSSI_VERSION=1.4.2
# Thu, 11 Aug 2022 00:57:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 11 Aug 2022 00:57:07 GMT
WORKDIR /home/user
# Thu, 11 Aug 2022 00:57:07 GMT
USER user
# Thu, 11 Aug 2022 00:57:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f065e627e6c1c7d3ab86640a59afda980873f8ed6a2d5625bb12bc90f13ca050`  
		Last Modified: Thu, 11 Aug 2022 00:57:30 GMT  
		Size: 8.9 MB (8871533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3001b01987980cec44d47936a4de97a930b97fbe50c31728522beef6d769fe4f`  
		Last Modified: Thu, 11 Aug 2022 00:57:29 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6bab3bbf35689a658c0c3cc820afec8c53e14d41acf8f9ca19daa3065d9ea5`  
		Last Modified: Thu, 11 Aug 2022 00:57:29 GMT  
		Size: 4.9 MB (4914141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.2-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:8b159bfe44ef61fe32554d34ea779177ff1e120d3cc57a538bc2d7015bfe861f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.8 MB (15829370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16323f4996b0a0df0c382fea80261be6277dda0c12eb1c60f95c396c296a786d`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:32:59 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 09 Aug 2022 19:32:59 GMT
ENV HOME=/home/user
# Tue, 09 Aug 2022 19:33:00 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 09 Aug 2022 19:33:00 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 19:33:00 GMT
ENV IRSSI_VERSION=1.4.2
# Tue, 09 Aug 2022 19:33:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 09 Aug 2022 19:33:52 GMT
WORKDIR /home/user
# Tue, 09 Aug 2022 19:33:52 GMT
USER user
# Tue, 09 Aug 2022 19:33:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08850f489e1f601ce2f8dccdba25847795fc54b3dcb55ba107f95cc3f0123c36`  
		Last Modified: Tue, 09 Aug 2022 19:34:37 GMT  
		Size: 8.7 MB (8718306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffe35cbcde0da632c5c0fcc26e3b31b10faaa0874d87de116244514f90f8c0e`  
		Last Modified: Tue, 09 Aug 2022 19:34:34 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa13f0efee7ddc81731da64d4d1c922ab8853f146bf3e306e18c059f5a7bfda`  
		Last Modified: Tue, 09 Aug 2022 19:34:36 GMT  
		Size: 4.7 MB (4692715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.2-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:5f850f4ffcb0ababe2a456df3f3a27bd2f9cce6c5b76c2c403d1237dfc3c96a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17237743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90ab0c573bef0378b6c1ecd6f732d1e6fc5da398e2a7b83ae38453d43eeb9cb1`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:41:15 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 09 Aug 2022 20:41:16 GMT
ENV HOME=/home/user
# Tue, 09 Aug 2022 20:41:17 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 09 Aug 2022 20:41:18 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 20:41:19 GMT
ENV IRSSI_VERSION=1.4.2
# Tue, 09 Aug 2022 20:41:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 09 Aug 2022 20:41:38 GMT
WORKDIR /home/user
# Tue, 09 Aug 2022 20:41:39 GMT
USER user
# Tue, 09 Aug 2022 20:41:40 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f71300e5989b171ff91b55662b5c6e60fccf216a94e2dc523fb031c0bd2f2d`  
		Last Modified: Tue, 09 Aug 2022 20:42:08 GMT  
		Size: 9.6 MB (9622410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1865821a3671b3a1c2071d9304bb84bd275ae43c8b888fce5b2aa36a468f1686`  
		Last Modified: Tue, 09 Aug 2022 20:42:06 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080c6a619db387601df0d0ecd28d2259a06d26d4c410545736f2f473094e99a6`  
		Last Modified: Tue, 09 Aug 2022 20:42:07 GMT  
		Size: 4.9 MB (4906415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.2-alpine` - linux; 386

```console
$ docker pull irssi@sha256:6ed3028eb1909171f0f91a347ae155d04518b668de604dfa934052b72917d244
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16910572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63a782321883e16ef8a4f3c93dce0d7e3f828b0b9fc0b011a31a0baeacc0caae`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 00:22:48 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 10 Aug 2022 00:22:49 GMT
ENV HOME=/home/user
# Wed, 10 Aug 2022 00:22:50 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 10 Aug 2022 00:22:51 GMT
ENV LANG=C.UTF-8
# Wed, 10 Aug 2022 00:22:52 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 10 Aug 2022 00:23:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 10 Aug 2022 00:23:13 GMT
WORKDIR /home/user
# Wed, 10 Aug 2022 00:23:14 GMT
USER user
# Wed, 10 Aug 2022 00:23:15 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978744516fa560e1c271bf8db3148e97ccde460713e502f8833989dfd642d5a1`  
		Last Modified: Wed, 10 Aug 2022 00:23:47 GMT  
		Size: 9.0 MB (9002955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4f72cf94df8e4f8de5d6d3b4997a3082e65894bc4a91137b1579fd4e4f02f2`  
		Last Modified: Wed, 10 Aug 2022 00:23:45 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22750e7e8147aff248d9c1a3b4b387ecaedba31a726ee7f9a1309cf6a34a5081`  
		Last Modified: Wed, 10 Aug 2022 00:23:46 GMT  
		Size: 5.1 MB (5099240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.2-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:1a5f3f068371c638326b4b99fee9bcea0d960bfcd57bc9744a00b26c611b6845
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17653661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd9d71d369cea216022e65e47ff44fa8eeea4c3efe3cba5141ccfb8d5c22b483`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:46:40 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 09 Aug 2022 18:46:41 GMT
ENV HOME=/home/user
# Tue, 09 Aug 2022 18:46:42 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 09 Aug 2022 18:46:43 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 18:46:43 GMT
ENV IRSSI_VERSION=1.4.2
# Tue, 09 Aug 2022 18:47:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 09 Aug 2022 18:47:11 GMT
WORKDIR /home/user
# Tue, 09 Aug 2022 18:47:11 GMT
USER user
# Tue, 09 Aug 2022 18:47:11 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c57991f4206038524a4bddff6977cdb787830ff801f4eec780f96cd71882ae2`  
		Last Modified: Tue, 09 Aug 2022 18:47:44 GMT  
		Size: 9.7 MB (9733766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6607afe69f399563a6af6716005e0c00534c535f907afa7ebd0640b067743527`  
		Last Modified: Tue, 09 Aug 2022 18:47:40 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fd143b8ec26961c67226fc801bda07f0f072ec60f57ac2968b6cffeb9e1c4b`  
		Last Modified: Tue, 09 Aug 2022 18:47:42 GMT  
		Size: 5.1 MB (5115292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.2-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:7154308b12b2df03369f01f2870ef87cca6c81f07dcd756dfb475df3d405fe4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17700482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:316be5f59a3520b319fac3924c1742e959a5ddc7e1c52e1056ac29beb4f8a7c5`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:09:55 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 09 Aug 2022 19:09:55 GMT
ENV HOME=/home/user
# Tue, 09 Aug 2022 19:09:56 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 09 Aug 2022 19:09:56 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 19:09:56 GMT
ENV IRSSI_VERSION=1.4.2
# Tue, 09 Aug 2022 19:10:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 09 Aug 2022 19:10:16 GMT
WORKDIR /home/user
# Tue, 09 Aug 2022 19:10:16 GMT
USER user
# Tue, 09 Aug 2022 19:10:16 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397bf195fe3fcd3305c8fc52aca185c710447ed85cea20e39fbe44d1bfa29a52`  
		Last Modified: Tue, 09 Aug 2022 19:10:48 GMT  
		Size: 10.1 MB (10078568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0a54068010fe482bca0eaa0c4dcad321f4e2364a0b993da60bb0a7be54ba62`  
		Last Modified: Tue, 09 Aug 2022 19:10:46 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e3c693e69e0ec940fb8c074ef90c5b6a37d65f58970fb54a46322648fe1f8`  
		Last Modified: Tue, 09 Aug 2022 19:10:47 GMT  
		Size: 5.0 MB (5030034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:alpine`

```console
$ docker pull irssi@sha256:f858ce918a2bf1e9a52aa3f8075c66d76539f2e02793d4f845780991fb79305e
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
$ docker pull irssi@sha256:ea6dd4cae5a87901d6561c4ec5905383f0ffd31dc072862ec3bfc9f52be51bdb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.5 MB (17470544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbdbd57b8e8f3d61feff52c3dd0e4a77b86c8ab0a60db7f5dd4f0b499ca1a9a6`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:41:24 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 09 Aug 2022 20:41:24 GMT
ENV HOME=/home/user
# Tue, 09 Aug 2022 20:41:25 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 09 Aug 2022 20:41:25 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 20:41:25 GMT
ENV IRSSI_VERSION=1.4.2
# Tue, 09 Aug 2022 20:41:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 09 Aug 2022 20:41:46 GMT
WORKDIR /home/user
# Tue, 09 Aug 2022 20:41:46 GMT
USER user
# Tue, 09 Aug 2022 20:41:46 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5d9a1c4c1f2ab14d46764ffc31eacb8ad8867425565610eddb4a37b96506dd`  
		Last Modified: Tue, 09 Aug 2022 20:42:05 GMT  
		Size: 9.6 MB (9641367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb63d9e300689b98b6818bc75a9d0f1240542f26918d5f03ee59744ca49b83c1`  
		Last Modified: Tue, 09 Aug 2022 20:42:05 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b9c190fc124c2012dca28f7fc3ac3c5efe9c138a52834b623b8bd71ac1a44a`  
		Last Modified: Tue, 09 Aug 2022 20:42:06 GMT  
		Size: 5.0 MB (5021842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:3da92cc14c4f54ed02a75e97d7ba365ad265097838c36ecc8f6060e32a6a3ac1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16400924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90c6f4fa312a222c721b14a72f090c7351868c8542685a135004eb2d408906ef`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:56:28 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 11 Aug 2022 00:56:28 GMT
ENV HOME=/home/user
# Thu, 11 Aug 2022 00:56:29 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 11 Aug 2022 00:56:29 GMT
ENV LANG=C.UTF-8
# Thu, 11 Aug 2022 00:56:29 GMT
ENV IRSSI_VERSION=1.4.2
# Thu, 11 Aug 2022 00:57:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 11 Aug 2022 00:57:07 GMT
WORKDIR /home/user
# Thu, 11 Aug 2022 00:57:07 GMT
USER user
# Thu, 11 Aug 2022 00:57:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f065e627e6c1c7d3ab86640a59afda980873f8ed6a2d5625bb12bc90f13ca050`  
		Last Modified: Thu, 11 Aug 2022 00:57:30 GMT  
		Size: 8.9 MB (8871533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3001b01987980cec44d47936a4de97a930b97fbe50c31728522beef6d769fe4f`  
		Last Modified: Thu, 11 Aug 2022 00:57:29 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6bab3bbf35689a658c0c3cc820afec8c53e14d41acf8f9ca19daa3065d9ea5`  
		Last Modified: Thu, 11 Aug 2022 00:57:29 GMT  
		Size: 4.9 MB (4914141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:8b159bfe44ef61fe32554d34ea779177ff1e120d3cc57a538bc2d7015bfe861f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.8 MB (15829370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16323f4996b0a0df0c382fea80261be6277dda0c12eb1c60f95c396c296a786d`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:32:59 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 09 Aug 2022 19:32:59 GMT
ENV HOME=/home/user
# Tue, 09 Aug 2022 19:33:00 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 09 Aug 2022 19:33:00 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 19:33:00 GMT
ENV IRSSI_VERSION=1.4.2
# Tue, 09 Aug 2022 19:33:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 09 Aug 2022 19:33:52 GMT
WORKDIR /home/user
# Tue, 09 Aug 2022 19:33:52 GMT
USER user
# Tue, 09 Aug 2022 19:33:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08850f489e1f601ce2f8dccdba25847795fc54b3dcb55ba107f95cc3f0123c36`  
		Last Modified: Tue, 09 Aug 2022 19:34:37 GMT  
		Size: 8.7 MB (8718306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffe35cbcde0da632c5c0fcc26e3b31b10faaa0874d87de116244514f90f8c0e`  
		Last Modified: Tue, 09 Aug 2022 19:34:34 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa13f0efee7ddc81731da64d4d1c922ab8853f146bf3e306e18c059f5a7bfda`  
		Last Modified: Tue, 09 Aug 2022 19:34:36 GMT  
		Size: 4.7 MB (4692715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:5f850f4ffcb0ababe2a456df3f3a27bd2f9cce6c5b76c2c403d1237dfc3c96a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17237743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90ab0c573bef0378b6c1ecd6f732d1e6fc5da398e2a7b83ae38453d43eeb9cb1`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:41:15 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 09 Aug 2022 20:41:16 GMT
ENV HOME=/home/user
# Tue, 09 Aug 2022 20:41:17 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 09 Aug 2022 20:41:18 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 20:41:19 GMT
ENV IRSSI_VERSION=1.4.2
# Tue, 09 Aug 2022 20:41:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 09 Aug 2022 20:41:38 GMT
WORKDIR /home/user
# Tue, 09 Aug 2022 20:41:39 GMT
USER user
# Tue, 09 Aug 2022 20:41:40 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f71300e5989b171ff91b55662b5c6e60fccf216a94e2dc523fb031c0bd2f2d`  
		Last Modified: Tue, 09 Aug 2022 20:42:08 GMT  
		Size: 9.6 MB (9622410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1865821a3671b3a1c2071d9304bb84bd275ae43c8b888fce5b2aa36a468f1686`  
		Last Modified: Tue, 09 Aug 2022 20:42:06 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080c6a619db387601df0d0ecd28d2259a06d26d4c410545736f2f473094e99a6`  
		Last Modified: Tue, 09 Aug 2022 20:42:07 GMT  
		Size: 4.9 MB (4906415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; 386

```console
$ docker pull irssi@sha256:6ed3028eb1909171f0f91a347ae155d04518b668de604dfa934052b72917d244
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16910572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63a782321883e16ef8a4f3c93dce0d7e3f828b0b9fc0b011a31a0baeacc0caae`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 00:22:48 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 10 Aug 2022 00:22:49 GMT
ENV HOME=/home/user
# Wed, 10 Aug 2022 00:22:50 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 10 Aug 2022 00:22:51 GMT
ENV LANG=C.UTF-8
# Wed, 10 Aug 2022 00:22:52 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 10 Aug 2022 00:23:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 10 Aug 2022 00:23:13 GMT
WORKDIR /home/user
# Wed, 10 Aug 2022 00:23:14 GMT
USER user
# Wed, 10 Aug 2022 00:23:15 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978744516fa560e1c271bf8db3148e97ccde460713e502f8833989dfd642d5a1`  
		Last Modified: Wed, 10 Aug 2022 00:23:47 GMT  
		Size: 9.0 MB (9002955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4f72cf94df8e4f8de5d6d3b4997a3082e65894bc4a91137b1579fd4e4f02f2`  
		Last Modified: Wed, 10 Aug 2022 00:23:45 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22750e7e8147aff248d9c1a3b4b387ecaedba31a726ee7f9a1309cf6a34a5081`  
		Last Modified: Wed, 10 Aug 2022 00:23:46 GMT  
		Size: 5.1 MB (5099240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:1a5f3f068371c638326b4b99fee9bcea0d960bfcd57bc9744a00b26c611b6845
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17653661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd9d71d369cea216022e65e47ff44fa8eeea4c3efe3cba5141ccfb8d5c22b483`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:46:40 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 09 Aug 2022 18:46:41 GMT
ENV HOME=/home/user
# Tue, 09 Aug 2022 18:46:42 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 09 Aug 2022 18:46:43 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 18:46:43 GMT
ENV IRSSI_VERSION=1.4.2
# Tue, 09 Aug 2022 18:47:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 09 Aug 2022 18:47:11 GMT
WORKDIR /home/user
# Tue, 09 Aug 2022 18:47:11 GMT
USER user
# Tue, 09 Aug 2022 18:47:11 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c57991f4206038524a4bddff6977cdb787830ff801f4eec780f96cd71882ae2`  
		Last Modified: Tue, 09 Aug 2022 18:47:44 GMT  
		Size: 9.7 MB (9733766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6607afe69f399563a6af6716005e0c00534c535f907afa7ebd0640b067743527`  
		Last Modified: Tue, 09 Aug 2022 18:47:40 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fd143b8ec26961c67226fc801bda07f0f072ec60f57ac2968b6cffeb9e1c4b`  
		Last Modified: Tue, 09 Aug 2022 18:47:42 GMT  
		Size: 5.1 MB (5115292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; s390x

```console
$ docker pull irssi@sha256:7154308b12b2df03369f01f2870ef87cca6c81f07dcd756dfb475df3d405fe4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17700482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:316be5f59a3520b319fac3924c1742e959a5ddc7e1c52e1056ac29beb4f8a7c5`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:09:55 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 09 Aug 2022 19:09:55 GMT
ENV HOME=/home/user
# Tue, 09 Aug 2022 19:09:56 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 09 Aug 2022 19:09:56 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 19:09:56 GMT
ENV IRSSI_VERSION=1.4.2
# Tue, 09 Aug 2022 19:10:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 09 Aug 2022 19:10:16 GMT
WORKDIR /home/user
# Tue, 09 Aug 2022 19:10:16 GMT
USER user
# Tue, 09 Aug 2022 19:10:16 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397bf195fe3fcd3305c8fc52aca185c710447ed85cea20e39fbe44d1bfa29a52`  
		Last Modified: Tue, 09 Aug 2022 19:10:48 GMT  
		Size: 10.1 MB (10078568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0a54068010fe482bca0eaa0c4dcad321f4e2364a0b993da60bb0a7be54ba62`  
		Last Modified: Tue, 09 Aug 2022 19:10:46 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e3c693e69e0ec940fb8c074ef90c5b6a37d65f58970fb54a46322648fe1f8`  
		Last Modified: Tue, 09 Aug 2022 19:10:47 GMT  
		Size: 5.0 MB (5030034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:latest`

```console
$ docker pull irssi@sha256:4db96ec9b6933517d7c7ced80d5a431de322d56e3902934e167c031b40839993
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
$ docker pull irssi@sha256:b1bcbdd80b73f4ae87e078dc59ee578c2c34093b1ea355431ab0c1631a3bce23
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51347952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d527f60d93d54762986cae22b527791861f7b1584ab0298a550917a7f29bad58`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:11:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:11:37 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 04:11:38 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 04:11:38 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 04:11:38 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 04:12:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 04:12:17 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 04:12:17 GMT
USER user
# Wed, 05 Oct 2022 04:12:17 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77bdc13b2e9374e6b09e9fd7914a2324820a068a5b6f9e657052f6d7b67dbe95`  
		Last Modified: Wed, 05 Oct 2022 04:12:36 GMT  
		Size: 15.4 MB (15448732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2311da599c35f52f01d838f912b22e3af729ec1c3c5e575755a7094821746e`  
		Last Modified: Wed, 05 Oct 2022 04:12:33 GMT  
		Size: 4.2 KB (4207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2738f49d9720ad13f5ea47e7e1c8b46ef94eeca692abb7f8f0e706df113993eb`  
		Last Modified: Wed, 05 Oct 2022 04:12:34 GMT  
		Size: 4.5 MB (4474911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm variant v5

```console
$ docker pull irssi@sha256:88740de9cca35c2163e8ab77e8f1f166cbfd5d6df038fc4aef033c614706b8c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47873450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5230135f43ca49675070ca5c9aac96ac2bd7312dfa3892a5eaf2a6edaeb7438`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Oct 2022 23:49:11 GMT
ADD file:effb9e2e2f8c7539e1a2200d069a2592e8ba20c9d034b5a73fbf173b6987193c in / 
# Tue, 04 Oct 2022 23:49:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:44:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:44:56 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 01:44:56 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 01:44:57 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 01:44:57 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 01:46:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 01:46:08 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 01:46:08 GMT
USER user
# Wed, 05 Oct 2022 01:46:08 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:7b9558bbfd8050a8e6af6e60560101c49bd53f81df6fa068419b44d028e465eb`  
		Last Modified: Tue, 04 Oct 2022 23:53:54 GMT  
		Size: 28.9 MB (28918381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926bcca95f828ebbc9b9335e97fb7ea77630d58d58cdd57f095c304cbaaa5445`  
		Last Modified: Wed, 05 Oct 2022 01:46:40 GMT  
		Size: 14.6 MB (14625022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38273d8025ef0cf0e39724333850dd022ee9855d34870a753a057c6253a7bae`  
		Last Modified: Wed, 05 Oct 2022 01:46:35 GMT  
		Size: 4.2 KB (4195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5d67be13c2c15c402de10807e4690cc8cd3b47d1039d23c1918ca0077d2864`  
		Last Modified: Wed, 05 Oct 2022 01:46:36 GMT  
		Size: 4.3 MB (4325852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm variant v7

```console
$ docker pull irssi@sha256:fd77837c1e9019a6315e4620169b8ce504ec742b5e319173e3a4f0e1d37ec9ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45142511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff37cf9a11943845b033f0e6918067f1250ce298cff0924b7314e0d9e9cea429`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 13 Sep 2022 03:42:37 GMT
ADD file:04b0c48a2d326e2ac4255df4a6165508f0d29d8a32147fb8df6bf9504b8f6b09 in / 
# Tue, 13 Sep 2022 03:42:37 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 11:39:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 11:39:07 GMT
ENV HOME=/home/user
# Tue, 13 Sep 2022 11:39:07 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 13 Sep 2022 11:39:08 GMT
ENV LANG=C.UTF-8
# Tue, 13 Sep 2022 11:39:08 GMT
ENV IRSSI_VERSION=1.4.2
# Tue, 13 Sep 2022 11:40:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Tue, 13 Sep 2022 11:40:23 GMT
WORKDIR /home/user
# Tue, 13 Sep 2022 11:40:23 GMT
USER user
# Tue, 13 Sep 2022 11:40:24 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:43caeee1782255456dd3403ae8e6ba191802c3deb004ca68ce0420b30368995d`  
		Last Modified: Tue, 13 Sep 2022 03:49:46 GMT  
		Size: 26.6 MB (26567059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d805b7c20340610b722146aba672823a39d3687d3816cf2cc01353f06476f569`  
		Last Modified: Tue, 13 Sep 2022 11:41:05 GMT  
		Size: 14.4 MB (14383616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be59b0b8bf1d750a007870d450e9d03125f62ff1f4b7b5c01baa939c6db0171c`  
		Last Modified: Tue, 13 Sep 2022 11:40:59 GMT  
		Size: 4.2 KB (4196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9351cace1f78aa2d855c828a2561e32e92804525197f378640aaba5b21bb2f5f`  
		Last Modified: Tue, 13 Sep 2022 11:41:01 GMT  
		Size: 4.2 MB (4187640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:276cb1d76f06ba8c2e067583632967b86be703d681b616e52772ca4ed9196706
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49359797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a3299bc6183d268d3238f72dc1cca2959c9f48f5f4a4b4ff45db50bd842be98`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:59:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:59:00 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 02:59:01 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 02:59:02 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 02:59:03 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 02:59:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 02:59:35 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 02:59:36 GMT
USER user
# Wed, 05 Oct 2022 02:59:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38058a32b36e9b598982dc9e84bc5b442f0d993d8b8cc35b705de77bd4079c0`  
		Last Modified: Wed, 05 Oct 2022 03:00:20 GMT  
		Size: 15.1 MB (15123612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f685d2ce9caca28651dcef318bf9d1b57f3436ad468d53f90454fb036dabf61`  
		Last Modified: Wed, 05 Oct 2022 03:00:16 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e265c31795984531031fa8f554c13cc2134981d630f4c585ef07c323f7592bf6`  
		Last Modified: Wed, 05 Oct 2022 03:00:17 GMT  
		Size: 4.2 MB (4167716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; 386

```console
$ docker pull irssi@sha256:ede4a5f54acdbac0bbef8dfff2d870f8721f8d7f0f56faf1c30d9cba2b3c1e57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.4 MB (51445349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:401ba8e2caef5aa3ad21791aaaaec357b7ff0c557e981b79ca2cdc752b4202fc`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:40 GMT
ADD file:a66b7a182260a23fdb8b219600a8b48a5079997715006d9a5324dda11f9d0a7f in / 
# Tue, 04 Oct 2022 23:39:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:07:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:07:47 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 02:07:48 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 02:07:49 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 02:07:50 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 02:08:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 02:08:28 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 02:08:29 GMT
USER user
# Wed, 05 Oct 2022 02:08:30 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:711839e532aa3f129f9cfaa5125d0e379ddefd47f3da44d0674372663dfc6a9b`  
		Last Modified: Tue, 04 Oct 2022 23:45:35 GMT  
		Size: 32.4 MB (32396290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3897b78423f5fe2b4ef1b6b44b72cdee85a02656d824e53a9b45fa05119820`  
		Last Modified: Wed, 05 Oct 2022 02:09:03 GMT  
		Size: 14.8 MB (14774804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d026efbb6b96c262146c2ab0678080af5ee43128a48525599459062b19ac933`  
		Last Modified: Wed, 05 Oct 2022 02:08:59 GMT  
		Size: 4.1 KB (4058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec42325882bba3a422ec9d255952eb5b7e7d64a612bc2b7803cc789529fc7af`  
		Last Modified: Wed, 05 Oct 2022 02:09:00 GMT  
		Size: 4.3 MB (4270197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; mips64le

```console
$ docker pull irssi@sha256:5a736737b0db202c5d148c37dfa0d6a9ad1541d1a27b4ed79f7b60ba1bf73303
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.4 MB (48373914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2431db016bb3697fac79163565a239a4ea51fcd6e82ed7582b0d258ff2f1837c`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 05 Oct 2022 00:10:26 GMT
ADD file:48da6b2f4e0315e4f502001a00e4b2abb58d553de11a41901ba859a461052bea in / 
# Wed, 05 Oct 2022 00:10:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:53:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:53:48 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 03:53:54 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 03:53:57 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 03:54:00 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 03:57:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 03:57:51 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 03:57:54 GMT
USER user
# Wed, 05 Oct 2022 03:57:57 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:3288c6e2e7130a1e313203f049bde0e57a05237441a3cab92c27f9ada139315b`  
		Last Modified: Wed, 05 Oct 2022 00:18:36 GMT  
		Size: 29.6 MB (29640851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c68a7b2d0fb0127b410b6897cb6f03d9db6c55bfe969cbd3cb7209008d21508`  
		Last Modified: Wed, 05 Oct 2022 03:58:33 GMT  
		Size: 14.4 MB (14412744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a9833b55885486e8305deeb21f45ab43e0ff76edc4d3007cbab9c95c85bf1b`  
		Last Modified: Wed, 05 Oct 2022 03:58:19 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786c7b4974b80e47439675806e47e06c5f1775807fec5db526c7817fd0c824dc`  
		Last Modified: Wed, 05 Oct 2022 03:58:22 GMT  
		Size: 4.3 MB (4316245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; ppc64le

```console
$ docker pull irssi@sha256:819bfaa2a3c2459299183936a909acc75c4f18b49efa6d236037778662df4d1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55723597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f58016534cac7aab90f0f1ea1595a6a430b875ea3636f3be483941e421de60d5`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:16:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:16:34 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 01:16:36 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 01:16:36 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 01:16:36 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 01:17:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 01:17:50 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 01:17:50 GMT
USER user
# Wed, 05 Oct 2022 01:17:51 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472b4724175e4977a01f80c36525225791a1eb6e26a326b32ae5fab2fdbe536e`  
		Last Modified: Wed, 05 Oct 2022 01:18:33 GMT  
		Size: 15.7 MB (15745778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e97a554db6119c4ed0483c00b8d52962bb5a4896298909894401c8e6d0770e6`  
		Last Modified: Wed, 05 Oct 2022 01:18:26 GMT  
		Size: 4.2 KB (4209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a61e2224e2a4f2b9ff30e2e0cd245a1a57e6eeeb67996f9592408f1caa38b45`  
		Last Modified: Wed, 05 Oct 2022 01:18:28 GMT  
		Size: 4.7 MB (4683026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; s390x

```console
$ docker pull irssi@sha256:821bc91e1f121cea233c4e0535908695024d5ac0c910516e23e55d33f6c951f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50152909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:759c93af933b6ce8cab5a4348f26ee85eea41e4a9bce2d80527f7c0712efdced`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 04 Oct 2022 23:42:42 GMT
ADD file:7acfe92be51da9cffeb5b063cc87926d1ce457729e3080de340603a38216a708 in / 
# Tue, 04 Oct 2022 23:42:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:20:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:20:20 GMT
ENV HOME=/home/user
# Wed, 05 Oct 2022 01:20:21 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 05 Oct 2022 01:20:21 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 01:20:21 GMT
ENV IRSSI_VERSION=1.4.2
# Wed, 05 Oct 2022 01:20:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		dirmngr 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 05 Oct 2022 01:20:52 GMT
WORKDIR /home/user
# Wed, 05 Oct 2022 01:20:52 GMT
USER user
# Wed, 05 Oct 2022 01:20:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:62990b94a520bfcf718ec711f8444f83c536af2c83c8e53fdfe1f89fdcb79826`  
		Last Modified: Tue, 04 Oct 2022 23:47:16 GMT  
		Size: 29.7 MB (29650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd450bf3c86a270a7a33ad03c5257dbce0d0ae0f3cc9fdc2a8626a8105d4376`  
		Last Modified: Wed, 05 Oct 2022 01:21:28 GMT  
		Size: 15.7 MB (15747107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c945f26082a746b0bee6c6e989dd587cef35bcf59f193649426d53cb13e017ea`  
		Last Modified: Wed, 05 Oct 2022 01:21:25 GMT  
		Size: 4.2 KB (4209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60785dc59a371d8e5d3115f1a33a517c7429b86fe85278305999544a2e8c188c`  
		Last Modified: Wed, 05 Oct 2022 01:21:25 GMT  
		Size: 4.8 MB (4750874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
