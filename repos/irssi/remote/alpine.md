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
