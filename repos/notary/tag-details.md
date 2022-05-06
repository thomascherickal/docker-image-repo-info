<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `notary`

-	[`notary:server`](#notaryserver)
-	[`notary:server-0.7.0`](#notaryserver-070)
-	[`notary:signer`](#notarysigner)
-	[`notary:signer-0.7.0`](#notarysigner-070)

## `notary:server`

```console
$ docker pull notary@sha256:a5d3416ce916d9bb8adde5ba6d0d899ceec41fc72b4a6dd33e1741e3b234ccce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `notary:server` - linux; amd64

```console
$ docker pull notary@sha256:01340e33eaa4eb2547b49d57e3c30761290c1180f5cb1f37c368ef4b5d30b9e3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8912185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1230af5d9d13460917775dc55aa93b0dbaa64345b273d5b2f7e863a435e835db`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:19 GMT
ADD file:c1aa87a3b464fca64d769444b5201bc0426a1f517c91c4a7916270e10f8b300b in / 
# Tue, 05 Apr 2022 00:20:19 GMT
CMD ["/bin/sh"]
# Fri, 06 May 2022 02:16:09 GMT
ENV TAG=v0.7.0
# Fri, 06 May 2022 02:16:10 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Fri, 06 May 2022 02:16:10 GMT
ENV INSTALLDIR=/notary/server
# Fri, 06 May 2022 02:16:10 GMT
EXPOSE 4443
# Fri, 06 May 2022 02:16:10 GMT
WORKDIR /notary/server
# Fri, 06 May 2022 02:16:25 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --version
# Fri, 06 May 2022 02:16:25 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Fri, 06 May 2022 02:16:26 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Fri, 06 May 2022 02:16:26 GMT
RUN adduser -D -H -g "" notary
# Fri, 06 May 2022 02:16:26 GMT
USER notary
# Fri, 06 May 2022 02:16:26 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Fri, 06 May 2022 02:16:26 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 06 May 2022 02:16:26 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:1b7ca6aea1ddfe716f3694edb811ab35114db9e93f3ce38d7dab6b4d9270cb0c`  
		Last Modified: Tue, 05 Apr 2022 00:21:10 GMT  
		Size: 2.8 MB (2808060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82e4c124d20ee7f1ee1e4a23eb0c05d29826bbba980169f660549ed9a58752d`  
		Last Modified: Fri, 06 May 2022 02:16:57 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d96230eb52d4407a263c809ef7c72c3905f8b3e6cf59242be06caeb4a44062b`  
		Last Modified: Fri, 06 May 2022 02:16:59 GMT  
		Size: 6.1 MB (6102010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45aaa15e1652d6d32df0ca0c85d56b27b23c6ee645fb625fde4fb386a3561a70`  
		Last Modified: Fri, 06 May 2022 02:16:57 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c2b5c4f81bade136cf1365b673ad1e982f0886632c1898177fa8f2bfd5be77`  
		Last Modified: Fri, 06 May 2022 02:16:57 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d073315224dd955b6e3ffb763af5fa35cfb0b43995631c302745411f0cb35d47`  
		Last Modified: Fri, 06 May 2022 02:16:57 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; arm variant v6

```console
$ docker pull notary@sha256:69715961d90afb23dcd00843121a87d8751c727b57bd1de273b00e0153a276d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8344745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7525cdb059004173bfdcb900a2593fc6a0bea45cbcf37fdd945fc9c6f9045ce`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Mon, 04 Apr 2022 23:50:18 GMT
ADD file:a62ad8c2b01195a2d42109e23b6d8ce69e2a816702518b2d823139f28c0ff799 in / 
# Mon, 04 Apr 2022 23:50:19 GMT
CMD ["/bin/sh"]
# Fri, 06 May 2022 02:05:11 GMT
ENV TAG=v0.7.0
# Fri, 06 May 2022 02:05:11 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Fri, 06 May 2022 02:05:12 GMT
ENV INSTALLDIR=/notary/server
# Fri, 06 May 2022 02:05:12 GMT
EXPOSE 4443
# Fri, 06 May 2022 02:05:13 GMT
WORKDIR /notary/server
# Fri, 06 May 2022 02:05:40 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --version
# Fri, 06 May 2022 02:05:40 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Fri, 06 May 2022 02:05:41 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Fri, 06 May 2022 02:05:42 GMT
RUN adduser -D -H -g "" notary
# Fri, 06 May 2022 02:05:43 GMT
USER notary
# Fri, 06 May 2022 02:05:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Fri, 06 May 2022 02:05:43 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 06 May 2022 02:05:44 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:6c4809594a4b80d650b9951499cc7be9a90fc7b306e1dd8052f821b60733ae0c`  
		Last Modified: Mon, 04 Apr 2022 23:52:09 GMT  
		Size: 2.6 MB (2605389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790b941e03c3da865a69f9d30c13dde97171fe28cef6d72a16781d9faf4445e1`  
		Last Modified: Fri, 06 May 2022 02:06:56 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec356af48d05d45cb3e0fbd603e3da6a0793554bbd480b1bfa8b42be1073be37`  
		Last Modified: Fri, 06 May 2022 02:06:59 GMT  
		Size: 5.7 MB (5737230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc2ffa839e593a064a7020b3f6bf522d356710cbed25b71abeeaa4cc6947ecc`  
		Last Modified: Fri, 06 May 2022 02:06:56 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420fc87c3fb11d297c4b09c6be560cd84143a3a7d584278ac45d763bdc64a3f8`  
		Last Modified: Fri, 06 May 2022 02:06:56 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d2fa141338a1dac3da46f56b7c2d9e738c559a593138f6b007433322036f5f`  
		Last Modified: Fri, 06 May 2022 02:06:56 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:9bcc59824e4db2194b96f114a58dcd02e8a5ee01bfcc57e088d634f2c7766b02
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8346196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad96cd15f3785f09c8a0dc678758238c222d5610476282c70b306ba865c1ee6b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:53 GMT
ADD file:a2a992b7f6af1e6f8f5648f329f4a4058d8c4377417ac23ae211290c0cdc8f4b in / 
# Mon, 04 Apr 2022 23:39:53 GMT
CMD ["/bin/sh"]
# Fri, 06 May 2022 01:04:59 GMT
ENV TAG=v0.7.0
# Fri, 06 May 2022 01:05:00 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Fri, 06 May 2022 01:05:01 GMT
ENV INSTALLDIR=/notary/server
# Fri, 06 May 2022 01:05:02 GMT
EXPOSE 4443
# Fri, 06 May 2022 01:05:03 GMT
WORKDIR /notary/server
# Fri, 06 May 2022 01:05:17 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --version
# Fri, 06 May 2022 01:05:18 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Fri, 06 May 2022 01:05:19 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Fri, 06 May 2022 01:05:19 GMT
RUN adduser -D -H -g "" notary
# Fri, 06 May 2022 01:05:20 GMT
USER notary
# Fri, 06 May 2022 01:05:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Fri, 06 May 2022 01:05:22 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 06 May 2022 01:05:23 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:0eeab5c200691bd777e227c6eea27f7ca3c8232b67118a76edac2dcde3186aa1`  
		Last Modified: Mon, 04 Apr 2022 23:41:02 GMT  
		Size: 2.7 MB (2716243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ed6330a9615a6e518283d07985b18d479a8f03c5c3f20015c6582538def18a`  
		Last Modified: Fri, 06 May 2022 01:06:14 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f91204882744da81d33ffcfc2d335958d94620b343be39e566107e354d4f2b9`  
		Last Modified: Fri, 06 May 2022 01:06:15 GMT  
		Size: 5.6 MB (5627862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b3c5e562a2e32c0984910ea2a31cbc0ebf70cfd1f0df3daca43466587ac161`  
		Last Modified: Fri, 06 May 2022 01:06:14 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2496335307234f487bccec5dd92b220fd206a951193aaaa8a893358ed5b3658`  
		Last Modified: Fri, 06 May 2022 01:06:14 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db8c9d2946bfc3596ae37b6aae0f362c1743c06274f0580f1d28bd048a53f44`  
		Last Modified: Fri, 06 May 2022 01:06:14 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; 386

```console
$ docker pull notary@sha256:37f2f429ef0f26e10ce0ffd80eb1db04075cc655e4ade968934feb015c81a5e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8660466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9890bfefc0e3351b820e016a71a528d1956569ab2df6944908ad9a909472f22`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:44 GMT
ADD file:c1616ef1514518ef1f90874b6fab7c42951a5736600b54942fd4ad4338a24b11 in / 
# Mon, 04 Apr 2022 23:38:44 GMT
CMD ["/bin/sh"]
# Fri, 06 May 2022 01:53:33 GMT
ENV TAG=v0.7.0
# Fri, 06 May 2022 01:53:34 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Fri, 06 May 2022 01:53:35 GMT
ENV INSTALLDIR=/notary/server
# Fri, 06 May 2022 01:53:36 GMT
EXPOSE 4443
# Fri, 06 May 2022 01:53:37 GMT
WORKDIR /notary/server
# Fri, 06 May 2022 01:53:52 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --version
# Fri, 06 May 2022 01:53:54 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Fri, 06 May 2022 01:53:55 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Fri, 06 May 2022 01:53:55 GMT
RUN adduser -D -H -g "" notary
# Fri, 06 May 2022 01:53:56 GMT
USER notary
# Fri, 06 May 2022 01:53:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Fri, 06 May 2022 01:53:58 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 06 May 2022 01:53:59 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:6f153ea7cf9623ea20df5792c26f8dfd80af131fecab00e40983e554e495421e`  
		Last Modified: Mon, 04 Apr 2022 23:39:57 GMT  
		Size: 2.8 MB (2798126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480520f3392b90043910d7268b537ecd1659ddbb5cb29c5adf77c88fef47d65a`  
		Last Modified: Fri, 06 May 2022 01:54:47 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00018550dcea7efab5be15d233fd261496846d3a597e4f07175aefc34a746117`  
		Last Modified: Fri, 06 May 2022 01:54:48 GMT  
		Size: 5.9 MB (5860251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddfb2fc3b62b892c8667daec55783ef3d63453ab4563b516c177934fcb49572`  
		Last Modified: Fri, 06 May 2022 01:54:47 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69e20ab1fa4892eca94c25948de9a1fdc3330ab23f1efffc98693352ee04fa5`  
		Last Modified: Fri, 06 May 2022 01:54:47 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c545d4343d941bfd383dd6acff9bdf6431eef4e14113eb33d31225edfe550c`  
		Last Modified: Fri, 06 May 2022 01:54:47 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; ppc64le

```console
$ docker pull notary@sha256:bae576e49f3c5ac60baf81b0cd47f6c7e292e3c1a2cc8b081d846e0cda62a5b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8348451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0495e05e0d7e4df038032361130b3a554797bc2a511c2c618a8890b845f212d3`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Tue, 05 Apr 2022 00:24:09 GMT
ADD file:53d4ef78df099d878ecfe359308c0a3ee650850966fefbe1fd7c05f3b2d89e1b in / 
# Tue, 05 Apr 2022 00:24:11 GMT
CMD ["/bin/sh"]
# Fri, 06 May 2022 01:48:47 GMT
ENV TAG=v0.7.0
# Fri, 06 May 2022 01:48:49 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Fri, 06 May 2022 01:48:53 GMT
ENV INSTALLDIR=/notary/server
# Fri, 06 May 2022 01:48:55 GMT
EXPOSE 4443
# Fri, 06 May 2022 01:49:00 GMT
WORKDIR /notary/server
# Fri, 06 May 2022 01:49:48 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --version
# Fri, 06 May 2022 01:49:50 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Fri, 06 May 2022 01:49:52 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Fri, 06 May 2022 01:49:57 GMT
RUN adduser -D -H -g "" notary
# Fri, 06 May 2022 01:50:01 GMT
USER notary
# Fri, 06 May 2022 01:50:03 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Fri, 06 May 2022 01:50:10 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 06 May 2022 01:50:17 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:57c1475d5a6dc8e68a1b09bd09db22cc33e8f163a3841ce5100e0569acefcabe`  
		Last Modified: Tue, 05 Apr 2022 00:25:31 GMT  
		Size: 2.8 MB (2806745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d113a2296216ff0801eaaa23faf16370c503b4070e9895dd7788112939579b`  
		Last Modified: Fri, 06 May 2022 01:53:18 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9969d0f4c7adddcdbd67e584df60bb9ef69365671ae03723b39dc9807ffb8f71`  
		Last Modified: Fri, 06 May 2022 01:53:19 GMT  
		Size: 5.5 MB (5539583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4601a5f5eccd51d842fb5c837594b84c44958c2d40ad210aa02f774d8ce2d99c`  
		Last Modified: Fri, 06 May 2022 01:53:18 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfede6060e49c4ea18bb60fce541803e16bc21a163f2c7bd1e0d65273ea9ca2`  
		Last Modified: Fri, 06 May 2022 01:53:18 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fe6431b53b4dcf01fbf89da7c8ab80fbd68973c9ed96993ba18843a532afe9`  
		Last Modified: Fri, 06 May 2022 01:53:18 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; s390x

```console
$ docker pull notary@sha256:4afee04ec8e9b0790a701647f0ff1b77cd92f5e9879d1c40adc4a57e1569e104
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8563040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2caadf55d6e37952159287606379cfe7dc9d745322fb06250c22ff7266cc335c`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Mon, 04 Apr 2022 23:42:02 GMT
ADD file:2a940ce0447ea6f2a90d7c07cabf71ef6d12cacfaca51f7101401f3c6a733ef6 in / 
# Mon, 04 Apr 2022 23:42:03 GMT
CMD ["/bin/sh"]
# Fri, 06 May 2022 01:56:48 GMT
ENV TAG=v0.7.0
# Fri, 06 May 2022 01:56:48 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Fri, 06 May 2022 01:56:48 GMT
ENV INSTALLDIR=/notary/server
# Fri, 06 May 2022 01:56:48 GMT
EXPOSE 4443
# Fri, 06 May 2022 01:56:48 GMT
WORKDIR /notary/server
# Fri, 06 May 2022 01:57:04 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --version
# Fri, 06 May 2022 01:57:05 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Fri, 06 May 2022 01:57:05 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Fri, 06 May 2022 01:57:05 GMT
RUN adduser -D -H -g "" notary
# Fri, 06 May 2022 01:57:06 GMT
USER notary
# Fri, 06 May 2022 01:57:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Fri, 06 May 2022 01:57:06 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 06 May 2022 01:57:06 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:1097ea795c9d7bf9c3f82172463982fdcb35c173957675c82cd2081c53d35a6d`  
		Last Modified: Mon, 04 Apr 2022 23:43:00 GMT  
		Size: 2.6 MB (2571889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e26ac170029ddba7ed2c65ed49b6dd876c8fcd497710d45be662e1c83b903fd`  
		Last Modified: Fri, 06 May 2022 01:57:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a60b52baad75bc90d14b253250778d510646336dd1a5fd9ecc5bdb70f67a45`  
		Last Modified: Fri, 06 May 2022 01:57:49 GMT  
		Size: 6.0 MB (5989032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8809a1522240c706e69c2c9866b1297a7126b0e4fa03b51e5bea7df441b51d`  
		Last Modified: Fri, 06 May 2022 01:57:49 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bb1c0f79aa4b7b58df61b2ce23ea6b0b9f26a572ceb192cb91fbe450cdc4a4`  
		Last Modified: Fri, 06 May 2022 01:57:48 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:facdfee29d8b7759a802b3fa79de8c0cc778c99dbd2579032791b5cc56d20f48`  
		Last Modified: Fri, 06 May 2022 01:57:49 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `notary:server-0.7.0`

```console
$ docker pull notary@sha256:a5d3416ce916d9bb8adde5ba6d0d899ceec41fc72b4a6dd33e1741e3b234ccce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `notary:server-0.7.0` - linux; amd64

```console
$ docker pull notary@sha256:01340e33eaa4eb2547b49d57e3c30761290c1180f5cb1f37c368ef4b5d30b9e3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8912185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1230af5d9d13460917775dc55aa93b0dbaa64345b273d5b2f7e863a435e835db`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:19 GMT
ADD file:c1aa87a3b464fca64d769444b5201bc0426a1f517c91c4a7916270e10f8b300b in / 
# Tue, 05 Apr 2022 00:20:19 GMT
CMD ["/bin/sh"]
# Fri, 06 May 2022 02:16:09 GMT
ENV TAG=v0.7.0
# Fri, 06 May 2022 02:16:10 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Fri, 06 May 2022 02:16:10 GMT
ENV INSTALLDIR=/notary/server
# Fri, 06 May 2022 02:16:10 GMT
EXPOSE 4443
# Fri, 06 May 2022 02:16:10 GMT
WORKDIR /notary/server
# Fri, 06 May 2022 02:16:25 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --version
# Fri, 06 May 2022 02:16:25 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Fri, 06 May 2022 02:16:26 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Fri, 06 May 2022 02:16:26 GMT
RUN adduser -D -H -g "" notary
# Fri, 06 May 2022 02:16:26 GMT
USER notary
# Fri, 06 May 2022 02:16:26 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Fri, 06 May 2022 02:16:26 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 06 May 2022 02:16:26 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:1b7ca6aea1ddfe716f3694edb811ab35114db9e93f3ce38d7dab6b4d9270cb0c`  
		Last Modified: Tue, 05 Apr 2022 00:21:10 GMT  
		Size: 2.8 MB (2808060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82e4c124d20ee7f1ee1e4a23eb0c05d29826bbba980169f660549ed9a58752d`  
		Last Modified: Fri, 06 May 2022 02:16:57 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d96230eb52d4407a263c809ef7c72c3905f8b3e6cf59242be06caeb4a44062b`  
		Last Modified: Fri, 06 May 2022 02:16:59 GMT  
		Size: 6.1 MB (6102010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45aaa15e1652d6d32df0ca0c85d56b27b23c6ee645fb625fde4fb386a3561a70`  
		Last Modified: Fri, 06 May 2022 02:16:57 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c2b5c4f81bade136cf1365b673ad1e982f0886632c1898177fa8f2bfd5be77`  
		Last Modified: Fri, 06 May 2022 02:16:57 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d073315224dd955b6e3ffb763af5fa35cfb0b43995631c302745411f0cb35d47`  
		Last Modified: Fri, 06 May 2022 02:16:57 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; arm variant v6

```console
$ docker pull notary@sha256:69715961d90afb23dcd00843121a87d8751c727b57bd1de273b00e0153a276d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8344745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7525cdb059004173bfdcb900a2593fc6a0bea45cbcf37fdd945fc9c6f9045ce`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Mon, 04 Apr 2022 23:50:18 GMT
ADD file:a62ad8c2b01195a2d42109e23b6d8ce69e2a816702518b2d823139f28c0ff799 in / 
# Mon, 04 Apr 2022 23:50:19 GMT
CMD ["/bin/sh"]
# Fri, 06 May 2022 02:05:11 GMT
ENV TAG=v0.7.0
# Fri, 06 May 2022 02:05:11 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Fri, 06 May 2022 02:05:12 GMT
ENV INSTALLDIR=/notary/server
# Fri, 06 May 2022 02:05:12 GMT
EXPOSE 4443
# Fri, 06 May 2022 02:05:13 GMT
WORKDIR /notary/server
# Fri, 06 May 2022 02:05:40 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --version
# Fri, 06 May 2022 02:05:40 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Fri, 06 May 2022 02:05:41 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Fri, 06 May 2022 02:05:42 GMT
RUN adduser -D -H -g "" notary
# Fri, 06 May 2022 02:05:43 GMT
USER notary
# Fri, 06 May 2022 02:05:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Fri, 06 May 2022 02:05:43 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 06 May 2022 02:05:44 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:6c4809594a4b80d650b9951499cc7be9a90fc7b306e1dd8052f821b60733ae0c`  
		Last Modified: Mon, 04 Apr 2022 23:52:09 GMT  
		Size: 2.6 MB (2605389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790b941e03c3da865a69f9d30c13dde97171fe28cef6d72a16781d9faf4445e1`  
		Last Modified: Fri, 06 May 2022 02:06:56 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec356af48d05d45cb3e0fbd603e3da6a0793554bbd480b1bfa8b42be1073be37`  
		Last Modified: Fri, 06 May 2022 02:06:59 GMT  
		Size: 5.7 MB (5737230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc2ffa839e593a064a7020b3f6bf522d356710cbed25b71abeeaa4cc6947ecc`  
		Last Modified: Fri, 06 May 2022 02:06:56 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420fc87c3fb11d297c4b09c6be560cd84143a3a7d584278ac45d763bdc64a3f8`  
		Last Modified: Fri, 06 May 2022 02:06:56 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d2fa141338a1dac3da46f56b7c2d9e738c559a593138f6b007433322036f5f`  
		Last Modified: Fri, 06 May 2022 02:06:56 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:9bcc59824e4db2194b96f114a58dcd02e8a5ee01bfcc57e088d634f2c7766b02
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8346196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad96cd15f3785f09c8a0dc678758238c222d5610476282c70b306ba865c1ee6b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:53 GMT
ADD file:a2a992b7f6af1e6f8f5648f329f4a4058d8c4377417ac23ae211290c0cdc8f4b in / 
# Mon, 04 Apr 2022 23:39:53 GMT
CMD ["/bin/sh"]
# Fri, 06 May 2022 01:04:59 GMT
ENV TAG=v0.7.0
# Fri, 06 May 2022 01:05:00 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Fri, 06 May 2022 01:05:01 GMT
ENV INSTALLDIR=/notary/server
# Fri, 06 May 2022 01:05:02 GMT
EXPOSE 4443
# Fri, 06 May 2022 01:05:03 GMT
WORKDIR /notary/server
# Fri, 06 May 2022 01:05:17 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --version
# Fri, 06 May 2022 01:05:18 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Fri, 06 May 2022 01:05:19 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Fri, 06 May 2022 01:05:19 GMT
RUN adduser -D -H -g "" notary
# Fri, 06 May 2022 01:05:20 GMT
USER notary
# Fri, 06 May 2022 01:05:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Fri, 06 May 2022 01:05:22 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 06 May 2022 01:05:23 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:0eeab5c200691bd777e227c6eea27f7ca3c8232b67118a76edac2dcde3186aa1`  
		Last Modified: Mon, 04 Apr 2022 23:41:02 GMT  
		Size: 2.7 MB (2716243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ed6330a9615a6e518283d07985b18d479a8f03c5c3f20015c6582538def18a`  
		Last Modified: Fri, 06 May 2022 01:06:14 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f91204882744da81d33ffcfc2d335958d94620b343be39e566107e354d4f2b9`  
		Last Modified: Fri, 06 May 2022 01:06:15 GMT  
		Size: 5.6 MB (5627862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b3c5e562a2e32c0984910ea2a31cbc0ebf70cfd1f0df3daca43466587ac161`  
		Last Modified: Fri, 06 May 2022 01:06:14 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2496335307234f487bccec5dd92b220fd206a951193aaaa8a893358ed5b3658`  
		Last Modified: Fri, 06 May 2022 01:06:14 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db8c9d2946bfc3596ae37b6aae0f362c1743c06274f0580f1d28bd048a53f44`  
		Last Modified: Fri, 06 May 2022 01:06:14 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; 386

```console
$ docker pull notary@sha256:37f2f429ef0f26e10ce0ffd80eb1db04075cc655e4ade968934feb015c81a5e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8660466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9890bfefc0e3351b820e016a71a528d1956569ab2df6944908ad9a909472f22`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:44 GMT
ADD file:c1616ef1514518ef1f90874b6fab7c42951a5736600b54942fd4ad4338a24b11 in / 
# Mon, 04 Apr 2022 23:38:44 GMT
CMD ["/bin/sh"]
# Fri, 06 May 2022 01:53:33 GMT
ENV TAG=v0.7.0
# Fri, 06 May 2022 01:53:34 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Fri, 06 May 2022 01:53:35 GMT
ENV INSTALLDIR=/notary/server
# Fri, 06 May 2022 01:53:36 GMT
EXPOSE 4443
# Fri, 06 May 2022 01:53:37 GMT
WORKDIR /notary/server
# Fri, 06 May 2022 01:53:52 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --version
# Fri, 06 May 2022 01:53:54 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Fri, 06 May 2022 01:53:55 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Fri, 06 May 2022 01:53:55 GMT
RUN adduser -D -H -g "" notary
# Fri, 06 May 2022 01:53:56 GMT
USER notary
# Fri, 06 May 2022 01:53:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Fri, 06 May 2022 01:53:58 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 06 May 2022 01:53:59 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:6f153ea7cf9623ea20df5792c26f8dfd80af131fecab00e40983e554e495421e`  
		Last Modified: Mon, 04 Apr 2022 23:39:57 GMT  
		Size: 2.8 MB (2798126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480520f3392b90043910d7268b537ecd1659ddbb5cb29c5adf77c88fef47d65a`  
		Last Modified: Fri, 06 May 2022 01:54:47 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00018550dcea7efab5be15d233fd261496846d3a597e4f07175aefc34a746117`  
		Last Modified: Fri, 06 May 2022 01:54:48 GMT  
		Size: 5.9 MB (5860251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddfb2fc3b62b892c8667daec55783ef3d63453ab4563b516c177934fcb49572`  
		Last Modified: Fri, 06 May 2022 01:54:47 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69e20ab1fa4892eca94c25948de9a1fdc3330ab23f1efffc98693352ee04fa5`  
		Last Modified: Fri, 06 May 2022 01:54:47 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c545d4343d941bfd383dd6acff9bdf6431eef4e14113eb33d31225edfe550c`  
		Last Modified: Fri, 06 May 2022 01:54:47 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; ppc64le

```console
$ docker pull notary@sha256:bae576e49f3c5ac60baf81b0cd47f6c7e292e3c1a2cc8b081d846e0cda62a5b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8348451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0495e05e0d7e4df038032361130b3a554797bc2a511c2c618a8890b845f212d3`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Tue, 05 Apr 2022 00:24:09 GMT
ADD file:53d4ef78df099d878ecfe359308c0a3ee650850966fefbe1fd7c05f3b2d89e1b in / 
# Tue, 05 Apr 2022 00:24:11 GMT
CMD ["/bin/sh"]
# Fri, 06 May 2022 01:48:47 GMT
ENV TAG=v0.7.0
# Fri, 06 May 2022 01:48:49 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Fri, 06 May 2022 01:48:53 GMT
ENV INSTALLDIR=/notary/server
# Fri, 06 May 2022 01:48:55 GMT
EXPOSE 4443
# Fri, 06 May 2022 01:49:00 GMT
WORKDIR /notary/server
# Fri, 06 May 2022 01:49:48 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --version
# Fri, 06 May 2022 01:49:50 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Fri, 06 May 2022 01:49:52 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Fri, 06 May 2022 01:49:57 GMT
RUN adduser -D -H -g "" notary
# Fri, 06 May 2022 01:50:01 GMT
USER notary
# Fri, 06 May 2022 01:50:03 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Fri, 06 May 2022 01:50:10 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 06 May 2022 01:50:17 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:57c1475d5a6dc8e68a1b09bd09db22cc33e8f163a3841ce5100e0569acefcabe`  
		Last Modified: Tue, 05 Apr 2022 00:25:31 GMT  
		Size: 2.8 MB (2806745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d113a2296216ff0801eaaa23faf16370c503b4070e9895dd7788112939579b`  
		Last Modified: Fri, 06 May 2022 01:53:18 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9969d0f4c7adddcdbd67e584df60bb9ef69365671ae03723b39dc9807ffb8f71`  
		Last Modified: Fri, 06 May 2022 01:53:19 GMT  
		Size: 5.5 MB (5539583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4601a5f5eccd51d842fb5c837594b84c44958c2d40ad210aa02f774d8ce2d99c`  
		Last Modified: Fri, 06 May 2022 01:53:18 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfede6060e49c4ea18bb60fce541803e16bc21a163f2c7bd1e0d65273ea9ca2`  
		Last Modified: Fri, 06 May 2022 01:53:18 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fe6431b53b4dcf01fbf89da7c8ab80fbd68973c9ed96993ba18843a532afe9`  
		Last Modified: Fri, 06 May 2022 01:53:18 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; s390x

```console
$ docker pull notary@sha256:4afee04ec8e9b0790a701647f0ff1b77cd92f5e9879d1c40adc4a57e1569e104
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8563040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2caadf55d6e37952159287606379cfe7dc9d745322fb06250c22ff7266cc335c`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Mon, 04 Apr 2022 23:42:02 GMT
ADD file:2a940ce0447ea6f2a90d7c07cabf71ef6d12cacfaca51f7101401f3c6a733ef6 in / 
# Mon, 04 Apr 2022 23:42:03 GMT
CMD ["/bin/sh"]
# Fri, 06 May 2022 01:56:48 GMT
ENV TAG=v0.7.0
# Fri, 06 May 2022 01:56:48 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Fri, 06 May 2022 01:56:48 GMT
ENV INSTALLDIR=/notary/server
# Fri, 06 May 2022 01:56:48 GMT
EXPOSE 4443
# Fri, 06 May 2022 01:56:48 GMT
WORKDIR /notary/server
# Fri, 06 May 2022 01:57:04 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --version
# Fri, 06 May 2022 01:57:05 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Fri, 06 May 2022 01:57:05 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Fri, 06 May 2022 01:57:05 GMT
RUN adduser -D -H -g "" notary
# Fri, 06 May 2022 01:57:06 GMT
USER notary
# Fri, 06 May 2022 01:57:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Fri, 06 May 2022 01:57:06 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 06 May 2022 01:57:06 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:1097ea795c9d7bf9c3f82172463982fdcb35c173957675c82cd2081c53d35a6d`  
		Last Modified: Mon, 04 Apr 2022 23:43:00 GMT  
		Size: 2.6 MB (2571889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e26ac170029ddba7ed2c65ed49b6dd876c8fcd497710d45be662e1c83b903fd`  
		Last Modified: Fri, 06 May 2022 01:57:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a60b52baad75bc90d14b253250778d510646336dd1a5fd9ecc5bdb70f67a45`  
		Last Modified: Fri, 06 May 2022 01:57:49 GMT  
		Size: 6.0 MB (5989032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8809a1522240c706e69c2c9866b1297a7126b0e4fa03b51e5bea7df441b51d`  
		Last Modified: Fri, 06 May 2022 01:57:49 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bb1c0f79aa4b7b58df61b2ce23ea6b0b9f26a572ceb192cb91fbe450cdc4a4`  
		Last Modified: Fri, 06 May 2022 01:57:48 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:facdfee29d8b7759a802b3fa79de8c0cc778c99dbd2579032791b5cc56d20f48`  
		Last Modified: Fri, 06 May 2022 01:57:49 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

## `notary:signer-0.7.0`

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

### `notary:signer-0.7.0` - linux; amd64

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

### `notary:signer-0.7.0` - linux; arm variant v6

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

### `notary:signer-0.7.0` - linux; arm64 variant v8

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

### `notary:signer-0.7.0` - linux; 386

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

### `notary:signer-0.7.0` - linux; ppc64le

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

### `notary:signer-0.7.0` - linux; s390x

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
