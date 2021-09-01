## `notary:signer-0.6.1-2`

```console
$ docker pull notary@sha256:04b7be35ca67b6c33522291fac2e04983d4be70e466b8c877e8da84226f55575
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `notary:signer-0.6.1-2` - linux; amd64

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

### `notary:signer-0.6.1-2` - linux; arm variant v6

```console
$ docker pull notary@sha256:08a7d986cde56e860f55d17b4865535fe9d883afe86e5d4f4e877f51a01cc644
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7571049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed52853824344951a125faedfb6fe047b5bb3a6167af2eff24278cd72b93a1f9`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Fri, 30 Jul 2021 17:49:55 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Fri, 30 Jul 2021 17:49:55 GMT
CMD ["/bin/sh"]
# Sat, 31 Jul 2021 02:43:20 GMT
ENV TAG=v0.6.1
# Sat, 31 Jul 2021 02:43:21 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Sat, 31 Jul 2021 02:44:02 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 31 Jul 2021 02:44:03 GMT
EXPOSE 4444
# Sat, 31 Jul 2021 02:44:03 GMT
EXPOSE 7899
# Sat, 31 Jul 2021 02:44:04 GMT
WORKDIR /notary/signer
# Sat, 31 Jul 2021 02:44:27 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Sat, 31 Jul 2021 02:44:27 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Sat, 31 Jul 2021 02:44:28 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Sat, 31 Jul 2021 02:44:29 GMT
RUN adduser -D -H -g "" notary
# Sat, 31 Jul 2021 02:44:29 GMT
USER notary
# Sat, 31 Jul 2021 02:44:30 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 31 Jul 2021 02:44:30 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 31 Jul 2021 02:44:31 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ae4806418df5794a462b18bc4b0ad607b204987f14c99da86397001fd19e45`  
		Last Modified: Sat, 31 Jul 2021 02:45:19 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a42e2070e5be5f259eaee7bf2fd0e62681ef7327242b0c1c59e3bd86766a26`  
		Last Modified: Sat, 31 Jul 2021 02:45:22 GMT  
		Size: 4.9 MB (4946856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d096c848d49da6651208f26cd0cc3e1afa855d014851256996dd48ff7cb0600`  
		Last Modified: Sat, 31 Jul 2021 02:45:19 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a673a7109ff10c4d9303475b671eb07c6c5812401f28560460c09c3442b9bef6`  
		Last Modified: Sat, 31 Jul 2021 02:45:19 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70335aa62b00dda3b49924d22426249b09e4ea87f49da413f7a0640aa5e14cf`  
		Last Modified: Sat, 31 Jul 2021 02:45:19 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.6.1-2` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:e19752489373db10f56262f344c89be563600cddb33e8c5d4a3abbc9acc5670e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7573089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2254205dd7846938c0ac120f7dbea8e1e599587ea179df8844cb31f07ff75ff8`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 18:41:01 GMT
ENV TAG=v0.6.1
# Mon, 28 Jun 2021 18:41:02 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Mon, 28 Jun 2021 18:41:24 GMT
ENV INSTALLDIR=/notary/signer
# Mon, 28 Jun 2021 18:41:24 GMT
EXPOSE 4444
# Mon, 28 Jun 2021 18:41:24 GMT
EXPOSE 7899
# Mon, 28 Jun 2021 18:41:25 GMT
WORKDIR /notary/signer
# Mon, 28 Jun 2021 18:41:37 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Mon, 28 Jun 2021 18:41:37 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Mon, 28 Jun 2021 18:41:37 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Mon, 28 Jun 2021 18:41:38 GMT
RUN adduser -D -H -g "" notary
# Mon, 28 Jun 2021 18:41:38 GMT
USER notary
# Mon, 28 Jun 2021 18:41:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Mon, 28 Jun 2021 18:41:39 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 28 Jun 2021 18:41:39 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e0fa12a850c2f663003533004002c3664154fb7307d828429951110aea9687`  
		Last Modified: Mon, 28 Jun 2021 18:42:10 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67cc19b70d16f873d8a25077e7bd2500fb24d123420d888749ffc0d11f7d59a`  
		Last Modified: Mon, 28 Jun 2021 18:42:12 GMT  
		Size: 4.9 MB (4859004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0cd0fde5328be58b614777c8091540330fd526e335bde638d0b9d821466686`  
		Last Modified: Mon, 28 Jun 2021 18:42:11 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc841fa62e30dfe11784ad16c822ba548417e18f4e6107ef0df194e876e28b62`  
		Last Modified: Mon, 28 Jun 2021 18:42:10 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd2c83faeb5b5184924d2676aec91258a21b56491aad1a5d32fbd57150b15f7`  
		Last Modified: Mon, 28 Jun 2021 18:42:10 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.6.1-2` - linux; 386

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

### `notary:signer-0.6.1-2` - linux; ppc64le

```console
$ docker pull notary@sha256:07e24637d49ca25088b120b1a1e9e9ea95814f67a9932503f32f19a2d9608837
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7549903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f879ba72b6cf7635744460b37589ef90aa5dd92888ba9f175f6dfae3efc4093`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Fri, 30 Jul 2021 17:24:49 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Fri, 30 Jul 2021 17:24:54 GMT
CMD ["/bin/sh"]
# Sat, 31 Jul 2021 04:43:11 GMT
ENV TAG=v0.6.1
# Sat, 31 Jul 2021 04:43:14 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Sat, 31 Jul 2021 04:44:37 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 31 Jul 2021 04:44:43 GMT
EXPOSE 4444
# Sat, 31 Jul 2021 04:44:46 GMT
EXPOSE 7899
# Sat, 31 Jul 2021 04:44:52 GMT
WORKDIR /notary/signer
# Sat, 31 Jul 2021 04:45:18 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Sat, 31 Jul 2021 04:45:20 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Sat, 31 Jul 2021 04:45:22 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Sat, 31 Jul 2021 04:45:29 GMT
RUN adduser -D -H -g "" notary
# Sat, 31 Jul 2021 04:45:32 GMT
USER notary
# Sat, 31 Jul 2021 04:45:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 31 Jul 2021 04:45:40 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 31 Jul 2021 04:45:44 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f507d39470f2c5dbd0d45592bb935dd4d178c24d06f55faf629c7830ca6b782c`  
		Last Modified: Sat, 31 Jul 2021 04:46:26 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4633495152cc67738176b22d6304f6bac68442d9400d454facaebca5c1715b1`  
		Last Modified: Sat, 31 Jul 2021 04:46:26 GMT  
		Size: 4.7 MB (4734705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c294a995bd497e8a8f5dc3527c67764585b872f34b6a125a015b9f141e8160b7`  
		Last Modified: Sat, 31 Jul 2021 04:46:25 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efaf1635ac000a3a3bd0786664864e12ccca533c659437d5e37a5575eb9cdcee`  
		Last Modified: Sat, 31 Jul 2021 04:46:25 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2713350a83c3c79ca672a40dccae1cff6a375406f069d7bbe703dc55f3e4d391`  
		Last Modified: Sat, 31 Jul 2021 04:46:25 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.6.1-2` - linux; s390x

```console
$ docker pull notary@sha256:37c424427968eb61b2a733cd84cfc11f2f03a0c95b33f4cbef497029e1076d2b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7712180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13230d5aa36d35fcd6fccbb6e3a7c53b3728c646d12e70f982f919b58de56553`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Fri, 30 Jul 2021 17:41:41 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Fri, 30 Jul 2021 17:41:42 GMT
CMD ["/bin/sh"]
# Sat, 31 Jul 2021 01:20:21 GMT
ENV TAG=v0.6.1
# Sat, 31 Jul 2021 01:20:21 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Sat, 31 Jul 2021 01:20:57 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 31 Jul 2021 01:20:58 GMT
EXPOSE 4444
# Sat, 31 Jul 2021 01:20:58 GMT
EXPOSE 7899
# Sat, 31 Jul 2021 01:20:58 GMT
WORKDIR /notary/signer
# Sat, 31 Jul 2021 01:21:14 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Sat, 31 Jul 2021 01:21:15 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Sat, 31 Jul 2021 01:21:15 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Sat, 31 Jul 2021 01:21:16 GMT
RUN adduser -D -H -g "" notary
# Sat, 31 Jul 2021 01:21:16 GMT
USER notary
# Sat, 31 Jul 2021 01:21:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 31 Jul 2021 01:21:17 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 31 Jul 2021 01:21:17 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b849a928a0f5ef07d106fec72d69a77a34a3925882e2cdc85f7caed0b391d019`  
		Last Modified: Sat, 31 Jul 2021 01:21:50 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d051d00442db8f302e58f0a77f90953a0cf0fde96321b977824a1631171cc8ce`  
		Last Modified: Sat, 31 Jul 2021 01:21:50 GMT  
		Size: 5.1 MB (5107467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e8df3e876d92c775e0ab86db86acaecb28750ef3efce00d672f7e2cf0b59a7`  
		Last Modified: Sat, 31 Jul 2021 01:21:49 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabf6a0e60ddf4da93740d97cfbd1c183a2bbf869f0c79f9984a3d42da1fe34d`  
		Last Modified: Sat, 31 Jul 2021 01:21:49 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3d7cc3ecb1c102d7cbca0ce30d7f5f4d8e6a884d1625d4a47fdd6e312e7cb6`  
		Last Modified: Sat, 31 Jul 2021 01:21:49 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
