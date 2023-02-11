## `spiped:alpine`

```console
$ docker pull spiped@sha256:78817eebdb2ae14db82b3ccbaad3585ef439c8282d4f8a3eba135a26579c9296
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

### `spiped:alpine` - linux; amd64

```console
$ docker pull spiped@sha256:8eb40fb8e554b827563f599dd3e61da57293486cae87cd856a891b4e8dba353e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5075384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dda802d4535ce910f8e00126e80c79abb0825f3bf7caf66a4bb950cb589cc74`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 20:03:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 20:03:05 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 20:03:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 20:03:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 20:03:16 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 20:03:16 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 20:03:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 20:03:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 20:03:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9fb896348696d642ef5674956097b03540bea28f8454d6287f5d9cb10b5b19`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1fb67340ae0e377cfa3a1ee1218a1ba6d31cf9f7cb2a302542d4354c848991`  
		Last Modified: Mon, 09 Jan 2023 20:03:33 GMT  
		Size: 1.5 MB (1481738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e228854dc2c8d78fdfe84ed1b99903b8567e21eff2fcf86757e6fdfa823872a`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 221.3 KB (221283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f486af83d26d338661f9edfe85a3574704c4d8e4a08cdea692294588749dde0`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35820a44b4998d9547534e80870c2e2a59cad7f381a4d6a82609d3f67126045d`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:cb751a21eae14bec751c4cd688311f6eafc98d6d1769aa245711e63d7182e21a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4554176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:341ba40bb3f41e998727f9c4967f67b001703e78dafe41ad92a70bf2791fca9b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 20:52:14 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 20:52:16 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 20:52:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 20:52:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 20:52:25 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 20:52:25 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 20:52:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 20:52:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 20:52:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fcf4fe7db4264a8e664de4d52478f1d4ba98146c38a7672ed85c122a2ec9ea`  
		Last Modified: Mon, 09 Jan 2023 20:52:44 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252aa0c5aa375a984c376376752105d7908cccb2ad2078305d2f12c857e58688`  
		Last Modified: Mon, 09 Jan 2023 20:52:45 GMT  
		Size: 1.2 MB (1238925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bcc6c04b36698f2894107a3dcd168ebf74dcadfaada1feb7c909e6d7d2e48c`  
		Last Modified: Mon, 09 Jan 2023 20:52:45 GMT  
		Size: 206.3 KB (206330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2b1d7fdda8e63c8009adec27201adf5aef01cb0be8ae5e126525f70f6ff253`  
		Last Modified: Mon, 09 Jan 2023 20:52:44 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cc764eff90255e712b5e4a850166371f439ffce5e23ec5a3902aeca546fce4`  
		Last Modified: Mon, 09 Jan 2023 20:52:44 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:5350876a3890b8b4c1a7262c4c48345b4046feb2b93df0f849b165f6d3862d43
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4233507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a136cbdcf03b9c140acc83ef95bd48dcdb73507ee82d16eed4339281865ff3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Tue, 10 Jan 2023 01:03:19 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 10 Jan 2023 01:03:20 GMT
RUN apk add --no-cache libssl1.1
# Tue, 10 Jan 2023 01:03:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 10 Jan 2023 01:03:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 10 Jan 2023 01:03:29 GMT
VOLUME [/spiped]
# Tue, 10 Jan 2023 01:03:29 GMT
WORKDIR /spiped
# Tue, 10 Jan 2023 01:03:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 10 Jan 2023 01:03:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Jan 2023 01:03:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c30dc917313d61894ccb7cfad12c5f3a278e251ca506df448c9f8e2a16ba910`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4704616a59a25f4e6a3979312202c02302fb7db16765696efeaf0136d5d871`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 1.2 MB (1166534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d943eecb9e0495c260d5786a0e7109c2f3f4c07c93eed00e71667a8fd3cd0a7`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 200.1 KB (200087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30309affe27d04051a0e8f9d361029624d0957f51f95f351a76921b3d10aa00e`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40cb5d940651ed07d3a8a9b5d7bb45557f66f56eb842f0db2c34496a0b49b3be`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:0213ccc252b274961ca65d4810e3e3adbfd0a45802938a1fc17b5260a5766747
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4838993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f334562e83a3560fd096b7555b628adde3f65f35e7d7f88d92cef036aa3b80e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:54:38 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 21:54:40 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 21:54:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 21:54:48 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 21:54:48 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 21:54:48 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 21:54:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 21:54:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 21:54:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a57c503886d17fc3a18ad5ac652d01a19c1d114d10d95fbbb6962eb5141a3c`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7deb227b2dbf5691407192d6e6164c40a313d06c2d63a713bcec3bfb588a82f1`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 1.4 MB (1362327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136d1ea11d30612c79aa77675c78fb75feede08c3a75327ad85af71c6acc55cc`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 215.7 KB (215692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c3012f3cfaea50c1e653e77ff8a01ac59681255c473f52fc3d3087f2ec06f1`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ff7343264af5878ae4a177e19ca1bc3ef5ed246ba09fa1c3c6e4e80c2c09b2`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:822b81d156b7c387e1ceda5cee3e6a6edd3268187a6ce26e8b85df4c68e09f5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5131561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4d91ebbd686f96b26164ad7739fcfca17552f6046e879f7ae2d57c3d3892739`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:23 GMT
ADD file:125f3514520a5cd29df2830a409aa026a2bc06a77a7a5d150133436404b33d41 in / 
# Fri, 10 Feb 2023 21:24:24 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:18:56 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 03:18:58 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 03:18:59 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 03:19:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 03:19:10 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 03:19:11 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 03:19:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 03:19:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 03:19:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b3e346c15c2377ec0e75cc9efa98baecd58b0e9bb92f0ec07eeda0bcc7e67fc7`  
		Last Modified: Fri, 10 Feb 2023 21:25:13 GMT  
		Size: 3.4 MB (3412353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7d8401c5bd9906ab3609377e9ee6deadd5d9c4ae39ecfa8e9cd01ede0b8281`  
		Last Modified: Sat, 11 Feb 2023 03:19:39 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469cab1d7427d43462f6a9628be5d2ff81ee2cd0f9f7541f9539bc00c92429f7`  
		Last Modified: Sat, 11 Feb 2023 03:19:40 GMT  
		Size: 1.5 MB (1486162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:272b1229ae2f459eb6817fe20b02d6f823f26e1e8c76b8ac51eb8934b9143027`  
		Last Modified: Sat, 11 Feb 2023 03:19:39 GMT  
		Size: 231.4 KB (231370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4adf5f9d6c3c73c3d7546a48714ef20383a01eeb6f321be386524c8e6e4212`  
		Last Modified: Sat, 11 Feb 2023 03:19:39 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35580a675ce6a64cc7a800a1f273d54f02d5e70f9b158be76b5a569da9cdb610`  
		Last Modified: Sat, 11 Feb 2023 03:19:39 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:6287dba41a56cf9c39be27c62b7a3bde3479b303d63e9230b446113020881fa9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5017699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ef59306a962c0b86d594be1281ca3dd3e91c0b16a046ee09218d60231e3a9cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:13 GMT
ADD file:9a1d27fdc0c915f387f2446c85193d5215b18020b313114f0bf2799efcc1baae in / 
# Mon, 09 Jan 2023 17:05:13 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:32:14 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 21:32:16 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 21:32:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 21:32:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 21:32:31 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 21:32:31 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 21:32:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 21:32:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 21:32:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f45bfda3aa14e255d9eb4c9a108eb3d8c6721946b4aa2e5808e5092242344a1c`  
		Last Modified: Mon, 09 Jan 2023 17:05:56 GMT  
		Size: 3.4 MB (3384562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd46f789ced0eaea980007a2e6a0f6b02b7711749489fdc0a30de08d248c3325`  
		Last Modified: Mon, 09 Jan 2023 21:33:00 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc9ef36d078710c0c6d69a2d1c19bc6701be12e5c554ec9fa1546fe495e59eb`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 1.4 MB (1411372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e8744b0f13a67b1002a7a426a2b3635f0b4a28fd095ef061c0f1fd5d85d909`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 220.0 KB (220028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc209dab70185705e5eee1e1710197c9bc735498e476d6719c4b850ae44fdaa`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe41dcc405bef6ddd7bb480eadf45d92a9cfd583bee884d68eb41037c93e1e23`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:c224a59dd171160cb9e3b3be6bac31704ad968f23bed4f4f8ae4d04d938951c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4608839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88032fe647cd1b9c54c93549e3978f1e53d8c0df71f2c0c2660b0545fc0b7ae3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:20:31 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 05:20:32 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 05:20:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 05:20:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 05:20:38 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 05:20:38 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 05:20:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 05:20:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 05:20:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb5c0ff1110b4315355f81e38de10bb31ba9fe44d99d3b7598f20a28f2c98e1`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ac27252903c2b21737926a9cd0721ecfa3aba4f2e52da7f7c114aea4da62df`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 1.2 MB (1223356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df30f40ce9a4931562f50ea55d6450396fd443fed95a0b2c0ea337f53f22ec25`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 208.6 KB (208631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9420167a9c04b73e787d02b0fa09ba21ff8b27917d0406146f9bc5a0df3034`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea129f4350d878551c457a2192ea0570f86ca7ee5c193a6b0d8e19727570f05b`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
