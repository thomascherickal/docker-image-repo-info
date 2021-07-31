<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `notary`

-	[`notary:server`](#notaryserver)
-	[`notary:server-0.6.1-2`](#notaryserver-061-2)
-	[`notary:signer`](#notarysigner)
-	[`notary:signer-0.6.1-2`](#notarysigner-061-2)

## `notary:server`

```console
$ docker pull notary@sha256:3e4b8d76235507b590fa4999ee43c73be492b8f083a5b6e345338cbf0a7ac908
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
$ docker pull notary@sha256:43f4409374b91208328c212fdf9363ac1e6dc22412eb7217aac751bc5c489dd2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8592976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:162689747d5ac7859de78f9aae1f4ffd15e68bac113e35a855e350a05886234f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 18:58:36 GMT
ENV TAG=v0.6.1
# Mon, 28 Jun 2021 18:58:36 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Mon, 28 Jun 2021 18:58:36 GMT
ENV INSTALLDIR=/notary/server
# Mon, 28 Jun 2021 18:58:36 GMT
EXPOSE 4443
# Mon, 28 Jun 2021 18:58:36 GMT
WORKDIR /notary/server
# Mon, 28 Jun 2021 18:58:52 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Mon, 28 Jun 2021 18:58:52 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Mon, 28 Jun 2021 18:58:52 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Mon, 28 Jun 2021 18:58:53 GMT
RUN adduser -D -H -g "" notary
# Mon, 28 Jun 2021 18:58:54 GMT
USER notary
# Mon, 28 Jun 2021 18:58:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Mon, 28 Jun 2021 18:58:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 28 Jun 2021 18:58:54 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77556963ef8a796bf41535d79d06ba6d80883bdaa9cd149853fa0cb7bf99da0`  
		Last Modified: Mon, 28 Jun 2021 18:59:27 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae7947d7e939530ca197852782ce0cf6546b2508f5b7f70a2ae9940803d415c`  
		Last Modified: Mon, 28 Jun 2021 18:59:28 GMT  
		Size: 5.8 MB (5778894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774741ed1bdb890d7e5e37e13c0a5eaada0dd7dde5d7d6c3dcfa47892f8fef4c`  
		Last Modified: Mon, 28 Jun 2021 18:59:27 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ff51d63b11312605581f793afe414169a074b16e9615348f61425edbfded20`  
		Last Modified: Mon, 28 Jun 2021 18:59:27 GMT  
		Size: 377.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abf3b1ab2eca193532a47a956e16b9412aa4a2724dee7c54260fd27d2acbbc3`  
		Last Modified: Mon, 28 Jun 2021 18:59:27 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; arm variant v6

```console
$ docker pull notary@sha256:ff39898ce819d2188dd777f1a57145af17bbd5a4bcdc9e067f794e4dea3d0e5e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8056890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:939b2a370a70aa61002a2f1e477e470b4c01b5884d8e0e8e82be0120bc28d0af`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Fri, 30 Jul 2021 17:49:55 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Fri, 30 Jul 2021 17:49:55 GMT
CMD ["/bin/sh"]
# Sat, 31 Jul 2021 02:43:20 GMT
ENV TAG=v0.6.1
# Sat, 31 Jul 2021 02:43:21 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Sat, 31 Jul 2021 02:43:21 GMT
ENV INSTALLDIR=/notary/server
# Sat, 31 Jul 2021 02:43:22 GMT
EXPOSE 4443
# Sat, 31 Jul 2021 02:43:22 GMT
WORKDIR /notary/server
# Sat, 31 Jul 2021 02:43:46 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Sat, 31 Jul 2021 02:43:47 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Sat, 31 Jul 2021 02:43:47 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Sat, 31 Jul 2021 02:43:49 GMT
RUN adduser -D -H -g "" notary
# Sat, 31 Jul 2021 02:43:49 GMT
USER notary
# Sat, 31 Jul 2021 02:43:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 31 Jul 2021 02:43:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 31 Jul 2021 02:43:50 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e77fd58416866367e345febdcf08c59429d19d8f01275032a50c325a5e9a31`  
		Last Modified: Sat, 31 Jul 2021 02:45:04 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe8099eed6f984b4359b510cafe4f98a39bc8e9bbaef9873eadc55ae13a1055`  
		Last Modified: Sat, 31 Jul 2021 02:45:07 GMT  
		Size: 5.4 MB (5432634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7e53dde6a1300008c12dbc069886423ccd0e757683017268e39d19a119dc88`  
		Last Modified: Sat, 31 Jul 2021 02:45:04 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a474d9428c87608e9116f76cc3d3b2f6dd49eb18196be94a2e27782537e78297`  
		Last Modified: Sat, 31 Jul 2021 02:45:04 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84db99b4e4a685f30b3bb4164e18d2ae5cc4997a8669d3f5744fea47fa983c0b`  
		Last Modified: Sat, 31 Jul 2021 02:45:04 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:84d37fa149b66ca8f676d231ea0a45a9fa9ee9b0b64c6f1ccd33882fcfe5634d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8049433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaff639380cc586b31a1e46dac0e3b2514e134ffbd03b651630a39a16d3afbba`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 18:41:01 GMT
ENV TAG=v0.6.1
# Mon, 28 Jun 2021 18:41:02 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Mon, 28 Jun 2021 18:41:02 GMT
ENV INSTALLDIR=/notary/server
# Mon, 28 Jun 2021 18:41:02 GMT
EXPOSE 4443
# Mon, 28 Jun 2021 18:41:02 GMT
WORKDIR /notary/server
# Mon, 28 Jun 2021 18:41:15 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Mon, 28 Jun 2021 18:41:15 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Mon, 28 Jun 2021 18:41:16 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Mon, 28 Jun 2021 18:41:17 GMT
RUN adduser -D -H -g "" notary
# Mon, 28 Jun 2021 18:41:17 GMT
USER notary
# Mon, 28 Jun 2021 18:41:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Mon, 28 Jun 2021 18:41:17 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 28 Jun 2021 18:41:17 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0adeb9de9824c29710e237b61cbcbe6fd3a06ee6d782b196281b43d9f6df8d`  
		Last Modified: Mon, 28 Jun 2021 18:41:58 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872551adbbf0fa99b194c79bf451d61f6737218d54a37eda8452f261299d5efa`  
		Last Modified: Mon, 28 Jun 2021 18:41:59 GMT  
		Size: 5.3 MB (5335286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833deb1d1fddec8beb3c60afa38b604c831f69fadded305c0e3c1f3013d69204`  
		Last Modified: Mon, 28 Jun 2021 18:41:57 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcdb1fdfa241c1d8481fd04253374894f79918d98f96d7b5c5d544a89489ec05`  
		Last Modified: Mon, 28 Jun 2021 18:41:57 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e165a9f59ac6310e9902f349c334a4bb56c0744e158a9bf9dcb78063263db3`  
		Last Modified: Mon, 28 Jun 2021 18:41:58 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; 386

```console
$ docker pull notary@sha256:e81817925f77d235fa795ae6392ccf0b31c27a053bd8535984123ed70ba3fe87
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8313192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84878aa0bc86752b72261a25fda7c3c6b001d9a92244bdb5a0437be09b3a69c8`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 18:42:39 GMT
ENV TAG=v0.6.1
# Mon, 28 Jun 2021 18:42:40 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Mon, 28 Jun 2021 18:42:40 GMT
ENV INSTALLDIR=/notary/server
# Mon, 28 Jun 2021 18:42:40 GMT
EXPOSE 4443
# Mon, 28 Jun 2021 18:42:41 GMT
WORKDIR /notary/server
# Mon, 28 Jun 2021 18:43:11 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Mon, 28 Jun 2021 18:43:11 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Mon, 28 Jun 2021 18:43:11 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Mon, 28 Jun 2021 18:43:13 GMT
RUN adduser -D -H -g "" notary
# Mon, 28 Jun 2021 18:43:13 GMT
USER notary
# Mon, 28 Jun 2021 18:43:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Mon, 28 Jun 2021 18:43:13 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 28 Jun 2021 18:43:14 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901d834306dca5d73c86b1a3e642b9623921b12ace19614b6b851c711ba34e30`  
		Last Modified: Mon, 28 Jun 2021 18:44:18 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7854fb2fa81e4225857d0903028f8d8b60388e6bc42d1db7fab53e6c00b69f6a`  
		Last Modified: Mon, 28 Jun 2021 18:44:20 GMT  
		Size: 5.5 MB (5492174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd57aef237b519a95608c73287c0f7025c19f6f8685b4a7c3715a37e29bb21e`  
		Last Modified: Mon, 28 Jun 2021 18:44:18 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b71b6aed3eeb286dd02ff8e1f0c537db2c147943ec0fbd066ec4930a26e4d8d`  
		Last Modified: Mon, 28 Jun 2021 18:44:18 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15732b114c4aed6d8e9f55bfd4e53745154b102cdae6ba7a4b33c54cbed03b4`  
		Last Modified: Mon, 28 Jun 2021 18:44:18 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; ppc64le

```console
$ docker pull notary@sha256:5af658ff448474bdc04b61290495abe2cfa04b70585be899b8b8f058dfa7c93d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8011999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc85a12e820d23ee2de31e4add23daf33eb053d49ffd6e096103a270e8b02f3f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Fri, 30 Jul 2021 17:24:49 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Fri, 30 Jul 2021 17:24:54 GMT
CMD ["/bin/sh"]
# Sat, 31 Jul 2021 04:43:11 GMT
ENV TAG=v0.6.1
# Sat, 31 Jul 2021 04:43:14 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Sat, 31 Jul 2021 04:43:17 GMT
ENV INSTALLDIR=/notary/server
# Sat, 31 Jul 2021 04:43:21 GMT
EXPOSE 4443
# Sat, 31 Jul 2021 04:43:24 GMT
WORKDIR /notary/server
# Sat, 31 Jul 2021 04:43:50 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Sat, 31 Jul 2021 04:43:55 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Sat, 31 Jul 2021 04:43:56 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Sat, 31 Jul 2021 04:44:05 GMT
RUN adduser -D -H -g "" notary
# Sat, 31 Jul 2021 04:44:09 GMT
USER notary
# Sat, 31 Jul 2021 04:44:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 31 Jul 2021 04:44:16 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 31 Jul 2021 04:44:22 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886622024fdd864b1d864bd6dd953482f48a95113ba1f4f92589687f06e16bb6`  
		Last Modified: Sat, 31 Jul 2021 04:46:12 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c5e441cbf4e490c2053585e3e9180cf7dc2f16dfcd730eb2d7a0be3601ab52`  
		Last Modified: Sat, 31 Jul 2021 04:46:14 GMT  
		Size: 5.2 MB (5196728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c784eefd4e69e7be5327cc56edd2d73361105f8737101e603dfd360b4381fc5e`  
		Last Modified: Sat, 31 Jul 2021 04:46:12 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b58b91d245a5327a1b77e124554c2013ce0dc154f618f6da5df2dfe09e51d77`  
		Last Modified: Sat, 31 Jul 2021 04:46:12 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6559516713934a384b6e852c2bd2755794d5df382e7df389aa448941b7b56b`  
		Last Modified: Sat, 31 Jul 2021 04:46:12 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; s390x

```console
$ docker pull notary@sha256:b6c53651085ccbc8bc0f8f0169308219fe52c3430fe62d2c3e4ae6e50640a53e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8213217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0db648c78e9c3a5a9476e44c9f42cddde0825570cf45623c3f97c050ff427b2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Fri, 30 Jul 2021 17:41:41 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Fri, 30 Jul 2021 17:41:42 GMT
CMD ["/bin/sh"]
# Sat, 31 Jul 2021 01:20:21 GMT
ENV TAG=v0.6.1
# Sat, 31 Jul 2021 01:20:21 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Sat, 31 Jul 2021 01:20:21 GMT
ENV INSTALLDIR=/notary/server
# Sat, 31 Jul 2021 01:20:22 GMT
EXPOSE 4443
# Sat, 31 Jul 2021 01:20:22 GMT
WORKDIR /notary/server
# Sat, 31 Jul 2021 01:20:43 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Sat, 31 Jul 2021 01:20:44 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Sat, 31 Jul 2021 01:20:44 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Sat, 31 Jul 2021 01:20:46 GMT
RUN adduser -D -H -g "" notary
# Sat, 31 Jul 2021 01:20:46 GMT
USER notary
# Sat, 31 Jul 2021 01:20:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 31 Jul 2021 01:20:47 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 31 Jul 2021 01:20:47 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de0651af8511dcdf0067a227e07950bb66b8d8f0f0bb97c9560ac438c432949`  
		Last Modified: Sat, 31 Jul 2021 01:21:39 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6534ae68ead77eb18e33c09fc2501369ce94e3b1bf2c8bd0274bd53525d3cd7e`  
		Last Modified: Sat, 31 Jul 2021 01:21:41 GMT  
		Size: 5.6 MB (5608446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae5a5ff10410ab5352f6434ec99b4d5add884cf04d5e6ad15e34ffbbdc2c509`  
		Last Modified: Sat, 31 Jul 2021 01:21:40 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a3d64e310f7e79ae4b04e9e65c984bcdaa3a2641f68ef7da57c06f98abeca2`  
		Last Modified: Sat, 31 Jul 2021 01:21:40 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb32b081a52b7042231fa9b0a14d61f13bfd2b2a565229c4fc8fcb35204486b8`  
		Last Modified: Sat, 31 Jul 2021 01:21:40 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `notary:server-0.6.1-2`

```console
$ docker pull notary@sha256:3e4b8d76235507b590fa4999ee43c73be492b8f083a5b6e345338cbf0a7ac908
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `notary:server-0.6.1-2` - linux; amd64

```console
$ docker pull notary@sha256:43f4409374b91208328c212fdf9363ac1e6dc22412eb7217aac751bc5c489dd2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8592976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:162689747d5ac7859de78f9aae1f4ffd15e68bac113e35a855e350a05886234f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 18:58:36 GMT
ENV TAG=v0.6.1
# Mon, 28 Jun 2021 18:58:36 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Mon, 28 Jun 2021 18:58:36 GMT
ENV INSTALLDIR=/notary/server
# Mon, 28 Jun 2021 18:58:36 GMT
EXPOSE 4443
# Mon, 28 Jun 2021 18:58:36 GMT
WORKDIR /notary/server
# Mon, 28 Jun 2021 18:58:52 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Mon, 28 Jun 2021 18:58:52 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Mon, 28 Jun 2021 18:58:52 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Mon, 28 Jun 2021 18:58:53 GMT
RUN adduser -D -H -g "" notary
# Mon, 28 Jun 2021 18:58:54 GMT
USER notary
# Mon, 28 Jun 2021 18:58:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Mon, 28 Jun 2021 18:58:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 28 Jun 2021 18:58:54 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77556963ef8a796bf41535d79d06ba6d80883bdaa9cd149853fa0cb7bf99da0`  
		Last Modified: Mon, 28 Jun 2021 18:59:27 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae7947d7e939530ca197852782ce0cf6546b2508f5b7f70a2ae9940803d415c`  
		Last Modified: Mon, 28 Jun 2021 18:59:28 GMT  
		Size: 5.8 MB (5778894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774741ed1bdb890d7e5e37e13c0a5eaada0dd7dde5d7d6c3dcfa47892f8fef4c`  
		Last Modified: Mon, 28 Jun 2021 18:59:27 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ff51d63b11312605581f793afe414169a074b16e9615348f61425edbfded20`  
		Last Modified: Mon, 28 Jun 2021 18:59:27 GMT  
		Size: 377.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abf3b1ab2eca193532a47a956e16b9412aa4a2724dee7c54260fd27d2acbbc3`  
		Last Modified: Mon, 28 Jun 2021 18:59:27 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.6.1-2` - linux; arm variant v6

```console
$ docker pull notary@sha256:ff39898ce819d2188dd777f1a57145af17bbd5a4bcdc9e067f794e4dea3d0e5e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8056890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:939b2a370a70aa61002a2f1e477e470b4c01b5884d8e0e8e82be0120bc28d0af`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Fri, 30 Jul 2021 17:49:55 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Fri, 30 Jul 2021 17:49:55 GMT
CMD ["/bin/sh"]
# Sat, 31 Jul 2021 02:43:20 GMT
ENV TAG=v0.6.1
# Sat, 31 Jul 2021 02:43:21 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Sat, 31 Jul 2021 02:43:21 GMT
ENV INSTALLDIR=/notary/server
# Sat, 31 Jul 2021 02:43:22 GMT
EXPOSE 4443
# Sat, 31 Jul 2021 02:43:22 GMT
WORKDIR /notary/server
# Sat, 31 Jul 2021 02:43:46 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Sat, 31 Jul 2021 02:43:47 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Sat, 31 Jul 2021 02:43:47 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Sat, 31 Jul 2021 02:43:49 GMT
RUN adduser -D -H -g "" notary
# Sat, 31 Jul 2021 02:43:49 GMT
USER notary
# Sat, 31 Jul 2021 02:43:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 31 Jul 2021 02:43:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 31 Jul 2021 02:43:50 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e77fd58416866367e345febdcf08c59429d19d8f01275032a50c325a5e9a31`  
		Last Modified: Sat, 31 Jul 2021 02:45:04 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe8099eed6f984b4359b510cafe4f98a39bc8e9bbaef9873eadc55ae13a1055`  
		Last Modified: Sat, 31 Jul 2021 02:45:07 GMT  
		Size: 5.4 MB (5432634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7e53dde6a1300008c12dbc069886423ccd0e757683017268e39d19a119dc88`  
		Last Modified: Sat, 31 Jul 2021 02:45:04 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a474d9428c87608e9116f76cc3d3b2f6dd49eb18196be94a2e27782537e78297`  
		Last Modified: Sat, 31 Jul 2021 02:45:04 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84db99b4e4a685f30b3bb4164e18d2ae5cc4997a8669d3f5744fea47fa983c0b`  
		Last Modified: Sat, 31 Jul 2021 02:45:04 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.6.1-2` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:84d37fa149b66ca8f676d231ea0a45a9fa9ee9b0b64c6f1ccd33882fcfe5634d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8049433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaff639380cc586b31a1e46dac0e3b2514e134ffbd03b651630a39a16d3afbba`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 18:41:01 GMT
ENV TAG=v0.6.1
# Mon, 28 Jun 2021 18:41:02 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Mon, 28 Jun 2021 18:41:02 GMT
ENV INSTALLDIR=/notary/server
# Mon, 28 Jun 2021 18:41:02 GMT
EXPOSE 4443
# Mon, 28 Jun 2021 18:41:02 GMT
WORKDIR /notary/server
# Mon, 28 Jun 2021 18:41:15 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Mon, 28 Jun 2021 18:41:15 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Mon, 28 Jun 2021 18:41:16 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Mon, 28 Jun 2021 18:41:17 GMT
RUN adduser -D -H -g "" notary
# Mon, 28 Jun 2021 18:41:17 GMT
USER notary
# Mon, 28 Jun 2021 18:41:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Mon, 28 Jun 2021 18:41:17 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 28 Jun 2021 18:41:17 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0adeb9de9824c29710e237b61cbcbe6fd3a06ee6d782b196281b43d9f6df8d`  
		Last Modified: Mon, 28 Jun 2021 18:41:58 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872551adbbf0fa99b194c79bf451d61f6737218d54a37eda8452f261299d5efa`  
		Last Modified: Mon, 28 Jun 2021 18:41:59 GMT  
		Size: 5.3 MB (5335286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833deb1d1fddec8beb3c60afa38b604c831f69fadded305c0e3c1f3013d69204`  
		Last Modified: Mon, 28 Jun 2021 18:41:57 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcdb1fdfa241c1d8481fd04253374894f79918d98f96d7b5c5d544a89489ec05`  
		Last Modified: Mon, 28 Jun 2021 18:41:57 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e165a9f59ac6310e9902f349c334a4bb56c0744e158a9bf9dcb78063263db3`  
		Last Modified: Mon, 28 Jun 2021 18:41:58 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.6.1-2` - linux; 386

```console
$ docker pull notary@sha256:e81817925f77d235fa795ae6392ccf0b31c27a053bd8535984123ed70ba3fe87
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8313192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84878aa0bc86752b72261a25fda7c3c6b001d9a92244bdb5a0437be09b3a69c8`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 18:42:39 GMT
ENV TAG=v0.6.1
# Mon, 28 Jun 2021 18:42:40 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Mon, 28 Jun 2021 18:42:40 GMT
ENV INSTALLDIR=/notary/server
# Mon, 28 Jun 2021 18:42:40 GMT
EXPOSE 4443
# Mon, 28 Jun 2021 18:42:41 GMT
WORKDIR /notary/server
# Mon, 28 Jun 2021 18:43:11 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Mon, 28 Jun 2021 18:43:11 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Mon, 28 Jun 2021 18:43:11 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Mon, 28 Jun 2021 18:43:13 GMT
RUN adduser -D -H -g "" notary
# Mon, 28 Jun 2021 18:43:13 GMT
USER notary
# Mon, 28 Jun 2021 18:43:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Mon, 28 Jun 2021 18:43:13 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 28 Jun 2021 18:43:14 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901d834306dca5d73c86b1a3e642b9623921b12ace19614b6b851c711ba34e30`  
		Last Modified: Mon, 28 Jun 2021 18:44:18 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7854fb2fa81e4225857d0903028f8d8b60388e6bc42d1db7fab53e6c00b69f6a`  
		Last Modified: Mon, 28 Jun 2021 18:44:20 GMT  
		Size: 5.5 MB (5492174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd57aef237b519a95608c73287c0f7025c19f6f8685b4a7c3715a37e29bb21e`  
		Last Modified: Mon, 28 Jun 2021 18:44:18 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b71b6aed3eeb286dd02ff8e1f0c537db2c147943ec0fbd066ec4930a26e4d8d`  
		Last Modified: Mon, 28 Jun 2021 18:44:18 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15732b114c4aed6d8e9f55bfd4e53745154b102cdae6ba7a4b33c54cbed03b4`  
		Last Modified: Mon, 28 Jun 2021 18:44:18 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.6.1-2` - linux; ppc64le

```console
$ docker pull notary@sha256:5af658ff448474bdc04b61290495abe2cfa04b70585be899b8b8f058dfa7c93d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8011999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc85a12e820d23ee2de31e4add23daf33eb053d49ffd6e096103a270e8b02f3f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Fri, 30 Jul 2021 17:24:49 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Fri, 30 Jul 2021 17:24:54 GMT
CMD ["/bin/sh"]
# Sat, 31 Jul 2021 04:43:11 GMT
ENV TAG=v0.6.1
# Sat, 31 Jul 2021 04:43:14 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Sat, 31 Jul 2021 04:43:17 GMT
ENV INSTALLDIR=/notary/server
# Sat, 31 Jul 2021 04:43:21 GMT
EXPOSE 4443
# Sat, 31 Jul 2021 04:43:24 GMT
WORKDIR /notary/server
# Sat, 31 Jul 2021 04:43:50 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Sat, 31 Jul 2021 04:43:55 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Sat, 31 Jul 2021 04:43:56 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Sat, 31 Jul 2021 04:44:05 GMT
RUN adduser -D -H -g "" notary
# Sat, 31 Jul 2021 04:44:09 GMT
USER notary
# Sat, 31 Jul 2021 04:44:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 31 Jul 2021 04:44:16 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 31 Jul 2021 04:44:22 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886622024fdd864b1d864bd6dd953482f48a95113ba1f4f92589687f06e16bb6`  
		Last Modified: Sat, 31 Jul 2021 04:46:12 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c5e441cbf4e490c2053585e3e9180cf7dc2f16dfcd730eb2d7a0be3601ab52`  
		Last Modified: Sat, 31 Jul 2021 04:46:14 GMT  
		Size: 5.2 MB (5196728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c784eefd4e69e7be5327cc56edd2d73361105f8737101e603dfd360b4381fc5e`  
		Last Modified: Sat, 31 Jul 2021 04:46:12 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b58b91d245a5327a1b77e124554c2013ce0dc154f618f6da5df2dfe09e51d77`  
		Last Modified: Sat, 31 Jul 2021 04:46:12 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6559516713934a384b6e852c2bd2755794d5df382e7df389aa448941b7b56b`  
		Last Modified: Sat, 31 Jul 2021 04:46:12 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.6.1-2` - linux; s390x

```console
$ docker pull notary@sha256:b6c53651085ccbc8bc0f8f0169308219fe52c3430fe62d2c3e4ae6e50640a53e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8213217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0db648c78e9c3a5a9476e44c9f42cddde0825570cf45623c3f97c050ff427b2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Fri, 30 Jul 2021 17:41:41 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Fri, 30 Jul 2021 17:41:42 GMT
CMD ["/bin/sh"]
# Sat, 31 Jul 2021 01:20:21 GMT
ENV TAG=v0.6.1
# Sat, 31 Jul 2021 01:20:21 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Sat, 31 Jul 2021 01:20:21 GMT
ENV INSTALLDIR=/notary/server
# Sat, 31 Jul 2021 01:20:22 GMT
EXPOSE 4443
# Sat, 31 Jul 2021 01:20:22 GMT
WORKDIR /notary/server
# Sat, 31 Jul 2021 01:20:43 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Sat, 31 Jul 2021 01:20:44 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Sat, 31 Jul 2021 01:20:44 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Sat, 31 Jul 2021 01:20:46 GMT
RUN adduser -D -H -g "" notary
# Sat, 31 Jul 2021 01:20:46 GMT
USER notary
# Sat, 31 Jul 2021 01:20:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 31 Jul 2021 01:20:47 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 31 Jul 2021 01:20:47 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de0651af8511dcdf0067a227e07950bb66b8d8f0f0bb97c9560ac438c432949`  
		Last Modified: Sat, 31 Jul 2021 01:21:39 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6534ae68ead77eb18e33c09fc2501369ce94e3b1bf2c8bd0274bd53525d3cd7e`  
		Last Modified: Sat, 31 Jul 2021 01:21:41 GMT  
		Size: 5.6 MB (5608446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae5a5ff10410ab5352f6434ec99b4d5add884cf04d5e6ad15e34ffbbdc2c509`  
		Last Modified: Sat, 31 Jul 2021 01:21:40 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a3d64e310f7e79ae4b04e9e65c984bcdaa3a2641f68ef7da57c06f98abeca2`  
		Last Modified: Sat, 31 Jul 2021 01:21:40 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb32b081a52b7042231fa9b0a14d61f13bfd2b2a565229c4fc8fcb35204486b8`  
		Last Modified: Sat, 31 Jul 2021 01:21:40 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

## `notary:signer-0.6.1-2`

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

### `notary:signer-0.6.1-2` - linux; amd64

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
