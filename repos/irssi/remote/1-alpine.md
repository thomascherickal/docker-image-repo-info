## `irssi:1-alpine`

```console
$ docker pull irssi@sha256:46938c7d6487be57267a8055d6ce5a2292840148aae70c9b088b2509d8cc2210
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
$ docker pull irssi@sha256:e9f7fca8e1035fed887c65299debd1c144dc2795ed2cd70897ea33a94537a663
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18637035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:200fcb1a18950b1666d02171cfd5fc98329498d7b47076b8c551e632f92cbb37`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Fri, 12 Mar 2021 11:06:48 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 12 Mar 2021 11:06:49 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 11:06:50 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 11:06:51 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 11:06:51 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 11:08:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 12 Mar 2021 11:08:21 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 11:08:21 GMT
USER user
# Fri, 12 Mar 2021 11:08:22 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ceb86e4dfc3e51177b0c9bebe5e21c4f62846f82bb31e9c3df05d61b12686b`  
		Last Modified: Fri, 12 Mar 2021 11:09:08 GMT  
		Size: 9.5 MB (9546291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcdb0e3bcaae9496a4170e17023710d0c83a9b50295582212ab80da6b1fea415`  
		Last Modified: Fri, 12 Mar 2021 11:09:05 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef393ac458300cb54e5348a4fad9fdacb7e8ff40df4246c6beec666e09f6bf22`  
		Last Modified: Fri, 12 Mar 2021 11:09:08 GMT  
		Size: 6.3 MB (6277814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:1f5c7f3acf830fde5a0b1b2a03c8d4c241c16f80075fa9354eee2fedcda705e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17380720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71696b9d35a21e30b8716ccac8b96700bd5f52f029875b05bbae25c07cf2482a`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 21:24:35 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 17 Feb 2021 21:24:36 GMT
ENV HOME=/home/user
# Wed, 17 Feb 2021 21:24:39 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 17 Feb 2021 21:24:40 GMT
ENV LANG=C.UTF-8
# Wed, 17 Feb 2021 21:24:41 GMT
ENV IRSSI_VERSION=1.2.2
# Wed, 17 Feb 2021 21:25:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 17 Feb 2021 21:25:34 GMT
WORKDIR /home/user
# Wed, 17 Feb 2021 21:25:35 GMT
USER user
# Wed, 17 Feb 2021 21:25:36 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ff4c5d9d970b7aea5a3154a048a8dffdecaa2ba25b1ca324fe17c97846b341`  
		Last Modified: Wed, 17 Feb 2021 21:25:58 GMT  
		Size: 8.8 MB (8779079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762491e3840e0e26a34e0b701ff53443ad7810f8597293077dc34d419566d287`  
		Last Modified: Wed, 17 Feb 2021 21:25:54 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8ff637f1f0558e9446a89673d71ef57ac31f70c30723de693a929ae08bef99`  
		Last Modified: Wed, 17 Feb 2021 21:25:56 GMT  
		Size: 6.0 MB (5978332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:98e9d26dba6b9d04ea95eb1c4db163a2e49b7f382231f090c359f4a2e62c0bb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16827140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7008468a20016e3e36be26bfef0107ff0772b2b1cb411175dbd3ff7ce17ccfc`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 17 Feb 2021 20:57:36 GMT
ADD file:efdd39e5243eaf378f12ad5a85d2222b44930850a90263e5f17e8a6b5e9bc9b8 in / 
# Wed, 17 Feb 2021 20:57:37 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 21:56:44 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 17 Feb 2021 21:56:46 GMT
ENV HOME=/home/user
# Wed, 17 Feb 2021 21:57:09 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 17 Feb 2021 21:57:15 GMT
ENV LANG=C.UTF-8
# Wed, 17 Feb 2021 21:57:19 GMT
ENV IRSSI_VERSION=1.2.2
# Wed, 17 Feb 2021 21:59:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 17 Feb 2021 21:59:18 GMT
WORKDIR /home/user
# Wed, 17 Feb 2021 21:59:22 GMT
USER user
# Wed, 17 Feb 2021 21:59:27 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f55b840e27d3dbe27e44497103a4397f043749f933eb0433d29e2f104b3435ef`  
		Last Modified: Wed, 17 Feb 2021 20:58:14 GMT  
		Size: 2.4 MB (2423892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fd61c3640b29fa2c56636a6beaba35f3feeaccdc0aa8f1b840d41e57d6567b`  
		Last Modified: Wed, 17 Feb 2021 22:00:02 GMT  
		Size: 8.6 MB (8630384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a207f2622f75244aef8808929a788c81bf2275a3a71b65b250ff28d176b528`  
		Last Modified: Wed, 17 Feb 2021 21:59:55 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38dc3cd80a9a70577dd247b0106d4642e934647618cbdde5dbd869111220070d`  
		Last Modified: Wed, 17 Feb 2021 22:00:02 GMT  
		Size: 5.8 MB (5771592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:cc4575c90f6dae0796fc4b154f3e1520bee80713e2f48bb6a6e5ce06fd2276b5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18483837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19d31b775f52fd13c91fbf2e66267a30ac75b69beda542d962c0b912be422d94`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 22:20:52 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 17 Feb 2021 22:20:53 GMT
ENV HOME=/home/user
# Wed, 17 Feb 2021 22:20:56 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 17 Feb 2021 22:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 17 Feb 2021 22:20:57 GMT
ENV IRSSI_VERSION=1.2.2
# Wed, 17 Feb 2021 22:21:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 17 Feb 2021 22:21:47 GMT
WORKDIR /home/user
# Wed, 17 Feb 2021 22:21:48 GMT
USER user
# Wed, 17 Feb 2021 22:21:49 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba8729f72053840091a8799e9dfe996d47acce7ec9c50c68be6f9b0483ab0ed`  
		Last Modified: Wed, 17 Feb 2021 22:22:12 GMT  
		Size: 9.5 MB (9542215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3392ed14425ae753e5fa75e2d36a80b6ce2d34546d951b2108d575a897acadd`  
		Last Modified: Wed, 17 Feb 2021 22:22:07 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f2dc0d6b1c298d0e87baecb85741a55d40a1e2b21029de8fd28c489b675edb`  
		Last Modified: Wed, 17 Feb 2021 22:22:10 GMT  
		Size: 6.2 MB (6228778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; 386

```console
$ docker pull irssi@sha256:49afd44f464da1b84ddcf8e51df63ffd9979e2153bd80e7173214c4a707ff320
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17697807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:211ce4bd9a3dc5572aad81dba7a21612585f9614faba8d2ed66c967de10a3c48`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 17 Feb 2021 21:38:34 GMT
ADD file:eaee53da3c87749799de55809e4a5b526c56855332b961a85b1184c660f1d65b in / 
# Wed, 17 Feb 2021 21:38:35 GMT
CMD ["/bin/sh"]
# Fri, 12 Mar 2021 21:14:56 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 12 Mar 2021 21:14:57 GMT
ENV HOME=/home/user
# Fri, 12 Mar 2021 21:14:58 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 12 Mar 2021 21:14:58 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 21:14:58 GMT
ENV IRSSI_VERSION=1.2.2
# Fri, 12 Mar 2021 21:16:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 12 Mar 2021 21:16:01 GMT
WORKDIR /home/user
# Fri, 12 Mar 2021 21:16:01 GMT
USER user
# Fri, 12 Mar 2021 21:16:01 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:86205afa28f6bc624469015a543d16608258d2828411a92c662f4fdc6d276e18`  
		Last Modified: Wed, 17 Feb 2021 21:39:07 GMT  
		Size: 2.8 MB (2818177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7518f51eb17409dde9e7f5077fdf061da3ef11f72f2e08f89e14ad2c449b2fb2`  
		Last Modified: Fri, 12 Mar 2021 21:17:15 GMT  
		Size: 8.9 MB (8913163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba34977e84e733d3bb27fa85fc868956524a54f2619965cd9c82a63f908a1c7`  
		Last Modified: Fri, 12 Mar 2021 21:17:10 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f52432e31eeadf48c81faf2c9989b3cf49acef20c9eabb4e0199dd51f5f9c81`  
		Last Modified: Fri, 12 Mar 2021 21:17:13 GMT  
		Size: 6.0 MB (5965200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:4c72b9ce99d13c413ceeceb34349195f0959ef6705bff3d990bfeb48f78627e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18937150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:961bc67276dce998669595ec39b93c4ffcdbb1deec2f14fb8a0812b19386c7ea`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 17 Feb 2021 21:17:29 GMT
ADD file:28f4377c61c0f8eb43a6b36e6a24ef5893f51d405d25b62e364988223537ae0b in / 
# Wed, 17 Feb 2021 21:17:37 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 22:25:30 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 17 Feb 2021 22:25:36 GMT
ENV HOME=/home/user
# Wed, 17 Feb 2021 22:25:50 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 17 Feb 2021 22:25:57 GMT
ENV LANG=C.UTF-8
# Wed, 17 Feb 2021 22:26:03 GMT
ENV IRSSI_VERSION=1.2.2
# Wed, 17 Feb 2021 22:26:56 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 17 Feb 2021 22:27:03 GMT
WORKDIR /home/user
# Wed, 17 Feb 2021 22:27:09 GMT
USER user
# Wed, 17 Feb 2021 22:27:18 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:cb672e0375a8f9bb3d33049ceb372ffa49b959bfc84fe6f72bfb97b682a608c8`  
		Last Modified: Wed, 17 Feb 2021 21:18:10 GMT  
		Size: 2.8 MB (2813081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4efc58752a0cef456150e07275a18c4d282e7f138583bc63eebf69a25987fcb`  
		Last Modified: Wed, 17 Feb 2021 22:27:41 GMT  
		Size: 9.6 MB (9642151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adfdf9f85897b5943354e70546f01697ecad63652ebce50231843a7d418da9fa`  
		Last Modified: Wed, 17 Feb 2021 22:27:38 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b758091d71fa62b6a338ad1b081e052c75f23628a3d668e49981c4c9b4ccfd`  
		Last Modified: Wed, 17 Feb 2021 22:27:40 GMT  
		Size: 6.5 MB (6480647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:bb161a5f89c42d7993ae06e05469df5c2eedbb3dca696493e7c99b92c8ec514e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.8 MB (18849592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81f41bb9023f99c5f41ab97ed1136f66f1ae78bdd04af43579ed469d90316ba0`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 17 Feb 2021 20:41:27 GMT
ADD file:630c66f8d774d75b51e32aff812b438d377ebd3389c4aa6c324fdf8c03b6fa13 in / 
# Wed, 17 Feb 2021 20:41:27 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 21:45:50 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 17 Feb 2021 21:45:53 GMT
ENV HOME=/home/user
# Wed, 17 Feb 2021 21:45:55 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 17 Feb 2021 21:45:56 GMT
ENV LANG=C.UTF-8
# Wed, 17 Feb 2021 21:45:56 GMT
ENV IRSSI_VERSION=1.2.2
# Wed, 17 Feb 2021 21:47:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 17 Feb 2021 21:47:19 GMT
WORKDIR /home/user
# Wed, 17 Feb 2021 21:47:20 GMT
USER user
# Wed, 17 Feb 2021 21:47:20 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ff5e8cb87555e9fa38a441f5cf0414e91353e2cd21cdb48d48b7de5bb39ce674`  
		Last Modified: Wed, 17 Feb 2021 20:41:58 GMT  
		Size: 2.6 MB (2602381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431c6777b2e72ebd239ef29f3af5bf3d5a0e20ef56f8555bd1d6755fafc88ffd`  
		Last Modified: Wed, 17 Feb 2021 21:47:46 GMT  
		Size: 10.0 MB (9983485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77dd0d64dafd0e587a28096db40881c63cf90c507b5d3ef6ad95545c2802949e`  
		Last Modified: Wed, 17 Feb 2021 21:47:43 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3dfea215a6802694908be57e3e737fe63e9897a13f70f22007fd537cf50351`  
		Last Modified: Wed, 17 Feb 2021 21:47:45 GMT  
		Size: 6.3 MB (6262456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
