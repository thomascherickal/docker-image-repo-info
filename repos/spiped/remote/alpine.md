## `spiped:alpine`

```console
$ docker pull spiped@sha256:a66b70ec9fed63f99d5ebb9a084fd6b4f2e48d3306b6d5963d5bab3a3554d099
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

### `spiped:alpine` - linux; amd64

```console
$ docker pull spiped@sha256:e72efc9006cc88e74da18f8909e9a6d6cb80c024bc171e1de9a3bfa8082c7e7d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3016730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af4cd33bc57ff09ba0929eb9a1846e003f8ab8d35ac7f715f376161a9209fb7e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:23:52 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 08:23:53 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 08:23:53 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 08:23:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 08:23:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 08:24:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 08:24:10 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 08:24:10 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 08:24:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:24:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2cfe9f1210973e807f22612ef44f79fdf4e9f1871ceb24da9c470ff4c6934a`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ebdc509a836b5478bba964b2f5c1712aa349a3761854c4f1193f580d18193`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 6.8 KB (6771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2055abf7179bbbbaca992858134f6d59becb2b5cb2f516330f97082d7f4d272`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 211.4 KB (211432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a723ed90b1f6fc5a4bc245ba955d04306500cc3613e897f36a9246cb119a856`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8823b92e870bcac9a4efd674a3b7605e55d9877e47bb6d81c8d47f8e80d12a4a`  
		Last Modified: Thu, 22 Oct 2020 08:24:23 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:a2c07b0fd8b8125bc764aec18cc6f9bc8bb426248f34561bd3ecc499d09346df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:677efa26ec938c048fee627507fc0da1cc62578addd97b08b687dd5b2ad77915`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:43:03 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 05:43:05 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 05:43:06 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 05:43:06 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 05:43:07 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 05:43:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 05:43:35 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 05:43:35 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 05:43:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:43:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:43:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d656e33abe3d3601b321a868fc727b9be9c99b7488b724d484186750afcda4`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1772247a79d18f5b7de3c61484f065ffad9fd2ac52c4bf1391e9391d27a4312`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 6.8 KB (6764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e976ba7bffb31272cb6237ecfa4bf695187d6b5efb425f524479464784e4b970`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 198.4 KB (198368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5beb20421fe898cdae2849e5ce6bbf79e1393ffd677dc4d82b8271eebfd5cbe`  
		Last Modified: Fri, 11 Dec 2020 05:43:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a68e820deaacde91763058f7c4d28c1853ff02d626aa4516ad41ab4a155873`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:1913a59773cf295dd8d96f26cc0ba23e5325c4b318f2e48b1668736a9a5ae532
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2605804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:648a07e74593903bb0b5a422c8c3f677102d278b79b31a76cba4b51e1be16af1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:59:33 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 02:59:41 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 02:59:42 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 02:59:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 02:59:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 03:00:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 03:00:11 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 03:00:12 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 03:00:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 03:00:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 03:00:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66d19d74400f766b7b4a9239a805587a1523517a166d14ed12a1bc5435fcca7`  
		Last Modified: Thu, 22 Oct 2020 03:00:32 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a534ce800d06acec8b2e639d97798306f250838441b482b3dba8a16bc6ff45f`  
		Last Modified: Thu, 22 Oct 2020 03:00:31 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194e2e34702b51562d461ab44982ea3720b4edf6bcf81e135005398c1f9bdc7`  
		Last Modified: Thu, 22 Oct 2020 03:00:32 GMT  
		Size: 191.6 KB (191642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d152e941e8212f73f472183f3c9742b6a5c8670c44519dd69234bc46428dcc04`  
		Last Modified: Thu, 22 Oct 2020 03:00:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe41531b30548b2b91cc5b6563486356d5a291b1e56c550ce60fa95fcd766c25`  
		Last Modified: Thu, 22 Oct 2020 03:00:32 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:22e076d0704999df6954352a61322c7aff9e84102fb209dca8c67047f0f9ec55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2918883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c12732fc9350260a757debfd45b04e105fa193198c820121c8fb104c75e4090e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:13:00 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 09:13:04 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 09:13:06 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 09:13:07 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 09:13:08 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 09:13:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 09:13:37 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 09:13:38 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 09:13:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:13:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:13:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460ac12de1615c4fcf136e9caab1c56384e869fa371fb1aa91fa6a50584aede8`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c49ab63c0d72d683d01704eb4d538cac06f6cccc649a32c793531090a507d758`  
		Last Modified: Thu, 22 Oct 2020 09:14:05 GMT  
		Size: 6.8 KB (6765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7c72e8f699aad2c97e9e3116224f712f7a66a5bacec74cb4db459e9275f8d2`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 203.8 KB (203833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cc60fd10df854316c0653b5c11cd733c7191a08efa7aa164d9d9e6cb76de12`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47396fd59d212f4a22fd40665e6647db1065fd9aebe2fe3394e3c973688ad64`  
		Last Modified: Thu, 22 Oct 2020 09:14:04 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:69a8f9d0101fda57680f27c30ca9864f021d69a013d0d876c7f010296105365d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3021046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aeca41fe853b4af9d83ed356e1a338abb14a58e5645c3cb4a0756640886dc5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 05:58:32 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 22 Oct 2020 05:58:33 GMT
RUN apk add --no-cache libssl1.1
# Thu, 22 Oct 2020 05:58:33 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 22 Oct 2020 05:58:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 22 Oct 2020 05:58:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 22 Oct 2020 05:58:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 22 Oct 2020 05:58:53 GMT
VOLUME [/spiped]
# Thu, 22 Oct 2020 05:58:53 GMT
WORKDIR /spiped
# Thu, 22 Oct 2020 05:58:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 22 Oct 2020 05:58:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 05:58:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076cf7cc4c20069210dbf0b03ab1fecd91e3d95b49c97e98cae7c670b28f0033`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf8eec65d1d720af4b0e901af92897e91841e174ac0414999f9174673879238`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 6.8 KB (6763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca18ab8a4b82f11e9d159625a64a3b9923866ef0471b97f803fb09071405476`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 221.2 KB (221209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cce939bb90551e9a0f849ecdfad6c57fde68602a16c1a208154aaa6a5d2c49b`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230d405b698f37c531145e3d12d6c2db6858a39fb6b5bd2a61b1e6dec0a9f38f`  
		Last Modified: Thu, 22 Oct 2020 05:59:07 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:8cfe707e6883e571a9e283c137fdf05c89795e813fea9d113d73243ef6e48f66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3030963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a0c32ce328376d6604c2cc1e3afddc420d50421031efcdfb5a64d471012cff0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 03:30:29 GMT
ADD file:9b4b44ee9eaddedc13f114bb55c9abeabceff6abd47f4a660734e431d22fcdce in / 
# Fri, 11 Dec 2020 03:30:32 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 04:26:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 04:26:42 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 04:26:46 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 04:26:51 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 04:26:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 04:27:23 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 04:27:29 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 04:27:38 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 04:27:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 04:27:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 04:27:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ed596bc4dd0a0c7ff1952005f6cae53a061e1c7998282289586bbfc17a2fd6db`  
		Last Modified: Fri, 11 Dec 2020 03:31:06 GMT  
		Size: 2.8 MB (2803424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cd13015bd20b24fa3de00964923d4174689fe24331cd6727149578ab140e77`  
		Last Modified: Fri, 11 Dec 2020 04:28:36 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b7f2c12df52bfd764a9425a51ff9ea78c401b7ae35f4fee967e6dc290fe8a9`  
		Last Modified: Fri, 11 Dec 2020 04:28:36 GMT  
		Size: 6.8 KB (6768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a24b5a19799707647440b61dd5ce769a9faa7b9744c65a66566489782fd707`  
		Last Modified: Fri, 11 Dec 2020 04:28:36 GMT  
		Size: 219.0 KB (219037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09209609f22c3956871b0ff04b1ee5a283f44fdac5054f39cdb898fbc3409c38`  
		Last Modified: Fri, 11 Dec 2020 04:28:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfeb1e3e8c1ae99b6192e09f333e05a6c38f2221cb348ac0f1aa336366022926`  
		Last Modified: Fri, 11 Dec 2020 04:28:35 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:f7bf86a59e1d8e7919ad60f3b4befb3cc3becb3510cd67ce32b77dad9078fc81
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2777502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28b6fc7550d85db051cb5ce945e2ff2f95ceb8d9e1618662ebd31a939f01e941`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 10:59:44 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 10:59:45 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 10:59:46 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 10:59:46 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 10:59:47 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 10:59:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 10:59:59 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 11:00:00 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 11:00:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 11:00:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 11:00:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37953528e8223e90b4e88a8a082c9401b1dd5031df1927c13c1d05f57f22bfcc`  
		Last Modified: Fri, 11 Dec 2020 11:00:33 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020488e0695a0946ae274aa0cd9236f69d418d2fb7e49221239ad9865fb65449`  
		Last Modified: Fri, 11 Dec 2020 11:00:33 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207c4586d11b5c35ec2fb1003a5758b677ff9ff4a429824c4d92df7d7776f9c8`  
		Last Modified: Fri, 11 Dec 2020 11:00:32 GMT  
		Size: 203.0 KB (203010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a94329927d876dd9e10fdb405a5efc5229c1dd1ea6378287049c464675dfd09`  
		Last Modified: Fri, 11 Dec 2020 11:00:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b732197a35fbacfe3e9f631341124aee7fef90f63a252187b86cbbcdba9534ae`  
		Last Modified: Fri, 11 Dec 2020 11:00:34 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
