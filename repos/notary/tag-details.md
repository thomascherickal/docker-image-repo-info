<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `notary`

-	[`notary:server`](#notaryserver)
-	[`notary:server-0.7.0`](#notaryserver-070)
-	[`notary:signer`](#notarysigner)
-	[`notary:signer-0.7.0`](#notarysigner-070)

## `notary:server`

```console
$ docker pull notary@sha256:ccc3642d089d17de7147ad871decc3982573b426fcdb603b4a5325096338727d
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
$ docker pull notary@sha256:6b31bfa488d68eeec5b00dbb10d2e9478c39d68c6185bca1bb35f787c667b7c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8208595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa3d36b2afa65b96aff75628e9f60aea0136135045717043b35aad1920ec7514`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:29:46 GMT
ENV TAG=v0.6.1
# Tue, 05 Apr 2022 10:29:46 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 05 Apr 2022 10:29:46 GMT
ENV INSTALLDIR=/notary/server
# Tue, 05 Apr 2022 10:29:46 GMT
EXPOSE 4443
# Tue, 05 Apr 2022 10:29:46 GMT
WORKDIR /notary/server
# Tue, 05 Apr 2022 10:30:01 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Tue, 05 Apr 2022 10:30:01 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Tue, 05 Apr 2022 10:30:01 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Tue, 05 Apr 2022 10:30:02 GMT
RUN adduser -D -H -g "" notary
# Tue, 05 Apr 2022 10:30:02 GMT
USER notary
# Tue, 05 Apr 2022 10:30:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 05 Apr 2022 10:30:02 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 05 Apr 2022 10:30:02 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce7872a467c81c2cebbf77c57a630500a0ccbbef8dcd892ffdca4bb0ee792c0`  
		Last Modified: Tue, 05 Apr 2022 10:30:32 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fdbc4096710704d136b0fa30e267f2474e0ffe99773c87955b8bab4780743d`  
		Last Modified: Tue, 05 Apr 2022 10:30:33 GMT  
		Size: 5.4 MB (5387173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9c1737b7b8f8d5419d60f8ecdbb82f2b9b079cf1a2dac3f492dc27661293ab`  
		Last Modified: Tue, 05 Apr 2022 10:30:32 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86fd630de30c259a81493f2d644cb43f0b9cf72aa612fcc6b9e6dafcda261970`  
		Last Modified: Tue, 05 Apr 2022 10:30:32 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30072905120a5c734bca8c05907d004ac9c6a6ac82c205a66b29ce5057b2d849`  
		Last Modified: Tue, 05 Apr 2022 10:30:32 GMT  
		Size: 1.2 KB (1167 bytes)  
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
$ docker pull notary@sha256:fce3d92b6b1ec37c354246581f91772c53d800c225d8ba6e59116e4054fefb22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7274736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d07a5e0f6c959b960d980ea3d464e5c692332d3c240cca7b8c428bcdd834476d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Thu, 28 Apr 2022 20:59:02 GMT
ENV TAG=v0.7.0
# Thu, 28 Apr 2022 20:59:03 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Thu, 28 Apr 2022 20:59:04 GMT
ENV INSTALLDIR=/notary/server
# Thu, 28 Apr 2022 20:59:05 GMT
EXPOSE 4443
# Thu, 28 Apr 2022 20:59:06 GMT
WORKDIR /notary/server
# Thu, 28 Apr 2022 20:59:19 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Thu, 28 Apr 2022 20:59:21 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Thu, 28 Apr 2022 20:59:22 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Thu, 28 Apr 2022 20:59:22 GMT
RUN adduser -D -H -g "" notary
# Thu, 28 Apr 2022 20:59:23 GMT
USER notary
# Thu, 28 Apr 2022 20:59:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Thu, 28 Apr 2022 20:59:25 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 28 Apr 2022 20:59:26 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c119ef803b4ec0fe0bb2435f63468e0138d93000a089716f429cb7d30e821ff3`  
		Last Modified: Thu, 28 Apr 2022 21:00:15 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ee52efa4dfc7a4bb9170de6f51e991bbab5e4b994ee086f2b03257a9dc38fb`  
		Last Modified: Thu, 28 Apr 2022 21:00:16 GMT  
		Size: 4.6 MB (4556160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c41ca8556c31df6f47fa1bd062e8151848d9e7aac668231d65b0fe9d73ad4674`  
		Last Modified: Thu, 28 Apr 2022 21:00:15 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8dcaade17e2a897e706121bae6ad26df48d5e7102c4083b2db4a7aa5915529e`  
		Last Modified: Thu, 28 Apr 2022 21:00:15 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23098e42e4ec2356ce5624c8132e781b719126ec8c9fa04555e7cedc6aa49df0`  
		Last Modified: Thu, 28 Apr 2022 21:00:15 GMT  
		Size: 1.2 KB (1183 bytes)  
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
$ docker pull notary@sha256:d246f52706baa526e2471411daceaac18c1cdfad58a0a9a88f281afddb20ff27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7618819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc442e8f20de6045d499b07abb4a3e3731be1f28d0a9f24ce587dd000549f631`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:56 GMT
ADD file:a9d5347a58c095f620406d9afc12b5ae4fd6c3994ea7e88e6415db7b09725289 in / 
# Tue, 05 Apr 2022 00:24:00 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:19:13 GMT
ENV TAG=v0.6.1
# Tue, 05 Apr 2022 11:19:15 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 05 Apr 2022 11:19:18 GMT
ENV INSTALLDIR=/notary/server
# Tue, 05 Apr 2022 11:19:21 GMT
EXPOSE 4443
# Tue, 05 Apr 2022 11:19:23 GMT
WORKDIR /notary/server
# Tue, 05 Apr 2022 11:19:52 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Tue, 05 Apr 2022 11:19:53 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Tue, 05 Apr 2022 11:19:55 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Tue, 05 Apr 2022 11:20:04 GMT
RUN adduser -D -H -g "" notary
# Tue, 05 Apr 2022 11:20:07 GMT
USER notary
# Tue, 05 Apr 2022 11:20:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 05 Apr 2022 11:20:12 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 05 Apr 2022 11:20:13 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:afbded953e7f469508815262f0ff60fc06823cc1701e4b7aa211eb10bca545bd`  
		Last Modified: Tue, 05 Apr 2022 00:25:18 GMT  
		Size: 2.8 MB (2814791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9d4b101d59127772fe29076100ab8c2da0bfe8471a86c6ca52943d1d64ece6`  
		Last Modified: Tue, 05 Apr 2022 11:21:48 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb281cb6061176b1cb2452285c2ec0a492d680d8cc3dcb7e939a6c349ef585fb`  
		Last Modified: Tue, 05 Apr 2022 11:21:49 GMT  
		Size: 4.8 MB (4801899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39350c84f3706e68b11642143abbae09e84547430b8e0c64ba8de9a90369800e`  
		Last Modified: Tue, 05 Apr 2022 11:21:48 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569b8c01cf16565735cd83f76e05f4f45d6c3207541907ea27dc8b59bc0e6f15`  
		Last Modified: Tue, 05 Apr 2022 11:21:48 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c023b243258d7c44f7b8311d3835f477e093714c35afdb24deb0adf35c83ffd`  
		Last Modified: Tue, 05 Apr 2022 11:21:48 GMT  
		Size: 1.2 KB (1176 bytes)  
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
$ docker pull notary@sha256:58cae8272cbc4961d5b1060da018e6e881596192671ec8fefff46eab083523c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; s390x

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
$ docker pull notary@sha256:fce3d92b6b1ec37c354246581f91772c53d800c225d8ba6e59116e4054fefb22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7274736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d07a5e0f6c959b960d980ea3d464e5c692332d3c240cca7b8c428bcdd834476d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Thu, 28 Apr 2022 20:59:02 GMT
ENV TAG=v0.7.0
# Thu, 28 Apr 2022 20:59:03 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Thu, 28 Apr 2022 20:59:04 GMT
ENV INSTALLDIR=/notary/server
# Thu, 28 Apr 2022 20:59:05 GMT
EXPOSE 4443
# Thu, 28 Apr 2022 20:59:06 GMT
WORKDIR /notary/server
# Thu, 28 Apr 2022 20:59:19 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Thu, 28 Apr 2022 20:59:21 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Thu, 28 Apr 2022 20:59:22 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Thu, 28 Apr 2022 20:59:22 GMT
RUN adduser -D -H -g "" notary
# Thu, 28 Apr 2022 20:59:23 GMT
USER notary
# Thu, 28 Apr 2022 20:59:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Thu, 28 Apr 2022 20:59:25 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 28 Apr 2022 20:59:26 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c119ef803b4ec0fe0bb2435f63468e0138d93000a089716f429cb7d30e821ff3`  
		Last Modified: Thu, 28 Apr 2022 21:00:15 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ee52efa4dfc7a4bb9170de6f51e991bbab5e4b994ee086f2b03257a9dc38fb`  
		Last Modified: Thu, 28 Apr 2022 21:00:16 GMT  
		Size: 4.6 MB (4556160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c41ca8556c31df6f47fa1bd062e8151848d9e7aac668231d65b0fe9d73ad4674`  
		Last Modified: Thu, 28 Apr 2022 21:00:15 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8dcaade17e2a897e706121bae6ad26df48d5e7102c4083b2db4a7aa5915529e`  
		Last Modified: Thu, 28 Apr 2022 21:00:15 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23098e42e4ec2356ce5624c8132e781b719126ec8c9fa04555e7cedc6aa49df0`  
		Last Modified: Thu, 28 Apr 2022 21:00:15 GMT  
		Size: 1.2 KB (1183 bytes)  
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
$ docker pull notary@sha256:964ae73f771f2393a06e641fb140563ac96dacfea10299ff8857ea4056df37c8
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
$ docker pull notary@sha256:44f117f30922793e76f4d48c38ea7e48801ffd70b6718b0bb8504e4c7dd63ce5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7690976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:785cf5694e3a633c4fe81218642e11df3f9a891c5bb3fbf493357cc343dd5454`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:29:46 GMT
ENV TAG=v0.6.1
# Tue, 05 Apr 2022 10:29:46 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 05 Apr 2022 10:30:05 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 05 Apr 2022 10:30:05 GMT
EXPOSE 4444
# Tue, 05 Apr 2022 10:30:06 GMT
EXPOSE 7899
# Tue, 05 Apr 2022 10:30:06 GMT
WORKDIR /notary/signer
# Tue, 05 Apr 2022 10:30:20 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Tue, 05 Apr 2022 10:30:20 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Tue, 05 Apr 2022 10:30:20 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Tue, 05 Apr 2022 10:30:21 GMT
RUN adduser -D -H -g "" notary
# Tue, 05 Apr 2022 10:30:21 GMT
USER notary
# Tue, 05 Apr 2022 10:30:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 05 Apr 2022 10:30:21 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 05 Apr 2022 10:30:21 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb410511d0d5e78ad31c5f248da2b0f0d7e88a25d2c6b58051dcf8b7fa3722b`  
		Last Modified: Tue, 05 Apr 2022 10:30:42 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74f6af36413f34a740b7a0ba1706a95db01175d2086fe02ecaae4bfa273d99b`  
		Last Modified: Tue, 05 Apr 2022 10:30:43 GMT  
		Size: 4.9 MB (4869606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074f61631574424b1185ce7e2c35720cd690dbb57c46fb7e493403fb51fafda7`  
		Last Modified: Tue, 05 Apr 2022 10:30:42 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0336feabce1e13b60b87793e745349d0e54f3424a15bb00223cf5b0bdb7f62`  
		Last Modified: Tue, 05 Apr 2022 10:30:42 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf7c16c3a9208773e09ddcd08178231872e84a5d6dd14c096a4b8264ebc023b`  
		Last Modified: Tue, 05 Apr 2022 10:30:42 GMT  
		Size: 1.2 KB (1171 bytes)  
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
$ docker pull notary@sha256:04fa2dc8ed10b9b436db7ed75adabef327c7b3986699a7229eccbcfff65be529
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6933666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7222c4c18e9c1bb80c942388327a4bbfb155d9f34286578b575a4fa510dbd2f0`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Thu, 28 Apr 2022 20:59:02 GMT
ENV TAG=v0.7.0
# Thu, 28 Apr 2022 20:59:03 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Thu, 28 Apr 2022 20:59:33 GMT
ENV INSTALLDIR=/notary/signer
# Thu, 28 Apr 2022 20:59:34 GMT
EXPOSE 4444
# Thu, 28 Apr 2022 20:59:35 GMT
EXPOSE 7899
# Thu, 28 Apr 2022 20:59:36 GMT
WORKDIR /notary/signer
# Thu, 28 Apr 2022 20:59:49 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Thu, 28 Apr 2022 20:59:51 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Thu, 28 Apr 2022 20:59:52 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Thu, 28 Apr 2022 20:59:52 GMT
RUN adduser -D -H -g "" notary
# Thu, 28 Apr 2022 20:59:53 GMT
USER notary
# Thu, 28 Apr 2022 20:59:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Thu, 28 Apr 2022 20:59:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 28 Apr 2022 20:59:56 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f724e35e24388ab569d2f65adde8a6c858d53b36bd0529cbfb3912760e1af6`  
		Last Modified: Thu, 28 Apr 2022 21:00:27 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1470d8c827979e9c08626df0742cbeed433e2aaa47d1f1f78f6b8ee5fddf6ff4`  
		Last Modified: Thu, 28 Apr 2022 21:00:28 GMT  
		Size: 4.2 MB (4215152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91966d37d2fd9b668e4aa9441f0f64ca9376961c8a5989a60bc5494e7833ebfa`  
		Last Modified: Thu, 28 Apr 2022 21:00:27 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ed5247d92ada7d48ed04629fe0a92c985335f71ade3f4b5ea3fad5ae1f76dd`  
		Last Modified: Thu, 28 Apr 2022 21:00:27 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8991868dd45b58b1df9d819c63fb545b3019a8f9db08c1cdecc837c787e324`  
		Last Modified: Thu, 28 Apr 2022 21:00:27 GMT  
		Size: 1.2 KB (1183 bytes)  
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
$ docker pull notary@sha256:11f853f0ab53e1ed5939953e13fb2fcb91447f7ac1833648512eb816b9d8b0f9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7154614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e58ed464da460d79e4acb9b1dc906baaefdae68b12785381b59eee94f6b4a90`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:56 GMT
ADD file:a9d5347a58c095f620406d9afc12b5ae4fd6c3994ea7e88e6415db7b09725289 in / 
# Tue, 05 Apr 2022 00:24:00 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:19:13 GMT
ENV TAG=v0.6.1
# Tue, 05 Apr 2022 11:19:15 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 05 Apr 2022 11:20:24 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 05 Apr 2022 11:20:26 GMT
EXPOSE 4444
# Tue, 05 Apr 2022 11:20:30 GMT
EXPOSE 7899
# Tue, 05 Apr 2022 11:20:33 GMT
WORKDIR /notary/signer
# Tue, 05 Apr 2022 11:20:56 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Tue, 05 Apr 2022 11:20:59 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Tue, 05 Apr 2022 11:21:00 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Tue, 05 Apr 2022 11:21:07 GMT
RUN adduser -D -H -g "" notary
# Tue, 05 Apr 2022 11:21:10 GMT
USER notary
# Tue, 05 Apr 2022 11:21:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 05 Apr 2022 11:21:18 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 05 Apr 2022 11:21:23 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:afbded953e7f469508815262f0ff60fc06823cc1701e4b7aa211eb10bca545bd`  
		Last Modified: Tue, 05 Apr 2022 00:25:18 GMT  
		Size: 2.8 MB (2814791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ed3d483d5b28cbb5ddbb7617f627ac98cb1be502de16f9f2142bf90be77ba4`  
		Last Modified: Tue, 05 Apr 2022 11:22:04 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f82a5122c73ebe87551600dedc06ef6346fa50d153d4c317ff178bdee27e6fc`  
		Last Modified: Tue, 05 Apr 2022 11:22:04 GMT  
		Size: 4.3 MB (4337769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab602ec3b6f8d575b40e9883a1d1e0dda91c5ab7a07f1df9b746b9dc3c88584e`  
		Last Modified: Tue, 05 Apr 2022 11:22:03 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec900c07dc4fd312c906966fdd0bf95ed247cdd7fe12c0dd87f66b0c663923ed`  
		Last Modified: Tue, 05 Apr 2022 11:22:03 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0337124674433fd9a3fa73816a42e56ee36b5a7de1de4b8f3c33c3dbafe6202b`  
		Last Modified: Tue, 05 Apr 2022 11:22:04 GMT  
		Size: 1.2 KB (1173 bytes)  
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
$ docker pull notary@sha256:a5dc4a9b8395e6d90598d8a3cdcfa12ccb56e990398c3c7df51acd12b7302726
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; s390x

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
$ docker pull notary@sha256:04fa2dc8ed10b9b436db7ed75adabef327c7b3986699a7229eccbcfff65be529
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6933666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7222c4c18e9c1bb80c942388327a4bbfb155d9f34286578b575a4fa510dbd2f0`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Thu, 28 Apr 2022 20:59:02 GMT
ENV TAG=v0.7.0
# Thu, 28 Apr 2022 20:59:03 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Thu, 28 Apr 2022 20:59:33 GMT
ENV INSTALLDIR=/notary/signer
# Thu, 28 Apr 2022 20:59:34 GMT
EXPOSE 4444
# Thu, 28 Apr 2022 20:59:35 GMT
EXPOSE 7899
# Thu, 28 Apr 2022 20:59:36 GMT
WORKDIR /notary/signer
# Thu, 28 Apr 2022 20:59:49 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Thu, 28 Apr 2022 20:59:51 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Thu, 28 Apr 2022 20:59:52 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Thu, 28 Apr 2022 20:59:52 GMT
RUN adduser -D -H -g "" notary
# Thu, 28 Apr 2022 20:59:53 GMT
USER notary
# Thu, 28 Apr 2022 20:59:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Thu, 28 Apr 2022 20:59:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 28 Apr 2022 20:59:56 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f724e35e24388ab569d2f65adde8a6c858d53b36bd0529cbfb3912760e1af6`  
		Last Modified: Thu, 28 Apr 2022 21:00:27 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1470d8c827979e9c08626df0742cbeed433e2aaa47d1f1f78f6b8ee5fddf6ff4`  
		Last Modified: Thu, 28 Apr 2022 21:00:28 GMT  
		Size: 4.2 MB (4215152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91966d37d2fd9b668e4aa9441f0f64ca9376961c8a5989a60bc5494e7833ebfa`  
		Last Modified: Thu, 28 Apr 2022 21:00:27 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ed5247d92ada7d48ed04629fe0a92c985335f71ade3f4b5ea3fad5ae1f76dd`  
		Last Modified: Thu, 28 Apr 2022 21:00:27 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8991868dd45b58b1df9d819c63fb545b3019a8f9db08c1cdecc837c787e324`  
		Last Modified: Thu, 28 Apr 2022 21:00:27 GMT  
		Size: 1.2 KB (1183 bytes)  
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
