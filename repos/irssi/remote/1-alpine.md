## `irssi:1-alpine`

```console
$ docker pull irssi@sha256:da16a3f4bf622e3df40c9635e4ec1696773607fb56d10829f508f0fe4f76f180
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
$ docker pull irssi@sha256:65920e4c2c8f774c9b252cb3bc7379cd2be94942cf95bc14a186fc59e96ff795
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18639978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54c36c4c42c43af82bedb1d5428891c3917f165afd8094687bd6d4af747f70da`
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
# Mon, 12 Apr 2021 18:50:22 GMT
ENV IRSSI_VERSION=1.2.3
# Mon, 12 Apr 2021 18:51:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Mon, 12 Apr 2021 18:51:04 GMT
WORKDIR /home/user
# Mon, 12 Apr 2021 18:51:04 GMT
USER user
# Mon, 12 Apr 2021 18:51:04 GMT
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
	-	`sha256:3a799bf5c296f2314276f11d615bd0fc87d60aa1f103760d9504bc935bf22491`  
		Last Modified: Mon, 12 Apr 2021 18:51:43 GMT  
		Size: 6.3 MB (6280506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:82a03638c37fe1406ac5cf70577c2185fdbe0bc1e6893d5ff985c90c38cdec94
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17384085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b389e22b38a27e571f403270a70b67d5abcd5fbc839a92cae739198e2b23a71`
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
# Mon, 12 Apr 2021 17:53:55 GMT
ENV IRSSI_VERSION=1.2.3
# Mon, 12 Apr 2021 17:55:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Mon, 12 Apr 2021 17:55:02 GMT
WORKDIR /home/user
# Mon, 12 Apr 2021 17:55:04 GMT
USER user
# Mon, 12 Apr 2021 17:55:05 GMT
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
	-	`sha256:e80cc75ae3ea40881429dfdc3d6d02dc498367f0fef1298e242311114d7e4b23`  
		Last Modified: Mon, 12 Apr 2021 17:55:37 GMT  
		Size: 6.0 MB (5981519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:c638b22898dbd208b7e8c8d854b93231f61b983c3b40386391877307a06a91ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16829435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f3f00408062e7fbf83e036fb9da70424628d2538ecca1f02c534ba37e8238eb`
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
# Mon, 12 Apr 2021 18:34:41 GMT
ENV IRSSI_VERSION=1.2.3
# Mon, 12 Apr 2021 18:35:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Mon, 12 Apr 2021 18:35:30 GMT
WORKDIR /home/user
# Mon, 12 Apr 2021 18:35:30 GMT
USER user
# Mon, 12 Apr 2021 18:35:31 GMT
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
	-	`sha256:660a8eec42303754417c11c851348e537c284e43e7878bf879d7b26b3aba1b7e`  
		Last Modified: Mon, 12 Apr 2021 18:36:01 GMT  
		Size: 5.8 MB (5773673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:6c397502adeb09df034b15af0f549d45eb1892e667782623fbc9557c14093f89
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18485009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3959d2b6db47de6cbd8b9b6bb4c1162c45a835112e46dace9c64bb9432674471`
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
# Mon, 12 Apr 2021 18:24:54 GMT
ENV IRSSI_VERSION=1.2.3
# Mon, 12 Apr 2021 18:25:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Mon, 12 Apr 2021 18:25:48 GMT
WORKDIR /home/user
# Mon, 12 Apr 2021 18:25:49 GMT
USER user
# Mon, 12 Apr 2021 18:25:49 GMT
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
	-	`sha256:7e5ae2c7c921976cae8b2b4b103eec12c32ee1cd714671b874d76884a7f3d132`  
		Last Modified: Mon, 12 Apr 2021 18:26:28 GMT  
		Size: 6.2 MB (6229650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; 386

```console
$ docker pull irssi@sha256:c0a02ae62a0fa722a90f60a672f9d5d9153f266b444cc1cb19ac6f496f4bf7e2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17700273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f54e49ac0c184ed895bd21c0e0573bd68c31806ad40e68811102f9bdb0cdf602`
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
# Mon, 12 Apr 2021 17:44:43 GMT
ENV IRSSI_VERSION=1.2.3
# Mon, 12 Apr 2021 17:45:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Mon, 12 Apr 2021 17:45:31 GMT
WORKDIR /home/user
# Mon, 12 Apr 2021 17:45:31 GMT
USER user
# Mon, 12 Apr 2021 17:45:31 GMT
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
	-	`sha256:202ad83a9c34355090e3d107258662310f2c18cbfb2c82263e393320e1df7b2b`  
		Last Modified: Mon, 12 Apr 2021 17:46:17 GMT  
		Size: 6.0 MB (5967139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:256a6c359a66a3f9d1f04a774857d4a72a7b4145909f3b0a9984c4e6d7fa3941
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18938474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:402e651aec4d3b41f5654ba2233674cbc8f57914698e3912014987ada1262585`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 31 Mar 2021 18:55:41 GMT
ADD file:1dd3315eb685a1b6729efb6f5b634e414f3da0f065078952bc6c0339dc09512d in / 
# Wed, 31 Mar 2021 18:55:49 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 21:21:46 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 01 Apr 2021 21:21:52 GMT
ENV HOME=/home/user
# Thu, 01 Apr 2021 21:22:04 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 01 Apr 2021 21:22:11 GMT
ENV LANG=C.UTF-8
# Mon, 12 Apr 2021 20:27:19 GMT
ENV IRSSI_VERSION=1.2.3
# Mon, 12 Apr 2021 20:28:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Mon, 12 Apr 2021 20:28:30 GMT
WORKDIR /home/user
# Mon, 12 Apr 2021 20:28:38 GMT
USER user
# Mon, 12 Apr 2021 20:28:49 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:dc4792b25345295bf964e1db1bceedb2338bfad8f0fb64f0cc07b152df9aef84`  
		Last Modified: Wed, 31 Mar 2021 18:57:19 GMT  
		Size: 2.8 MB (2813219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f856cf191fffec3b31157243ce77432f98ec4c5c52b6e575952d07028dd0bcce`  
		Last Modified: Thu, 01 Apr 2021 21:24:14 GMT  
		Size: 9.6 MB (9642256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2072d47b2861c7294bc7054ea367f3b5cf27581592b0fadacf08033f70171863`  
		Last Modified: Thu, 01 Apr 2021 21:24:11 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df60fc902c74b13f44bad9a62014fd39093c725af709cc1275be283f9ca4a8bd`  
		Last Modified: Mon, 12 Apr 2021 20:29:40 GMT  
		Size: 6.5 MB (6481725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:d8f3ede4dc11ab5985cffb486b693ef49756957838136a92a2ca6892b52d5086
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18852303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:711464eab7d295fcbdda1295344ca9cf05620d43fef1d54f9a4bc12e6a6b0825`
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
# Mon, 12 Apr 2021 18:07:14 GMT
ENV IRSSI_VERSION=1.2.3
# Mon, 12 Apr 2021 18:07:56 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Mon, 12 Apr 2021 18:07:56 GMT
WORKDIR /home/user
# Mon, 12 Apr 2021 18:07:57 GMT
USER user
# Mon, 12 Apr 2021 18:07:57 GMT
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
	-	`sha256:012b410b8c1fd81801d20599b90441000bcb3c7ca57cdc57d11f17ca1ae80093`  
		Last Modified: Mon, 12 Apr 2021 18:08:23 GMT  
		Size: 6.3 MB (6264901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
