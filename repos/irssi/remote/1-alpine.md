## `irssi:1-alpine`

```console
$ docker pull irssi@sha256:554d2243f8a34d09fa6a15bf3304eba7030550de34bdfa653b497cd752f287ba
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
$ docker pull irssi@sha256:df33162f0e50c52c10cbc95a42f1cb42a89705f6c83ffd7afd7cbec9443a8f8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18276585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f1af4d2f8b92472032db235e289cb9962144969514aff20659771cbd821edea`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 05:44:22 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 15 Jun 2023 05:44:22 GMT
ENV HOME=/home/user
# Thu, 15 Jun 2023 05:44:23 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 15 Jun 2023 05:44:23 GMT
ENV LANG=C.UTF-8
# Thu, 15 Jun 2023 05:44:23 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 15 Jun 2023 05:44:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 15 Jun 2023 05:44:42 GMT
WORKDIR /home/user
# Thu, 15 Jun 2023 05:44:42 GMT
USER user
# Thu, 15 Jun 2023 05:44:42 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16db5ccbd16300cfe3a0c9f34b1f542069afdc21f717b410fae474a86e85c61f`  
		Last Modified: Thu, 15 Jun 2023 05:44:58 GMT  
		Size: 9.7 MB (9730952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d12740aa5ddf98127801ec314bbae032c68524b23c82d8e1e35a4a1ee5343e7`  
		Last Modified: Thu, 15 Jun 2023 05:44:57 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87af7c88801970c57df2d16564333d097ce75a779c2f1d3efe0b0a4a6683bb96`  
		Last Modified: Thu, 15 Jun 2023 05:44:58 GMT  
		Size: 5.2 MB (5169637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:bb597fb239a0bd0ab274a3954a976e7a8bd496662eeb66a9ea540606d3d8de35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17261761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcd756feb5566228922fc9f7d0e3904d76d421749b294dd3a4643d1c7274f5c7`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 00:58:29 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 00:58:31 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:58:32 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:58:32 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:58:32 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:58:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 00:58:52 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:58:52 GMT
USER user
# Thu, 22 Jun 2023 00:58:52 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da40b022b0296d6aa3db9bdeeb4c2e75c57f15429e1b6af2b7027548372ca8b`  
		Last Modified: Thu, 22 Jun 2023 00:59:06 GMT  
		Size: 8.9 MB (8873416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b96767a0ecd78f7941b675b0af4b50cbecb0d5152dab111a5a441594ae6603`  
		Last Modified: Thu, 22 Jun 2023 00:59:03 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b501eb48ba4f12d62b8aea88131359fb8f39cb356fac11d0259549db8e77d8`  
		Last Modified: Thu, 22 Jun 2023 00:59:04 GMT  
		Size: 5.2 MB (5243707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:0b986f46e3300def597e471838a101aa352def1ae0b5f7f9f42c97dfbd11b83b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16562586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1d80e6235adbd2367ceeee4bb15c7b1e544f7a8e7fee19f67d6676360de3ebd`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:20 GMT
ADD file:5e92075a8d9a5898d661caf9c2be8a83fb25742251b4ebdc0c3d448a6dc58e4a in / 
# Wed, 14 Jun 2023 22:36:20 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 02:36:44 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 15 Jun 2023 02:36:44 GMT
ENV HOME=/home/user
# Thu, 15 Jun 2023 02:36:44 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 15 Jun 2023 02:36:45 GMT
ENV LANG=C.UTF-8
# Thu, 15 Jun 2023 02:36:45 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 15 Jun 2023 02:37:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 15 Jun 2023 02:37:02 GMT
WORKDIR /home/user
# Thu, 15 Jun 2023 02:37:03 GMT
USER user
# Thu, 15 Jun 2023 02:37:03 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f929d112168394cf1fbe294a86fbe5173dd92df4daac8cb09437b17dfc5df802`  
		Last Modified: Wed, 14 Jun 2023 22:37:01 GMT  
		Size: 2.9 MB (2868554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19564852001304e25333fcaab3ff6b786fa9b4fd00951a0de7f21590421663c0`  
		Last Modified: Thu, 15 Jun 2023 02:37:17 GMT  
		Size: 8.9 MB (8862221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e9266e16eb957d32cfe744ce2a3e2816dcf23785557fc6f7a16823a7ca1555`  
		Last Modified: Thu, 15 Jun 2023 02:37:14 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7eca2cc340821a140c2b4125d47f2e4ede76abc67c397ae6956bd9f4fcab86`  
		Last Modified: Thu, 15 Jun 2023 02:37:15 GMT  
		Size: 4.8 MB (4830526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:22b4938b5405529664397a96505be6a0a68216bc5e4dfd1a21212650e8767e73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18305951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f25464e2094646ab0d15f3b07d9f086640cf1fe1514bbde35957288c200e8ce`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:00:36 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:00:36 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:00:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:00:37 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:00:37 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:00:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:00:49 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:00:49 GMT
USER user
# Thu, 22 Jun 2023 01:00:49 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f2b2cec23be63b100192d36d65457ca5a26f7eea16d8e43ade7f2a71b93ae6`  
		Last Modified: Thu, 22 Jun 2023 01:01:31 GMT  
		Size: 9.7 MB (9666778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f96463864962e4e3fb7c345cfbcf0bec7c4339f64ac2033fdc156dad9ef918`  
		Last Modified: Thu, 22 Jun 2023 01:01:29 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795ebb03672fc4e273a972202f51cdb3b57a46535e2e027c0ec705d277af2c6e`  
		Last Modified: Thu, 22 Jun 2023 01:01:30 GMT  
		Size: 5.3 MB (5308640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; 386

```console
$ docker pull irssi@sha256:fddae328f37731c13d5bf17a3946f5cd460fa8a1877b2c4eefcd83b0dd7b543a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.5 MB (17544572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b0dbc2e51d5bf9a3b7bd5cd8d2f1e40fa598f375d7750df018959bc790c1eb5`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:22 GMT
ADD file:94bec00e2c0c7f47c81ec4355a29ca23a81b439797d037b1a5a455f36a25dab4 in / 
# Wed, 14 Jun 2023 22:33:22 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 00:53:45 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 00:53:45 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 00:53:46 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 00:53:46 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 00:53:46 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 00:54:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 00:54:19 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 00:54:19 GMT
USER user
# Thu, 22 Jun 2023 00:54:19 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:b3f50075abd13aad1cb7d8c1427aa59d7fcac88f3690d3f9c3efdbec80fd0856`  
		Last Modified: Wed, 14 Jun 2023 22:33:48 GMT  
		Size: 3.2 MB (3233951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af01bb2560a285c7c3f49f618c91cddeddaae06f68de1d63318a35d08ddd335`  
		Last Modified: Thu, 22 Jun 2023 00:55:14 GMT  
		Size: 8.9 MB (8896518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400b4f5222097fceb2802b1b4c86df1e17d9c756033d35b1bbe932496bb67d55`  
		Last Modified: Thu, 22 Jun 2023 00:55:11 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4f83428ff29063f3abf5ecdcdade0657f4c35089baf0e5a17abf0284dde4e9`  
		Last Modified: Thu, 22 Jun 2023 00:55:13 GMT  
		Size: 5.4 MB (5412820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:edbac3bc69ae83f6a98c2aad44f19c80a109631cb22bd3fa7f0c500242c62faf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18484325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e94c29de632503a0823c113d66340f5bc25c0af8ef7e8bff75880144aa1c2f0`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:56 GMT
ADD file:1c25b0be52aae22767603d9404fb777e27c5dd1bcd627221aac7517ac1bce1e3 in / 
# Thu, 15 Jun 2023 00:39:57 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 02:12:08 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 15 Jun 2023 02:12:09 GMT
ENV HOME=/home/user
# Thu, 15 Jun 2023 02:12:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 15 Jun 2023 02:12:10 GMT
ENV LANG=C.UTF-8
# Thu, 15 Jun 2023 02:12:11 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 15 Jun 2023 02:12:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 15 Jun 2023 02:12:35 GMT
WORKDIR /home/user
# Thu, 15 Jun 2023 02:12:35 GMT
USER user
# Thu, 15 Jun 2023 02:12:35 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8436307590cda5ccded8a952bb1d66684f8700d07029527293dd695eac6fabc9`  
		Last Modified: Thu, 15 Jun 2023 00:40:39 GMT  
		Size: 3.4 MB (3389905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864111a1d0261ae544596480b7c499eeaf06cbbe1bc28790c10c4f7c970266cc`  
		Last Modified: Thu, 15 Jun 2023 02:12:54 GMT  
		Size: 9.8 MB (9819563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0ad87a302112668f0b2d1aa81c90fea805716562d224e498f265e8fbc40ed9`  
		Last Modified: Thu, 15 Jun 2023 02:12:51 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc50b4b50b6a0ce01de8d1e1e0c6e619054efd5e6110152ccb85f0d07e940776`  
		Last Modified: Thu, 15 Jun 2023 02:12:52 GMT  
		Size: 5.3 MB (5273573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:dbf8a6d36f09f574725d7cc6f6284a867c447eb0ca83eb1cc60b6f88c1cc23c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18463228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ac2b28856e91692db99f7d4ddc3224676a32846026bfd08d2ee7c118a4f36f9`
-	Default Command: `["irssi"]`

```dockerfile
# Thu, 15 Jun 2023 05:19:50 GMT
ADD file:8ad8a62cf274ba5a6568f68473359114136cb5c7704bfdfce6c38efef3081782 in / 
# Thu, 15 Jun 2023 05:19:51 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 07:28:51 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 16 Jun 2023 07:28:52 GMT
ENV HOME=/home/user
# Fri, 16 Jun 2023 07:28:53 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 16 Jun 2023 07:28:54 GMT
ENV LANG=C.UTF-8
# Fri, 16 Jun 2023 07:28:54 GMT
ENV IRSSI_VERSION=1.4.4
# Fri, 16 Jun 2023 07:29:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 16 Jun 2023 07:29:18 GMT
WORKDIR /home/user
# Fri, 16 Jun 2023 07:29:18 GMT
USER user
# Fri, 16 Jun 2023 07:29:18 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:eb857838eb854a669f87c5df4d936d905fb3129287a93ef485da9454c11d83cd`  
		Last Modified: Thu, 15 Jun 2023 05:30:48 GMT  
		Size: 3.2 MB (3174898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7aaa04f45ef848c1c2f0c93b981862cc5a7e75fa94769dc25fa6e6c90124bb7`  
		Last Modified: Fri, 16 Jun 2023 07:33:42 GMT  
		Size: 10.2 MB (10161596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5466510fd4b694305a4d3e46080afb8ed895bded299c98d7284313b5de554715`  
		Last Modified: Fri, 16 Jun 2023 07:33:40 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd30109dad033bd844acba0eb497941214a16aadd9b6dd7d208ec1550930aaca`  
		Last Modified: Fri, 16 Jun 2023 07:33:41 GMT  
		Size: 5.1 MB (5125449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
