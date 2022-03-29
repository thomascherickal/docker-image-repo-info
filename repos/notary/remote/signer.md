## `notary:signer`

```console
$ docker pull notary@sha256:59a13eb12fdbb10830b7058fcb3e83e668ec9cf26c2404f974d3cc30faff9b82
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
$ docker pull notary@sha256:5a597b68b254bf6117fbb7b0985cb52a0c0e86d17f91a3e2f68b82a5e60ed6c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7690874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a1b0c0a51a29722cfcf864a2d028631e0853919ca0fc059237081377ad639a0`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:46 GMT
ADD file:a2ef39a587aac85256b55bee81f17d73aaa7154b2a32a31527c7803fb889f2e7 in / 
# Tue, 29 Mar 2022 00:19:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 15:56:36 GMT
ENV TAG=v0.6.1
# Tue, 29 Mar 2022 15:56:36 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 29 Mar 2022 15:56:55 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 29 Mar 2022 15:56:56 GMT
EXPOSE 4444
# Tue, 29 Mar 2022 15:56:56 GMT
EXPOSE 7899
# Tue, 29 Mar 2022 15:56:56 GMT
WORKDIR /notary/signer
# Tue, 29 Mar 2022 15:57:10 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Tue, 29 Mar 2022 15:57:10 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Tue, 29 Mar 2022 15:57:10 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Tue, 29 Mar 2022 15:57:11 GMT
RUN adduser -D -H -g "" notary
# Tue, 29 Mar 2022 15:57:11 GMT
USER notary
# Tue, 29 Mar 2022 15:57:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 29 Mar 2022 15:57:11 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 29 Mar 2022 15:57:11 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:b9c05db88786fd3c89b78787631257301391f898c03ba50553b556630046a741`  
		Last Modified: Tue, 29 Mar 2022 00:20:43 GMT  
		Size: 2.8 MB (2819223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb1082d1643807ceaeb8e590f3432e78d20f6f87149b4b38ea6990bce6a906f`  
		Last Modified: Tue, 29 Mar 2022 15:57:33 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b54f98c8f2aaa0488352c699dc96fbe5687447f43efe4f1e38e3bbc65fd3f4b`  
		Last Modified: Tue, 29 Mar 2022 15:57:34 GMT  
		Size: 4.9 MB (4869596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc364a837c60fc420eaa9f49d15469346627cbed5c2a05c01288d87976ee4233`  
		Last Modified: Tue, 29 Mar 2022 15:57:33 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a7dffcbe64d230591ae8b8763c1ab40e881c5a3d02554bcd52c3e8a6fedf63`  
		Last Modified: Tue, 29 Mar 2022 15:57:33 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7005a3d5fd6b1e09b7b2ef641c2e305005d980afab194064bf4f42963325eb04`  
		Last Modified: Tue, 29 Mar 2022 15:57:33 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; arm variant v6

```console
$ docker pull notary@sha256:e43398af5a51dc91344e33abe8cc1b68c5877cd257a122abb30dc1385d78bd82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7182318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b32666262b52eb80dee7cf63f70dc6ad985b2ca0504e03407b78717525355f4`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:56 GMT
ADD file:23d913551f75313e359a4e93592ea0a9655e1a7c2bec5fddd210717d70c3114b in / 
# Tue, 29 Mar 2022 00:49:57 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:33:10 GMT
ENV TAG=v0.6.1
# Tue, 29 Mar 2022 08:33:11 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 29 Mar 2022 08:34:00 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 29 Mar 2022 08:34:01 GMT
EXPOSE 4444
# Tue, 29 Mar 2022 08:34:01 GMT
EXPOSE 7899
# Tue, 29 Mar 2022 08:34:01 GMT
WORKDIR /notary/signer
# Tue, 29 Mar 2022 08:34:25 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Tue, 29 Mar 2022 08:34:26 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Tue, 29 Mar 2022 08:34:26 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Tue, 29 Mar 2022 08:34:28 GMT
RUN adduser -D -H -g "" notary
# Tue, 29 Mar 2022 08:34:28 GMT
USER notary
# Tue, 29 Mar 2022 08:34:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 29 Mar 2022 08:34:29 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 29 Mar 2022 08:34:30 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:eba0847afba90891ea7dae672f5dadfa405a822df0bc9c00b9e3328fd5fd889c`  
		Last Modified: Tue, 29 Mar 2022 00:51:57 GMT  
		Size: 2.6 MB (2625139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b26d26abde63c15b13e6af115c7c6fb9fc2d22d642357f055785de91cb6483`  
		Last Modified: Tue, 29 Mar 2022 08:35:16 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c91bc37bc68a86160c7f6ab4b50a14877de14d73ea8610a6f44e63e7abb6669`  
		Last Modified: Tue, 29 Mar 2022 08:35:19 GMT  
		Size: 4.6 MB (4555116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4902016b7476344058a8d7a4bba669b89b6270d157c495fbe967027f2de91d9c`  
		Last Modified: Tue, 29 Mar 2022 08:35:15 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:650c019ee1d8315a41d3aa9680e78efd657ec14b10b7de7ad84d2140ab8c539a`  
		Last Modified: Tue, 29 Mar 2022 08:35:16 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0607eba904a7eb637730de293342b19501b3bb9a8af2563aa3cc3e7fb089ac7c`  
		Last Modified: Tue, 29 Mar 2022 08:35:16 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:7a186215872f1c3801ca640e32df5bef70f3d4dda626b07f8d1c4578ec127daa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7176931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d3cefe647af844bbe0906f558647bb943d54c43ffa98ab5367b4bfb557d8c69`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:19 GMT
ADD file:0bbbf3ca52651bbef2547689474beafcef779899da63743efd8166a01d9f3f7a in / 
# Thu, 17 Mar 2022 18:43:20 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 01:06:40 GMT
ENV TAG=v0.6.1
# Sat, 19 Mar 2022 01:06:41 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Sat, 19 Mar 2022 01:07:07 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 19 Mar 2022 01:07:08 GMT
EXPOSE 4444
# Sat, 19 Mar 2022 01:07:09 GMT
EXPOSE 7899
# Sat, 19 Mar 2022 01:07:10 GMT
WORKDIR /notary/signer
# Sat, 19 Mar 2022 01:07:20 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Sat, 19 Mar 2022 01:07:22 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Sat, 19 Mar 2022 01:07:23 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Sat, 19 Mar 2022 01:07:23 GMT
RUN adduser -D -H -g "" notary
# Sat, 19 Mar 2022 01:07:24 GMT
USER notary
# Sat, 19 Mar 2022 01:07:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 19 Mar 2022 01:07:26 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 19 Mar 2022 01:07:27 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:6b5c040bf1f18956758f68628afdc8e179044ac75bcd411134da39a661a772e0`  
		Last Modified: Thu, 17 Mar 2022 18:44:11 GMT  
		Size: 2.7 MB (2719134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d31637a795a9f059af1f95be8849f6be791dde68237d7c86c01454dd572b52a`  
		Last Modified: Sat, 19 Mar 2022 01:07:58 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6255a8d20621a4455617d12053f107406d4975d78567f8c39b3da448abfb2bb8`  
		Last Modified: Sat, 19 Mar 2022 01:07:58 GMT  
		Size: 4.5 MB (4455766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0160fc393462056b86027a87648ed7fea282ec77af91cef287afb242f901e311`  
		Last Modified: Sat, 19 Mar 2022 01:07:58 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:279ee1fa1db3cede4134d5e6f895becf8d3a8fc735510014fc1a38333270ac29`  
		Last Modified: Sat, 19 Mar 2022 01:07:58 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030e2bf09c2d22c09c9c233270e2b5ddd5c4ef8df32d41a0c7ec854801f21ec1`  
		Last Modified: Sat, 19 Mar 2022 01:07:58 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; 386

```console
$ docker pull notary@sha256:d1e41ca16127354a473ab50ecfe3dbb2218900e7bba3d58ad7848907e8b04b44
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7435786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b279ce042847ab5e2613ba443ddfadec0be78dc452c1685075cbb0f95c94cf5e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Tue, 29 Mar 2022 00:38:45 GMT
ADD file:f1abe5c2930209c2d735059c8e767e630c0818cc18a4fd10b0b90e6efbc675e2 in / 
# Tue, 29 Mar 2022 00:38:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 06:00:06 GMT
ENV TAG=v0.6.1
# Tue, 29 Mar 2022 06:00:07 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 29 Mar 2022 06:00:37 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 29 Mar 2022 06:00:38 GMT
EXPOSE 4444
# Tue, 29 Mar 2022 06:00:39 GMT
EXPOSE 7899
# Tue, 29 Mar 2022 06:00:40 GMT
WORKDIR /notary/signer
# Tue, 29 Mar 2022 06:00:51 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Tue, 29 Mar 2022 06:00:53 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Tue, 29 Mar 2022 06:00:54 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Tue, 29 Mar 2022 06:00:54 GMT
RUN adduser -D -H -g "" notary
# Tue, 29 Mar 2022 06:00:55 GMT
USER notary
# Tue, 29 Mar 2022 06:00:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 29 Mar 2022 06:00:57 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 29 Mar 2022 06:00:58 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:dadad3128a09e6d507e89afe042cb1d48da14a72b28ca79dec7c6acf971bd9e6`  
		Last Modified: Tue, 29 Mar 2022 00:40:03 GMT  
		Size: 2.8 MB (2820388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007901d388885795e87bab30fa93738b38540997491c7aa9d5394e7dff978b44`  
		Last Modified: Tue, 29 Mar 2022 06:01:33 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4523fcd851d986eca1f25991fe3c80057aed1c4903505b2483a87641d32d7343`  
		Last Modified: Tue, 29 Mar 2022 06:01:34 GMT  
		Size: 4.6 MB (4613377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6d2f8bbfc6dcd19caf60def2df525745794e7a9333ca5d643ad3d725dd7a0b`  
		Last Modified: Tue, 29 Mar 2022 06:01:33 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36549517e1365949e5f08a32766861b7173556953c36fe39bf205238d2222057`  
		Last Modified: Tue, 29 Mar 2022 06:01:33 GMT  
		Size: 377.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0245f15cec6fc67c4540204f8a118c234d2dd595864055da21543eb145d79d7e`  
		Last Modified: Tue, 29 Mar 2022 06:01:33 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; ppc64le

```console
$ docker pull notary@sha256:28d32bbc4575f6f5b205f3c8d731c9c7fe4f5d18539add28757e9da27d57e65c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7154680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab1b5007de5cc8d26eacefb2bbd7fc47b0d52ad52826d8183409a33bc26f9aec`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Tue, 29 Mar 2022 00:17:21 GMT
ADD file:0f301305d95e2e1e0580ec71f76edab57a1c18ed0adba5d09708b587ec19e622 in / 
# Tue, 29 Mar 2022 00:17:25 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 12:40:53 GMT
ENV TAG=v0.6.1
# Tue, 29 Mar 2022 12:40:54 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 29 Mar 2022 12:42:06 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 29 Mar 2022 12:42:09 GMT
EXPOSE 4444
# Tue, 29 Mar 2022 12:42:12 GMT
EXPOSE 7899
# Tue, 29 Mar 2022 12:42:15 GMT
WORKDIR /notary/signer
# Tue, 29 Mar 2022 12:42:39 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Tue, 29 Mar 2022 12:42:40 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Tue, 29 Mar 2022 12:42:42 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Tue, 29 Mar 2022 12:42:50 GMT
RUN adduser -D -H -g "" notary
# Tue, 29 Mar 2022 12:42:59 GMT
USER notary
# Tue, 29 Mar 2022 12:43:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 29 Mar 2022 12:43:09 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 29 Mar 2022 12:43:13 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:77fcf2c0cc10658b5d6b4e43a75682b8bebbdc2e47895412dd1241c0422b8368`  
		Last Modified: Tue, 29 Mar 2022 00:18:56 GMT  
		Size: 2.8 MB (2814846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cacff4a4ed250261b3768bbfc9708d3da1b5331717d25f86c4c0928e2609079`  
		Last Modified: Tue, 29 Mar 2022 12:43:53 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222b02a3c69a5071e2847e33f670374acb913d4475da9ba50a6783ba1d451b25`  
		Last Modified: Tue, 29 Mar 2022 12:43:54 GMT  
		Size: 4.3 MB (4337776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295ab1754665b939a567857c6fbcf38d773ba83562ac53546e1e3246c54cd41a`  
		Last Modified: Tue, 29 Mar 2022 12:43:53 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542bb77cdd69cc247f93a9cdef415bbd42df299d501c84c773cb89c00c8d133c`  
		Last Modified: Tue, 29 Mar 2022 12:43:53 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7634254911f718d0571952c1c88cdbcf08b66ce4a7266e150a10dda53d468bed`  
		Last Modified: Tue, 29 Mar 2022 12:43:53 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; s390x

```console
$ docker pull notary@sha256:4297e4e5302259953bbfd0747d42575db953ab665fcaf1a6b76c6a0fc9f9ffe3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7313790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17bf63d014899545474153c839259f8d7003c462d6119e39f30bcf88bc7105b9`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:45 GMT
ADD file:08b65c73088f2cc387829e0ce9aa160db404a3e5fa0e4fda048cdbc02d8f64c2 in / 
# Tue, 29 Mar 2022 00:41:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:18:16 GMT
ENV TAG=v0.6.1
# Tue, 29 Mar 2022 11:18:16 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 29 Mar 2022 11:18:38 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 29 Mar 2022 11:18:38 GMT
EXPOSE 4444
# Tue, 29 Mar 2022 11:18:38 GMT
EXPOSE 7899
# Tue, 29 Mar 2022 11:18:38 GMT
WORKDIR /notary/signer
# Tue, 29 Mar 2022 11:18:53 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Tue, 29 Mar 2022 11:18:54 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Tue, 29 Mar 2022 11:18:54 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Tue, 29 Mar 2022 11:18:54 GMT
RUN adduser -D -H -g "" notary
# Tue, 29 Mar 2022 11:18:54 GMT
USER notary
# Tue, 29 Mar 2022 11:18:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 29 Mar 2022 11:18:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 29 Mar 2022 11:18:55 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:89a2ea5c1a3e1d541ae66fbd95d215b39b560c537460c3fc76ad6826582893fe`  
		Last Modified: Tue, 29 Mar 2022 00:47:35 GMT  
		Size: 2.6 MB (2605074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ac5d8b5943f179b16c64910bc48fd499aa21c41988b7624c0dc68d00722ae6`  
		Last Modified: Tue, 29 Mar 2022 11:21:19 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cdafac6ccb7a2b11c2a1af545276b22159c24598c08634bc09222e69d5c613`  
		Last Modified: Tue, 29 Mar 2022 11:21:19 GMT  
		Size: 4.7 MB (4706660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3a581a27946ea536cc943d404787a0689ce4cf258d70b8b332f6395775953b`  
		Last Modified: Tue, 29 Mar 2022 11:21:15 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318594e20762541b71ff092618a6ee9c9ff373980c82bc3b65e5adaff577df54`  
		Last Modified: Tue, 29 Mar 2022 11:21:19 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b195fb8bc296e2295a27228fe70d834c0317902f1d723e80b5fe606ad4d950b`  
		Last Modified: Tue, 29 Mar 2022 11:21:19 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
