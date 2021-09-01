## `irssi:alpine`

```console
$ docker pull irssi@sha256:8d5676506929c033a4eeb0cd811293cedbbb146f6f61affc9f25abe20cb85e28
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
$ docker pull irssi@sha256:54aed9f5ddc6bee89036e630761957063ff928e3c6ef2e0e8363fe809a8feba7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17385687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e266e61cffd958b16e73f67497cc55cc5db19d8826a9ae1327dcf1581d017f4`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:33 GMT
ADD file:ed2b5e0fbd1e7ae37ab8f808c827d23c6841ce1edd7427552d5bf741d67ebcc0 in / 
# Tue, 31 Aug 2021 22:30:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 02:11:33 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 01 Sep 2021 02:11:34 GMT
ENV HOME=/home/user
# Wed, 01 Sep 2021 02:11:35 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 01 Sep 2021 02:11:36 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 02:11:36 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 01 Sep 2021 02:12:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 01 Sep 2021 02:12:56 GMT
WORKDIR /home/user
# Wed, 01 Sep 2021 02:12:56 GMT
USER user
# Wed, 01 Sep 2021 02:12:57 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:840d18d84f6afdc3231d126fdd3f84f23f0335b61cbfa9cb8808b888a4308919`  
		Last Modified: Tue, 31 Aug 2021 22:32:11 GMT  
		Size: 2.6 MB (2623761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ed59610ed0e26b96cf4a619ae089b03ca8487d89d1398b0d881365adb3816`  
		Last Modified: Wed, 01 Sep 2021 02:13:40 GMT  
		Size: 8.8 MB (8779090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b5953e6888c716c93f83ac82d756d7fad6ab1398374be9b4faa64fb74f839c`  
		Last Modified: Wed, 01 Sep 2021 02:13:33 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572f84990f032217161d7e04873df7b2800348bf11f825abd52ec5e1176deae8`  
		Last Modified: Wed, 01 Sep 2021 02:13:36 GMT  
		Size: 6.0 MB (5981568 bytes)  
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
$ docker pull irssi@sha256:8901a76ae5d7d2a6292f82fee8a3062d7a4524b75a07a22f96c55b7bd912e3d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18888710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f68838494c740b213ccefec79a0884a0f58b84157d768cec9309735317594305`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 00:50:32 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 16 Jun 2021 00:50:32 GMT
ENV HOME=/home/user
# Wed, 16 Jun 2021 00:50:33 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 16 Jun 2021 00:50:33 GMT
ENV LANG=C.UTF-8
# Wed, 16 Jun 2021 00:50:33 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 16 Jun 2021 00:51:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 16 Jun 2021 00:51:13 GMT
WORKDIR /home/user
# Wed, 16 Jun 2021 00:51:13 GMT
USER user
# Wed, 16 Jun 2021 00:51:14 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b965bd99a1e00750f46cad20b652bf2f49423700ba12f451e5869fca77b6364`  
		Last Modified: Wed, 16 Jun 2021 00:51:49 GMT  
		Size: 9.5 MB (9542333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5a44ebf8eaa044462df7aea225d25dd162b34d0ffa737ce0a3462eb000e72f`  
		Last Modified: Wed, 16 Jun 2021 00:51:46 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604d3f7cf8caf56e972de08a9a60aab9da74b4ddf2bd340c73cbb266d418344f`  
		Last Modified: Wed, 16 Jun 2021 00:51:47 GMT  
		Size: 6.6 MB (6633078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; 386

```console
$ docker pull irssi@sha256:ae400d3d4e4862e7e1e7a92583689d09081637ac3a86dc6eb944369b8b4e3b24
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17702584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bd9062a31296f7446077703755c7c5bbdd21b9e30781ec5ebcdabedef28ae15`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 31 Aug 2021 21:23:28 GMT
ADD file:fb9d541cffc3a5660d23426ba847aa696b59a9d7f14e00ba0a63b28c9ec272c0 in / 
# Tue, 31 Aug 2021 21:23:29 GMT
CMD ["/bin/sh"]
# Tue, 31 Aug 2021 23:24:46 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 31 Aug 2021 23:24:47 GMT
ENV HOME=/home/user
# Tue, 31 Aug 2021 23:24:48 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 31 Aug 2021 23:24:48 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 23:24:48 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 31 Aug 2021 23:25:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 31 Aug 2021 23:25:53 GMT
WORKDIR /home/user
# Tue, 31 Aug 2021 23:25:54 GMT
USER user
# Tue, 31 Aug 2021 23:25:54 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4ed7d06bd90bc8d13b87220ccc6204a7d235ec943be9fb4289d856f9ff0a5b7b`  
		Last Modified: Tue, 31 Aug 2021 21:24:28 GMT  
		Size: 2.8 MB (2821095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d367faa95879f9303da2e7cb4a054e41ca5a85dce40b90fe4cbf4509a0a5a94`  
		Last Modified: Tue, 31 Aug 2021 23:26:38 GMT  
		Size: 8.9 MB (8913200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f7d791c97392256116e1ecde37f46e67749ca4ef1930f10a4df793456eb62e`  
		Last Modified: Tue, 31 Aug 2021 23:26:34 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff77a5fb4632c0811cd3f1fd8544a1295e13d25f3fdf9c421c825630bb039e7e`  
		Last Modified: Tue, 31 Aug 2021 23:26:36 GMT  
		Size: 6.0 MB (5967017 bytes)  
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
$ docker pull irssi@sha256:eeb9936461441aa33c489b1c980437cccbfd87d3eec122c2740df622e70ef0ff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.3 MB (19252818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c31ff155530c4e5f7c0c771e15469b9065ae9d3721fc704b31a85c0a99b13e9a`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 30 Jul 2021 17:41:41 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Fri, 30 Jul 2021 17:41:42 GMT
CMD ["/bin/sh"]
# Fri, 30 Jul 2021 23:52:12 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 30 Jul 2021 23:52:13 GMT
ENV HOME=/home/user
# Fri, 30 Jul 2021 23:52:14 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 30 Jul 2021 23:52:14 GMT
ENV LANG=C.UTF-8
# Fri, 30 Jul 2021 23:52:14 GMT
ENV IRSSI_VERSION=1.2.3
# Fri, 30 Jul 2021 23:52:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 30 Jul 2021 23:52:44 GMT
WORKDIR /home/user
# Fri, 30 Jul 2021 23:52:45 GMT
USER user
# Fri, 30 Jul 2021 23:52:45 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9a936ba51e79197a5e9098a09140c21158e7e319c190ceda6d65e60b2fa761`  
		Last Modified: Fri, 30 Jul 2021 23:53:16 GMT  
		Size: 10.0 MB (9983415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99acc767a00b86b35f77f9042164914c5622825086723a00b80d0d05839c7166`  
		Last Modified: Fri, 30 Jul 2021 23:53:14 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed333f96ebce4ac0cb196a542c485bdef878dd2043f10db2fdb8aced17e07316`  
		Last Modified: Fri, 30 Jul 2021 23:53:16 GMT  
		Size: 6.7 MB (6665480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
