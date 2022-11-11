## `irssi:alpine`

```console
$ docker pull irssi@sha256:fdd0045fd18a27adb30b80e7ba4e7dea2a12e3778d2e52023cb5be3d8f170fd4
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
$ docker pull irssi@sha256:a138fb7c5a7f29b97595c3d1931ed165b004eb1ed20071f2216568b9516063c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.5 MB (17471136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e788de2b86e371837a5e85fe4b38024c00678c723a9fb4310529c309ff1d4c32`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:46:20 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 06 Oct 2022 22:46:20 GMT
ENV HOME=/home/user
# Thu, 06 Oct 2022 22:46:21 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 06 Oct 2022 22:46:21 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2022 19:28:01 GMT
ENV IRSSI_VERSION=1.4.3
# Mon, 31 Oct 2022 19:28:23 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Mon, 31 Oct 2022 19:28:23 GMT
WORKDIR /home/user
# Mon, 31 Oct 2022 19:28:23 GMT
USER user
# Mon, 31 Oct 2022 19:28:23 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ff79af72bb12b49e71f6508ebe4aa9b7ba12e5c1c2037f0953067fcc50546d`  
		Last Modified: Thu, 06 Oct 2022 22:47:00 GMT  
		Size: 9.6 MB (9641364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11abf0b311aa35dce58e3aa729ed8b52ce47c211c776e639f37cd3e2ed7f41fd`  
		Last Modified: Thu, 06 Oct 2022 22:46:58 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a698d457dc10eb85ac57f79cf84d647959077776acd831b726973ad89b84b281`  
		Last Modified: Mon, 31 Oct 2022 19:28:56 GMT  
		Size: 5.0 MB (5022433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:3adb1e997d9b65f77ceadb19caa835b3af51d776d8db5abd354638ea1e5e21e9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.2 MB (18155327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1191e396b61b85d7d0604bf114237601f7e9bf0d4bdfc8328980d6dde8912a05`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:27 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Thu, 10 Nov 2022 20:49:27 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:32:58 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 11 Nov 2022 11:32:59 GMT
ENV HOME=/home/user
# Fri, 11 Nov 2022 11:32:59 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 11 Nov 2022 11:32:59 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 11:32:59 GMT
ENV IRSSI_VERSION=1.4.3
# Fri, 11 Nov 2022 11:33:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 11 Nov 2022 11:33:22 GMT
WORKDIR /home/user
# Fri, 11 Nov 2022 11:33:22 GMT
USER user
# Fri, 11 Nov 2022 11:33:22 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dcd422b1dd2a9f8903d61dd4b28b255e969215bd843ea9cb5308963b201a702`  
		Last Modified: Fri, 11 Nov 2022 11:33:45 GMT  
		Size: 8.9 MB (8871291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114dfbd980f9b6609bba2107bde04425b26c011a020532b14ad30bdef842fc6c`  
		Last Modified: Fri, 11 Nov 2022 11:33:43 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d76d844c3b4121cdd1e9eb1cba56469260400c96de85eeed616143a08186c9a`  
		Last Modified: Fri, 11 Nov 2022 11:33:44 GMT  
		Size: 6.7 MB (6668812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:1e9d8f43d619176d165ecfafd68db660bccf680f9b42538fca214a02f4e2d5eb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.5 MB (17482576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:833f4e8ce5872cf55c1fef2252e0c7e3354838d4bb0d7aa18090e97e16c27e24`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 10 Nov 2022 19:57:31 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Thu, 10 Nov 2022 19:57:31 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 07:03:28 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 11 Nov 2022 07:03:29 GMT
ENV HOME=/home/user
# Fri, 11 Nov 2022 07:03:29 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 11 Nov 2022 07:03:29 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 07:03:29 GMT
ENV IRSSI_VERSION=1.4.3
# Fri, 11 Nov 2022 07:03:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 11 Nov 2022 07:03:49 GMT
WORKDIR /home/user
# Fri, 11 Nov 2022 07:03:49 GMT
USER user
# Fri, 11 Nov 2022 07:03:49 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6893d7c7fa8053022c2fceb23fcf9e129d250d28c3bf0d9fb84a55aa8f4b5074`  
		Last Modified: Fri, 11 Nov 2022 07:04:26 GMT  
		Size: 8.7 MB (8718339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7a3b50c98ab8b0569f8d61a613bd4911a41da7e778a450476962ac8cf007b5`  
		Last Modified: Fri, 11 Nov 2022 07:04:24 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6728981a0b1e37450b86628b724055fd62bbfc54bbeba81218c6d2c88d52eb`  
		Last Modified: Fri, 11 Nov 2022 07:04:25 GMT  
		Size: 6.3 MB (6345912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:0a3995c5d6da11692151b211500ab9a0f8849bce9b2949f176a76598972a2107
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.1 MB (19121465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df690d3b92a469a8d30921af1d7aa578138a2d885829ba157875904b34a35f02`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Thu, 10 Nov 2022 20:39:41 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:44:20 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 10 Nov 2022 21:44:20 GMT
ENV HOME=/home/user
# Thu, 10 Nov 2022 21:44:21 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 10 Nov 2022 21:44:21 GMT
ENV LANG=C.UTF-8
# Thu, 10 Nov 2022 21:44:21 GMT
ENV IRSSI_VERSION=1.4.3
# Thu, 10 Nov 2022 21:44:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 10 Nov 2022 21:44:35 GMT
WORKDIR /home/user
# Thu, 10 Nov 2022 21:44:35 GMT
USER user
# Thu, 10 Nov 2022 21:44:35 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2507a840456a8ee30e0beabc3e0fd3340b042b0e078d3a8ec51cd66d03c4ae66`  
		Last Modified: Thu, 10 Nov 2022 21:44:55 GMT  
		Size: 9.6 MB (9623582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28552c93fd99f72724a9ee9c771082127246b2eb389069b484444fcdc8ebbfa2`  
		Last Modified: Thu, 10 Nov 2022 21:44:54 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be69c0427773c855e3c10bc29efec558598d8d4a51390f0881bcf3506b947b05`  
		Last Modified: Thu, 10 Nov 2022 21:44:54 GMT  
		Size: 6.8 MB (6788935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; 386

```console
$ docker pull irssi@sha256:1c3f0f7f74a1c7a2d3f058cee1bd0ed3c3c8f10ab1b24951e9444e59c937ca48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16911093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb6c61e02f929ef713e587b403d9af3c3b707e569aebbc22ac932f9f818e6026`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:29:42 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 06 Oct 2022 20:29:43 GMT
ENV HOME=/home/user
# Thu, 06 Oct 2022 20:29:44 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 06 Oct 2022 20:29:45 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2022 19:39:22 GMT
ENV IRSSI_VERSION=1.4.3
# Mon, 31 Oct 2022 19:39:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Mon, 31 Oct 2022 19:39:44 GMT
WORKDIR /home/user
# Mon, 31 Oct 2022 19:39:45 GMT
USER user
# Mon, 31 Oct 2022 19:39:46 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6998e76f864cbaf06e7debbc8cc223f98c373cb95b806cfe44aca74812c27568`  
		Last Modified: Thu, 06 Oct 2022 20:30:40 GMT  
		Size: 9.0 MB (9003050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3b2d0f1f5305fc69e974d644c6d4eb9805269f1617bdb0f4f866bcce3d175e`  
		Last Modified: Thu, 06 Oct 2022 20:30:39 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c0fac54e9da775128723c744e0d0e07a343ff9c89bb65dc8252eea11653564`  
		Last Modified: Mon, 31 Oct 2022 19:40:32 GMT  
		Size: 5.1 MB (5099662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:b8b2258ad46e6d455f06ea782ef633955c475e40e5243dbc954fb36d1ac27c62
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17654198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:542ce2bd2661d46105c20fddf8d81bb4beb44cff11ef8b3a8fad51ad2605969c`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:56:59 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 06 Oct 2022 20:57:01 GMT
ENV HOME=/home/user
# Thu, 06 Oct 2022 20:57:02 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 06 Oct 2022 20:57:02 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2022 19:18:30 GMT
ENV IRSSI_VERSION=1.4.3
# Mon, 31 Oct 2022 19:18:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Mon, 31 Oct 2022 19:18:56 GMT
WORKDIR /home/user
# Mon, 31 Oct 2022 19:18:56 GMT
USER user
# Mon, 31 Oct 2022 19:18:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e828760c7aed6b7ea142e4ddd204ad174b2c95d098e2633076001bfdaae94b05`  
		Last Modified: Thu, 06 Oct 2022 20:58:03 GMT  
		Size: 9.7 MB (9733821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afdbf73ae465e0b650b562e211dd0d81f1f48adebf51b97ff74087f6f76b85a`  
		Last Modified: Thu, 06 Oct 2022 20:58:00 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fbe67a8e3876ac0b972adfbfb45bd688860cc0f5d7933249c0352e4c00f9342`  
		Last Modified: Mon, 31 Oct 2022 19:19:47 GMT  
		Size: 5.1 MB (5115770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; s390x

```console
$ docker pull irssi@sha256:213205b9d0ee13924d79ec6230a15b00cfc0c929a6f2a350ed04ebc6aa54d4d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17701330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15726a95fb8e6fe8e915f885271192207483bb6960ccd07020dcb9f58cc92596`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:43:49 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 06 Oct 2022 20:43:52 GMT
ENV HOME=/home/user
# Thu, 06 Oct 2022 20:43:53 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 06 Oct 2022 20:43:54 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2022 19:42:52 GMT
ENV IRSSI_VERSION=1.4.3
# Mon, 31 Oct 2022 19:43:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Mon, 31 Oct 2022 19:43:14 GMT
WORKDIR /home/user
# Mon, 31 Oct 2022 19:43:14 GMT
USER user
# Mon, 31 Oct 2022 19:43:14 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2430a4cf39192531130610f08c2327bb9edca6b0c252c358f0c3104c4c334e`  
		Last Modified: Thu, 06 Oct 2022 20:44:57 GMT  
		Size: 10.1 MB (10078985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a949d247b8ba59f1b64589832f6a3f50f78334cf88303f86704b6f0934e613c2`  
		Last Modified: Thu, 06 Oct 2022 20:44:56 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f3c9e1401ad4c79d6ec6c95cc39844a4e25575dd579647dc206c9e5dfec751`  
		Last Modified: Mon, 31 Oct 2022 19:44:00 GMT  
		Size: 5.0 MB (5030462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
