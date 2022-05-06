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
