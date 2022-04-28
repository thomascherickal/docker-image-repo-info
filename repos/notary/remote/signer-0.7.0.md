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
