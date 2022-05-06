## `notary:signer`

```console
$ docker pull notary@sha256:20b0331c2ee1bd5cd925e351fdf216ebac3e5097444cc6718e2bd78e6b0e396d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `notary:signer` - linux; amd64

```console
$ docker pull notary@sha256:2f763cf1b81280dcc619ae939dcf5b68e6293f26558c4714f5c2e3dcfd106c26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7386127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5edde2ddf99a773bf18a849896655bb5990aa961a23400d04432f8e29a44e2e6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Thu, 28 Apr 2022 21:36:58 GMT
ENV TAG=v0.7.0
# Thu, 28 Apr 2022 21:36:58 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Thu, 28 Apr 2022 21:37:18 GMT
ENV INSTALLDIR=/notary/signer
# Thu, 28 Apr 2022 21:37:18 GMT
EXPOSE 4444
# Thu, 28 Apr 2022 21:37:18 GMT
EXPOSE 7899
# Thu, 28 Apr 2022 21:37:18 GMT
WORKDIR /notary/signer
# Thu, 28 Apr 2022 21:37:36 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Thu, 28 Apr 2022 21:37:36 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Thu, 28 Apr 2022 21:37:36 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Thu, 28 Apr 2022 21:37:37 GMT
RUN adduser -D -H -g "" notary
# Thu, 28 Apr 2022 21:37:37 GMT
USER notary
# Thu, 28 Apr 2022 21:37:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Thu, 28 Apr 2022 21:37:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 28 Apr 2022 21:37:37 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31628c9a541bb82803f9004a7305095e1b7cb39d126593e9804c142df371cad9`  
		Last Modified: Thu, 28 Apr 2022 21:38:00 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d580c01df9d33abde1c529727fcb94adf353f4ecaefe780ca1cf294b4e37428`  
		Last Modified: Thu, 28 Apr 2022 21:38:01 GMT  
		Size: 4.6 MB (4569496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689c44b54e9065c0ff0a3c2ba4dcc8c99cbc27d833bd3b1dcc849b20a7069969`  
		Last Modified: Thu, 28 Apr 2022 21:38:00 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e35bc4a1d17aeefcc4e7a29ff3aa2056821ece2283a0a4e0911ffcf6d62ade`  
		Last Modified: Thu, 28 Apr 2022 21:38:00 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43020eb6c4608db60cace8eabdff8e0f4a87bb1f132f73edb567e2ed97cb7b0a`  
		Last Modified: Thu, 28 Apr 2022 21:38:00 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; arm variant v6

```console
$ docker pull notary@sha256:8d4888dd7e5145ba2af72ab0cb9575317446a766a3bac6deb3393610230716bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6879729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:612404cd2c4fc5d894c89434d87a0c32b476d973ff35691d9867f0cbbe771ad9`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Thu, 28 Apr 2022 20:49:39 GMT
ENV TAG=v0.7.0
# Thu, 28 Apr 2022 20:49:40 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Thu, 28 Apr 2022 20:50:29 GMT
ENV INSTALLDIR=/notary/signer
# Thu, 28 Apr 2022 20:50:30 GMT
EXPOSE 4444
# Thu, 28 Apr 2022 20:50:30 GMT
EXPOSE 7899
# Thu, 28 Apr 2022 20:50:31 GMT
WORKDIR /notary/signer
# Thu, 28 Apr 2022 20:51:06 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Thu, 28 Apr 2022 20:51:06 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Thu, 28 Apr 2022 20:51:07 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Thu, 28 Apr 2022 20:51:08 GMT
RUN adduser -D -H -g "" notary
# Thu, 28 Apr 2022 20:51:09 GMT
USER notary
# Thu, 28 Apr 2022 20:51:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Thu, 28 Apr 2022 20:51:10 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 28 Apr 2022 20:51:10 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf102d23343dedb09bcb9a119f319ba580bf1940bd352dfd6432baa28729ede`  
		Last Modified: Thu, 28 Apr 2022 20:51:53 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041ab37ba1051a2a7588da13a05e6937ea5138f13b1dde78ec12d063b14e7cec`  
		Last Modified: Thu, 28 Apr 2022 20:51:56 GMT  
		Size: 4.3 MB (4255685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d98acc7eab3092876444f74ff4b02a80458e0406edd70f53c9c7917eb71187`  
		Last Modified: Thu, 28 Apr 2022 20:51:53 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48577230ef1fdcfc2a42ed9e03fc2e342a8e62c376f4966ac2b7563323c7b0c5`  
		Last Modified: Thu, 28 Apr 2022 20:51:53 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c5eb4bdd89492ad6a078706b98c6086325b801a81e2339b68d6bfd29420f44`  
		Last Modified: Thu, 28 Apr 2022 20:51:53 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:7a9a154671aae54e66ae934eda9d351a9f0e94e6f6051e25152fd89557207154
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7841091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2cef4bf442a1e88d5a920d55d9dd600f99ba2784e4c81a33821ceb0ec4220c6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:53 GMT
ADD file:a2a992b7f6af1e6f8f5648f329f4a4058d8c4377417ac23ae211290c0cdc8f4b in / 
# Mon, 04 Apr 2022 23:39:53 GMT
CMD ["/bin/sh"]
# Fri, 06 May 2022 01:04:59 GMT
ENV TAG=v0.7.0
# Fri, 06 May 2022 01:05:00 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Fri, 06 May 2022 01:05:31 GMT
ENV INSTALLDIR=/notary/signer
# Fri, 06 May 2022 01:05:31 GMT
EXPOSE 4444
# Fri, 06 May 2022 01:05:32 GMT
EXPOSE 7899
# Fri, 06 May 2022 01:05:33 GMT
WORKDIR /notary/signer
# Fri, 06 May 2022 01:05:46 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --version
# Fri, 06 May 2022 01:05:48 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Fri, 06 May 2022 01:05:49 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Fri, 06 May 2022 01:05:49 GMT
RUN adduser -D -H -g "" notary
# Fri, 06 May 2022 01:05:50 GMT
USER notary
# Fri, 06 May 2022 01:05:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Fri, 06 May 2022 01:05:52 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 06 May 2022 01:05:53 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:0eeab5c200691bd777e227c6eea27f7ca3c8232b67118a76edac2dcde3186aa1`  
		Last Modified: Mon, 04 Apr 2022 23:41:02 GMT  
		Size: 2.7 MB (2716243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97cf437e97bb18b23e8738bd6a0b24c57c968229af758dedf8b88b43bfa29d71`  
		Last Modified: Fri, 06 May 2022 01:06:26 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8de63c68835afb5132d090b373b5f01a96af21d75898f7d83c864542cfda612`  
		Last Modified: Fri, 06 May 2022 01:06:27 GMT  
		Size: 5.1 MB (5122824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:addcd789570140c19b150e5762cf103cae080a8afe76d68fef8343278994ba36`  
		Last Modified: Fri, 06 May 2022 01:06:26 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5183beb303d6ceff1b263a554d7672189d3c9289feb6ab244e1927a892d16ae`  
		Last Modified: Fri, 06 May 2022 01:06:26 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18a0736d73a7eab449dff23e209e70596bfb2cbaecb420c43af812eb10d5cec`  
		Last Modified: Fri, 06 May 2022 01:06:26 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; 386

```console
$ docker pull notary@sha256:7a72bcfc153b68bae8a8db4e158eab27d9da5ba345d71a5339ae9c1f9f6cd022
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7103425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccac34f5c37e0296ce92f89327c4181c70dc331a6bbcc409e40b73835632b475`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Thu, 28 Apr 2022 20:58:57 GMT
ENV TAG=v0.7.0
# Thu, 28 Apr 2022 20:58:58 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Thu, 28 Apr 2022 20:59:34 GMT
ENV INSTALLDIR=/notary/signer
# Thu, 28 Apr 2022 20:59:34 GMT
EXPOSE 4444
# Thu, 28 Apr 2022 20:59:35 GMT
EXPOSE 7899
# Thu, 28 Apr 2022 20:59:36 GMT
WORKDIR /notary/signer
# Thu, 28 Apr 2022 20:59:51 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Thu, 28 Apr 2022 20:59:53 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Thu, 28 Apr 2022 20:59:54 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Thu, 28 Apr 2022 20:59:54 GMT
RUN adduser -D -H -g "" notary
# Thu, 28 Apr 2022 20:59:55 GMT
USER notary
# Thu, 28 Apr 2022 20:59:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Thu, 28 Apr 2022 20:59:57 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 28 Apr 2022 20:59:58 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f724e35e24388ab569d2f65adde8a6c858d53b36bd0529cbfb3912760e1af6`  
		Last Modified: Thu, 28 Apr 2022 21:00:27 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c160316c33705a9a1f8d102a9e0c1d45be84daef8276803929f1f87bac9d52`  
		Last Modified: Thu, 28 Apr 2022 21:00:28 GMT  
		Size: 4.3 MB (4282413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5eb9e649152fe79f790cc90eb6a533fc9fd5b83842b73675fae264ea7e8097`  
		Last Modified: Thu, 28 Apr 2022 21:00:27 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ddc4763819956851c5946237b7083d88018975410da6ec420806f7a17040cb`  
		Last Modified: Thu, 28 Apr 2022 21:00:27 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ee26a298d6ca79d29a7a5ba201cf40df27f9a6fecbddb4e84866702f7ca53f`  
		Last Modified: Thu, 28 Apr 2022 21:00:27 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; ppc64le

```console
$ docker pull notary@sha256:f2b6b54a3a591c6497cb5f15d4452c7f3cd9263bdb26d784492a019857a25560
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6842333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:970f517e4a7642341ebffdd6be225be8e6ad42a0119280910895f41e61d4195e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Thu, 28 Apr 2022 22:16:20 GMT
ENV TAG=v0.7.0
# Thu, 28 Apr 2022 22:16:25 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Thu, 28 Apr 2022 22:17:30 GMT
ENV INSTALLDIR=/notary/signer
# Thu, 28 Apr 2022 22:17:32 GMT
EXPOSE 4444
# Thu, 28 Apr 2022 22:17:35 GMT
EXPOSE 7899
# Thu, 28 Apr 2022 22:17:38 GMT
WORKDIR /notary/signer
# Thu, 28 Apr 2022 22:18:05 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Thu, 28 Apr 2022 22:18:07 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Thu, 28 Apr 2022 22:18:08 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Thu, 28 Apr 2022 22:18:14 GMT
RUN adduser -D -H -g "" notary
# Thu, 28 Apr 2022 22:18:16 GMT
USER notary
# Thu, 28 Apr 2022 22:18:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Thu, 28 Apr 2022 22:18:19 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 28 Apr 2022 22:18:21 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907bd996df5e20f736e244be138c5d0a13d12aacf80718430fd93d0c8adf8ce0`  
		Last Modified: Thu, 28 Apr 2022 22:18:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7f22e435770e2e981fb63a2d7b19dfc205b522c8b813b704abc93155ccb045`  
		Last Modified: Thu, 28 Apr 2022 22:18:59 GMT  
		Size: 4.0 MB (4029083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09106367f05991bc9040f5042746c30f113c814e4ce8cdf24343facf5287cb42`  
		Last Modified: Thu, 28 Apr 2022 22:18:57 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de253ec42299bef9121626500b8a626e9baa5187a1b4ea992573982a833ff996`  
		Last Modified: Thu, 28 Apr 2022 22:18:57 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7503605b578eee040405bed3c5df273d3988111f62a3ffa8f67075698bfeb3bf`  
		Last Modified: Thu, 28 Apr 2022 22:18:57 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; s390x

```console
$ docker pull notary@sha256:f5e5eddff3b98a08b2ee358d90716e7596453d606f243cc0adbb5180b32f3b98
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6957362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0395633a6a7cf89896434466267ae131de4e4104e4b341ad36d948492f9999b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Thu, 28 Apr 2022 20:56:22 GMT
ENV TAG=v0.7.0
# Thu, 28 Apr 2022 20:56:22 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Thu, 28 Apr 2022 20:56:46 GMT
ENV INSTALLDIR=/notary/signer
# Thu, 28 Apr 2022 20:56:46 GMT
EXPOSE 4444
# Thu, 28 Apr 2022 20:56:46 GMT
EXPOSE 7899
# Thu, 28 Apr 2022 20:56:47 GMT
WORKDIR /notary/signer
# Thu, 28 Apr 2022 20:57:02 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Thu, 28 Apr 2022 20:57:02 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Thu, 28 Apr 2022 20:57:02 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Thu, 28 Apr 2022 20:57:03 GMT
RUN adduser -D -H -g "" notary
# Thu, 28 Apr 2022 20:57:03 GMT
USER notary
# Thu, 28 Apr 2022 20:57:03 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Thu, 28 Apr 2022 20:57:03 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 28 Apr 2022 20:57:03 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba6f43699879f123f5489bad9babf4720c55c8f1a1be8ba46a383c198239f8e`  
		Last Modified: Thu, 28 Apr 2022 20:57:28 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea2ec1522796e14148aa6955a72be1bb92fb15b78ab2b10f71ae533d5e285fc`  
		Last Modified: Thu, 28 Apr 2022 20:57:29 GMT  
		Size: 4.4 MB (4354924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec10649c4b92c851be3e160f239feda2e97e44ef71f24473b510cad6b2c3cb0`  
		Last Modified: Thu, 28 Apr 2022 20:57:28 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99fb5cd81aa7d5bc7d7c388f85056ee87ef2f9c0e4f29defd7d8392608dec5c1`  
		Last Modified: Thu, 28 Apr 2022 20:57:28 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882ba3748fb331d1d484843ea8ec672ab49944ca31fe9bf4f13132179abc4639`  
		Last Modified: Thu, 28 Apr 2022 20:57:28 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
