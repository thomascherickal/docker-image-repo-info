## `spiped:alpine`

```console
$ docker pull spiped@sha256:df67424ae1b5f50fe62e3c8f7584a176cef62ba9d479ccd376f70587ae42ca61
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
$ docker pull spiped@sha256:b1000f43786f16a20a805fa353f6e29da279735ce16fc397001fde0e351cadab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3038963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:319549bf17a1c296f365e261889f2573a629fda0ca36fa2dac3efc79c233dc4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:41:12 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 09:41:13 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 09:41:13 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 09:41:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 09:41:22 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 09:41:23 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 09:41:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 09:41:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 09:41:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735044c06e8b73c2bb88467804d54b359bfc8226cf975772cc666adc9f029f5c`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8b16fcaec70a3de42b4e850be4a851eaffa96a04fb49668b0d55b15bdf9675`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 7.8 KB (7783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79236b25532d68c328b81af71a0f8c4eca102b7030a98d650ffc9a7e35d113be`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 214.9 KB (214880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f429bef29fed68fb012179a10893c62fd5167934a7d62e7d3db15361601d47e9`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1703108ce26f514d42179cf03051a6082b57e184d89f7bab08377819025c74d9`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:ae66fb10272b529530524084a214a11e65777dff6517d5a90d71357e60416246
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2830615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aae9a0570520cf722d24d3a84685d936a04a06d1b8e35de44be52daca29219ea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:32 GMT
ADD file:44acf536d487bec7f7bf16561f4ec90e60d4447b3cbabfeca66953c4491aabeb in / 
# Tue, 29 Mar 2022 00:49:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:24:39 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 29 Mar 2022 08:24:41 GMT
RUN apk add --no-cache libssl1.1
# Tue, 29 Mar 2022 08:24:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 29 Mar 2022 08:25:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 29 Mar 2022 08:25:01 GMT
VOLUME [/spiped]
# Tue, 29 Mar 2022 08:25:02 GMT
WORKDIR /spiped
# Tue, 29 Mar 2022 08:25:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 29 Mar 2022 08:25:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 08:25:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:84f033dabe5013c0dfae4263abd951011719d0a15adc3c7312c5be994deff030`  
		Last Modified: Tue, 29 Mar 2022 00:51:25 GMT  
		Size: 2.6 MB (2621943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc4ea1012b3262fa7706463586c4d41a0cf0a329238cbe52ea6d03bfbc07fae`  
		Last Modified: Tue, 29 Mar 2022 08:25:35 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5659ae5d68adc8e4012f07c665ea352c4068ee821e83350f8bc165b6aea5583`  
		Last Modified: Tue, 29 Mar 2022 08:25:35 GMT  
		Size: 7.8 KB (7774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf4925cebf49f63997a8c7389e423c3623dc4cd2e6c701e4282c664293e789b`  
		Last Modified: Tue, 29 Mar 2022 08:25:35 GMT  
		Size: 199.2 KB (199158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eac1b140b33266f585c96310939c5cdbac7bde1fcbc0bd4e8cde9f9f0dd5171`  
		Last Modified: Tue, 29 Mar 2022 08:25:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b13e602bdbc874391ee6aee0f8abffe1e74ee57061d9e1faed46aa76ad44a0`  
		Last Modified: Tue, 29 Mar 2022 08:25:35 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:1533669bdce5be15027cb96650fabea206274558c0195f437de5245079d89f0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2626515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52a32db31d94e7ea2f1af7b835d809d1b42c16deff1071fe4b3f2e720bc3688c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 02:13:28 GMT
ADD file:8c959b80e3661beea7b3468017b88897d981bf52ed43c074e7c87ecb753e9059 in / 
# Tue, 29 Mar 2022 02:13:28 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 16:38:17 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 30 Mar 2022 16:38:19 GMT
RUN apk add --no-cache libssl1.1
# Wed, 30 Mar 2022 16:38:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 16:38:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 30 Mar 2022 16:38:38 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 16:38:39 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 16:38:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 16:38:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 16:38:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:22b1e5a07a97d7af6fdc335e3b3a975b73908fa19b084289c408a00814da0398`  
		Last Modified: Tue, 29 Mar 2022 02:15:28 GMT  
		Size: 2.4 MB (2424303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b864dcb6ac61a275d83b41f5e533000faf52fae810b4fc0513796337285828`  
		Last Modified: Wed, 30 Mar 2022 16:39:51 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3aed778a3d8f2984cc57d3cbd49d0974e4d48f31a548da40051a676285fcb98`  
		Last Modified: Wed, 30 Mar 2022 16:39:51 GMT  
		Size: 7.8 KB (7781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23bc58fbe93b76dec15870d5507d4377afa5e3cd4e9ddd68e1117ed5fb9b1953`  
		Last Modified: Wed, 30 Mar 2022 16:39:52 GMT  
		Size: 192.7 KB (192691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f1a66e69919430ccc221d6a8b42a90a4ebdee7a41b426b4cabbd472c3d62a3`  
		Last Modified: Wed, 30 Mar 2022 16:39:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6342a8067391971e5056968d5d26841d53aeaab30109c42bb6c53a227f694cab`  
		Last Modified: Wed, 30 Mar 2022 16:39:51 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:c0d28956af21c9ad7d0e3d4cf972b301ea28efa0c8755d1ee62841b09754b0ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2933013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a11675ed63f0f0f4c5e2d5175c06bade440268d204f7a4b104eba50db3f998da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:05 GMT
ADD file:24e8b04304ef91bbf949674909ccaf2c66e3dcd096c3c307a0510569eadf576f in / 
# Tue, 29 Mar 2022 00:40:05 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 01:02:13 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 30 Mar 2022 01:02:15 GMT
RUN apk add --no-cache libssl1.1
# Wed, 30 Mar 2022 01:02:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 01:02:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 30 Mar 2022 01:02:35 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 01:02:36 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 01:02:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 01:02:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 01:02:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:80fa7f07ec7b717ec5f8e2717b91e3d659e129052ec3def2570a5674322688d9`  
		Last Modified: Tue, 29 Mar 2022 00:41:08 GMT  
		Size: 2.7 MB (2716347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef7ee2c7f3dc7bcaf9752a844248d8127145ffd675ae5de72b4be177fc37cd5`  
		Last Modified: Wed, 30 Mar 2022 01:03:39 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c53830f06d1a108ac255dbff68c71fabc58723d0a42943fec7681cbebe653a`  
		Last Modified: Wed, 30 Mar 2022 01:03:38 GMT  
		Size: 7.8 KB (7751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1f94f19caf7b781c37e261530b5861447ecd5ab33d55ad4d2f12a932db1cf8`  
		Last Modified: Wed, 30 Mar 2022 01:03:39 GMT  
		Size: 207.2 KB (207237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b259955a7b787ff533a05f42050e5172ba829db902cac41506236e30a45be04e`  
		Last Modified: Wed, 30 Mar 2022 01:03:38 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29db0547b8fb18568f5c6616a8622211952741a2a93da0e86cb506b1ee4c941c`  
		Last Modified: Wed, 30 Mar 2022 01:03:39 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:dcbb93128deb3206337ac10573e41e27b4a95816cd3f931412c655201fef2396
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb9526919356b65e45d7bc9a9bd2aaddd7da8a1e62f023b9511a320a431df64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:51:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 06:51:24 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 06:51:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 06:51:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 06:51:35 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 06:51:36 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 06:51:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 06:51:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 06:51:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5043c44edf55100d2df153f657912b53abf987ef0c6286b113dcef298998f359`  
		Last Modified: Tue, 05 Apr 2022 06:52:09 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc9d36e654ea336dd74dc00574768a6502edd5ef5cd785b695e516f6254be55`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 7.8 KB (7750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0401735f1a5cdc5a0248a778049579b8858a6f7cc0fc6fdcdaea211930d4a386`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 225.4 KB (225416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a85e3f263e110e3fa50aada2a3ca6314a5a6e67e8f211881a826585a5db409`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f113efbe13d3511b57cb0428e99f2725a51cb3980e75b1f1be3fc0d715b19`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:d27c5eb0ad348fe2a50b65e808e4b825f0f479572187d81757b9a82ce2ad9e50
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1853309ab0785a26d0b48053b424c5b8c4ffd6367504032c68e3377b9fc92eba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:16:52 GMT
ADD file:9e7b65a431d59070abaadae56d9c3fc59c899af881939e4353b1f524b2bd5185 in / 
# Tue, 29 Mar 2022 00:16:55 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 05:25:40 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 30 Mar 2022 05:25:50 GMT
RUN apk add --no-cache libssl1.1
# Wed, 30 Mar 2022 05:25:53 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 05:26:20 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 30 Mar 2022 05:26:24 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 05:26:28 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 05:26:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 05:26:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 05:26:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1c611bca4fa49cac5bc1e3826ad53fee85ed659d24bffcccd86c3f04be07339a`  
		Last Modified: Tue, 29 Mar 2022 00:18:26 GMT  
		Size: 2.8 MB (2811009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61e9d70cfabe50a7554945008b067920fffa673936b1b8c50f29cdbc07fad93`  
		Last Modified: Wed, 30 Mar 2022 05:27:51 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9a458bb0005f54d005e938aa01a6aeeb1d7c48486de6811d1c16a9846b1239`  
		Last Modified: Wed, 30 Mar 2022 05:27:51 GMT  
		Size: 7.8 KB (7774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8c858ba1f6886855b0312ec6b3618c916bea4577c858d028e6709d67f05939`  
		Last Modified: Wed, 30 Mar 2022 05:27:51 GMT  
		Size: 213.1 KB (213149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d4e4cb20d1bd858c134eae12aac2cab24001fbae386ee7f84b1e8dc6c6ef76`  
		Last Modified: Wed, 30 Mar 2022 05:27:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20cb5033835d271b66d87c37a113ae41ee09c6b1c5b462196462cb06687e3352`  
		Last Modified: Wed, 30 Mar 2022 05:27:51 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:851d4d1e8b82de6d455e9a562bd6b75539fe737213c9f3cf01ce7b44e11abeb4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2811594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e240f56e6000d053b4d3e20632b54b88daaa8dad76ecda720ce9f76c82bfe394`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:09:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 06:09:45 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 06:09:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 06:09:50 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 06:09:50 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 06:09:51 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 06:09:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 06:09:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 06:09:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffc8ec477cbe2d575e99a9232e9328db8cc40109dbe067d93c2033302576850`  
		Last Modified: Tue, 05 Apr 2022 06:10:22 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee008c7ec71319091cda7b7cbf1063414ee758f739581409a2e7089e90882c9`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 7.8 KB (7788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3edcb5212f084eabfd1bad6e332d8b53bd7756099c4da3e410ee23f869a701b`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 201.7 KB (201693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd099e1efb05ce5fa06c5e18ba7d057b5df318c462022f1ac443f45e86fdc809`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbab95e29c022d6828d869e5e4442b139373571c747f8fc6470b8bd257337a4`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
