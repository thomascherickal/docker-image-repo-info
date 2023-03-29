## `irssi:1-alpine`

```console
$ docker pull irssi@sha256:b0c054f7f3218865e6b15df4a3797932e2c99f675c2fb82ff34f11b9b5d48e6e
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
$ docker pull irssi@sha256:1f2e5d245ed112f9e7cf9eda27a373f8e78d7ecd1016db7052933246806e8858
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.5 MB (17472866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de3b5216db23e966343a70e9dd1da1b5a8b118d6a09e50d117078603fbcc43ce`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 09:49:46 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 11 Feb 2023 09:49:46 GMT
ENV HOME=/home/user
# Sat, 11 Feb 2023 09:49:47 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 11 Feb 2023 09:49:47 GMT
ENV LANG=C.UTF-8
# Sat, 11 Feb 2023 09:49:47 GMT
ENV IRSSI_VERSION=1.4.3
# Sat, 11 Feb 2023 09:50:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 11 Feb 2023 09:50:08 GMT
WORKDIR /home/user
# Sat, 11 Feb 2023 09:50:08 GMT
USER user
# Sat, 11 Feb 2023 09:50:08 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc72a698bd939a0cee17ad6c98aa3d61530f30a966505073522b09f9d64dfc0`  
		Last Modified: Sat, 11 Feb 2023 09:50:25 GMT  
		Size: 9.6 MB (9641412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa8e046f24538449d3c85ada3fa85c849e055140096fe45c5a19fddb52a40cf`  
		Last Modified: Sat, 11 Feb 2023 09:50:24 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e948eb29d0c0ba780cb5c326b6c08c7fb39bcf620aa14af901acecad187db051`  
		Last Modified: Sat, 11 Feb 2023 09:50:24 GMT  
		Size: 5.0 MB (5022411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:925ee068ce2c9b212e36b9477395d145047c067552d35861109eb89b9284e2b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16404140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:895a57772a83ae27eb19357bd4c9c30e727e3cffc0632b7f3077f53208400737`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:48 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Mon, 13 Mar 2023 16:12:48 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 17:17:33 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Mon, 13 Mar 2023 17:17:34 GMT
ENV HOME=/home/user
# Mon, 13 Mar 2023 17:17:34 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Mon, 13 Mar 2023 17:17:34 GMT
ENV LANG=C.UTF-8
# Mon, 13 Mar 2023 17:17:34 GMT
ENV IRSSI_VERSION=1.4.3
# Mon, 13 Mar 2023 17:17:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Mon, 13 Mar 2023 17:17:58 GMT
WORKDIR /home/user
# Mon, 13 Mar 2023 17:17:58 GMT
USER user
# Mon, 13 Mar 2023 17:17:58 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26614f723700669e4808149e3e900f24d13d4e624e393a6c55f38b3dce9d190`  
		Last Modified: Mon, 13 Mar 2023 17:18:15 GMT  
		Size: 8.9 MB (8871533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb416bbbea2b95b3c23cba45986fac13281c1e14f611b9dd31b0645d7816771`  
		Last Modified: Mon, 13 Mar 2023 17:18:13 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0344e20c93f7bab3d30c3cfd697c40955d0b84cf4fba6554e193bba0f2b3260f`  
		Last Modified: Mon, 13 Mar 2023 17:18:14 GMT  
		Size: 4.9 MB (4914544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:7d9652df0ae62079d75c7c25f460e7a5478b39d92e245f36a40684865616fd5a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.8 MB (15833363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5e92bcbf5d4f53c6d4faac9335c4cb8e66b2ef6f3c15f85d15e584fc317a3de`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:37 GMT
ADD file:193f48d48ed2e90a0e81663757e372f59806151c17e82113f03443db0ef723c3 in / 
# Fri, 10 Feb 2023 21:51:37 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 05:25:48 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 01 Mar 2023 05:25:48 GMT
ENV HOME=/home/user
# Wed, 01 Mar 2023 05:25:49 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 01 Mar 2023 05:25:49 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 05:25:49 GMT
ENV IRSSI_VERSION=1.4.3
# Wed, 01 Mar 2023 05:26:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 01 Mar 2023 05:26:07 GMT
WORKDIR /home/user
# Wed, 01 Mar 2023 05:26:07 GMT
USER user
# Wed, 01 Mar 2023 05:26:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:beefe5ad637c7db32e6afc68103fc4e779630219979216a625338ab55f7d191c`  
		Last Modified: Fri, 10 Feb 2023 21:52:51 GMT  
		Size: 2.4 MB (2420494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433b18ac14bacd30fc0bde644f88e245f227470c02ef28cb6f6b8dd14549b27f`  
		Last Modified: Wed, 01 Mar 2023 05:26:56 GMT  
		Size: 8.7 MB (8718352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3831e824f2104378fa24e527af0e31e144068115042a9bde3123c9026735d8d`  
		Last Modified: Wed, 01 Mar 2023 05:26:53 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c679aa491cc63df960a2a96c7f8b5171391f77022e5a417dea2d7277be5a9ea`  
		Last Modified: Wed, 01 Mar 2023 05:26:54 GMT  
		Size: 4.7 MB (4693233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:1b68bede90f6efbc2e3c8ea83c01bf430a01f02a2a8da57eeca60fac4e09d7c4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17241785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3a65804f9281d256c915fe07274fdaeae288a160f85fa1c777877140c4ea635`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:56:30 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Fri, 10 Feb 2023 22:56:31 GMT
ENV HOME=/home/user
# Fri, 10 Feb 2023 22:56:31 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Fri, 10 Feb 2023 22:56:31 GMT
ENV LANG=C.UTF-8
# Fri, 10 Feb 2023 22:56:31 GMT
ENV IRSSI_VERSION=1.4.3
# Fri, 10 Feb 2023 22:56:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Fri, 10 Feb 2023 22:56:46 GMT
WORKDIR /home/user
# Fri, 10 Feb 2023 22:56:46 GMT
USER user
# Fri, 10 Feb 2023 22:56:46 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6a5ee17fad7e8c8a634267b69a942d3a19ebba84071f2803acb14b7e3a72f7`  
		Last Modified: Fri, 10 Feb 2023 22:57:06 GMT  
		Size: 9.6 MB (9623579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c418e10d63094551a62b962b5d1e683af92c2a90d9c8450ab60b63d869deebf`  
		Last Modified: Fri, 10 Feb 2023 22:57:04 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98dc66c46e3d202d30aec1adda56847ccd4cecbdaae7fc34b614ebb974b24e9`  
		Last Modified: Fri, 10 Feb 2023 22:57:05 GMT  
		Size: 4.9 MB (4907420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; 386

```console
$ docker pull irssi@sha256:6b7fcb7f7729b2ca11dd7a413d56c4e654d9bfb32e4b0f79d4a30cb5bb7f8cde
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16916580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:033aaa478a0865467972e0c84205bb3445c956a038249984731f25e5ba63d24d`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:29 GMT
ADD file:59ac1f8f33f9b9727892b7e45b33f54ef3c20d9d876c49d6a4c057641821d68f in / 
# Fri, 10 Feb 2023 21:24:29 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 09:21:20 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 01 Mar 2023 09:21:21 GMT
ENV HOME=/home/user
# Wed, 01 Mar 2023 09:21:21 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 01 Mar 2023 09:21:21 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 09:21:21 GMT
ENV IRSSI_VERSION=1.4.3
# Wed, 01 Mar 2023 09:21:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 01 Mar 2023 09:22:00 GMT
WORKDIR /home/user
# Wed, 01 Mar 2023 09:22:00 GMT
USER user
# Wed, 01 Mar 2023 09:22:00 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:0987f51cd58a7d03bc7d6ff0a3a0a843c1a3fefcd41e3c8adc3999ddde7441e8`  
		Last Modified: Fri, 10 Feb 2023 21:25:30 GMT  
		Size: 2.8 MB (2810653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca098b9ff5a0825c92a00dd6926a396fa99564a770eafc93d7efc27703b568e`  
		Last Modified: Wed, 01 Mar 2023 09:22:46 GMT  
		Size: 9.0 MB (9004250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc46fc511d16b879963fcd2d93814a643c8d8952b990f3976f842ed0cb19c3e1`  
		Last Modified: Wed, 01 Mar 2023 09:22:43 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ea1732d6f502080cf9e4c4d34cee874e8caa54982a5d77864a14fe85079aa5`  
		Last Modified: Wed, 01 Mar 2023 09:22:44 GMT  
		Size: 5.1 MB (5100393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:774a540cd7e075160de20426df2ab512cb57005aa973ff0cac1d121489235453
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17655529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:879d0c98573bd337e5c9579b09447f399150be87a1ecbcf37c69a195424c4b13`
-	Default Command: `["irssi"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 09:42:09 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Sat, 11 Feb 2023 09:42:10 GMT
ENV HOME=/home/user
# Sat, 11 Feb 2023 09:42:11 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 11 Feb 2023 09:42:12 GMT
ENV LANG=C.UTF-8
# Sat, 11 Feb 2023 09:42:12 GMT
ENV IRSSI_VERSION=1.4.3
# Sat, 11 Feb 2023 09:42:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Sat, 11 Feb 2023 09:42:44 GMT
WORKDIR /home/user
# Sat, 11 Feb 2023 09:42:44 GMT
USER user
# Sat, 11 Feb 2023 09:42:45 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:075ed516071aa420377ceeb0ee81bdefb3bde1b250916036a14949718db13873`  
		Last Modified: Sat, 11 Feb 2023 09:43:21 GMT  
		Size: 9.7 MB (9733850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97e6240adb7b310b2543ea2abc50ee62c42fef4d67c9643713423661217c40e7`  
		Last Modified: Sat, 11 Feb 2023 09:43:18 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cd76bc3ede52db8a1e5198d81bd9f5a3e8155f08d92d7bc721d068c1afe413`  
		Last Modified: Sat, 11 Feb 2023 09:43:19 GMT  
		Size: 5.1 MB (5115770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:2e60e6e239481450d54db34d86510c666412f2707203f468e64352ffe3e9beea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17704051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43c9949e1344fe9af302ed763b04ad9d1fca84e80dd4f0b6455115f95461bd62`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:47:06 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Wed, 29 Mar 2023 18:47:07 GMT
ENV HOME=/home/user
# Wed, 29 Mar 2023 18:47:07 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 29 Mar 2023 18:47:07 GMT
ENV LANG=C.UTF-8
# Wed, 29 Mar 2023 18:47:07 GMT
ENV IRSSI_VERSION=1.4.3
# Wed, 29 Mar 2023 18:47:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Wed, 29 Mar 2023 18:47:29 GMT
WORKDIR /home/user
# Wed, 29 Mar 2023 18:47:30 GMT
USER user
# Wed, 29 Mar 2023 18:47:30 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:95cbbfdf0c760cbcde91603c8eee15ec60d4aa5f874b4a538babcd2df1709174`  
		Last Modified: Wed, 29 Mar 2023 17:42:37 GMT  
		Size: 2.6 MB (2593389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06c03195f7041f32a296c69af1282b626f998bc2dbefe179029374aba4b33a8e`  
		Last Modified: Wed, 29 Mar 2023 18:47:51 GMT  
		Size: 10.1 MB (10079011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144be28453822317c17c0cb1711ca490599a6e30f212d0c3aa3d8f59f45091f6`  
		Last Modified: Wed, 29 Mar 2023 18:47:49 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f976c958bb772c9bb3bb1e4c6c9d983ee4a8553b914ddf4985106426914139bb`  
		Last Modified: Wed, 29 Mar 2023 18:47:50 GMT  
		Size: 5.0 MB (5030367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
