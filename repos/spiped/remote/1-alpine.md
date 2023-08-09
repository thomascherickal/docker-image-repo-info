## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:9e0a090f395df640e73bdda9b2387d3fbadf14c6cb5d789c43f1da21368acb5c
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

### `spiped:1-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:49da7ccf4fd259700f2ac1db19a287d31a9ecf3a44e405470bf84179e4a151db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5057629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0439a8b1da8e9de36492d0a058f2acbdbfba92eb2bb87d48f767e0a31237098`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:03:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 09 Aug 2023 04:03:24 GMT
RUN apk add --no-cache libssl1.1
# Wed, 09 Aug 2023 04:03:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 09 Aug 2023 04:03:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 09 Aug 2023 04:03:34 GMT
VOLUME [/spiped]
# Wed, 09 Aug 2023 04:03:34 GMT
WORKDIR /spiped
# Wed, 09 Aug 2023 04:03:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 09 Aug 2023 04:03:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Aug 2023 04:03:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5158fd3e69013bf879861985939c5aac2cbc46278db264aeae05ee1344222b07`  
		Last Modified: Wed, 09 Aug 2023 04:03:47 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcfba2e005bb6d82f820494ca9e65f63ae7042f6d1e2b54a8c6784c76b725a9d`  
		Last Modified: Wed, 09 Aug 2023 04:03:47 GMT  
		Size: 1.4 MB (1433002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1118bcda9b744a84a9c764eadd2a58bd39cba589942a2f8f7c6489d77a0f2d9a`  
		Last Modified: Wed, 09 Aug 2023 04:03:47 GMT  
		Size: 221.3 KB (221274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76e498c240a7f12cb65ca8ed5d392aa245b449c370b5f77cc48781b7b0fe2e0`  
		Last Modified: Wed, 09 Aug 2023 04:03:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffd21f5dcda92cc1313530a1f07e075d96091d58e595b5ab77b810ff6b80125`  
		Last Modified: Wed, 09 Aug 2023 04:03:47 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:92c72514aab4032a46bd337535d95862b853d6c7e90cb1e86e689409cc93616f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4589191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93b3dd418f5fe3e7be9bbb2632a3fd0fbbedad7f67e01d907d0d41c06bb6ce98`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:36:07 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 08 Aug 2023 23:36:09 GMT
RUN apk add --no-cache libssl1.1
# Tue, 08 Aug 2023 23:36:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 08 Aug 2023 23:36:17 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 08 Aug 2023 23:36:17 GMT
VOLUME [/spiped]
# Tue, 08 Aug 2023 23:36:17 GMT
WORKDIR /spiped
# Tue, 08 Aug 2023 23:36:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 08 Aug 2023 23:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 23:36:18 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ffd38f9a9109fd6f2d98e59fac671a21acbcbd826d953a190916b8e28c4d7c`  
		Last Modified: Tue, 08 Aug 2023 23:36:25 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dafe31ddd32f93d6462563149d47e652289246cae76c3d69e2ae22c7f2dc157`  
		Last Modified: Tue, 08 Aug 2023 23:36:25 GMT  
		Size: 1.2 MB (1236777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711c8b1ac9af3a0357e5e2ae10175a62c27bdea58e2e79fb7d413e2fa3a10138`  
		Last Modified: Tue, 08 Aug 2023 23:36:25 GMT  
		Size: 205.9 KB (205868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d2f76630a196bedcec1d4f1f0542336e3189757e62aa7c83bd7f7e8f58680c`  
		Last Modified: Tue, 08 Aug 2023 23:36:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f674889b446c00cdd7da82689ee81ea78c84e02c462ad671bf3f9afd926afb1`  
		Last Modified: Tue, 08 Aug 2023 23:36:25 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:6b4ce7a3a962f7016da46f810228189be1cd6de1de0409f784505adca9fee42d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4264646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01f8b18499e87820bcff1593b1ccee12dbf54a9a32e6f7412af5d5c00268ce73`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 21:51:39 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 08 Aug 2023 21:51:41 GMT
RUN apk add --no-cache libssl1.1
# Tue, 08 Aug 2023 21:51:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 08 Aug 2023 21:51:51 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 08 Aug 2023 21:51:52 GMT
VOLUME [/spiped]
# Tue, 08 Aug 2023 21:51:52 GMT
WORKDIR /spiped
# Tue, 08 Aug 2023 21:51:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 08 Aug 2023 21:51:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 21:51:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd254e37c3835d8a90d159f62497146fa2c0a51539455baafa4b5f3ad94073a`  
		Last Modified: Tue, 08 Aug 2023 21:52:09 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b87a0e27917b2f49aabe18b41a38f10f52561eaed9cd75ecbf9bb54dd5ad657`  
		Last Modified: Tue, 08 Aug 2023 21:52:10 GMT  
		Size: 1.2 MB (1163899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9a3f71f875284eede5e8bb82a4d0706d42594a0fec380b98dd516f0f75ed88`  
		Last Modified: Tue, 08 Aug 2023 21:52:09 GMT  
		Size: 199.5 KB (199532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0eec6ac7d1270176b9ec72709b3186f9c9af79d5c747bdd03ac4818437e4b9`  
		Last Modified: Tue, 08 Aug 2023 21:52:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da618866e96da51da8e7f96815a2d1e87198583082d2e819eaea328e7698149`  
		Last Modified: Tue, 08 Aug 2023 21:52:09 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:dfe860acf255915c9dcaae09dee878429e2b4c60798c048d82792352553d097d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4910891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a9eb2d7445a05df9d201e84087d63696ade07ba940606d9e9deff249fd99f3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:24:54 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 09 Aug 2023 04:24:56 GMT
RUN apk add --no-cache libssl1.1
# Wed, 09 Aug 2023 04:24:56 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 09 Aug 2023 04:25:03 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 09 Aug 2023 04:25:03 GMT
VOLUME [/spiped]
# Wed, 09 Aug 2023 04:25:03 GMT
WORKDIR /spiped
# Wed, 09 Aug 2023 04:25:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 09 Aug 2023 04:25:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Aug 2023 04:25:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa528de18ca9d8d7a81ae0d2ae78e694dca22d0e57c1adfd51230a5e72d602e`  
		Last Modified: Wed, 09 Aug 2023 04:25:15 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4370e4fd5a67983765277bfaecb212d7f59e20db8264e69a6addca35b95526`  
		Last Modified: Wed, 09 Aug 2023 04:25:16 GMT  
		Size: 1.4 MB (1362701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4605f0c15e8832deb396dd75011d9b8192e38e7b774733cea490c48a6c601da8`  
		Last Modified: Wed, 09 Aug 2023 04:25:15 GMT  
		Size: 215.7 KB (215688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261765f25ad95a25543e0e6a6027cde75c58f6d3ceff188b0603ddcac15e32dd`  
		Last Modified: Wed, 09 Aug 2023 04:25:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777264984131985e8771b4c25137123bf218b95e4de8ca97a58fe188f07340e6`  
		Last Modified: Wed, 09 Aug 2023 04:25:15 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:3b9156620133e8bd472e78fcdc63367c0bd8ce4728e9b37100cecab16f9ba20b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4822397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38ba2e93561dabc36ed836ecddc93cde747f6c0533764e243a1059c63a1ea4f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:26 GMT
ADD file:4b33c52e11b19fde30197c62ead0b77bde28d34edaa08346a5302cd892d3cebe in / 
# Mon, 07 Aug 2023 19:38:27 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 22:25:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 08 Aug 2023 22:25:18 GMT
RUN apk add --no-cache libssl1.1
# Tue, 08 Aug 2023 22:25:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 08 Aug 2023 22:25:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 08 Aug 2023 22:25:30 GMT
VOLUME [/spiped]
# Tue, 08 Aug 2023 22:25:30 GMT
WORKDIR /spiped
# Tue, 08 Aug 2023 22:25:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 08 Aug 2023 22:25:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 22:25:30 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:95dc695758361a4038a2d9026959d72e1f531114edb0341be7ce47d912ef069e`  
		Last Modified: Mon, 07 Aug 2023 19:38:56 GMT  
		Size: 3.2 MB (3235144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000c31dcd775c39ea60679a161fbb3ec0114ed4a665986290232a4978c9b6a4e`  
		Last Modified: Tue, 08 Aug 2023 22:25:42 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d724475632ebc1a22d1c3ca248315c7f4e6f7c5296f4eae98f587b0b3d246cb8`  
		Last Modified: Tue, 08 Aug 2023 22:25:42 GMT  
		Size: 1.4 MB (1353881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436a4abf10ff23af34214cad41a3ae8c5d722d0e578c719b02dcc3b303fa33ba`  
		Last Modified: Tue, 08 Aug 2023 22:25:42 GMT  
		Size: 231.6 KB (231630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9efbd75e8157b70348066566d4008a9c0bada288c04ada82ba412b78dc02e0c`  
		Last Modified: Tue, 08 Aug 2023 22:25:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06b78bd941b6d435a0daeb98222178fc6fdbd36c9b3cf1c59533e4bb87eb77b`  
		Last Modified: Tue, 08 Aug 2023 22:25:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:b970c43232a9d83311742cddc2169c379db8304ab7409d9da95ff993ac82fbcf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4929752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45510f2b3a9a17d1bb74f84ca2abab8ed1061dff0e55839a3e8754e2c3290639`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:49:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 08 Aug 2023 23:49:46 GMT
RUN apk add --no-cache libssl1.1
# Tue, 08 Aug 2023 23:49:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 08 Aug 2023 23:50:02 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 08 Aug 2023 23:50:03 GMT
VOLUME [/spiped]
# Tue, 08 Aug 2023 23:50:04 GMT
WORKDIR /spiped
# Tue, 08 Aug 2023 23:50:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 08 Aug 2023 23:50:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 23:50:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc475aa02ec0250350b4a331524b0a1e029de0aa51afc8d13cde5114f9a38f3`  
		Last Modified: Tue, 08 Aug 2023 23:50:26 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64752c695a009aa97f4b6b21ee3618c0e6a15c1ccff9682ad7b50a01c411c09a`  
		Last Modified: Tue, 08 Aug 2023 23:50:27 GMT  
		Size: 1.4 MB (1361737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d6958824bc296d0ee662dc09b65827f4c19cf6d08b0bc88c29c0aac7daef4b`  
		Last Modified: Tue, 08 Aug 2023 23:50:26 GMT  
		Size: 220.0 KB (220022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbe94a7a7ea3e66fec66bafea8a8825cb0e1e4d4e13a6dd126caa55abc4368d`  
		Last Modified: Tue, 08 Aug 2023 23:50:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465d36cfcde9b1ab7cc6cd3e055bd3be46da17fbb42fd44094957dc575cb2aef`  
		Last Modified: Tue, 08 Aug 2023 23:50:26 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:7a35ce80545ef01185c3169716056ca5ee9520f1581c67074f5bd685d4f12ef6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4646060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b6af800db14443eb1061db4d4abf6affd33538028addd00c5cd1c46f9cbb00c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:16:01 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 09 Aug 2023 04:16:02 GMT
RUN apk add --no-cache libssl1.1
# Wed, 09 Aug 2023 04:16:02 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 09 Aug 2023 04:16:08 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 09 Aug 2023 04:16:08 GMT
VOLUME [/spiped]
# Wed, 09 Aug 2023 04:16:08 GMT
WORKDIR /spiped
# Wed, 09 Aug 2023 04:16:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 09 Aug 2023 04:16:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Aug 2023 04:16:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c947b711155cc9344e62be76da2fecb7e905aca9dad8fc53f2cb638fe84aa6`  
		Last Modified: Wed, 09 Aug 2023 04:16:26 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705178608b8d1386cffd5a0ae5a7f41f2e6f580e6fb623ad053b6f8210fef7b1`  
		Last Modified: Wed, 09 Aug 2023 04:16:26 GMT  
		Size: 1.2 MB (1221485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1daaf6c162e1789b8a3c771759f74ad7c9ef9d19c7b7b614f9bea92f6f181874`  
		Last Modified: Wed, 09 Aug 2023 04:16:26 GMT  
		Size: 208.6 KB (208644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998e9625b69d1551e16c0e8f95bc6eb00c95fbff0b0343391700336a2adb0752`  
		Last Modified: Wed, 09 Aug 2023 04:16:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d852c787e2ceba069513a1f75d40922510e58442a2924c5668f7cefd24fff1c7`  
		Last Modified: Wed, 09 Aug 2023 04:16:26 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
