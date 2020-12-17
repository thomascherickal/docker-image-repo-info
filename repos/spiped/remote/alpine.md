## `spiped:alpine`

```console
$ docker pull spiped@sha256:5bf3e8fb913f9a25973b850e0b61c38cd2995a845088624348e8acb4af679460
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
$ docker pull spiped@sha256:b36665543fb15f1237e247cdc1e31c5a124077203da11818b3b0fb136d17aaf5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3016820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00fb5c0620d02cde7a18e4d721e93454411385f48f32a609809dba66e0f15fd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 13:48:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 13:48:52 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 13:48:53 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 13:48:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 13:48:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 13:49:17 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 13:49:17 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 13:49:17 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 13:49:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 13:49:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 13:49:18 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b71fbe7bc43fd8f5c2e88856836ab0cb20daedafbb7d94c94fc57e33b77175d`  
		Last Modified: Fri, 11 Dec 2020 13:49:42 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d0dffb6112c85d6e2f2b928b1631fe4cdf436c387dbc9c951cb07f02b25232`  
		Last Modified: Fri, 11 Dec 2020 13:49:41 GMT  
		Size: 6.8 KB (6767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa205c2404dd6d7a1c86ee038388ed3bd317b221dcfcd16cdd143b894862490`  
		Last Modified: Fri, 11 Dec 2020 13:49:42 GMT  
		Size: 211.4 KB (211440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502754e69f8659cd0de6baec7bff058cbb3e7ee303310b7b52e9bf4ee6c1e29b`  
		Last Modified: Fri, 11 Dec 2020 13:49:41 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712ab91ea61b13fda64e87e604f0e50c14c822f3f9b713992cfef0ff3bdf91dc`  
		Last Modified: Fri, 11 Dec 2020 13:49:41 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:b3a90a9d2dfda78464003631c5ced5e74a88e33d37fb7e00706247c06e3e62fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2605829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:226c0c47a888b294c38da1db4714cf43ea4146f1aa8e7f1f389209d83f6aa5b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:20:33 GMT
ADD file:0e85952ec585d17378d9bb15a94ddc10c3ed8f766f275cf50fb36be1126f35d2 in / 
# Fri, 11 Dec 2020 02:20:34 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 15:29:45 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 15:29:50 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 15:29:52 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 15:29:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 15:29:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 15:30:21 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 15:30:22 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 15:30:23 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 15:30:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 15:30:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 15:30:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f70c74f2e22556cebd0cbbff78c03d4f0560d76979bf799d67730340a639aa57`  
		Last Modified: Fri, 11 Dec 2020 02:21:18 GMT  
		Size: 2.4 MB (2405692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b2d4dad8d362fffcdec7d8c1d7c97d7de39e9a5eece83234d8c2cd84903f68`  
		Last Modified: Fri, 11 Dec 2020 15:31:22 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e9922214e3002ea40e3cd5f9128f90dab186be6cbb6d1858ca0c46123b8d04`  
		Last Modified: Fri, 11 Dec 2020 15:31:22 GMT  
		Size: 6.8 KB (6763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e926fd9cf24045ba66a4570c4770800908a41ff32640a231d5a67e7124a7dba`  
		Last Modified: Fri, 11 Dec 2020 15:31:22 GMT  
		Size: 191.6 KB (191641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1908264eb97b44ff1f2c1f2d4580427ff5759da2c07e1271041f84708cf626d7`  
		Last Modified: Fri, 11 Dec 2020 15:31:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b49057b37c88c17261eba50168832ff2fb073dcde023aaebaf12222e1c0fb54`  
		Last Modified: Fri, 11 Dec 2020 15:31:22 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:877752aaceeae2daafd99b99639b48e6e2edfdab8c4eec7ab65073ff51e3aec1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2921363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22ad953bc3ea727f1b993a5bf8e70f4a74892a11ccd04bd121db0ef4ff8c9923`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:38:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 04:38:57 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 04:38:58 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 04:38:59 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 04:39:00 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 04:39:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 04:39:36 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 04:39:37 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 04:39:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 04:39:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 04:39:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3712d49e6440c4dc671fba2339c89f5d20467413745b8be19d70e0caaa651b25`  
		Last Modified: Thu, 17 Dec 2020 04:40:12 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46c964edde07c97f1a27616640abab3ba174358903d509990270ad0a2c6dc5d`  
		Last Modified: Thu, 17 Dec 2020 04:40:13 GMT  
		Size: 6.8 KB (6768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb0f4f45b7c8150ecdffd49a2be270290efe1d1914ddf26da323f04a09203f1`  
		Last Modified: Thu, 17 Dec 2020 04:40:12 GMT  
		Size: 203.8 KB (203819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea32c0c99096d4ce306eaff76344fbcde6b609125bce5cec33ed8cc8aaf3e8e2`  
		Last Modified: Thu, 17 Dec 2020 04:40:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c655ecb1758a97af788cb42b035b9eacbee75d2ffe44c098d8bdeeb2996a42`  
		Last Modified: Thu, 17 Dec 2020 04:40:13 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:04b442844d79a30e1bf8265a917b2017e5dac178c8353a7b91f93ed7f37a9873
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3021170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29a29fcba7c398a1c8d8e9bf496c410859b4e94baedd16580dd239eb348bb960`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 11 Dec 2020 02:01:14 GMT
ADD file:8812e502f26af2dc4efdfb7387f8bf99f2a098b6c95b9f6abf900df2ce74e3da in / 
# Fri, 11 Dec 2020 02:01:14 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 21:44:15 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 11 Dec 2020 21:44:16 GMT
RUN apk add --no-cache libssl1.1
# Fri, 11 Dec 2020 21:44:16 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 11 Dec 2020 21:44:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 11 Dec 2020 21:44:17 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 11 Dec 2020 21:44:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 11 Dec 2020 21:44:35 GMT
VOLUME [/spiped]
# Fri, 11 Dec 2020 21:44:35 GMT
WORKDIR /spiped
# Fri, 11 Dec 2020 21:44:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 11 Dec 2020 21:44:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 21:44:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b62269920a7a62a905817c7c1b33f33b6e658121e9a054715ff052a23f7de3a0`  
		Last Modified: Fri, 11 Dec 2020 02:01:43 GMT  
		Size: 2.8 MB (2791504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9711e94e3d4acb87ac979443e476919a1d9433dcc45d2167186c7c8de6918b8`  
		Last Modified: Fri, 11 Dec 2020 21:45:08 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb34a0ca99748b461d39274e5cb1333c4f4c120b7f9e257381d6ae484dac90f`  
		Last Modified: Fri, 11 Dec 2020 21:45:07 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f73a702f9c5fe81bbc01d32a43dbcad48785f544c26f9e8484188b6c02bf825`  
		Last Modified: Fri, 11 Dec 2020 21:45:07 GMT  
		Size: 221.2 KB (221227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177df2fbfd860811a4ba157fa1d25cd799c8425d6f5cc09767bad5a13434cc2f`  
		Last Modified: Fri, 11 Dec 2020 21:45:07 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4486cd174808c0b19cec9b2349bc1fd370857e063a0c0a09ff78cacafd19f25a`  
		Last Modified: Fri, 11 Dec 2020 21:45:07 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:27472699e225b3cecb93aff593715a1b1e593b3c5ccaee677f61c0532eb269d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ff055d1554a2790d3299ce836ec2184d1da25b67626dff0e7975227bf3b8bf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:36:11 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 02:36:22 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 02:36:27 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 02:36:31 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 02:36:39 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 02:37:03 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 02:37:08 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 02:37:13 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 02:37:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 02:37:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:37:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e42c0a7b0024477cc166777ef19c2e1cd63e0a016df217c81f1ad17d6e867e`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ed98d2a30fae7fccd64cce03806134befaaadcf8dd7390c74a3cec0b8c8d55`  
		Last Modified: Thu, 17 Dec 2020 02:37:57 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d69d8e55782510c684534af422909754a79f1945e12e464301f021c043e02de`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 219.0 KB (219044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d639ec471f63a1b41aa949a7db2bf31a68ebb304787e4d0d24a16985a5b8c882`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ccb1b04ca97a7dd2ac55b1dc8fc9f953df9822d19116e86af691d4ded7d0ad`  
		Last Modified: Thu, 17 Dec 2020 02:37:58 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:22d84d581716a2a5f1de6d10cc10546736d493a1a1845c11cc0f032874ef4b2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2778532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3afb9e2f140472d2b9e0335b33e697b677876f1df6e2c3a8ba34faf287acfa4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:22:52 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 17 Dec 2020 01:22:53 GMT
RUN apk add --no-cache libssl1.1
# Thu, 17 Dec 2020 01:22:54 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 17 Dec 2020 01:22:54 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 17 Dec 2020 01:22:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 17 Dec 2020 01:23:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 17 Dec 2020 01:23:07 GMT
VOLUME [/spiped]
# Thu, 17 Dec 2020 01:23:08 GMT
WORKDIR /spiped
# Thu, 17 Dec 2020 01:23:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 17 Dec 2020 01:23:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:23:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e28749ff9b137302419a963c66675081a7a31fb1f635d6857c5d209dcda5a6c`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7f79fb0545a28cb5372937795983c817914013736f6a9846b56e453ec52dd4`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a676d107f0804a389a41a4d1fcb3c102fdceee14a9dffd21de8183a741b432d`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 203.0 KB (203013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d3efd6ce468d1c41c42a12f96a4727eed04b45646906ff3af1dfb105340eb2`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c497abbb6277ccc692da7032b7c6a8fa32562381af33b6ee86a4529970ec1aa3`  
		Last Modified: Thu, 17 Dec 2020 01:23:34 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
