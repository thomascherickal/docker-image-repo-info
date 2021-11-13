## `spiped:alpine`

```console
$ docker pull spiped@sha256:8ba838d15be43ab424d58baf2d063bc16de0f673a93df7e8b62a04b2070ea66a
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
$ docker pull spiped@sha256:5759c6e68d7e93789c7fc574722f42f3d3bafcaab2c4a8aeeeac5bb4772012a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3045597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cc3e3a8422cee08ac18b30d97939a3a6bd28e94a61d0caaaa96ff86dd8f425c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 07:30:36 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Nov 2021 07:30:37 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Nov 2021 07:30:37 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Nov 2021 07:31:02 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Nov 2021 07:31:02 GMT
VOLUME [/spiped]
# Sat, 13 Nov 2021 07:31:03 GMT
WORKDIR /spiped
# Sat, 13 Nov 2021 07:31:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Nov 2021 07:31:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 07:31:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d272f2608cb29aaf56aaa58c4e8245793833d52257971c0a4a90c1445945548`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588bebf547583661fb31be182d777849262971941c241f7b072c041f54e3c4ff`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 7.8 KB (7767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687f41a1ab4447065d651caf78075639eb1027290f0756c4d489a10c43a745af`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 213.1 KB (213113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d7a22ad75e07e938780270586c7d97ddd070bf6b70ee31e6fbe14b6c79cda6`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b484100590c35b883633e127830518528f9cc47bce7f4b864394b4bd85acb54`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:e54c9ae8aa1651b3704440b6b74cbdd5ac80086e8fa25252df5ffbe44591eade
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2847905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6b358d015e8acc6b6eac3e79c5fc5302785d8bce806dc4640e51e684fc73495`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:56:43 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Nov 2021 06:56:48 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Nov 2021 06:56:49 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Nov 2021 06:57:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Nov 2021 06:57:27 GMT
VOLUME [/spiped]
# Sat, 13 Nov 2021 06:57:27 GMT
WORKDIR /spiped
# Sat, 13 Nov 2021 06:57:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Nov 2021 06:57:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:57:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbee8633a3e2da897713dd8453113fc924e1ad102e43bc673e5aa4e72a3c5ff6`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b421d84dfbecebc99f29f801626a8781142421b8affb55b6dac49de522afdd86`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 7.8 KB (7780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c67a331696441ca0da524281edcd53ee4b8d52a24b4fdaab4f5b2e3833ab74a`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 203.0 KB (202993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ab514374a45d9fd16341748dc013e94fd9ddf0b15c2f3666bea84a2c2db7dd`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526ec51047ed2d4267785d4387f46cebef6e388cb755c73b640a73e44db871b6`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:8b3e418343ca28cc6af7c79a9c92f500d16214863644d56f2e6a6c6a66f457d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2644452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3edd8179550b7c42a3827056d11ba4da9c0f384e1b5ac66177b911a1a9f75acc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:09:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 19:09:21 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 19:09:22 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 19:09:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 19:09:55 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 19:09:56 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 19:09:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 19:09:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 19:09:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2462c3e2387f9df1b6daae812a3674ccd49db10b9b7251881ea1a034a39185b`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e4892bdd8b9be427ec2794ea13c95ec6cca78353d3c032d0fd2ba5acf9bae3`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 7.8 KB (7791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624ff05273c8a204e1361bc188430fe618799c3ec5471284aa49a1f9bd365020`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 196.3 KB (196302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f127d56c30dd5e8a58309b3d42c9c4f974256b6b1f1f9ff32b0ff78d8c372b3b`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab7e0d291c6010513c0721d4abf0cd1f407a631c23f515859004dddf983c5f5`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:cbaa0533059fb17c768fe05790c3675b5b5cecf35f0b461e5347d763b1322af8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2932006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a49787cc7861893f9d6020342db1639e60d7af6850ca4866d08840d8438a2b0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:19:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 18:19:33 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 18:19:34 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 18:19:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 18:19:55 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 18:19:56 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 18:19:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 18:19:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 18:19:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbcce6bf922e4817964b0a9575d547fbb39004874a87c290658dcbb8939209e`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b342172a90f6f6a837eeb8f0025e02facad5a97fdd12c0aeac68c2411928d16f`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 7.8 KB (7751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8a670bc36ab2f74e650d7cb573c4c3542673b9488e2659efbc0d6b9db67529`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 204.9 KB (204879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698de19c09a4c9763fb04c4946f3bffafe6556fcfe73a3d55bbb4255f65bd458`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d1aa9a890181cdc95e60ea01849306cb72c967e13716722baa68c7bca76fdb`  
		Last Modified: Fri, 12 Nov 2021 18:20:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:ed9db1b4a0c65f0ca88573ca4e82bafaedde5032f465971dba93432ddcf67f67
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3064332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04afce967f7cf45ad1faa0b6e1d955f2bad9d1aff37c3659db5e809170762140`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 20:40:39 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 20:40:41 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 20:40:41 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 20:41:13 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 20:41:14 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 20:41:14 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 20:41:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 20:41:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 20:41:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abea20678ed9ffc78867f8fc9674162184169da3d7c198cd24ec6b7439e0c88`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f04cc4ba71752a6b9075421e6b0b7f08625406fb105f85e23547c4eb23b25f3`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 7.8 KB (7770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae957cbfbd7f9f36494cb3954e91d1ead35e68d61bbddf48904c4b6133c4c878`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 223.9 KB (223875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911b8888c5d7d41e887ed34d5f9c93d1d3241ad814e69f4d7def6b5debc96ae8`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d46a3df042754e1b8e655e102bf789f899a1f3758442759be66fe90573dbd2`  
		Last Modified: Fri, 12 Nov 2021 20:41:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:3c83af52715b14ccfd27cc89b7b988ae73b9d05500efd053b99b027c0328f14d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f59b6df7881927f19f4b2dcab5974d93c4284e7e9ba9c21098a82d888389b26`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:36:44 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 27 Aug 2021 21:36:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 27 Aug 2021 21:37:02 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 27 Aug 2021 21:37:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 27 Aug 2021 21:37:41 GMT
VOLUME [/spiped]
# Fri, 27 Aug 2021 21:37:48 GMT
WORKDIR /spiped
# Fri, 27 Aug 2021 21:37:54 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 27 Aug 2021 21:38:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:38:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f143c775bd94ef9de49da05aab2353301bc02ceb74a237332f8d9b23e193234b`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9067169d42bea9851adf89b67776e5a280513855fb73120a8d2c5f0051a1097b`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 7.3 KB (7292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe10232ba40d32a7b84a0fe16aa0a2b418d2bdf093335c9fbaf56b08e751c54e`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 221.2 KB (221238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c7d84f077aa3ad717767ac56d4b1ea509bc7a9c81e57e3f4e210fe09205ee9`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c90dd2a4fa5a2acd662ddc7f2ec01550257e4bbaae18ab7a94fdd288523cf8`  
		Last Modified: Fri, 27 Aug 2021 21:38:57 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:118a8c071df238ccc4affa6c1ad90ecaa58fd6f20861ee190449b34b1f5734bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2824562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a068554fae2e46941a18261fe2601c6c40df867a7b227b9bf154694451ba5390`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:55:55 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 19:55:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 19:55:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 19:56:06 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 19:56:06 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 19:56:06 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 19:56:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 19:56:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 19:56:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc797db23a37010d6b83bb8a9eaa1336ed352043857e5a44d68a4b8efad9e0b5`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44e810eed7330856c73daba855bc8adf50fdde87ccab6697c3416ee314886ca`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 7.8 KB (7775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95a425358f95dbc88c89aac4c0c745bacaceb3d4598a051af18b0df4a28d76e`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 205.8 KB (205773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9c7009eddad4f11d690d41e57f47828edf66b3f5113d35cf2a68eee8beed75`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5522513383757fa4cc180054c6b6b641c302050e0dce5ddfdd2a8881e7efcfa2`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
