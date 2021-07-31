## `notary:signer`

```console
$ docker pull notary@sha256:bc95cfa9fff50241f55206e5aace8a456c10b8e6974317b3d79119cc7afc3cf8
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
$ docker pull notary@sha256:ef452f69cb0136c87ef982cd9865fffb0192804c40173c9c9424ba70f0023e1d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8074897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31c0d72e66a1e64dfb64930956bd35c02bb493d2e1ef07ad4d22001eec04efe4`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 18:58:36 GMT
ENV TAG=v0.6.1
# Mon, 28 Jun 2021 18:58:36 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Mon, 28 Jun 2021 18:58:57 GMT
ENV INSTALLDIR=/notary/signer
# Mon, 28 Jun 2021 18:58:58 GMT
EXPOSE 4444
# Mon, 28 Jun 2021 18:58:58 GMT
EXPOSE 7899
# Mon, 28 Jun 2021 18:58:58 GMT
WORKDIR /notary/signer
# Mon, 28 Jun 2021 18:59:13 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Mon, 28 Jun 2021 18:59:13 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Mon, 28 Jun 2021 18:59:14 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Mon, 28 Jun 2021 18:59:15 GMT
RUN adduser -D -H -g "" notary
# Mon, 28 Jun 2021 18:59:15 GMT
USER notary
# Mon, 28 Jun 2021 18:59:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Mon, 28 Jun 2021 18:59:15 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 28 Jun 2021 18:59:16 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae06682cc74aa8466b3054395843766c23120c08700730d982412a347acbd357`  
		Last Modified: Mon, 28 Jun 2021 18:59:39 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022ee6e7927e718ca2d541751d63f2ad8566f9e5ef7c0e8796fcc5874462afce`  
		Last Modified: Mon, 28 Jun 2021 18:59:40 GMT  
		Size: 5.3 MB (5260868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d436ae8c1f852ceff180862c1fb9f94c26c0f4e84e247c2d140c16fd33a7cb7f`  
		Last Modified: Mon, 28 Jun 2021 18:59:39 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d5760f441337852538af88eb3dfdeb457f91fc92fd98266abe4a07be6a14ea`  
		Last Modified: Mon, 28 Jun 2021 18:59:39 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4333e4c4880d9a95b9641756fe7b44a8a89f7a4211c90c2b3c2e224ca1acaf87`  
		Last Modified: Mon, 28 Jun 2021 18:59:39 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; arm variant v6

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

### `notary:signer` - linux; arm64 variant v8

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

### `notary:signer` - linux; 386

```console
$ docker pull notary@sha256:a77c5117d447096a45dfdbc9c96f8dceb7ac812af2313b3f5ef318d5a9ab6be0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7827291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5fd81c0349dc3ae9d3c371739ac979143231a119f8d0c6ba9a4fed520a29b1f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 18:42:39 GMT
ENV TAG=v0.6.1
# Mon, 28 Jun 2021 18:42:40 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Mon, 28 Jun 2021 18:43:24 GMT
ENV INSTALLDIR=/notary/signer
# Mon, 28 Jun 2021 18:43:24 GMT
EXPOSE 4444
# Mon, 28 Jun 2021 18:43:24 GMT
EXPOSE 7899
# Mon, 28 Jun 2021 18:43:25 GMT
WORKDIR /notary/signer
# Mon, 28 Jun 2021 18:43:51 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Mon, 28 Jun 2021 18:43:51 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Mon, 28 Jun 2021 18:43:51 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Mon, 28 Jun 2021 18:43:53 GMT
RUN adduser -D -H -g "" notary
# Mon, 28 Jun 2021 18:43:53 GMT
USER notary
# Mon, 28 Jun 2021 18:43:53 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Mon, 28 Jun 2021 18:43:53 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 28 Jun 2021 18:43:54 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d582fd18e358e07f4b30fada572cdf6e1e982085d7817893216ab3869c1b6e9`  
		Last Modified: Mon, 28 Jun 2021 18:44:33 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42f58a11c6ddc2c120eb603e6a5f89be19a72fdc1b3a4689c7c1283e795f956`  
		Last Modified: Mon, 28 Jun 2021 18:44:34 GMT  
		Size: 5.0 MB (5006330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c9c0b37a49135e20513806760b105056477a33ce4e73d61fad7d66e755afef`  
		Last Modified: Mon, 28 Jun 2021 18:44:33 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cc9cacf53edb0f2cc407630af58061218c31aacee52b18a5e99aa909ddf5af`  
		Last Modified: Mon, 28 Jun 2021 18:44:33 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61176d5608e956b55974fc3102a3779c89d4b397e32dbe2e8375ec84392a6831`  
		Last Modified: Mon, 28 Jun 2021 18:44:33 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; ppc64le

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

### `notary:signer` - linux; s390x

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
