## `notary:signer`

```console
$ docker pull notary@sha256:758f9afe17a364540290cc6c0199469cd314fe84e2fe642c5cc1cc53f57fe4e1
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
$ docker pull notary@sha256:a3024c444f372965bb9e02409cbd51cf83cf64e34eb6c2cb59cda240ca1df125
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7688013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26aad70f50d38c07bd7f33356fcb4df3bdaaec3a4831c088d8b272bda896ccef`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 03:13:51 GMT
ENV TAG=v0.6.1
# Wed, 01 Sep 2021 03:13:51 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Wed, 01 Sep 2021 03:14:17 GMT
ENV INSTALLDIR=/notary/signer
# Wed, 01 Sep 2021 03:14:17 GMT
EXPOSE 4444
# Wed, 01 Sep 2021 03:14:17 GMT
EXPOSE 7899
# Wed, 01 Sep 2021 03:14:17 GMT
WORKDIR /notary/signer
# Wed, 01 Sep 2021 03:14:36 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Wed, 01 Sep 2021 03:14:36 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Wed, 01 Sep 2021 03:14:36 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Wed, 01 Sep 2021 03:14:37 GMT
RUN adduser -D -H -g "" notary
# Wed, 01 Sep 2021 03:14:37 GMT
USER notary
# Wed, 01 Sep 2021 03:14:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Wed, 01 Sep 2021 03:14:38 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Sep 2021 03:14:38 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0640cea0fffa153e8a43f0cc1bba1b442e6294eba3a414a7326a92ae1774d9e`  
		Last Modified: Wed, 01 Sep 2021 03:15:03 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3826f26db296ff4a05ad4906679d7baae10106106a52ebe02a1d5eade5d6177f`  
		Last Modified: Wed, 01 Sep 2021 03:15:04 GMT  
		Size: 4.9 MB (4871876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e403c8609bed446927d18879dab4a45d49fa3bfac062d23d1f193b6912542a`  
		Last Modified: Wed, 01 Sep 2021 03:15:03 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2d426533852ba181bb1c0526d7e9d9947021478043d28a381f7252ced4a368`  
		Last Modified: Wed, 01 Sep 2021 03:15:03 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70ee8e69aa78933fce9ce6c3d810dee7282f82b7277216c5129e46719bc091d`  
		Last Modified: Wed, 01 Sep 2021 03:15:03 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; arm variant v6

```console
$ docker pull notary@sha256:94a6194b7f7b65743f0222dd458b930025c28a770911640c79fad7ca26034b52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7182693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75506eef87a7ee2f483c5172bef11d439f155faebc2b51e581f746c187e02e38`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:33 GMT
ADD file:ed2b5e0fbd1e7ae37ab8f808c827d23c6841ce1edd7427552d5bf741d67ebcc0 in / 
# Tue, 31 Aug 2021 22:30:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 05:40:38 GMT
ENV TAG=v0.6.1
# Wed, 01 Sep 2021 05:40:39 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Wed, 01 Sep 2021 05:41:21 GMT
ENV INSTALLDIR=/notary/signer
# Wed, 01 Sep 2021 05:41:22 GMT
EXPOSE 4444
# Wed, 01 Sep 2021 05:41:23 GMT
EXPOSE 7899
# Wed, 01 Sep 2021 05:41:23 GMT
WORKDIR /notary/signer
# Wed, 01 Sep 2021 05:41:47 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Wed, 01 Sep 2021 05:41:47 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Wed, 01 Sep 2021 05:41:48 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Wed, 01 Sep 2021 05:41:49 GMT
RUN adduser -D -H -g "" notary
# Wed, 01 Sep 2021 05:41:50 GMT
USER notary
# Wed, 01 Sep 2021 05:41:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Wed, 01 Sep 2021 05:41:51 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Sep 2021 05:41:51 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:840d18d84f6afdc3231d126fdd3f84f23f0335b61cbfa9cb8808b888a4308919`  
		Last Modified: Tue, 31 Aug 2021 22:32:11 GMT  
		Size: 2.6 MB (2623761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba84200730013aecb1dcbb2f93f6f7b5c2077317205083389d1ab8544b6c1809`  
		Last Modified: Wed, 01 Sep 2021 05:42:37 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d1061ec4ca2d75dcb091b4aaf6ca4fcc558e626a50113ae6876a02841a3e6c`  
		Last Modified: Wed, 01 Sep 2021 05:42:39 GMT  
		Size: 4.6 MB (4556877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db861ba970aa473981dd5c166a69c29cae305e43fb9742de19c7723eac82079d`  
		Last Modified: Wed, 01 Sep 2021 05:42:37 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba3cdee7eedcaf8d17f5e5291b723564fb8ff012432b70654f56c5451a40e0c`  
		Last Modified: Wed, 01 Sep 2021 05:42:37 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d66f578ac7a54250a9c6b87880a389618b43fb59cd18f3432e5468d962f0daa`  
		Last Modified: Wed, 01 Sep 2021 05:42:37 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:fb7ed690830af9669d67a1ae75c8f4dffb17b7e6025c560b67b63ca53a4eb7ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7175654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:741f4abba1301674a5f4bff763c16fa6b4662476eb21fed799cf5dbbce1bf253`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 13:14:47 GMT
ENV TAG=v0.6.1
# Wed, 01 Sep 2021 13:14:47 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Wed, 01 Sep 2021 13:15:06 GMT
ENV INSTALLDIR=/notary/signer
# Wed, 01 Sep 2021 13:15:07 GMT
EXPOSE 4444
# Wed, 01 Sep 2021 13:15:07 GMT
EXPOSE 7899
# Wed, 01 Sep 2021 13:15:07 GMT
WORKDIR /notary/signer
# Wed, 01 Sep 2021 13:15:19 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Wed, 01 Sep 2021 13:15:19 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Wed, 01 Sep 2021 13:15:19 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Wed, 01 Sep 2021 13:15:20 GMT
RUN adduser -D -H -g "" notary
# Wed, 01 Sep 2021 13:15:20 GMT
USER notary
# Wed, 01 Sep 2021 13:15:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Wed, 01 Sep 2021 13:15:20 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Sep 2021 13:15:20 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2a89ad623fd23dea61788687043be7a36d91a8c2238a5e6a347f587c9dae56`  
		Last Modified: Wed, 01 Sep 2021 13:15:50 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814bdc9ac02933fd670bc30b3981eab3f74fba20c03a283bffda528bff02b685`  
		Last Modified: Wed, 01 Sep 2021 13:15:51 GMT  
		Size: 4.5 MB (4460587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9acac57c1bf0d266951fdabc122a7ec888493dd2682f60a11bea1dd343056d5`  
		Last Modified: Wed, 01 Sep 2021 13:15:50 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6238c358e25f642bf7c4ca3ad169c4ceb05947461bd6cb6b2aaf98b02f659818`  
		Last Modified: Wed, 01 Sep 2021 13:15:51 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f238274b5d9b157f8ba92b90dacab2a5ae21a8308ed1506195f2172d9f149ad`  
		Last Modified: Wed, 01 Sep 2021 13:15:51 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; 386

```console
$ docker pull notary@sha256:f1c03eb045dc97ea17197a0c1cb777c201234ba78a0b54b4df42209369d0df3b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7441323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b4fee68e4fe3c14a89ac9b77ae2d4512de54f2e5123bfc1a0feed63bdbe2855`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Tue, 31 Aug 2021 21:23:28 GMT
ADD file:fb9d541cffc3a5660d23426ba847aa696b59a9d7f14e00ba0a63b28c9ec272c0 in / 
# Tue, 31 Aug 2021 21:23:29 GMT
CMD ["/bin/sh"]
# Tue, 31 Aug 2021 23:39:54 GMT
ENV TAG=v0.6.1
# Tue, 31 Aug 2021 23:39:54 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 31 Aug 2021 23:40:21 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 31 Aug 2021 23:40:22 GMT
EXPOSE 4444
# Tue, 31 Aug 2021 23:40:22 GMT
EXPOSE 7899
# Tue, 31 Aug 2021 23:40:22 GMT
WORKDIR /notary/signer
# Tue, 31 Aug 2021 23:40:42 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Tue, 31 Aug 2021 23:40:42 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Tue, 31 Aug 2021 23:40:43 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Tue, 31 Aug 2021 23:40:43 GMT
RUN adduser -D -H -g "" notary
# Tue, 31 Aug 2021 23:40:44 GMT
USER notary
# Tue, 31 Aug 2021 23:40:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 31 Aug 2021 23:40:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 31 Aug 2021 23:40:44 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:4ed7d06bd90bc8d13b87220ccc6204a7d235ec943be9fb4289d856f9ff0a5b7b`  
		Last Modified: Tue, 31 Aug 2021 21:24:28 GMT  
		Size: 2.8 MB (2821095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081c6e54401247246c2ca4756cf927b72d3e7fe0475427eadf3336126ce70fe8`  
		Last Modified: Tue, 31 Aug 2021 23:41:18 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab536c085215585c4faa4355b6337e17697a20c900ae81f252fb5ffc08f33c31`  
		Last Modified: Tue, 31 Aug 2021 23:41:19 GMT  
		Size: 4.6 MB (4618168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3590fe1d8ea9b1aa7ce1509eff698d62dde081fc7e7747ce9d7997aed7af424f`  
		Last Modified: Tue, 31 Aug 2021 23:41:18 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f255fd7b742ec8e3a6ffbb7edc13de9a72bae61b6944b8d6a34d17aedf9f6451`  
		Last Modified: Tue, 31 Aug 2021 23:41:18 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b07363a7b86ee845044145d80b1f3c112a0316d572fd6ec35d130a4a7b38e5`  
		Last Modified: Tue, 31 Aug 2021 23:41:19 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; ppc64le

```console
$ docker pull notary@sha256:4bdeca529937e2850a303695eba03e4f9ab2c31628723f9029b741b4673a107d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7158965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f76f7a1a7f6c6fd115cc253ddbb2c90a97051427efa82730d437d78661e38192`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Wed, 01 Sep 2021 02:42:40 GMT
ADD file:07a51f1a2f818bd1c1651832ce63cb1e0046a57994724cda6a20ff1a2a685295 in / 
# Wed, 01 Sep 2021 02:42:41 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 11:31:28 GMT
ENV TAG=v0.6.1
# Wed, 01 Sep 2021 11:31:32 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Wed, 01 Sep 2021 11:32:39 GMT
ENV INSTALLDIR=/notary/signer
# Wed, 01 Sep 2021 11:32:41 GMT
EXPOSE 4444
# Wed, 01 Sep 2021 11:32:44 GMT
EXPOSE 7899
# Wed, 01 Sep 2021 11:32:46 GMT
WORKDIR /notary/signer
# Wed, 01 Sep 2021 11:33:14 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Wed, 01 Sep 2021 11:33:15 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Wed, 01 Sep 2021 11:33:16 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Wed, 01 Sep 2021 11:33:22 GMT
RUN adduser -D -H -g "" notary
# Wed, 01 Sep 2021 11:33:25 GMT
USER notary
# Wed, 01 Sep 2021 11:33:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Wed, 01 Sep 2021 11:33:29 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Sep 2021 11:33:34 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:39d9bf63205258fe1d085fd596101e6fc46ff796cda8d3ba2983e166a25b74db`  
		Last Modified: Wed, 01 Sep 2021 02:43:53 GMT  
		Size: 2.8 MB (2814813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a2eff0e92e1ad53c9428e166d4364b007ea8dc3f120a46c44e66b1a9793285`  
		Last Modified: Wed, 01 Sep 2021 11:34:03 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62201ab14baff5eca6c77fe9987be6337c33a61be5459a19d3f82519bce46e68`  
		Last Modified: Wed, 01 Sep 2021 11:34:04 GMT  
		Size: 4.3 MB (4342093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d50f16d86cb7eae39bdab52b4419b44fda4c9c49078615634783e6309b8b6b`  
		Last Modified: Wed, 01 Sep 2021 11:34:03 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4c51e955773f2c1779e4e3c9e46078b1dc534f548fd509bafc5104b40737d9`  
		Last Modified: Wed, 01 Sep 2021 11:34:03 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25c98aa2bbaf8a780b35a62035f88c8ec612bf27e2c2136aa7be3a037df0528`  
		Last Modified: Wed, 01 Sep 2021 11:34:03 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; s390x

```console
$ docker pull notary@sha256:9cd276ae0e3588f236d22894ce69e6ceccfbc962b0750703e943dca1748a4323
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7319621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e955703f6b7232fb67908b577b13716c8281a6160955a18805977ffb25a4351d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Wed, 01 Sep 2021 01:15:21 GMT
ADD file:def74c9e73d87d3c8b94cc0200f2723aea3a7462f8d2e0852db9da25c19855ac in / 
# Wed, 01 Sep 2021 01:15:22 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 13:35:20 GMT
ENV TAG=v0.6.1
# Wed, 01 Sep 2021 13:35:20 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Wed, 01 Sep 2021 13:35:57 GMT
ENV INSTALLDIR=/notary/signer
# Wed, 01 Sep 2021 13:35:57 GMT
EXPOSE 4444
# Wed, 01 Sep 2021 13:35:58 GMT
EXPOSE 7899
# Wed, 01 Sep 2021 13:35:58 GMT
WORKDIR /notary/signer
# Wed, 01 Sep 2021 13:36:14 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Wed, 01 Sep 2021 13:36:15 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Wed, 01 Sep 2021 13:36:15 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Wed, 01 Sep 2021 13:36:16 GMT
RUN adduser -D -H -g "" notary
# Wed, 01 Sep 2021 13:36:17 GMT
USER notary
# Wed, 01 Sep 2021 13:36:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Wed, 01 Sep 2021 13:36:18 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Sep 2021 13:36:18 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:c1d78e8a87395f597d24b8eb78423ccdcfd404846906154e15aea8be9541c3ae`  
		Last Modified: Wed, 01 Sep 2021 01:16:19 GMT  
		Size: 2.6 MB (2604390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb43008fee62b5e3e3ec5c53808af01d83b36eca3389e51b59fd8b8dd7b3062`  
		Last Modified: Wed, 01 Sep 2021 13:36:45 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310856cfdf753cbc9e3d836e7649c47f1384e28310c7e40fde761adea4922de0`  
		Last Modified: Wed, 01 Sep 2021 13:36:46 GMT  
		Size: 4.7 MB (4713171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98aa310a457c135c24463592cb9a4faaf72feaf1d5f7e09b2b1f0d6e48fd4df`  
		Last Modified: Wed, 01 Sep 2021 13:36:45 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b77b283a7995fc60d37fe27da24a1f6fa2995915704557dacfd75bcedc2b820`  
		Last Modified: Wed, 01 Sep 2021 13:36:45 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b404d1871da6d1dc6f0bbb47907b6667ce2058ae7bf86c0acb083e63c5cbde3`  
		Last Modified: Wed, 01 Sep 2021 13:36:45 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
