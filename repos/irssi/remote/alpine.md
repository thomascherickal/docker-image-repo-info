## `irssi:alpine`

```console
$ docker pull irssi@sha256:ad80a5613dab2d926fc0132327414220b349ff48aa66568b37809625cc862d64
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
$ docker pull irssi@sha256:6aa8245ac190e819881112a308c41cd09bd93d41980ef73221c7219428590122
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18637236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c754e2a9ef5dcab8d24d3d1993311a9b7d4d4df93919e67d48847f62d225bbab`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 14:21:07 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 01 Apr 2021 14:21:07 GMT
ENV HOME=/home/user
# Thu, 01 Apr 2021 14:21:08 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 01 Apr 2021 14:21:08 GMT
ENV LANG=C.UTF-8
# Thu, 01 Apr 2021 14:21:09 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 01 Apr 2021 14:21:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 01 Apr 2021 14:21:52 GMT
WORKDIR /home/user
# Thu, 01 Apr 2021 14:21:53 GMT
USER user
# Thu, 01 Apr 2021 14:21:53 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf98002477b29d79c536f6fe960fbff731a22cfffabdde2e766d94f5a1359aed`  
		Last Modified: Thu, 01 Apr 2021 14:22:22 GMT  
		Size: 9.5 MB (9546255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95a84af2f1d5f12aa7f8c0cc6db60e25ec343c746947b99982de31ed937d3ba3`  
		Last Modified: Thu, 01 Apr 2021 14:22:20 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84375c7f5c94d59d56224562c9396fe6790a2e2b0c0a918bd03f0f835725a19`  
		Last Modified: Thu, 01 Apr 2021 14:22:24 GMT  
		Size: 6.3 MB (6277764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:a5484aec4352506ff330f7ea7bc492a47148eece9fd4e9255b20f190a3feb330
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17381084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed5e6ef92139fcc854ddc395969e461ba3a4b85709a13603a7f0e21ad2b65d50`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 19:39:13 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 31 Mar 2021 19:39:14 GMT
ENV HOME=/home/user
# Wed, 31 Mar 2021 19:39:16 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 31 Mar 2021 19:39:17 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 19:39:18 GMT
ENV IRSSI_VERSION=1.2.2
# Wed, 31 Mar 2021 19:40:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 31 Mar 2021 19:40:13 GMT
WORKDIR /home/user
# Wed, 31 Mar 2021 19:40:14 GMT
USER user
# Wed, 31 Mar 2021 19:40:16 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9d6dbeb68e60f789c16d0a29ced7a6fdb6fd8789758413a17bf6530543e59c`  
		Last Modified: Wed, 31 Mar 2021 19:40:38 GMT  
		Size: 8.8 MB (8779182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d479af9d22c450538158351d074165effcacf6f3a1542311ee062576def4a01d`  
		Last Modified: Wed, 31 Mar 2021 19:40:35 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29d17823d0d6e7c7e5fba6d5bf878f6e118514f2968088f452129753ea6efbc`  
		Last Modified: Wed, 31 Mar 2021 19:40:36 GMT  
		Size: 6.0 MB (5978518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:35cd06153e647cd56d0c0b34406cf5482d4c00326a5ce4d2e30f84c28d863d95
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16827505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d34a6f2531b9244d964dc8276401bcb77770a9ec8c49bd70bec4c6c8184fa695`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 10:28:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 01 Apr 2021 10:28:11 GMT
ENV HOME=/home/user
# Thu, 01 Apr 2021 10:28:14 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 01 Apr 2021 10:28:14 GMT
ENV LANG=C.UTF-8
# Thu, 01 Apr 2021 10:28:15 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 01 Apr 2021 10:29:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 01 Apr 2021 10:29:02 GMT
WORKDIR /home/user
# Thu, 01 Apr 2021 10:29:03 GMT
USER user
# Thu, 01 Apr 2021 10:29:04 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27e0c08dab991e9c9b54d975027c235de229050c4f7acdcb370483ae7f7f0d5`  
		Last Modified: Thu, 01 Apr 2021 10:29:27 GMT  
		Size: 8.6 MB (8630384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373cf907f776f7c6b0e6bd7b3bcd4ce6c12f4aa28c93e00b4c245e5ee327cc98`  
		Last Modified: Thu, 01 Apr 2021 10:29:22 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5201d620640835d5845da90c33ff060a06c042588e6e263e92afeb27c3e6106`  
		Last Modified: Thu, 01 Apr 2021 10:29:26 GMT  
		Size: 5.8 MB (5771743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:9ce9509d3f22445d97f347a05545c7aa92c8c607ce3b1ba26820d7bd709ee544
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18484195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7422f9ddae7f35534a0a4b9bd7380b8697b9d61c6b889bea5b20e4119f39009`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:37:25 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 01 Apr 2021 13:37:26 GMT
ENV HOME=/home/user
# Thu, 01 Apr 2021 13:37:28 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 01 Apr 2021 13:37:29 GMT
ENV LANG=C.UTF-8
# Thu, 01 Apr 2021 13:37:29 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 01 Apr 2021 13:38:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 01 Apr 2021 13:38:19 GMT
WORKDIR /home/user
# Thu, 01 Apr 2021 13:38:20 GMT
USER user
# Thu, 01 Apr 2021 13:38:21 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601660d1905962d2139c2087d48348cae80a1f978caa668bc1964cf445aa1e49`  
		Last Modified: Thu, 01 Apr 2021 13:38:42 GMT  
		Size: 9.5 MB (9542170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be2979d02b8f49de34d09cae43b8c9e1e5d676dedb8329fea8448b0160311b1`  
		Last Modified: Thu, 01 Apr 2021 13:38:39 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db215482ffbdab3161545d224ef3d62aa1e7d40779d9aa294fca1f0931ffe53f`  
		Last Modified: Thu, 01 Apr 2021 13:38:41 GMT  
		Size: 6.2 MB (6228836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; 386

```console
$ docker pull irssi@sha256:ccdf3e517979ecfabd8193db9b88f9fa32f288387d86f2c867020d5f3edd40ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17698327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e2111091c5e69158ec3f178c6faae27fc2997cfde1cdaeeeb333f2985df85c4`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:00 GMT
ADD file:245767f958e2b5e6fad41d45d3361849e7c6b2255303e3c785f0f2c86019553a in / 
# Wed, 31 Mar 2021 17:43:00 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 06:08:03 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 01 Apr 2021 06:08:03 GMT
ENV HOME=/home/user
# Thu, 01 Apr 2021 06:08:04 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 01 Apr 2021 06:08:04 GMT
ENV LANG=C.UTF-8
# Thu, 01 Apr 2021 06:08:05 GMT
ENV IRSSI_VERSION=1.2.2
# Thu, 01 Apr 2021 06:09:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 01 Apr 2021 06:09:04 GMT
WORKDIR /home/user
# Thu, 01 Apr 2021 06:09:04 GMT
USER user
# Thu, 01 Apr 2021 06:09:04 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b22e590ebf70a9a5901c380b07232ef3c07cb13440402934dfdffb8f8721a949`  
		Last Modified: Wed, 31 Mar 2021 17:44:05 GMT  
		Size: 2.8 MB (2818802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd1baef9801e78a08e6a89ead5214f97087c9469d24b24f066defd26ea9d49b`  
		Last Modified: Thu, 01 Apr 2021 06:09:41 GMT  
		Size: 8.9 MB (8913062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2223a7731b3d636d550400e0313b717a969d0083bfc49f9777f7b0f944efb56`  
		Last Modified: Thu, 01 Apr 2021 06:09:38 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f6068139ebf7aca77bc2919f0303cc06d53329864def142aabd1c9da71a547`  
		Last Modified: Thu, 01 Apr 2021 06:09:40 GMT  
		Size: 6.0 MB (5965193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:3d1948a0ceda5993a4cfdeefa7dd4d31fd815055235e99ae4c1e0d904dd1412a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18937265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe6dfa6dd0254312eba3b51ef834249b06061fa100633addef7bbbf84c42b637`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:28 GMT
ADD file:f91f8e0aa646cb847f6e210056280f9332382ad2f8d6a8839fd9aa69b81c4a2a in / 
# Thu, 25 Mar 2021 22:22:30 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:18:40 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 26 Mar 2021 01:18:48 GMT
ENV HOME=/home/user
# Fri, 26 Mar 2021 01:19:13 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 26 Mar 2021 01:19:21 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:19:27 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 26 Mar 2021 01:20:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 26 Mar 2021 01:20:35 GMT
WORKDIR /home/user
# Fri, 26 Mar 2021 01:20:45 GMT
USER user
# Fri, 26 Mar 2021 01:20:55 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f3b2866c25f0a9167af050d646a7a740ccc88d46e068c90ff28a5c2ec2ee0030`  
		Last Modified: Thu, 25 Mar 2021 22:24:08 GMT  
		Size: 2.8 MB (2813115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c86a2b2846b9a05e2deb4452ef826e8aa09d0d3b0b0ad866470ca47fcc0010b`  
		Last Modified: Fri, 26 Mar 2021 01:21:23 GMT  
		Size: 9.6 MB (9642108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f273ec2efe1d38112809f70cfe7a4c8f2912c0d43d784b03bfd2584665034e`  
		Last Modified: Fri, 26 Mar 2021 01:21:18 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a46d376716d33d6040dc26a63f40a6c19a9ea7b6a3680fc69e4bc7405792b55`  
		Last Modified: Fri, 26 Mar 2021 01:21:22 GMT  
		Size: 6.5 MB (6480769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; s390x

```console
$ docker pull irssi@sha256:044bfab7c7fd62f7622d1dd4d6f02dccace6760cd2d50120001d3c7e2c1573b4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18849908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3128ea142000185ece5d05a21f1a9ac32e08b9160576e33eef7808475bc1729`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 31 Mar 2021 17:14:58 GMT
ADD file:3f5fe04867af3c9f2cfc5b315d97097145ae11343399985386321a8db21d7786 in / 
# Wed, 31 Mar 2021 17:14:58 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:54:42 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 31 Mar 2021 18:54:43 GMT
ENV HOME=/home/user
# Wed, 31 Mar 2021 18:54:44 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 31 Mar 2021 18:54:44 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 18:54:44 GMT
ENV IRSSI_VERSION=1.2.2
# Wed, 31 Mar 2021 18:55:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 31 Mar 2021 18:55:17 GMT
WORKDIR /home/user
# Wed, 31 Mar 2021 18:55:17 GMT
USER user
# Wed, 31 Mar 2021 18:55:17 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1d4058bbeedf5296bcaf5ae8f37c8cd58152acad3ec45a536e08b83f5d3abe83`  
		Last Modified: Wed, 31 Mar 2021 17:15:36 GMT  
		Size: 2.6 MB (2602591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80e3f3ec4adc52c58c33d0777ff16da8d3991a133f827fa95a0d676a349bc73`  
		Last Modified: Wed, 31 Mar 2021 18:55:37 GMT  
		Size: 10.0 MB (9983542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120aa4aeb1bc265921d93e5a1f48fcb1dbfeceb2198b948dbf6929114905a479`  
		Last Modified: Wed, 31 Mar 2021 18:55:35 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cee1d7ad5c76239f8d82c5c346e691329521bfdeb1c2bc8ef766feb6fecb199`  
		Last Modified: Wed, 31 Mar 2021 18:55:36 GMT  
		Size: 6.3 MB (6262506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
