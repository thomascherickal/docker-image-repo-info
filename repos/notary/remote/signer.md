## `notary:signer`

```console
$ docker pull notary@sha256:19f5a46fe28ad052158889e7532648ae94184021a1059f19046bb3886929d94a
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
$ docker pull notary@sha256:c1817ce185ca18a6c3d4862bb97defc47f26ecbbbe8f6c696780ec16db6c65a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8364241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5abf773ac8cd02369a31368431b08103726cc068bbe878fbd38360600c257405`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:19 GMT
ADD file:c1aa87a3b464fca64d769444b5201bc0426a1f517c91c4a7916270e10f8b300b in / 
# Tue, 05 Apr 2022 00:20:19 GMT
CMD ["/bin/sh"]
# Fri, 06 May 2022 02:16:09 GMT
ENV TAG=v0.7.0
# Fri, 06 May 2022 02:16:10 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Fri, 06 May 2022 02:16:29 GMT
ENV INSTALLDIR=/notary/signer
# Fri, 06 May 2022 02:16:29 GMT
EXPOSE 4444
# Fri, 06 May 2022 02:16:29 GMT
EXPOSE 7899
# Fri, 06 May 2022 02:16:29 GMT
WORKDIR /notary/signer
# Fri, 06 May 2022 02:16:43 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --version
# Fri, 06 May 2022 02:16:43 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Fri, 06 May 2022 02:16:43 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Fri, 06 May 2022 02:16:44 GMT
RUN adduser -D -H -g "" notary
# Fri, 06 May 2022 02:16:44 GMT
USER notary
# Fri, 06 May 2022 02:16:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Fri, 06 May 2022 02:16:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 06 May 2022 02:16:44 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:1b7ca6aea1ddfe716f3694edb811ab35114db9e93f3ce38d7dab6b4d9270cb0c`  
		Last Modified: Tue, 05 Apr 2022 00:21:10 GMT  
		Size: 2.8 MB (2808060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4903c57b83cca9f1a4b3bb0df929227757e4ab2ce638a482f0c58705b2df0ae4`  
		Last Modified: Fri, 06 May 2022 02:17:08 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbf42816fb6753892686730c3ab27fe445e7026f417e0ffa12c858020231b12`  
		Last Modified: Fri, 06 May 2022 02:17:09 GMT  
		Size: 5.6 MB (5554129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5638bd3072eff25df58f628b236c0f844e800eca5f857cc96c085d8d1018f52`  
		Last Modified: Fri, 06 May 2022 02:17:09 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ce0bfbe59061a70885cf001b4d5b28f2d87332877965a4e59e1744794c0912`  
		Last Modified: Fri, 06 May 2022 02:17:08 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941d4c76df9739633166f31f2defa2217408aabe4973e7e7cd12414aefdd63ca`  
		Last Modified: Fri, 06 May 2022 02:17:08 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; arm variant v6

```console
$ docker pull notary@sha256:ecc9599c6083d660954554c662039feba162e63849b27526878b778b1a20d76e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7832442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3946c21e7d54f760243b7fe6da3fa1f3e09a59649bf464ad052c616407f7efc`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Mon, 04 Apr 2022 23:50:18 GMT
ADD file:a62ad8c2b01195a2d42109e23b6d8ce69e2a816702518b2d823139f28c0ff799 in / 
# Mon, 04 Apr 2022 23:50:19 GMT
CMD ["/bin/sh"]
# Fri, 06 May 2022 02:05:11 GMT
ENV TAG=v0.7.0
# Fri, 06 May 2022 02:05:11 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Fri, 06 May 2022 02:05:55 GMT
ENV INSTALLDIR=/notary/signer
# Fri, 06 May 2022 02:05:55 GMT
EXPOSE 4444
# Fri, 06 May 2022 02:05:55 GMT
EXPOSE 7899
# Fri, 06 May 2022 02:05:56 GMT
WORKDIR /notary/signer
# Fri, 06 May 2022 02:06:20 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --version
# Fri, 06 May 2022 02:06:21 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Fri, 06 May 2022 02:06:21 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Fri, 06 May 2022 02:06:23 GMT
RUN adduser -D -H -g "" notary
# Fri, 06 May 2022 02:06:23 GMT
USER notary
# Fri, 06 May 2022 02:06:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Fri, 06 May 2022 02:06:24 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 06 May 2022 02:06:25 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:6c4809594a4b80d650b9951499cc7be9a90fc7b306e1dd8052f821b60733ae0c`  
		Last Modified: Mon, 04 Apr 2022 23:52:09 GMT  
		Size: 2.6 MB (2605389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97413f849b39c68cf917253d769bfb48a252f9a5bfbae0bea43eef9dbbba6faf`  
		Last Modified: Fri, 06 May 2022 02:07:10 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391b456a9486091521ee65ecf7b8e9a5137eb9e6f3812873383016b612e4e0af`  
		Last Modified: Fri, 06 May 2022 02:07:14 GMT  
		Size: 5.2 MB (5224994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668a57ee2bed83f59845981c57d3e90a8738c1b5639c2007a1b9092a81a5eac0`  
		Last Modified: Fri, 06 May 2022 02:07:10 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82410eb437488395040d7b0b4553beb7b1ca392267473dfbc4dd3464e6213846`  
		Last Modified: Fri, 06 May 2022 02:07:11 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d33fb84c26d75e7d4b61c2bc1209a34c90463e06b2abef8f24d9e80f26ca3e0`  
		Last Modified: Fri, 06 May 2022 02:07:10 GMT  
		Size: 1.2 KB (1175 bytes)  
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
$ docker pull notary@sha256:3bf2e3e5f997f20c914c26a7cf8e8df4722b7360fd4ec45837a1d26efeb50da8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8140731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e31a389c769d279bad2efe63a14376da2e2c1e974aac94ce7d03ace8db49a4d7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:44 GMT
ADD file:c1616ef1514518ef1f90874b6fab7c42951a5736600b54942fd4ad4338a24b11 in / 
# Mon, 04 Apr 2022 23:38:44 GMT
CMD ["/bin/sh"]
# Fri, 06 May 2022 01:53:33 GMT
ENV TAG=v0.7.0
# Fri, 06 May 2022 01:53:34 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Fri, 06 May 2022 01:54:04 GMT
ENV INSTALLDIR=/notary/signer
# Fri, 06 May 2022 01:54:05 GMT
EXPOSE 4444
# Fri, 06 May 2022 01:54:06 GMT
EXPOSE 7899
# Fri, 06 May 2022 01:54:07 GMT
WORKDIR /notary/signer
# Fri, 06 May 2022 01:54:20 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --version
# Fri, 06 May 2022 01:54:22 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Fri, 06 May 2022 01:54:23 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Fri, 06 May 2022 01:54:23 GMT
RUN adduser -D -H -g "" notary
# Fri, 06 May 2022 01:54:24 GMT
USER notary
# Fri, 06 May 2022 01:54:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Fri, 06 May 2022 01:54:26 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 06 May 2022 01:54:27 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:6f153ea7cf9623ea20df5792c26f8dfd80af131fecab00e40983e554e495421e`  
		Last Modified: Mon, 04 Apr 2022 23:39:57 GMT  
		Size: 2.8 MB (2798126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9771b285e704a9bcfed3caf1883e833870862183e8e96a407ea0e7f22ebacc39`  
		Last Modified: Fri, 06 May 2022 01:54:58 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e40381195b49324230c92a904af28546b44616df3c2b304a3063338f61e946`  
		Last Modified: Fri, 06 May 2022 01:54:59 GMT  
		Size: 5.3 MB (5340578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2278e8233aaa0be43027a19ccdec3ad0a653158c3c66ba7f4fb4d35bd199b380`  
		Last Modified: Fri, 06 May 2022 01:54:58 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6fc02ebfb9b86df12f26ab0aeb99c4d823e9c0db6452495eaade43b9ba9b15`  
		Last Modified: Fri, 06 May 2022 01:54:58 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b53293a74204d6f4cb670ed5ca76b6b009700011c785dffb863d982a793021`  
		Last Modified: Fri, 06 May 2022 01:54:58 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; ppc64le

```console
$ docker pull notary@sha256:f9e05866c3f37b70a1ca602fa70173f3bcf428b70b9f5423d342bec7ee19dd53
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7850404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:974555b30dc83be4d8f3540998769870dd78f8a8fc7cacf1f1c7cce357210d74`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Tue, 05 Apr 2022 00:24:09 GMT
ADD file:53d4ef78df099d878ecfe359308c0a3ee650850966fefbe1fd7c05f3b2d89e1b in / 
# Tue, 05 Apr 2022 00:24:11 GMT
CMD ["/bin/sh"]
# Fri, 06 May 2022 01:48:47 GMT
ENV TAG=v0.7.0
# Fri, 06 May 2022 01:48:49 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Fri, 06 May 2022 01:50:42 GMT
ENV INSTALLDIR=/notary/signer
# Fri, 06 May 2022 01:50:48 GMT
EXPOSE 4444
# Fri, 06 May 2022 01:50:54 GMT
EXPOSE 7899
# Fri, 06 May 2022 01:51:03 GMT
WORKDIR /notary/signer
# Fri, 06 May 2022 01:52:07 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --version
# Fri, 06 May 2022 01:52:11 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Fri, 06 May 2022 01:52:12 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Fri, 06 May 2022 01:52:21 GMT
RUN adduser -D -H -g "" notary
# Fri, 06 May 2022 01:52:27 GMT
USER notary
# Fri, 06 May 2022 01:52:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Fri, 06 May 2022 01:52:35 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 06 May 2022 01:52:45 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:57c1475d5a6dc8e68a1b09bd09db22cc33e8f163a3841ce5100e0569acefcabe`  
		Last Modified: Tue, 05 Apr 2022 00:25:31 GMT  
		Size: 2.8 MB (2806745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eb2f6a2acaca474fa57ed221c8af545cb3427bac48728f5c70f290aa41bd6b`  
		Last Modified: Fri, 06 May 2022 01:53:32 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7742f817347981ecc0a3f52f67d4ceab6bf4efa2500da0ba0374f3f05b13090e`  
		Last Modified: Fri, 06 May 2022 01:53:33 GMT  
		Size: 5.0 MB (5041595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920db4815a208e2208166e0eba0142dd5b1482e797804a0ee3f73073b1dd9831`  
		Last Modified: Fri, 06 May 2022 01:53:32 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5ae35dd84126fb8dd98d4f50f77ae759328e7ce783394b59439efe31a25057`  
		Last Modified: Fri, 06 May 2022 01:53:33 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153896dbbb4d18a59a23b52989f2d3b868c82a9a0915a5c3b3fda53ccc195c73`  
		Last Modified: Fri, 06 May 2022 01:53:32 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; s390x

```console
$ docker pull notary@sha256:100aa1535d3e6025081ddb36c9029d15707e01bcb60b02eb246c776409d33386
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8035598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfc066c060fc75731cfc48884bee29da3347a17de3de895d818863700a36c208`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Mon, 04 Apr 2022 23:42:02 GMT
ADD file:2a940ce0447ea6f2a90d7c07cabf71ef6d12cacfaca51f7101401f3c6a733ef6 in / 
# Mon, 04 Apr 2022 23:42:03 GMT
CMD ["/bin/sh"]
# Fri, 06 May 2022 01:56:48 GMT
ENV TAG=v0.7.0
# Fri, 06 May 2022 01:56:48 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Fri, 06 May 2022 01:57:12 GMT
ENV INSTALLDIR=/notary/signer
# Fri, 06 May 2022 01:57:12 GMT
EXPOSE 4444
# Fri, 06 May 2022 01:57:12 GMT
EXPOSE 7899
# Fri, 06 May 2022 01:57:13 GMT
WORKDIR /notary/signer
# Fri, 06 May 2022 01:57:27 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --version
# Fri, 06 May 2022 01:57:27 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Fri, 06 May 2022 01:57:27 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Fri, 06 May 2022 01:57:28 GMT
RUN adduser -D -H -g "" notary
# Fri, 06 May 2022 01:57:28 GMT
USER notary
# Fri, 06 May 2022 01:57:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Fri, 06 May 2022 01:57:28 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 06 May 2022 01:57:28 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:1097ea795c9d7bf9c3f82172463982fdcb35c173957675c82cd2081c53d35a6d`  
		Last Modified: Mon, 04 Apr 2022 23:43:00 GMT  
		Size: 2.6 MB (2571889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f514c7c7fd3bce09a98dd400ba42a977f68e18d847f28e00680f9c46f0b91615`  
		Last Modified: Fri, 06 May 2022 01:57:56 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb86d61abcad91e27ace9a5afbfabfd5d9241bf6c410b09e58bf7ae9dc1b291`  
		Last Modified: Fri, 06 May 2022 01:57:57 GMT  
		Size: 5.5 MB (5461648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05aabf661f7b6c545c9e29f2a6e1fe1dac19a3bc30f36952e23adaa2b07efe6a`  
		Last Modified: Fri, 06 May 2022 01:57:56 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f86159107448188b6f13049281a5bef18bc976d763ef3bf461e582605cd83a`  
		Last Modified: Fri, 06 May 2022 01:57:56 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3ac01df17b11880cdea1141cdebf3e9180117f64e869d6474f877fb3ecbd4a`  
		Last Modified: Fri, 06 May 2022 01:57:56 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
