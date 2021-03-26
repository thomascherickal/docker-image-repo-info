## `irssi:1-alpine`

```console
$ docker pull irssi@sha256:54160b4a384e8e3fc2a157f3d70050fa83500c72d3a439c43c5fd9a896df38cf
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
$ docker pull irssi@sha256:24245295c1987dbb28c45431251089c88db5593372b5c5bee58e6506f4ba1677
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18636803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33f1ad55fcaa399e70caa279af2732c9b508aaecbe3efd9212127c30ec8aac75`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 09:44:41 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 26 Mar 2021 09:44:42 GMT
ENV HOME=/home/user
# Fri, 26 Mar 2021 09:44:43 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 26 Mar 2021 09:44:43 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 09:44:43 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 26 Mar 2021 09:45:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 26 Mar 2021 09:45:27 GMT
WORKDIR /home/user
# Fri, 26 Mar 2021 09:45:27 GMT
USER user
# Fri, 26 Mar 2021 09:45:27 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d2d88871cb6e0fc83e97c6078b9ed323e6ca68d38275fb37cabc6f290a1b8c`  
		Last Modified: Fri, 26 Mar 2021 09:45:48 GMT  
		Size: 9.5 MB (9546024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c7dff9e599f16164191fc5378bfdfe7270eec9577a1b7cc2593aa007ccb7c2`  
		Last Modified: Fri, 26 Mar 2021 09:45:45 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022ebe3897589b88e30888edbdd435f59b90fe59c7836f067ad94b58d540bd55`  
		Last Modified: Fri, 26 Mar 2021 09:45:46 GMT  
		Size: 6.3 MB (6277829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:946134c5d8e710cbbf179b0117ba2af422f93f529d86e2aecc01ff446b4003bb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17381011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e8407668016d8f4bb959fd4cf18ceb8ef7c5fa9d2de3e0adac7d5c9374a6e0e`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 25 Mar 2021 22:50:09 GMT
ADD file:ca4136238cb9a01d079efd129bccd1470945d7d4320da61373af90645a4b1146 in / 
# Thu, 25 Mar 2021 22:50:28 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:53:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 26 Mar 2021 05:53:12 GMT
ENV HOME=/home/user
# Fri, 26 Mar 2021 05:53:18 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 26 Mar 2021 05:53:20 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 05:53:21 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 26 Mar 2021 05:54:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 26 Mar 2021 05:54:51 GMT
WORKDIR /home/user
# Fri, 26 Mar 2021 05:54:52 GMT
USER user
# Fri, 26 Mar 2021 05:54:54 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:bca6a70a54896d072b6919d2ae18d3ef685bc7aed783731f68a4adac0fb93d52`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 2.6 MB (2622062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a0397c64367c9dec559dac8d419934b67b7966c50465607bca7d874d7bd2ea`  
		Last Modified: Fri, 26 Mar 2021 05:55:20 GMT  
		Size: 8.8 MB (8779146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71a78ce431823df192612d678e60543912ede7e588e99fcd71038d65388c545`  
		Last Modified: Fri, 26 Mar 2021 05:55:14 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd05c3db859506e42c6679cce73f177f1950632c0745d4c54b81e62e6f9ea61`  
		Last Modified: Fri, 26 Mar 2021 05:55:18 GMT  
		Size: 6.0 MB (5978536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:115a46cdc50bac16442fd75d0074f03fb6cd0a34fbed184d1c54c510721362f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16827376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca8749a9d6b447f282bbe9655d0f57d542f83ba2d22f455135da140d63b51ccc`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 25 Mar 2021 22:05:53 GMT
ADD file:44ef6cff6e7d37a67c5846eb792fec65025702c00c56ff96801ac79bf81b0cc3 in / 
# Thu, 25 Mar 2021 22:05:55 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:34:24 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 26 Mar 2021 01:34:27 GMT
ENV HOME=/home/user
# Fri, 26 Mar 2021 01:34:43 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 26 Mar 2021 01:34:57 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:34:58 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 26 Mar 2021 01:36:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 26 Mar 2021 01:36:30 GMT
WORKDIR /home/user
# Fri, 26 Mar 2021 01:36:32 GMT
USER user
# Fri, 26 Mar 2021 01:36:33 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6c1162af251f0d5ab4945f8506f3265b86d0a03cda37f703c2446a71a233bc20`  
		Last Modified: Thu, 25 Mar 2021 22:07:21 GMT  
		Size: 2.4 MB (2423999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc3e3c0e1237dab78d7546291ec3af3710654eb21a6a41d24735358183e2ef4`  
		Last Modified: Fri, 26 Mar 2021 01:37:10 GMT  
		Size: 8.6 MB (8630420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46da2938095dda6c27bc8a3751401e2068f53541132e174a7ab8d3da0c47260e`  
		Last Modified: Fri, 26 Mar 2021 01:37:03 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b70fe4c17acc8e06c03a1657b143ba9dcfb902d3e8bb458944dc57ad752b3f`  
		Last Modified: Fri, 26 Mar 2021 01:37:07 GMT  
		Size: 5.8 MB (5771687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:7e952f73bc19dba012551a010556a9f2830354aafeabc65ab98b99fb46b78be0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18484286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fba76d5f44622ab0ff706b71f209a569b5444a6d04f17ffb9db797df41fa954`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:25:09 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 26 Mar 2021 01:25:11 GMT
ENV HOME=/home/user
# Fri, 26 Mar 2021 01:25:14 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 26 Mar 2021 01:25:15 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:25:16 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 26 Mar 2021 01:26:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 26 Mar 2021 01:26:17 GMT
WORKDIR /home/user
# Fri, 26 Mar 2021 01:26:19 GMT
USER user
# Fri, 26 Mar 2021 01:26:20 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26913993fc81df5a50e2d87a7112af3450e67ba4062fd5b9165a12009ab102f2`  
		Last Modified: Fri, 26 Mar 2021 01:26:54 GMT  
		Size: 9.5 MB (9542280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7fd25418e612aa429275628f3f13f275019cecdb3a1fb98b1afa34d975ca4d7`  
		Last Modified: Fri, 26 Mar 2021 01:26:50 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9349288f06be1425b975ad9bdf02398a063d15cadeb878a254a09595abc9d5f9`  
		Last Modified: Fri, 26 Mar 2021 01:26:52 GMT  
		Size: 6.2 MB (6228838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; 386

```console
$ docker pull irssi@sha256:6a0279ffd88af96276b4e6f77f91af191a67083b06160756a00f6fd1e3009982
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17697705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:227f5732bdf7871068257a1c48d0bb2904bccbbbea092e0f8cae703b70f791cb`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 25 Mar 2021 22:38:25 GMT
ADD file:8953415d4b98f486af17a39ba53b38f7262aa590734c18ff9318927e5a705baf in / 
# Thu, 25 Mar 2021 22:38:26 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:59:51 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 26 Mar 2021 01:59:52 GMT
ENV HOME=/home/user
# Fri, 26 Mar 2021 01:59:53 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 26 Mar 2021 01:59:53 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:59:53 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 26 Mar 2021 02:00:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 26 Mar 2021 02:00:50 GMT
WORKDIR /home/user
# Fri, 26 Mar 2021 02:00:50 GMT
USER user
# Fri, 26 Mar 2021 02:00:50 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1fbd1c9912b638ce64a4740e3af7a3a03452f8705b8103950d677f1d79ae8164`  
		Last Modified: Thu, 25 Mar 2021 22:39:34 GMT  
		Size: 2.8 MB (2818129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1a8934e2dc515a457fca6334af810a53eb34db25494b16839f0b133883627c`  
		Last Modified: Fri, 26 Mar 2021 02:01:26 GMT  
		Size: 8.9 MB (8913129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2783e7c652bc8b874a3a033a780ab09a31d28cfee03a5b91e6c08f0d46c28db`  
		Last Modified: Fri, 26 Mar 2021 02:01:23 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6391518bf9cffe8e3d6ce27412a2de4c2fd1d1d0cb4da142b31eb2a2b507f7`  
		Last Modified: Fri, 26 Mar 2021 02:01:25 GMT  
		Size: 6.0 MB (5965177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; ppc64le

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

### `irssi:1-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:3c9d5482055f570989dac4b779ed2dd61aa3962b700a0a86135c9e9bb94205f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18849651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d3485e43acc5bf841c450ebc9d4ec75ea06ba436106b891755b7f4395339b5`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:34 GMT
ADD file:44e2c7cd992fc98df702bef7022e0f8c4ee86312c311ab5ae185fd5fc878edf9 in / 
# Thu, 25 Mar 2021 22:41:34 GMT
CMD ["/bin/sh"]
# Thu, 25 Mar 2021 23:59:56 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 25 Mar 2021 23:59:57 GMT
ENV HOME=/home/user
# Thu, 25 Mar 2021 23:59:58 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 25 Mar 2021 23:59:58 GMT
ENV LANG=C.UTF-8
# Thu, 25 Mar 2021 23:59:58 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 26 Mar 2021 00:00:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 26 Mar 2021 00:00:48 GMT
WORKDIR /home/user
# Fri, 26 Mar 2021 00:00:49 GMT
USER user
# Fri, 26 Mar 2021 00:00:49 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a266c0a9554add02ea09a46b8584cb36b7f606b7b4398b9ad7369f899f8360df`  
		Last Modified: Thu, 25 Mar 2021 22:42:07 GMT  
		Size: 2.6 MB (2602387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3247e0e05b318025a2d06f5368689c9847b298d64ed74c4f1595537be0b5c108`  
		Last Modified: Fri, 26 Mar 2021 00:01:17 GMT  
		Size: 10.0 MB (9983489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc605ff0a3f649f05afe38576d87bcc3ec1b087706cf95b44cfba2fdec1d77f`  
		Last Modified: Fri, 26 Mar 2021 00:01:15 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed45869f07cd143be2d9406f2a3ea7493dd8536819c152ecea64b0ad8c9da02`  
		Last Modified: Fri, 26 Mar 2021 00:01:16 GMT  
		Size: 6.3 MB (6262509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
