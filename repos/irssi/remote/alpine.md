## `irssi:alpine`

```console
$ docker pull irssi@sha256:d79e47f5ec9ace6fdb92508b5b06bef131e715d504caf1bef6d56b0908210622
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
$ docker pull irssi@sha256:a768693cbea894b7b6135922520f7d532a6245dff8a3863024244a8ef9ffb14e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18439974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6be6e0e30722062f7d0e647c925e5239badb1739c57c83238d83b8a422b169fe`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 22 Jun 2023 01:28:06 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Thu, 22 Jun 2023 01:28:06 GMT
ENV HOME=/home/user
# Thu, 22 Jun 2023 01:28:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Thu, 22 Jun 2023 01:28:07 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jun 2023 01:28:07 GMT
ENV IRSSI_VERSION=1.4.4
# Thu, 22 Jun 2023 01:28:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Thu, 22 Jun 2023 01:28:26 GMT
WORKDIR /home/user
# Thu, 22 Jun 2023 01:28:26 GMT
USER user
# Thu, 22 Jun 2023 01:28:26 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdb311d04d5ef03d3a3d6136863478ca52e56c787391712823006f36d8d5b9e`  
		Last Modified: Thu, 22 Jun 2023 01:29:12 GMT  
		Size: 9.6 MB (9637888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c8f7b98870f87f73429e0fb3e302a979d79d0c313dc49f64bd4b6d52763c08`  
		Last Modified: Thu, 22 Jun 2023 01:29:10 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3e36b711d362f59b8801dbb9ce1a3ec3bcaa5edd5b2366634e350cf308faee`  
		Last Modified: Thu, 22 Jun 2023 01:29:11 GMT  
		Size: 5.4 MB (5402922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v6

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

### `irssi:alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:39b31754b9607eb4e40ba490b5ae796dc050555cd971df5f147971f98bec2c2e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16622956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57a425c83559c38fd9ea04fed3dac60c590bf233aea6eafce96946682652757b`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:18:32 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 08 Aug 2023 01:18:32 GMT
ENV HOME=/home/user
# Tue, 08 Aug 2023 01:18:32 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 08 Aug 2023 01:18:32 GMT
ENV LANG=C.UTF-8
# Tue, 08 Aug 2023 01:18:32 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 08 Aug 2023 01:18:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 08 Aug 2023 01:18:49 GMT
WORKDIR /home/user
# Tue, 08 Aug 2023 01:18:49 GMT
USER user
# Tue, 08 Aug 2023 01:18:49 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50072b4c9927347770448dba84676c4165e9810f8c7e8d5167049698e97e379e`  
		Last Modified: Tue, 08 Aug 2023 01:19:13 GMT  
		Size: 8.7 MB (8713691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c42151aa91c6c6334c01ecae667b1b758cb1729f97bda99ed99a4902ff2180e`  
		Last Modified: Tue, 08 Aug 2023 01:19:11 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca598d51edc21ae9f5780c6d6bbea24c6805c906019921d7cca80767ba4342f`  
		Last Modified: Tue, 08 Aug 2023 01:19:12 GMT  
		Size: 5.0 MB (5008501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm64 variant v8

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

### `irssi:alpine` - linux; 386

```console
$ docker pull irssi@sha256:0db563ef1d4943e099d9b94c6d3a5373f9d609015588878e7ef5a534f6f7892e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.5 MB (17545633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9685d5c50bd27f896c7a71a716392d71c14abdd0b147821f10d6b43b460f82fa`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:26 GMT
ADD file:4b33c52e11b19fde30197c62ead0b77bde28d34edaa08346a5302cd892d3cebe in / 
# Mon, 07 Aug 2023 19:38:27 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:44:50 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Mon, 07 Aug 2023 21:44:50 GMT
ENV HOME=/home/user
# Mon, 07 Aug 2023 21:44:50 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 07 Aug 2023 21:44:50 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 21:44:50 GMT
ENV IRSSI_VERSION=1.4.4
# Mon, 07 Aug 2023 21:45:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Mon, 07 Aug 2023 21:45:24 GMT
WORKDIR /home/user
# Mon, 07 Aug 2023 21:45:24 GMT
USER user
# Mon, 07 Aug 2023 21:45:24 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:95dc695758361a4038a2d9026959d72e1f531114edb0341be7ce47d912ef069e`  
		Last Modified: Mon, 07 Aug 2023 19:38:56 GMT  
		Size: 3.2 MB (3235144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046b2528594cd9fc777d0153d709fb2809d8b44f8c99420ff232919922d33053`  
		Last Modified: Mon, 07 Aug 2023 21:45:51 GMT  
		Size: 8.9 MB (8896294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b9a58d32089d32752297064b4653251abf366ea9158a7abc0b90b15ceee675`  
		Last Modified: Mon, 07 Aug 2023 21:45:48 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca72c81c6201ee5c211d024845b1b6f7075f4e89132dfb205d68e8a03c277947`  
		Last Modified: Mon, 07 Aug 2023 21:45:50 GMT  
		Size: 5.4 MB (5412910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:f8e8ee83d966507b0fea53462b618401b83daf7f523ddfcbf02ecab0daa79d33
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18706016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6c95884f1cff2c5b774e56fc9ef56bdb289893205f4b7095309f0875c1dfd97`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:04:07 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 08 Aug 2023 01:04:10 GMT
ENV HOME=/home/user
# Tue, 08 Aug 2023 01:04:13 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 08 Aug 2023 01:04:13 GMT
ENV LANG=C.UTF-8
# Tue, 08 Aug 2023 01:04:14 GMT
ENV IRSSI_VERSION=1.4.4
# Tue, 08 Aug 2023 01:04:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 08 Aug 2023 01:04:40 GMT
WORKDIR /home/user
# Tue, 08 Aug 2023 01:04:42 GMT
USER user
# Tue, 08 Aug 2023 01:04:44 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03fb6d6b3d88160311a208a89abce6a55248b5806df64524162295110f7fe85`  
		Last Modified: Tue, 08 Aug 2023 01:05:26 GMT  
		Size: 9.7 MB (9726946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90dd339118965df2c5c58f96440da6daf2ca178448b019c2646e1aa6c618ea2b`  
		Last Modified: Tue, 08 Aug 2023 01:05:23 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8adb7c2a30ee10ee6d4ba10643644281a19908dee300bbeeb1683620eee9396f`  
		Last Modified: Tue, 08 Aug 2023 01:05:24 GMT  
		Size: 5.6 MB (5631536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; s390x

```console
$ docker pull irssi@sha256:18a16ccf400d1703510731058f8fa96ac4e12fc2f3a69182ba0992e8aac09772
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18701981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:974c8c6125900610e54c7c70bfc633a88d8f6ab68d95460cee662e84b3742ff0`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:34:00 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Mon, 07 Aug 2023 20:34:02 GMT
ENV HOME=/home/user
# Mon, 07 Aug 2023 20:34:03 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 07 Aug 2023 20:34:04 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 20:34:04 GMT
ENV IRSSI_VERSION=1.4.4
# Mon, 07 Aug 2023 20:34:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Mon, 07 Aug 2023 20:34:25 GMT
WORKDIR /home/user
# Mon, 07 Aug 2023 20:34:25 GMT
USER user
# Mon, 07 Aug 2023 20:34:25 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac529dad188f0aa87b371b0436c2c5069d189ea8aa8a91cff51a6d65f6345af7`  
		Last Modified: Mon, 07 Aug 2023 20:34:55 GMT  
		Size: 10.1 MB (10078915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5671f425cf9f2932a941fdd2470f63eecc9f4838ef35aa0eeecc96fc1c7a7ddc`  
		Last Modified: Mon, 07 Aug 2023 20:34:53 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d6fcd32d935e7ccc5e845731384b2f627fbc1db6521e0146b91d0193536067`  
		Last Modified: Mon, 07 Aug 2023 20:34:54 GMT  
		Size: 5.4 MB (5407590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
