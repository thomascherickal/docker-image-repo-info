## `irssi:1-alpine`

```console
$ docker pull irssi@sha256:936baa99fd27d3142f027620403f5c4261966714f240ffb2cbfbaf41e646df29
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
$ docker pull irssi@sha256:d7bbd05aae77230148f9a3af4a07717c5626cdb254caa1dc239bfc8866124f3e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18648371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b63678d9d2827a5a4d447b135a05921b9b618d639a9641f3970ce71fbad41c58`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:46 GMT
ADD file:a2ef39a587aac85256b55bee81f17d73aaa7154b2a32a31527c7803fb889f2e7 in / 
# Tue, 29 Mar 2022 00:19:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 16:40:04 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 16:40:04 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 16:40:05 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 16:40:05 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 16:40:05 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 16:40:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 16:40:49 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 16:40:49 GMT
USER user
# Tue, 29 Mar 2022 16:40:49 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b9c05db88786fd3c89b78787631257301391f898c03ba50553b556630046a741`  
		Last Modified: Tue, 29 Mar 2022 00:20:43 GMT  
		Size: 2.8 MB (2819223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c516145633461419b5a658706a7453eb731aaf449afd25b5996b275b8692bb0e`  
		Last Modified: Tue, 29 Mar 2022 16:41:30 GMT  
		Size: 9.5 MB (9540598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d5246be564bab1c71a70cfe50bdab883825a0ec36ed4a79b2c6730ee23849f`  
		Last Modified: Tue, 29 Mar 2022 16:41:28 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0543c4eb94b3e7485a55ed115e70d48d246fc300c3430bf71f774b156b56f7`  
		Last Modified: Tue, 29 Mar 2022 16:41:29 GMT  
		Size: 6.3 MB (6287279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:8f4fc787e0e6164fcc251c034c9fbff27d3a81fdda0c2a82c859312e16aa677a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17385391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:facc4fa1f84eebf576961df4f191b9e7763fd7f790ee44517915d56ab994e139`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:56 GMT
ADD file:23d913551f75313e359a4e93592ea0a9655e1a7c2bec5fddd210717d70c3114b in / 
# Tue, 29 Mar 2022 00:49:57 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 14:24:05 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 14:24:06 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 14:24:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 14:24:08 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 14:24:08 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 14:25:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 14:25:17 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 14:25:18 GMT
USER user
# Tue, 29 Mar 2022 14:25:18 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:eba0847afba90891ea7dae672f5dadfa405a822df0bc9c00b9e3328fd5fd889c`  
		Last Modified: Tue, 29 Mar 2022 00:51:57 GMT  
		Size: 2.6 MB (2625139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475d9671ce28a72461f25c4368162f9eac018ffced5ee61d17852dac61f60923`  
		Last Modified: Tue, 29 Mar 2022 14:25:59 GMT  
		Size: 8.8 MB (8771957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223ba1931ceb81e998f74a59ac08d88367fa3be50d7864242a41937e0a744bb8`  
		Last Modified: Tue, 29 Mar 2022 14:25:51 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9769077f19f3aaf8bd8f635611ddc58ab0133ca7a4207c1e68a6b84b68056afa`  
		Last Modified: Tue, 29 Mar 2022 14:25:55 GMT  
		Size: 6.0 MB (5987025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:e312fc3402a23fb5351bad650fcca9a110829b70b283e8e7df8c37ea4112cc45
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16842191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ab99ef1387aa082a983c091f006d251f2a6b319553055cc7a8bd70031b0e9b2`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 17 Mar 2022 17:21:20 GMT
ADD file:f344062e779295f3ffdf5aa2a96f612ea43641e0f16f7e57aea76397d3f4fa73 in / 
# Thu, 17 Mar 2022 17:21:20 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 21:49:36 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 17 Mar 2022 21:49:36 GMT
ENV HOME=/home/user
# Thu, 17 Mar 2022 21:49:38 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 17 Mar 2022 21:49:38 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 21:49:39 GMT
ENV IRSSI_VERSION=1.2.3
# Thu, 17 Mar 2022 21:50:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 17 Mar 2022 21:50:50 GMT
WORKDIR /home/user
# Thu, 17 Mar 2022 21:50:51 GMT
USER user
# Thu, 17 Mar 2022 21:50:51 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:3d0ef912dbf7e079651f96dee1bc54906d1031f15a218fccfb8fba8a499725c5`  
		Last Modified: Thu, 17 Mar 2022 17:22:57 GMT  
		Size: 2.4 MB (2430582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ca123aec7b214ed63c82d8bfbcb8edcfa2e900ae7ffb3f71870c7bc1b0919f`  
		Last Modified: Thu, 17 Mar 2022 21:52:25 GMT  
		Size: 8.6 MB (8626346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7096c42e6b59ea41b1f98c5daa696137c808f11744d82646d1d79851132839`  
		Last Modified: Thu, 17 Mar 2022 21:52:17 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c6a11add432286e33c96a2001551f6d613435e163b97021d36fdf909900e2d`  
		Last Modified: Thu, 17 Mar 2022 21:52:20 GMT  
		Size: 5.8 MB (5783992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:dfc50492eaf70eaec1101ec66e1039ff67a7db7dd5800d74dc45a4a739e02c20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18505715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39eb77e04653f1fe9557fb01ddbcf5aa051eb2f6c3c10529e6e8c1dda25085a7`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:18 GMT
ADD file:3b8e0dac20ca40faf2aaf084b69476a222952f177c0e6ec90804a10c91a51feb in / 
# Tue, 29 Mar 2022 00:40:19 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:59:34 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 11:59:35 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 11:59:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 11:59:37 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 11:59:38 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 12:00:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 12:00:38 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 12:00:39 GMT
USER user
# Tue, 29 Mar 2022 12:00:40 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4e7dd0becbc2dc968b69cba46c81a25fa500c88a644832ce17a5bb090925fa79`  
		Last Modified: Tue, 29 Mar 2022 00:41:37 GMT  
		Size: 2.7 MB (2720845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac63509931e219bc0df384426086bba93e5441adbe04844a6c56a7735dac3694`  
		Last Modified: Tue, 29 Mar 2022 12:01:26 GMT  
		Size: 9.5 MB (9536372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a61c76a95903e39d6d820ac1aa943f60dadb3928830a7cdca8225e25f8adef9`  
		Last Modified: Tue, 29 Mar 2022 12:01:24 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a666811bc4a9b90ef3fd8809c2eee8110d7113f8ec0ff856025534ae9399d8`  
		Last Modified: Tue, 29 Mar 2022 12:01:25 GMT  
		Size: 6.2 MB (6247254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; 386

```console
$ docker pull irssi@sha256:2bf221ef68d0a83a2116f20883a82c6ce6a7e0b4a5dfd71aa071b1db35aba964
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17703944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9afa5090692aa67a79e6c4008981e2926490e0d02199c568434f36da260714c`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:38:45 GMT
ADD file:f1abe5c2930209c2d735059c8e767e630c0818cc18a4fd10b0b90e6efbc675e2 in / 
# Tue, 29 Mar 2022 00:38:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 05:49:58 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 05:49:58 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 05:49:59 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 05:50:00 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 05:50:01 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 05:50:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 05:50:35 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 05:50:36 GMT
USER user
# Tue, 29 Mar 2022 05:50:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:dadad3128a09e6d507e89afe042cb1d48da14a72b28ca79dec7c6acf971bd9e6`  
		Last Modified: Tue, 29 Mar 2022 00:40:03 GMT  
		Size: 2.8 MB (2820388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101c682f90c53e18b63f7d30a8a7307eac0253f42c2fd84242c34fe251569421`  
		Last Modified: Tue, 29 Mar 2022 05:51:27 GMT  
		Size: 8.9 MB (8904321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:749bdf2ce2f439246606355222bf5bc711659dab2fa692f263642488f30cf45a`  
		Last Modified: Tue, 29 Mar 2022 05:51:26 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83177ea77693953b946bef5957dce55878d366d9332cb8cb61db7f190ce662f4`  
		Last Modified: Tue, 29 Mar 2022 05:51:27 GMT  
		Size: 6.0 MB (5977991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:977677327cf46ebee97c359921786db207de5c7cb4ab7d9b116d4c1d33ce4a80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18941144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:608f69d4d0976fd802228409ecdc55faff220c9aee1b43137f96bf8338f677f6`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:17:21 GMT
ADD file:0f301305d95e2e1e0580ec71f76edab57a1c18ed0adba5d09708b587ec19e622 in / 
# Tue, 29 Mar 2022 00:17:25 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:40:24 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 07:40:29 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 07:40:34 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 07:40:36 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 07:40:39 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 07:41:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 07:41:37 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 07:41:39 GMT
USER user
# Tue, 29 Mar 2022 07:41:41 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:77fcf2c0cc10658b5d6b4e43a75682b8bebbdc2e47895412dd1241c0422b8368`  
		Last Modified: Tue, 29 Mar 2022 00:18:56 GMT  
		Size: 2.8 MB (2814846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02339d74c6ee81495a0e118ded4e0419f26ccf80513936bca81454dcccb4a9ef`  
		Last Modified: Tue, 29 Mar 2022 07:42:43 GMT  
		Size: 9.6 MB (9632820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a2e134a3a26a9a610f884b36fc8c7c4515c3f8a6e496e0b30c88fe5bc2334d`  
		Last Modified: Tue, 29 Mar 2022 07:42:41 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b666408c25fa0d0d140d842ae855c147d353f9dfec2689327143be5d97c77a34`  
		Last Modified: Tue, 29 Mar 2022 07:42:42 GMT  
		Size: 6.5 MB (6492208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:a1996310e95fe58903b86881db102fc711c686616d690e464a1201242c01da6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18854963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bd0c6b0836f9d3340e3865bed234d2efe13b8dd8a243f3a3d4eb695106c636f`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:45 GMT
ADD file:08b65c73088f2cc387829e0ce9aa160db404a3e5fa0e4fda048cdbc02d8f64c2 in / 
# Tue, 29 Mar 2022 00:41:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 15:59:07 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 29 Mar 2022 15:59:08 GMT
ENV HOME=/home/user
# Tue, 29 Mar 2022 15:59:08 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 29 Mar 2022 15:59:08 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 15:59:08 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 29 Mar 2022 15:59:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 29 Mar 2022 15:59:44 GMT
WORKDIR /home/user
# Tue, 29 Mar 2022 15:59:44 GMT
USER user
# Tue, 29 Mar 2022 15:59:44 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:89a2ea5c1a3e1d541ae66fbd95d215b39b560c537460c3fc76ad6826582893fe`  
		Last Modified: Tue, 29 Mar 2022 00:47:35 GMT  
		Size: 2.6 MB (2605074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1a5a4806a9221ab47409adcf5e27285f18845563e348e4bff66f36a4ec7727`  
		Last Modified: Tue, 29 Mar 2022 16:03:04 GMT  
		Size: 10.0 MB (9971979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ef67480f26d7536af4b650290ddd1955b0ef1afd6b33b3cdb1fcf4f4756f42`  
		Last Modified: Tue, 29 Mar 2022 16:03:04 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cffa0c352647c43ea9c6e7c65920a410f592c9417d32b6fba1f0bad1646fc40e`  
		Last Modified: Tue, 29 Mar 2022 16:03:05 GMT  
		Size: 6.3 MB (6276640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
