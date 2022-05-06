<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `notary`

-	[`notary:server`](#notaryserver)
-	[`notary:server-0.7.0`](#notaryserver-070)
-	[`notary:signer`](#notarysigner)
-	[`notary:signer-0.7.0`](#notarysigner-070)

## `notary:server`

```console
$ docker pull notary@sha256:62757be488556ede7da5bd59283c46016b07342266c031b1e06b7d52e721a14b
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
$ docker pull notary@sha256:4674260446d7a73c3f496c752d2ddac3004e182e67040830cb78100bd8284b18
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7753837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79d079083c2b38767518098ace2c6dc1eb7bd8c77f8c7c95a80f60e37f8f7513`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Thu, 28 Apr 2022 21:36:58 GMT
ENV TAG=v0.7.0
# Thu, 28 Apr 2022 21:36:58 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Thu, 28 Apr 2022 21:36:58 GMT
ENV INSTALLDIR=/notary/server
# Thu, 28 Apr 2022 21:36:58 GMT
EXPOSE 4443
# Thu, 28 Apr 2022 21:36:58 GMT
WORKDIR /notary/server
# Thu, 28 Apr 2022 21:37:13 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Thu, 28 Apr 2022 21:37:13 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Thu, 28 Apr 2022 21:37:14 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Thu, 28 Apr 2022 21:37:14 GMT
RUN adduser -D -H -g "" notary
# Thu, 28 Apr 2022 21:37:15 GMT
USER notary
# Thu, 28 Apr 2022 21:37:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Thu, 28 Apr 2022 21:37:15 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 28 Apr 2022 21:37:15 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe8a924f45f7c281c6f5094e5178dc68f022c38326042f43c32ecd50c63acdb`  
		Last Modified: Thu, 28 Apr 2022 21:37:50 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b80533c4d967b4e02ff602bc7968977cf12dd30ca019b3efd762d159fa6b2e`  
		Last Modified: Thu, 28 Apr 2022 21:37:50 GMT  
		Size: 4.9 MB (4937155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584457574f4c95d7f96cdb2c2122d523f12e2b53d23b0110da46b6c6991f194b`  
		Last Modified: Thu, 28 Apr 2022 21:37:50 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf61a1ed3ba555ef09ef0043326dc2071b8e4fe291fa8a31a1cca32a1dd068c`  
		Last Modified: Thu, 28 Apr 2022 21:37:50 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c102fcc61f5e3d1a76864b80c53ee1d3e77b4539895c198ec90a190c030522c`  
		Last Modified: Thu, 28 Apr 2022 21:37:50 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; arm variant v6

```console
$ docker pull notary@sha256:04756f332d3c754b7023b7e2133be2f24e8a43a2a9e0e520a32eb363819b673c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7235935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74b356e59aca62520ccbb384f35da7a00bb2428fdab7104eb35dda1a25672127`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Thu, 28 Apr 2022 20:49:39 GMT
ENV TAG=v0.7.0
# Thu, 28 Apr 2022 20:49:40 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Thu, 28 Apr 2022 20:49:40 GMT
ENV INSTALLDIR=/notary/server
# Thu, 28 Apr 2022 20:49:41 GMT
EXPOSE 4443
# Thu, 28 Apr 2022 20:49:41 GMT
WORKDIR /notary/server
# Thu, 28 Apr 2022 20:50:13 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Thu, 28 Apr 2022 20:50:13 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Thu, 28 Apr 2022 20:50:14 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Thu, 28 Apr 2022 20:50:15 GMT
RUN adduser -D -H -g "" notary
# Thu, 28 Apr 2022 20:50:16 GMT
USER notary
# Thu, 28 Apr 2022 20:50:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Thu, 28 Apr 2022 20:50:17 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 28 Apr 2022 20:50:17 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48adbbc574869c00eb579dbffc35fa365ce1f2c4fca0e4235ec8dd50e627aa01`  
		Last Modified: Thu, 28 Apr 2022 20:51:38 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba90fdc902b07726f8f8b4b7e63e93799a5cf111373ae4a634455debdfc7f28`  
		Last Modified: Thu, 28 Apr 2022 20:51:41 GMT  
		Size: 4.6 MB (4611826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9697deaeac362e43baeeee6da258f87c17c14490e6e66c4a754d0615430c778`  
		Last Modified: Thu, 28 Apr 2022 20:51:38 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d5c3fe154637f1ca01d69167800affffb84b80a84548bd27ac873fa212c8ba`  
		Last Modified: Thu, 28 Apr 2022 20:51:38 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823bd7b4830119c1d7312679ce70606d562c73e16074d8273673df5f06d4a59f`  
		Last Modified: Thu, 28 Apr 2022 20:51:38 GMT  
		Size: 1.2 KB (1185 bytes)  
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
$ docker pull notary@sha256:212bf0a21fcb393cdebcc40077a507b7c9268f5e075042143c640a34a1fb02be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7459426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8ba6dd8a425da479a83e7b7b3fc8185cc6b4e3b9981ed4d8369b744e6b721b2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Thu, 28 Apr 2022 20:58:57 GMT
ENV TAG=v0.7.0
# Thu, 28 Apr 2022 20:58:58 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Thu, 28 Apr 2022 20:58:59 GMT
ENV INSTALLDIR=/notary/server
# Thu, 28 Apr 2022 20:59:00 GMT
EXPOSE 4443
# Thu, 28 Apr 2022 20:59:01 GMT
WORKDIR /notary/server
# Thu, 28 Apr 2022 20:59:17 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Thu, 28 Apr 2022 20:59:19 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Thu, 28 Apr 2022 20:59:20 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Thu, 28 Apr 2022 20:59:20 GMT
RUN adduser -D -H -g "" notary
# Thu, 28 Apr 2022 20:59:21 GMT
USER notary
# Thu, 28 Apr 2022 20:59:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Thu, 28 Apr 2022 20:59:23 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 28 Apr 2022 20:59:24 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0fbe394599acca5b3306739ef20396a34ecbe6436479c45f59347a60b4dfc5`  
		Last Modified: Thu, 28 Apr 2022 21:00:16 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec5a757f1509eb69280bcd844c5445241e34dd7d89d83bd47b2642e6585e23b`  
		Last Modified: Thu, 28 Apr 2022 21:00:16 GMT  
		Size: 4.6 MB (4638351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95a29e888fc0a814de7c46ec0816a38b1fd19747d058a43f67f88533034d5dfa`  
		Last Modified: Thu, 28 Apr 2022 21:00:15 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e23dfa086492f979777742fae9aa2314e900c6a0dddee45cec1370de2c1bee`  
		Last Modified: Thu, 28 Apr 2022 21:00:15 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9647bd875f86c9487e3f546a94239631c089672da3be912b348f3c0507ed423b`  
		Last Modified: Thu, 28 Apr 2022 21:00:15 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; ppc64le

```console
$ docker pull notary@sha256:4b8c0ed5bbccb8e35c7410af94d05b3f5d6f8c632c6d81b219e7b50d7de9c8b2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7172214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f849a8c0825e901d1a6ec9335f193fc228bedfa19b185f358ad4488343b7a46`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Thu, 28 Apr 2022 22:16:20 GMT
ENV TAG=v0.7.0
# Thu, 28 Apr 2022 22:16:25 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Thu, 28 Apr 2022 22:16:28 GMT
ENV INSTALLDIR=/notary/server
# Thu, 28 Apr 2022 22:16:30 GMT
EXPOSE 4443
# Thu, 28 Apr 2022 22:16:32 GMT
WORKDIR /notary/server
# Thu, 28 Apr 2022 22:17:04 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Thu, 28 Apr 2022 22:17:07 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Thu, 28 Apr 2022 22:17:09 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Thu, 28 Apr 2022 22:17:13 GMT
RUN adduser -D -H -g "" notary
# Thu, 28 Apr 2022 22:17:15 GMT
USER notary
# Thu, 28 Apr 2022 22:17:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Thu, 28 Apr 2022 22:17:19 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 28 Apr 2022 22:17:20 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd4e35284ff4e2528fc4509fdcc57e793a7cf4b9a1e48d31805d597a351fae6`  
		Last Modified: Thu, 28 Apr 2022 22:18:42 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f72be742f2ec3385e539f11c19c6c5743b14164e5407ca5ca7999922ecfb2d`  
		Last Modified: Thu, 28 Apr 2022 22:18:43 GMT  
		Size: 4.4 MB (4358892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3457a5e7c2fed48cc8d424cf340f8491c478514eaa6a086368fc43d3655fdf1c`  
		Last Modified: Thu, 28 Apr 2022 22:18:42 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ec375101f50ea0a064e255a340baa8d627347a515c500909afad2c74d436dd`  
		Last Modified: Thu, 28 Apr 2022 22:18:42 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3404bf3d7605da6136b104f3adec48f23abe7befb46c3841379ab5b63c82356e`  
		Last Modified: Thu, 28 Apr 2022 22:18:42 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; s390x

```console
$ docker pull notary@sha256:3c38a6b8c7ef9aacba8e745cc320e692d6a5d4b29b564716c7c7cb3e5c34d0dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7311810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59e7cfdd673403786d855100fff14aaeb47ea2db3103488d947f9b4a5bebbff6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Thu, 28 Apr 2022 20:56:22 GMT
ENV TAG=v0.7.0
# Thu, 28 Apr 2022 20:56:22 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Thu, 28 Apr 2022 20:56:22 GMT
ENV INSTALLDIR=/notary/server
# Thu, 28 Apr 2022 20:56:22 GMT
EXPOSE 4443
# Thu, 28 Apr 2022 20:56:22 GMT
WORKDIR /notary/server
# Thu, 28 Apr 2022 20:56:37 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Thu, 28 Apr 2022 20:56:38 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Thu, 28 Apr 2022 20:56:38 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Thu, 28 Apr 2022 20:56:38 GMT
RUN adduser -D -H -g "" notary
# Thu, 28 Apr 2022 20:56:39 GMT
USER notary
# Thu, 28 Apr 2022 20:56:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Thu, 28 Apr 2022 20:56:39 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 28 Apr 2022 20:56:39 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2ffdf68c103a5f646cae2c69e06544a5ff7d3e460eb735a78b0f460442a035`  
		Last Modified: Thu, 28 Apr 2022 20:57:21 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c085591744a0872ee02429229f5599df4964da062487d4a85387a79929d73a`  
		Last Modified: Thu, 28 Apr 2022 20:57:22 GMT  
		Size: 4.7 MB (4709303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef456144add5878362b5cdcb1644104a6c7fc02c8d5e156e9210565b330ad1f`  
		Last Modified: Thu, 28 Apr 2022 20:57:21 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fc0b4ce37faa9ba2fda5101118e99e43221c9cc5a89cb114da758d7a86946b`  
		Last Modified: Thu, 28 Apr 2022 20:57:21 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5a983a5b9022fd966b73cec456653c86787fe8104b95e43361b148898c7b5f`  
		Last Modified: Thu, 28 Apr 2022 20:57:21 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `notary:server-0.7.0`

```console
$ docker pull notary@sha256:62757be488556ede7da5bd59283c46016b07342266c031b1e06b7d52e721a14b
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
$ docker pull notary@sha256:4674260446d7a73c3f496c752d2ddac3004e182e67040830cb78100bd8284b18
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7753837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79d079083c2b38767518098ace2c6dc1eb7bd8c77f8c7c95a80f60e37f8f7513`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Thu, 28 Apr 2022 21:36:58 GMT
ENV TAG=v0.7.0
# Thu, 28 Apr 2022 21:36:58 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Thu, 28 Apr 2022 21:36:58 GMT
ENV INSTALLDIR=/notary/server
# Thu, 28 Apr 2022 21:36:58 GMT
EXPOSE 4443
# Thu, 28 Apr 2022 21:36:58 GMT
WORKDIR /notary/server
# Thu, 28 Apr 2022 21:37:13 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Thu, 28 Apr 2022 21:37:13 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Thu, 28 Apr 2022 21:37:14 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Thu, 28 Apr 2022 21:37:14 GMT
RUN adduser -D -H -g "" notary
# Thu, 28 Apr 2022 21:37:15 GMT
USER notary
# Thu, 28 Apr 2022 21:37:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Thu, 28 Apr 2022 21:37:15 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 28 Apr 2022 21:37:15 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe8a924f45f7c281c6f5094e5178dc68f022c38326042f43c32ecd50c63acdb`  
		Last Modified: Thu, 28 Apr 2022 21:37:50 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b80533c4d967b4e02ff602bc7968977cf12dd30ca019b3efd762d159fa6b2e`  
		Last Modified: Thu, 28 Apr 2022 21:37:50 GMT  
		Size: 4.9 MB (4937155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584457574f4c95d7f96cdb2c2122d523f12e2b53d23b0110da46b6c6991f194b`  
		Last Modified: Thu, 28 Apr 2022 21:37:50 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf61a1ed3ba555ef09ef0043326dc2071b8e4fe291fa8a31a1cca32a1dd068c`  
		Last Modified: Thu, 28 Apr 2022 21:37:50 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c102fcc61f5e3d1a76864b80c53ee1d3e77b4539895c198ec90a190c030522c`  
		Last Modified: Thu, 28 Apr 2022 21:37:50 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; arm variant v6

```console
$ docker pull notary@sha256:04756f332d3c754b7023b7e2133be2f24e8a43a2a9e0e520a32eb363819b673c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7235935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74b356e59aca62520ccbb384f35da7a00bb2428fdab7104eb35dda1a25672127`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Thu, 28 Apr 2022 20:49:39 GMT
ENV TAG=v0.7.0
# Thu, 28 Apr 2022 20:49:40 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Thu, 28 Apr 2022 20:49:40 GMT
ENV INSTALLDIR=/notary/server
# Thu, 28 Apr 2022 20:49:41 GMT
EXPOSE 4443
# Thu, 28 Apr 2022 20:49:41 GMT
WORKDIR /notary/server
# Thu, 28 Apr 2022 20:50:13 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Thu, 28 Apr 2022 20:50:13 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Thu, 28 Apr 2022 20:50:14 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Thu, 28 Apr 2022 20:50:15 GMT
RUN adduser -D -H -g "" notary
# Thu, 28 Apr 2022 20:50:16 GMT
USER notary
# Thu, 28 Apr 2022 20:50:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Thu, 28 Apr 2022 20:50:17 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 28 Apr 2022 20:50:17 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48adbbc574869c00eb579dbffc35fa365ce1f2c4fca0e4235ec8dd50e627aa01`  
		Last Modified: Thu, 28 Apr 2022 20:51:38 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba90fdc902b07726f8f8b4b7e63e93799a5cf111373ae4a634455debdfc7f28`  
		Last Modified: Thu, 28 Apr 2022 20:51:41 GMT  
		Size: 4.6 MB (4611826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9697deaeac362e43baeeee6da258f87c17c14490e6e66c4a754d0615430c778`  
		Last Modified: Thu, 28 Apr 2022 20:51:38 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d5c3fe154637f1ca01d69167800affffb84b80a84548bd27ac873fa212c8ba`  
		Last Modified: Thu, 28 Apr 2022 20:51:38 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823bd7b4830119c1d7312679ce70606d562c73e16074d8273673df5f06d4a59f`  
		Last Modified: Thu, 28 Apr 2022 20:51:38 GMT  
		Size: 1.2 KB (1185 bytes)  
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
$ docker pull notary@sha256:212bf0a21fcb393cdebcc40077a507b7c9268f5e075042143c640a34a1fb02be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7459426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8ba6dd8a425da479a83e7b7b3fc8185cc6b4e3b9981ed4d8369b744e6b721b2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Thu, 28 Apr 2022 20:58:57 GMT
ENV TAG=v0.7.0
# Thu, 28 Apr 2022 20:58:58 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Thu, 28 Apr 2022 20:58:59 GMT
ENV INSTALLDIR=/notary/server
# Thu, 28 Apr 2022 20:59:00 GMT
EXPOSE 4443
# Thu, 28 Apr 2022 20:59:01 GMT
WORKDIR /notary/server
# Thu, 28 Apr 2022 20:59:17 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Thu, 28 Apr 2022 20:59:19 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Thu, 28 Apr 2022 20:59:20 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Thu, 28 Apr 2022 20:59:20 GMT
RUN adduser -D -H -g "" notary
# Thu, 28 Apr 2022 20:59:21 GMT
USER notary
# Thu, 28 Apr 2022 20:59:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Thu, 28 Apr 2022 20:59:23 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 28 Apr 2022 20:59:24 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0fbe394599acca5b3306739ef20396a34ecbe6436479c45f59347a60b4dfc5`  
		Last Modified: Thu, 28 Apr 2022 21:00:16 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec5a757f1509eb69280bcd844c5445241e34dd7d89d83bd47b2642e6585e23b`  
		Last Modified: Thu, 28 Apr 2022 21:00:16 GMT  
		Size: 4.6 MB (4638351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95a29e888fc0a814de7c46ec0816a38b1fd19747d058a43f67f88533034d5dfa`  
		Last Modified: Thu, 28 Apr 2022 21:00:15 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e23dfa086492f979777742fae9aa2314e900c6a0dddee45cec1370de2c1bee`  
		Last Modified: Thu, 28 Apr 2022 21:00:15 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9647bd875f86c9487e3f546a94239631c089672da3be912b348f3c0507ed423b`  
		Last Modified: Thu, 28 Apr 2022 21:00:15 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; ppc64le

```console
$ docker pull notary@sha256:4b8c0ed5bbccb8e35c7410af94d05b3f5d6f8c632c6d81b219e7b50d7de9c8b2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7172214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f849a8c0825e901d1a6ec9335f193fc228bedfa19b185f358ad4488343b7a46`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Thu, 28 Apr 2022 22:16:20 GMT
ENV TAG=v0.7.0
# Thu, 28 Apr 2022 22:16:25 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Thu, 28 Apr 2022 22:16:28 GMT
ENV INSTALLDIR=/notary/server
# Thu, 28 Apr 2022 22:16:30 GMT
EXPOSE 4443
# Thu, 28 Apr 2022 22:16:32 GMT
WORKDIR /notary/server
# Thu, 28 Apr 2022 22:17:04 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Thu, 28 Apr 2022 22:17:07 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Thu, 28 Apr 2022 22:17:09 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Thu, 28 Apr 2022 22:17:13 GMT
RUN adduser -D -H -g "" notary
# Thu, 28 Apr 2022 22:17:15 GMT
USER notary
# Thu, 28 Apr 2022 22:17:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Thu, 28 Apr 2022 22:17:19 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 28 Apr 2022 22:17:20 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd4e35284ff4e2528fc4509fdcc57e793a7cf4b9a1e48d31805d597a351fae6`  
		Last Modified: Thu, 28 Apr 2022 22:18:42 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f72be742f2ec3385e539f11c19c6c5743b14164e5407ca5ca7999922ecfb2d`  
		Last Modified: Thu, 28 Apr 2022 22:18:43 GMT  
		Size: 4.4 MB (4358892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3457a5e7c2fed48cc8d424cf340f8491c478514eaa6a086368fc43d3655fdf1c`  
		Last Modified: Thu, 28 Apr 2022 22:18:42 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ec375101f50ea0a064e255a340baa8d627347a515c500909afad2c74d436dd`  
		Last Modified: Thu, 28 Apr 2022 22:18:42 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3404bf3d7605da6136b104f3adec48f23abe7befb46c3841379ab5b63c82356e`  
		Last Modified: Thu, 28 Apr 2022 22:18:42 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; s390x

```console
$ docker pull notary@sha256:3c38a6b8c7ef9aacba8e745cc320e692d6a5d4b29b564716c7c7cb3e5c34d0dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7311810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59e7cfdd673403786d855100fff14aaeb47ea2db3103488d947f9b4a5bebbff6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Thu, 28 Apr 2022 20:56:22 GMT
ENV TAG=v0.7.0
# Thu, 28 Apr 2022 20:56:22 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Thu, 28 Apr 2022 20:56:22 GMT
ENV INSTALLDIR=/notary/server
# Thu, 28 Apr 2022 20:56:22 GMT
EXPOSE 4443
# Thu, 28 Apr 2022 20:56:22 GMT
WORKDIR /notary/server
# Thu, 28 Apr 2022 20:56:37 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Thu, 28 Apr 2022 20:56:38 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Thu, 28 Apr 2022 20:56:38 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Thu, 28 Apr 2022 20:56:38 GMT
RUN adduser -D -H -g "" notary
# Thu, 28 Apr 2022 20:56:39 GMT
USER notary
# Thu, 28 Apr 2022 20:56:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Thu, 28 Apr 2022 20:56:39 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 28 Apr 2022 20:56:39 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2ffdf68c103a5f646cae2c69e06544a5ff7d3e460eb735a78b0f460442a035`  
		Last Modified: Thu, 28 Apr 2022 20:57:21 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c085591744a0872ee02429229f5599df4964da062487d4a85387a79929d73a`  
		Last Modified: Thu, 28 Apr 2022 20:57:22 GMT  
		Size: 4.7 MB (4709303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef456144add5878362b5cdcb1644104a6c7fc02c8d5e156e9210565b330ad1f`  
		Last Modified: Thu, 28 Apr 2022 20:57:21 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fc0b4ce37faa9ba2fda5101118e99e43221c9cc5a89cb114da758d7a86946b`  
		Last Modified: Thu, 28 Apr 2022 20:57:21 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5a983a5b9022fd966b73cec456653c86787fe8104b95e43361b148898c7b5f`  
		Last Modified: Thu, 28 Apr 2022 20:57:21 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

## `notary:signer-0.7.0`

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

### `notary:signer-0.7.0` - linux; amd64

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

### `notary:signer-0.7.0` - linux; arm variant v6

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

### `notary:signer-0.7.0` - linux; ppc64le

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

### `notary:signer-0.7.0` - linux; s390x

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
