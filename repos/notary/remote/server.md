## `notary:server`

```console
$ docker pull notary@sha256:05005f5a886a74fac32d05f49c8080405d61d2bae1e4175de3efc02e46d5ffa4
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
$ docker pull notary@sha256:67ffe7a46b7806128d92bda4c1b690b26ea4a2f0ba810a82fbc7142ddb2943cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8207893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cca52a83cf1a2a6216ae2be361a5a75be35478313ecc9177fbda0a59af156a2d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 03:13:51 GMT
ENV TAG=v0.6.1
# Wed, 01 Sep 2021 03:13:51 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Wed, 01 Sep 2021 03:13:52 GMT
ENV INSTALLDIR=/notary/server
# Wed, 01 Sep 2021 03:13:52 GMT
EXPOSE 4443
# Wed, 01 Sep 2021 03:13:52 GMT
WORKDIR /notary/server
# Wed, 01 Sep 2021 03:14:11 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Wed, 01 Sep 2021 03:14:11 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Wed, 01 Sep 2021 03:14:11 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Wed, 01 Sep 2021 03:14:12 GMT
RUN adduser -D -H -g "" notary
# Wed, 01 Sep 2021 03:14:13 GMT
USER notary
# Wed, 01 Sep 2021 03:14:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Wed, 01 Sep 2021 03:14:13 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Sep 2021 03:14:13 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7563319b599f4b2880de541811e7aa09df2d754a7aff1c29f2bd82734f00f63b`  
		Last Modified: Wed, 01 Sep 2021 03:14:51 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a9ac2020932ed3fa1dd909e958fe0de479168166ac890c02f5aababd9e94d6`  
		Last Modified: Wed, 01 Sep 2021 03:14:53 GMT  
		Size: 5.4 MB (5391688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cc192082178ba426f4668d919fd331ed9ffadaa27dc421222e4ec486c4794a`  
		Last Modified: Wed, 01 Sep 2021 03:14:51 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6d214a7821c7637a982e72d16658a619473d1d83151e101582ff51bf9d5d9f`  
		Last Modified: Wed, 01 Sep 2021 03:14:51 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3416e2a15f0632f19e8488e51c5016e6f8da1e459ed5b6cc8108bd8f71f01f9a`  
		Last Modified: Wed, 01 Sep 2021 03:14:51 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; arm variant v6

```console
$ docker pull notary@sha256:c9a63790b120cdbfc708dcda2bd2a5e33d0b4b7c24ac091e5188554c4d9b83cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7669520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79f6b34f2daf1485b896a6fd665e468b70ba83169a21a3afbc098dbf3e4a5e46`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:33 GMT
ADD file:ed2b5e0fbd1e7ae37ab8f808c827d23c6841ce1edd7427552d5bf741d67ebcc0 in / 
# Tue, 31 Aug 2021 22:30:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 05:40:38 GMT
ENV TAG=v0.6.1
# Wed, 01 Sep 2021 05:40:39 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Wed, 01 Sep 2021 05:40:39 GMT
ENV INSTALLDIR=/notary/server
# Wed, 01 Sep 2021 05:40:40 GMT
EXPOSE 4443
# Wed, 01 Sep 2021 05:40:40 GMT
WORKDIR /notary/server
# Wed, 01 Sep 2021 05:41:05 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Wed, 01 Sep 2021 05:41:05 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Wed, 01 Sep 2021 05:41:06 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Wed, 01 Sep 2021 05:41:07 GMT
RUN adduser -D -H -g "" notary
# Wed, 01 Sep 2021 05:41:08 GMT
USER notary
# Wed, 01 Sep 2021 05:41:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Wed, 01 Sep 2021 05:41:09 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Sep 2021 05:41:09 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:840d18d84f6afdc3231d126fdd3f84f23f0335b61cbfa9cb8808b888a4308919`  
		Last Modified: Tue, 31 Aug 2021 22:32:11 GMT  
		Size: 2.6 MB (2623761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9791b32cb2bee0a0b775d8371df3e8c553536fb8eea6b87917960002d729a8d4`  
		Last Modified: Wed, 01 Sep 2021 05:42:22 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1829517afacd837ea27a38cfeb23b911d1800a10c4716a3c0e4f991167e17cea`  
		Last Modified: Wed, 01 Sep 2021 05:42:24 GMT  
		Size: 5.0 MB (5043640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df17778e7033a45144aa86f0dd5a1ca55f56889651c7c018c7002dd39b9c2d1c`  
		Last Modified: Wed, 01 Sep 2021 05:42:22 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67729e596106cdd9114ac21e8c4bfc0fc7ac3d1421fecd99044eefcefdb04909`  
		Last Modified: Wed, 01 Sep 2021 05:42:22 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721b9740d73d966ff04dd47698ac8ecb6daa1e55a2a087b23c8828cda0c2a4e3`  
		Last Modified: Wed, 01 Sep 2021 05:42:23 GMT  
		Size: 1.2 KB (1170 bytes)  
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
$ docker pull notary@sha256:7bd21d589d36965d05f8ea2c22cb3f1f4927559f0c7cd93beb1d6007c72457c7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7925543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aed58ef6de2cc5ba00a2e02b0ccd753e0ea362c744c8c8ad4ff9f1b9203e704b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Tue, 31 Aug 2021 21:23:28 GMT
ADD file:fb9d541cffc3a5660d23426ba847aa696b59a9d7f14e00ba0a63b28c9ec272c0 in / 
# Tue, 31 Aug 2021 21:23:29 GMT
CMD ["/bin/sh"]
# Tue, 31 Aug 2021 23:39:54 GMT
ENV TAG=v0.6.1
# Tue, 31 Aug 2021 23:39:54 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Tue, 31 Aug 2021 23:39:54 GMT
ENV INSTALLDIR=/notary/server
# Tue, 31 Aug 2021 23:39:55 GMT
EXPOSE 4443
# Tue, 31 Aug 2021 23:39:55 GMT
WORKDIR /notary/server
# Tue, 31 Aug 2021 23:40:14 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Tue, 31 Aug 2021 23:40:14 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Tue, 31 Aug 2021 23:40:14 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Tue, 31 Aug 2021 23:40:15 GMT
RUN adduser -D -H -g "" notary
# Tue, 31 Aug 2021 23:40:16 GMT
USER notary
# Tue, 31 Aug 2021 23:40:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 31 Aug 2021 23:40:16 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 31 Aug 2021 23:40:16 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:4ed7d06bd90bc8d13b87220ccc6204a7d235ec943be9fb4289d856f9ff0a5b7b`  
		Last Modified: Tue, 31 Aug 2021 21:24:28 GMT  
		Size: 2.8 MB (2821095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f309a72780c0ae33127f3d9648feaa3dd524ff498129bc563de603752c5825`  
		Last Modified: Tue, 31 Aug 2021 23:41:05 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28501c64e3369880c178e46a15a6e74b8afb5623d2de0f4ba2155c0a9c84689`  
		Last Modified: Tue, 31 Aug 2021 23:41:06 GMT  
		Size: 5.1 MB (5102327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:887ed1e71237dd3118e189e7b0b716daa96d6358eb59c33eb4c2ce1afb9b8d1a`  
		Last Modified: Tue, 31 Aug 2021 23:41:05 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4debc595f02ce78ea65231fc7907840b8888dc35f4811bcb5d0cc3e8dcc2d5b2`  
		Last Modified: Tue, 31 Aug 2021 23:41:05 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5679870d8918954f4852fa7e70aa4cc8a33feee628d5a035446a67eed3398cd`  
		Last Modified: Tue, 31 Aug 2021 23:41:05 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; ppc64le

```console
$ docker pull notary@sha256:5ebfcc4e2ce9fba290bb3dce5f72828507f4b391a86824248f20d276628b8bc4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7625145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdc726b8e6fdee456c512b7b4669685327a649b5c8336a23499f941f3f6d850e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--help"]`

```dockerfile
# Wed, 01 Sep 2021 02:42:40 GMT
ADD file:07a51f1a2f818bd1c1651832ce63cb1e0046a57994724cda6a20ff1a2a685295 in / 
# Wed, 01 Sep 2021 02:42:41 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 11:31:28 GMT
ENV TAG=v0.6.1
# Wed, 01 Sep 2021 11:31:32 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Wed, 01 Sep 2021 11:31:38 GMT
ENV INSTALLDIR=/notary/server
# Wed, 01 Sep 2021 11:31:43 GMT
EXPOSE 4443
# Wed, 01 Sep 2021 11:31:47 GMT
WORKDIR /notary/server
# Wed, 01 Sep 2021 11:32:09 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-server;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-server ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-server --help
# Wed, 01 Sep 2021 11:32:10 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Wed, 01 Sep 2021 11:32:11 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Wed, 01 Sep 2021 11:32:19 GMT
RUN adduser -D -H -g "" notary
# Wed, 01 Sep 2021 11:32:20 GMT
USER notary
# Wed, 01 Sep 2021 11:32:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Wed, 01 Sep 2021 11:32:24 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Sep 2021 11:32:26 GMT
CMD ["notary-server" "--help"]
```

-	Layers:
	-	`sha256:39d9bf63205258fe1d085fd596101e6fc46ff796cda8d3ba2983e166a25b74db`  
		Last Modified: Wed, 01 Sep 2021 02:43:53 GMT  
		Size: 2.8 MB (2814813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c975bde7d3c508db3b7430faa12453ba1fcb4b38930168a6c482c5f16122adfe`  
		Last Modified: Wed, 01 Sep 2021 11:33:51 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1bbe6c8c639d47e3a0363729bb630caf92f6eb77f8c27186dbf9c1ffb61490`  
		Last Modified: Wed, 01 Sep 2021 11:33:52 GMT  
		Size: 4.8 MB (4808212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d167ff7519a7e7657df22f676e7b6693d1845213f43feeac7f8b504985ccfb6`  
		Last Modified: Wed, 01 Sep 2021 11:33:51 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de91a48bec8aa3318a6ffb570b17be8ae9cece4ddf092e0d4cd80461ff8acf2`  
		Last Modified: Wed, 01 Sep 2021 11:33:51 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf45fde51aee48def303ba9b620770e78af2bb1281c50a4841ac1d7025f7ee1`  
		Last Modified: Wed, 01 Sep 2021 11:33:51 GMT  
		Size: 1.2 KB (1171 bytes)  
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
