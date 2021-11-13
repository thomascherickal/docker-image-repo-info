## `irssi:alpine`

```console
$ docker pull irssi@sha256:10000906da742eb74e681787dae810f8476cfe2c3cfe72e51b9e21429564a5bd
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
$ docker pull irssi@sha256:9051c084de77ff4daaf3422d23e397cf445d654d28ad782c80a47565e92ecef7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18641632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e872f1d1a64037f0c87f699ce6328fb406d308379574ce606a800c87c1e102b8`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 03:02:25 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 01 Sep 2021 03:02:25 GMT
ENV HOME=/home/user
# Wed, 01 Sep 2021 03:02:26 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 01 Sep 2021 03:02:26 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 03:02:27 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 01 Sep 2021 03:03:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 01 Sep 2021 03:03:22 GMT
WORKDIR /home/user
# Wed, 01 Sep 2021 03:03:23 GMT
USER user
# Wed, 01 Sep 2021 03:03:23 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78773bacdc01801bea4e2107c946e0f1106ae79b898f74d08d2dce7d8bc91501`  
		Last Modified: Wed, 01 Sep 2021 03:03:51 GMT  
		Size: 9.5 MB (9545814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7210028db7e036583db26ee52789e6cc4487ff97ce9081e4b2093ddcbf3c3831`  
		Last Modified: Wed, 01 Sep 2021 03:03:49 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf6de07cdffea641704602dcc0f013a265e1569cf80662a74afbb0668b00f77`  
		Last Modified: Wed, 01 Sep 2021 03:03:50 GMT  
		Size: 6.3 MB (6280469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:411622af3811853615c7098dfa1b54089cbfd39ee2b84ad609555f5667f92b82
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17394658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da6d2fa6232e825db829628177a338984e9d93065e36f18f273ddbbbf1230bba`
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
# Sat, 13 Nov 2021 03:08:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 13 Nov 2021 03:08:38 GMT
WORKDIR /home/user
# Sat, 13 Nov 2021 03:08:38 GMT
USER user
# Sat, 13 Nov 2021 03:08:38 GMT
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
	-	`sha256:e71524eae839c07718e925705fc282eabdc5f7bdf00917807520a46cd4952a20`  
		Last Modified: Sat, 13 Nov 2021 03:09:16 GMT  
		Size: 6.0 MB (5982098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:b88bc8fb1b57e8a533af304eededa163cb97529147cd7726a34dcf37b9e8b638
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16830642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d28630f93e647cb7978dc33e5ae2918144387c9ed08307c9349ca643272f2d18`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 01 Sep 2021 01:26:54 GMT
ADD file:4a3cd5b6e6a9e76edf236ec86eb493ae8b09bf3220a8c0fdcaa474b9d6135ad3 in / 
# Wed, 01 Sep 2021 01:26:55 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 10:56:42 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 01 Sep 2021 10:56:42 GMT
ENV HOME=/home/user
# Wed, 01 Sep 2021 10:56:44 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 01 Sep 2021 10:56:44 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 10:56:45 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 01 Sep 2021 10:57:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 01 Sep 2021 10:57:48 GMT
WORKDIR /home/user
# Wed, 01 Sep 2021 10:57:48 GMT
USER user
# Wed, 01 Sep 2021 10:57:49 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:48fad15491f9799a77d01e4a4a3b0e201ca2aba6f0849c39afa1160d6f3d905a`  
		Last Modified: Wed, 01 Sep 2021 01:28:39 GMT  
		Size: 2.4 MB (2425373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e768984e9c79920576c0b67a399f6ddf660a432c86027d50acbb972c68345d16`  
		Last Modified: Wed, 01 Sep 2021 10:58:55 GMT  
		Size: 8.6 MB (8630407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ce826298200c99f6d224d3d8c736ce190e897c2c16ab488e7fd8dd0aa944a6`  
		Last Modified: Wed, 01 Sep 2021 10:58:48 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956933be27afd02f1421e1fc71b92496066e9cf1016b02b157c769e19ad259de`  
		Last Modified: Wed, 01 Sep 2021 10:58:51 GMT  
		Size: 5.8 MB (5773593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:3fe8bace1cabd46811dd923aee5bced4433493bbd9fdd3675042f5ccf51af05e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18486264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd0c909a90e5da3cc3cfcc4213896505fcc25893d3bb88b2fb1b5fcd00e7aba9`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 13:07:35 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 01 Sep 2021 13:07:35 GMT
ENV HOME=/home/user
# Wed, 01 Sep 2021 13:07:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 01 Sep 2021 13:07:36 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 13:07:36 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 01 Sep 2021 13:08:23 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 01 Sep 2021 13:08:23 GMT
WORKDIR /home/user
# Wed, 01 Sep 2021 13:08:24 GMT
USER user
# Wed, 01 Sep 2021 13:08:24 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacbc4dc9a363ad7955524cae4e6b69570d158a01e572250a05f3a20233abc71`  
		Last Modified: Wed, 01 Sep 2021 13:08:59 GMT  
		Size: 9.5 MB (9542396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a5cb6f2ce708912ba3cc36df8eac0da91fe0e16b0699626ba6bef170d4f5dc`  
		Last Modified: Wed, 01 Sep 2021 13:08:57 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f50ff8b703b23a6435393f1c3c8bb0672f201b7da9990d3b4d226dde28dbc0`  
		Last Modified: Wed, 01 Sep 2021 13:08:58 GMT  
		Size: 6.2 MB (6229590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; 386

```console
$ docker pull irssi@sha256:e1533792e9821046cba4fd97ad160b36c6943d86078fde47a356e79b1184755a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17711979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1216a4299c56d5ac15112c6e1df985afef515bf2dbaeaa74ac5b8479b4080fbf`
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
# Sat, 13 Nov 2021 04:45:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 13 Nov 2021 04:45:13 GMT
WORKDIR /home/user
# Sat, 13 Nov 2021 04:45:13 GMT
USER user
# Sat, 13 Nov 2021 04:45:13 GMT
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
	-	`sha256:19698f734fdb7985e49d87a08629d95fecae4a127bcb935a6cb36b5e2f1eed82`  
		Last Modified: Sat, 13 Nov 2021 04:45:56 GMT  
		Size: 6.0 MB (5967572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:4c7135146a0d30e8a84286bda483fe115c65acdd817d5c868c73bd56db0ba8a6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18940781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b86a326048b45fc1f3ab2566a821cbc126f36af5fa19f61012317a112bb7164`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 01 Sep 2021 02:42:40 GMT
ADD file:07a51f1a2f818bd1c1651832ce63cb1e0046a57994724cda6a20ff1a2a685295 in / 
# Wed, 01 Sep 2021 02:42:41 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 11:13:08 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 01 Sep 2021 11:13:11 GMT
ENV HOME=/home/user
# Wed, 01 Sep 2021 11:13:19 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 01 Sep 2021 11:13:23 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 11:13:26 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 01 Sep 2021 11:14:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 01 Sep 2021 11:14:27 GMT
WORKDIR /home/user
# Wed, 01 Sep 2021 11:14:28 GMT
USER user
# Wed, 01 Sep 2021 11:14:31 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:39d9bf63205258fe1d085fd596101e6fc46ff796cda8d3ba2983e166a25b74db`  
		Last Modified: Wed, 01 Sep 2021 02:43:53 GMT  
		Size: 2.8 MB (2814813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e160cc2a572b0d023d7043ba811e9539165af1b4fca43ca959548c0ecca438d2`  
		Last Modified: Wed, 01 Sep 2021 11:15:02 GMT  
		Size: 9.6 MB (9642199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77e56bbc5942c5bd69e9f605902b97e18783ee9ccacb77e3e2d005e5c1f599c`  
		Last Modified: Wed, 01 Sep 2021 11:15:00 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:115c5b26e554443efd5d38d6afa1cabde5a66d009929ee9854952bfc2f1b16e1`  
		Last Modified: Wed, 01 Sep 2021 11:15:01 GMT  
		Size: 6.5 MB (6482499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; s390x

```console
$ docker pull irssi@sha256:4508d5ff1fb06c6ca41ad14725242a83a585019ba2c7523518098e9662766edf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18862132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aed48119bc23818d5a430a4e15912061316a5a404add032ef2b41ae01f4c0b7d`
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
# Fri, 12 Nov 2021 21:47:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 12 Nov 2021 21:47:14 GMT
WORKDIR /home/user
# Fri, 12 Nov 2021 21:47:14 GMT
USER user
# Fri, 12 Nov 2021 21:47:14 GMT
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
	-	`sha256:41e0e764314fb955762494927c095f9cc4118e7b8a19b75971a7202a131ebdc4`  
		Last Modified: Fri, 12 Nov 2021 21:47:45 GMT  
		Size: 6.3 MB (6266946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
