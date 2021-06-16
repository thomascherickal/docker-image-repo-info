## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:b611f87cb8a8b2e94c240963e034606320ee732a29c0de5f7ee6bdd32f1427db
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

### `spiped:1-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:c21bef0140d90218ac109935fb4800c498f43c180f4ef1b10bde2642880be2a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbdf08613600d4c931da69207d9120e5ed8613c25036007e69cb1601a3e8f772`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:43:02 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 03:43:04 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 03:43:05 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 03:43:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 03:43:32 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 03:43:33 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 03:43:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 03:43:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 03:43:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbdc5fa8a3b40bca444e39933121d87e99aab35af8b484d33aff845dc9223dc`  
		Last Modified: Thu, 15 Apr 2021 03:44:02 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa32c269d5d00d85d7899e4eacf26aaba16e1172161bbf98004432c88ed2a5d8`  
		Last Modified: Thu, 15 Apr 2021 03:44:02 GMT  
		Size: 7.0 KB (7043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60da1f1e01411c7d0f98a00b95e704a5e48286ab9625f96f051b85dd593d8e0`  
		Last Modified: Thu, 15 Apr 2021 03:44:02 GMT  
		Size: 212.3 KB (212302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f836cc7647fd0c009041eafa0c5d574e4b5b58b6dc0918744c3c00cedeef407`  
		Last Modified: Thu, 15 Apr 2021 03:44:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6dbf788a05da46939128eed6640869c6cd0ac3b637549bc7a664148c1d27cf`  
		Last Modified: Thu, 15 Apr 2021 03:44:02 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:750e4a3e2b269c49615e43d6e3699988889b406b0c536a97f01713538717f8a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2833181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a6f4c383515708ecc75ec2c2164878f9c74553e6927b9614c53355f96bd64ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 06:12:22 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 06:12:25 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 06:12:26 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 06:13:00 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 06:13:02 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 06:13:03 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 06:13:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 06:13:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 06:13:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05304d4235002a8177d88a9a370a4001b168e9562193801a5939dcb96d98b928`  
		Last Modified: Thu, 15 Apr 2021 06:13:24 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11429747878607e1935e81d7c9bf1da46083ab17322cfb24cdd9756402bf9eb`  
		Last Modified: Thu, 15 Apr 2021 06:13:24 GMT  
		Size: 7.0 KB (7048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6b2ca69864f244fd48c69f52a2aacb2cd2c1252a8c344bfda821704c3bb45c`  
		Last Modified: Thu, 15 Apr 2021 06:13:24 GMT  
		Size: 202.3 KB (202275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd931a38883a95739ed26193356b8fa3a119d0971dc2de02eea8268fcb8d53d`  
		Last Modified: Thu, 15 Apr 2021 06:13:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fd7e5e7757c92528d5a3fba0796309aca6a4e0e8a8ef9a0c9a8326f210bfa1`  
		Last Modified: Thu, 15 Apr 2021 06:13:24 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:efce446ba8870e78476a9d75dcb1e52c175534d2b7ade2a215d811f2394fc147
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2628471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f48264b8ddafa8e951f93dc62b494ff4c0702ad2ed5d97967abeb08eca761330`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 06:35:37 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 06:35:41 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 06:35:42 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 06:36:12 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 06:36:13 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 06:36:15 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 06:36:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 06:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 06:36:18 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498ba0cc83ce00b13dfa2f2b0f032008609655b0256c5050ef42ac51b4ac118a`  
		Last Modified: Thu, 15 Apr 2021 06:36:38 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afde2e53b89bdc9bd82427372b10450afed8a06f7c059c1026a36d942d3ce4e9`  
		Last Modified: Thu, 15 Apr 2021 06:36:38 GMT  
		Size: 7.1 KB (7056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b9dc4c988b74b93e18af14d3edbf234cbb4c959d0ec118f1f35c4b93ec8d19`  
		Last Modified: Thu, 15 Apr 2021 06:36:38 GMT  
		Size: 195.5 KB (195542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0a6650f750be3485d508aa8a969ee6542ea8f7c77318469b7276e9376e5037`  
		Last Modified: Thu, 15 Apr 2021 06:36:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514661aafe8081d75ec940a2e1e4fcbfecc2361f2a487ee7cadab8e66f187275`  
		Last Modified: Thu, 15 Apr 2021 06:36:38 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:91c1773cab1581d76d4d48e8b17a155fdf6fa54339e449958132b7ab0e664b7f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3324815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5620d28ab14686bc056b383ca94e121a1961a59dfa98a9a4e24992d49ccaf583`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:13:43 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 11:13:44 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 11:13:44 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 16 Jun 2021 11:14:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Wed, 16 Jun 2021 11:14:01 GMT
VOLUME [/spiped]
# Wed, 16 Jun 2021 11:14:01 GMT
WORKDIR /spiped
# Wed, 16 Jun 2021 11:14:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Jun 2021 11:14:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:14:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be0802b4de23117d6b04cc1a7237f151ac257b9b6ae94c41543add13a721211`  
		Last Modified: Wed, 16 Jun 2021 11:14:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1598d38937e859a5682a8b4222572712c05ed3cd91911fc2b0402c4d3610bd1f`  
		Last Modified: Wed, 16 Jun 2021 11:14:50 GMT  
		Size: 7.1 KB (7060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93daa195a9f9aae8df4b499ba4d793860c0aab39686330ecc6a410b8f7bf58e6`  
		Last Modified: Wed, 16 Jun 2021 11:14:50 GMT  
		Size: 604.0 KB (603997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011245e695623945bea926d3f62bed142c2caf7f2ff394931342b395e9bf2c6a`  
		Last Modified: Wed, 16 Jun 2021 11:14:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a47c9f4da08454bed52a6c03bb7e750ec3ad498ed63773d6e46ddaccca505a5`  
		Last Modified: Wed, 16 Jun 2021 11:14:49 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:d1f976abe7dc36865966c36ace3442df28cc760cfbc4325a00a692997a8bf0f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3050959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc0614ad90a95b7cd1f85bb13128b580a0c2f29ed00db4f65e968730c4f04440`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 07:28:07 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 07:28:08 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 07:28:09 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 07:28:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 07:28:26 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 07:28:26 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 07:28:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 07:28:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:28:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171a4072559715dd3774427ca5bfad06c46001c1d90638f2010ecca1cecb9435`  
		Last Modified: Thu, 15 Apr 2021 07:28:56 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6417969d29e4f1c0fa56959b290e90527faca258d4dc8f876d5781b5a1d2ee7a`  
		Last Modified: Thu, 15 Apr 2021 07:28:56 GMT  
		Size: 7.0 KB (7049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08261970831fa426d9408c0c3cf638ab7d1ff006feef591eb4b6481ec2714464`  
		Last Modified: Thu, 15 Apr 2021 07:28:56 GMT  
		Size: 223.3 KB (223281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9dc16c21bb57966882a6696907c801efc77eccc10a5ad026e9bbb1e5316a800`  
		Last Modified: Thu, 15 Apr 2021 07:28:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff154aa157546b5d51db233328ebbed740e8854de199b27d502820e45e65bbad`  
		Last Modified: Thu, 15 Apr 2021 07:28:56 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:9d383336851f89b74885b174acf82891ef2bf8c945a6373dec31ca6676fd1107
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2fd56c4b0659f3c04e8bff71019d31b85529f0f9a53b88c69fb81d0bfe3351c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 07:03:12 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Apr 2021 07:03:27 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Apr 2021 07:03:35 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 15 Apr 2021 07:04:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 15 Apr 2021 07:04:28 GMT
VOLUME [/spiped]
# Thu, 15 Apr 2021 07:04:35 GMT
WORKDIR /spiped
# Thu, 15 Apr 2021 07:04:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Apr 2021 07:04:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:04:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602add23d4a6d2eadfe98b28abe912c5fcac90dbe9c2a51a54f428ad33d692ee`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451504af2e04d8b41445eedc1f1f9c76a59c85eb2be170be0d8aa078d0aa93e9`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 7.1 KB (7065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd1d09b1e4f40662048b2b792797406a48e2cb33e7e0c06a3b60ff7f189ee3e`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 221.0 KB (220986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38387eb6968cbda04a7e8b097378ba4eba871862d73839fa97fc66d70f606c32`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b42ba1d6389eba3e53edf2210a840a60b804cc8e51a81a4f42bcc86848d85a`  
		Last Modified: Thu, 15 Apr 2021 07:05:19 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:6ec14094d3594e86c89a330bd9ac7db9109578591c71a7fc895ef583f56a0ebc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2816473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8e10c73436dfd94b9788c63d5d89c26217f62795e62170bfee7bb5fddea096c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:06:26 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 14 Apr 2021 20:06:27 GMT
RUN apk add --no-cache libssl1.1
# Wed, 14 Apr 2021 20:06:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 14 Apr 2021 20:06:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Wed, 14 Apr 2021 20:06:37 GMT
VOLUME [/spiped]
# Wed, 14 Apr 2021 20:06:37 GMT
WORKDIR /spiped
# Wed, 14 Apr 2021 20:06:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:06:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:06:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64390452532879e125a5bb8a9120ef0206a6ffed9b7b45143408593823449b69`  
		Last Modified: Wed, 14 Apr 2021 20:06:56 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe161c1af56f1ac1b902a43d31cc07ce45e66ce5deaae0c37c972f8d4d505530`  
		Last Modified: Wed, 14 Apr 2021 20:06:59 GMT  
		Size: 7.1 KB (7054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62195a09ae764bb27e5a0afa4b95616824bbb859a891aaf48c9f5979d1482176`  
		Last Modified: Wed, 14 Apr 2021 20:06:55 GMT  
		Size: 205.0 KB (205043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c57dc974a3fd6357043b304379826936777167d99e198e01a3341c951c15b9`  
		Last Modified: Wed, 14 Apr 2021 20:06:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113c0808aca0ef9883bd02b957ed90398dbfabff1dcf1d5e822af51ba8e53d69`  
		Last Modified: Wed, 14 Apr 2021 20:06:56 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
