## `notary:signer`

```console
$ docker pull notary@sha256:fdc627881634875cd4b1ebeb2300d1d07b62d2ddacf48aad4e0845254b19741c
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
$ docker pull notary@sha256:a3024c444f372965bb9e02409cbd51cf83cf64e34eb6c2cb59cda240ca1df125
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7688013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26aad70f50d38c07bd7f33356fcb4df3bdaaec3a4831c088d8b272bda896ccef`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 03:13:51 GMT
ENV TAG=v0.6.1
# Wed, 01 Sep 2021 03:13:51 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Wed, 01 Sep 2021 03:14:17 GMT
ENV INSTALLDIR=/notary/signer
# Wed, 01 Sep 2021 03:14:17 GMT
EXPOSE 4444
# Wed, 01 Sep 2021 03:14:17 GMT
EXPOSE 7899
# Wed, 01 Sep 2021 03:14:17 GMT
WORKDIR /notary/signer
# Wed, 01 Sep 2021 03:14:36 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Wed, 01 Sep 2021 03:14:36 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Wed, 01 Sep 2021 03:14:36 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Wed, 01 Sep 2021 03:14:37 GMT
RUN adduser -D -H -g "" notary
# Wed, 01 Sep 2021 03:14:37 GMT
USER notary
# Wed, 01 Sep 2021 03:14:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Wed, 01 Sep 2021 03:14:38 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Sep 2021 03:14:38 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0640cea0fffa153e8a43f0cc1bba1b442e6294eba3a414a7326a92ae1774d9e`  
		Last Modified: Wed, 01 Sep 2021 03:15:03 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3826f26db296ff4a05ad4906679d7baae10106106a52ebe02a1d5eade5d6177f`  
		Last Modified: Wed, 01 Sep 2021 03:15:04 GMT  
		Size: 4.9 MB (4871876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e403c8609bed446927d18879dab4a45d49fa3bfac062d23d1f193b6912542a`  
		Last Modified: Wed, 01 Sep 2021 03:15:03 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2d426533852ba181bb1c0526d7e9d9947021478043d28a381f7252ced4a368`  
		Last Modified: Wed, 01 Sep 2021 03:15:03 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70ee8e69aa78933fce9ce6c3d810dee7282f82b7277216c5129e46719bc091d`  
		Last Modified: Wed, 01 Sep 2021 03:15:03 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; arm variant v6

```console
$ docker pull notary@sha256:52b275fa4534a12411d36cbce68be3d6c4b11a1070146bc8ba94be7072903fee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7192790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3415f4441be11444f9ded9795017d4e6e0f25da238a7a69afd18ac925db1f386`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 03:01:40 GMT
ENV TAG=v0.6.1
# Sat, 13 Nov 2021 03:01:41 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Sat, 13 Nov 2021 03:02:20 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 13 Nov 2021 03:02:21 GMT
EXPOSE 4444
# Sat, 13 Nov 2021 03:02:21 GMT
EXPOSE 7899
# Sat, 13 Nov 2021 03:02:22 GMT
WORKDIR /notary/signer
# Sat, 13 Nov 2021 03:02:44 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Sat, 13 Nov 2021 03:02:44 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Sat, 13 Nov 2021 03:02:45 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Sat, 13 Nov 2021 03:02:46 GMT
RUN adduser -D -H -g "" notary
# Sat, 13 Nov 2021 03:02:47 GMT
USER notary
# Sat, 13 Nov 2021 03:02:47 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 13 Nov 2021 03:02:47 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 13 Nov 2021 03:02:48 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee33bfcf4a31088b99022e05c8ded85a1d465df40835ad3942751b9f9e981bb`  
		Last Modified: Sat, 13 Nov 2021 03:03:33 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd59c06a753746120bdbe12e14684ef2b3bed8aa76ead284db954163a3e1d838`  
		Last Modified: Sat, 13 Nov 2021 03:03:36 GMT  
		Size: 4.6 MB (4557382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910596fc4e438a3e10dfee3276b779b36378ec5000f3b220956007fd89b2e794`  
		Last Modified: Sat, 13 Nov 2021 03:03:33 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6102c7c03a66a09b142055fa0a619db8f7e835ed4436263da6665fe41c44198`  
		Last Modified: Sat, 13 Nov 2021 03:03:33 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f6c3313243bc4bf7e5361aa2048989bf950271bc8ffc5b7b2ee840b00792fe`  
		Last Modified: Sat, 13 Nov 2021 03:03:33 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:6fefe152b56505b59cfd4e97cebbfd7514d1e8685dc9810c756f79fa6f697c9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7182203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ade0436dde6056ffa83df7107a2af83084291618c1e1d4749b943e2b42f0250`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 00:13:38 GMT
ENV TAG=v0.6.1
# Sat, 13 Nov 2021 00:13:39 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Sat, 13 Nov 2021 00:14:09 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 13 Nov 2021 00:14:10 GMT
EXPOSE 4444
# Sat, 13 Nov 2021 00:14:11 GMT
EXPOSE 7899
# Sat, 13 Nov 2021 00:14:12 GMT
WORKDIR /notary/signer
# Sat, 13 Nov 2021 00:14:25 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Sat, 13 Nov 2021 00:14:27 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Sat, 13 Nov 2021 00:14:28 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Sat, 13 Nov 2021 00:14:28 GMT
RUN adduser -D -H -g "" notary
# Sat, 13 Nov 2021 00:14:29 GMT
USER notary
# Sat, 13 Nov 2021 00:14:30 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 13 Nov 2021 00:14:31 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 13 Nov 2021 00:14:32 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73c68a67445be4c877ecd7986db3857403f81b0cbe4b276300309b7c953d1bd`  
		Last Modified: Sat, 13 Nov 2021 00:15:04 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8ad0750bbda32429d887e25820911a19ef9034a569020bae511ba5425fd7f9`  
		Last Modified: Sat, 13 Nov 2021 00:15:05 GMT  
		Size: 4.5 MB (4460538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb140f321bcfa502e9644d0bbdefa46dbb3c613c4d15846be69394dbf49bdef`  
		Last Modified: Sat, 13 Nov 2021 00:15:04 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c4c1544d842ec5effc5fa006170c896ffc224754c701b25c089d89caa2bfae`  
		Last Modified: Sat, 13 Nov 2021 00:15:04 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97f073fab2f7a16c2b02d0032b3a3b108086dca2d0b8f1c9beb95630caa5888`  
		Last Modified: Sat, 13 Nov 2021 00:15:05 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; 386

```console
$ docker pull notary@sha256:30b75cf3e322759b637ec9ee819aa036550c6a647dbedbad4ee36490417a08db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7449187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d769449a79988332053a03c1deec9baf3d9b16f653f09a4f2a7e8b5d84e9bf9`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 04:13:15 GMT
ENV TAG=v0.6.1
# Sat, 13 Nov 2021 04:13:15 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Sat, 13 Nov 2021 04:13:46 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 13 Nov 2021 04:13:47 GMT
EXPOSE 4444
# Sat, 13 Nov 2021 04:13:47 GMT
EXPOSE 7899
# Sat, 13 Nov 2021 04:13:47 GMT
WORKDIR /notary/signer
# Sat, 13 Nov 2021 04:14:15 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Sat, 13 Nov 2021 04:14:15 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Sat, 13 Nov 2021 04:14:16 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Sat, 13 Nov 2021 04:14:18 GMT
RUN adduser -D -H -g "" notary
# Sat, 13 Nov 2021 04:14:19 GMT
USER notary
# Sat, 13 Nov 2021 04:14:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 13 Nov 2021 04:14:19 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 13 Nov 2021 04:14:20 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d9bf320ba904d74784c7ba72789e44cc6155b482b364574496c9da530dae61`  
		Last Modified: Sat, 13 Nov 2021 04:15:04 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e59433f6d3793f0cf6a91aa8bbe071fd258255a93c4426d8019be23d23fe05e`  
		Last Modified: Sat, 13 Nov 2021 04:15:05 GMT  
		Size: 4.6 MB (4618315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b901b70b7dcb2c1ddc6ecf21a980b87f2fa289916165e5a88a007618ee7ad0`  
		Last Modified: Sat, 13 Nov 2021 04:15:04 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bfffb9f83c0d0ebba065f929f47e266cad1118b0834ee9500bbed5acb03653`  
		Last Modified: Sat, 13 Nov 2021 04:15:04 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbe4637c9d8576e28d31c726be50cd73a7fbf5c4445863b92bfdf98cf13b7c0`  
		Last Modified: Sat, 13 Nov 2021 04:15:04 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; ppc64le

```console
$ docker pull notary@sha256:493607ba1fada0e01470e66ad860d24f4b7e8d01d2dc9dba65dd4272d0813604
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7165484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeb36cabaf3c6d9bba0bf5fe0bd64343f835b76426767942092c51f35a975a3f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:25 GMT
ADD file:f7216323de17450e653f77c86d2c1e2e8ec01e1133e93f29c515761b3e9d8f7d in / 
# Fri, 12 Nov 2021 21:18:28 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 02:54:59 GMT
ENV TAG=v0.6.1
# Sat, 13 Nov 2021 02:55:04 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Sat, 13 Nov 2021 02:56:54 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 13 Nov 2021 02:56:57 GMT
EXPOSE 4444
# Sat, 13 Nov 2021 02:57:00 GMT
EXPOSE 7899
# Sat, 13 Nov 2021 02:57:04 GMT
WORKDIR /notary/signer
# Sat, 13 Nov 2021 02:57:39 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Sat, 13 Nov 2021 02:57:44 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Sat, 13 Nov 2021 02:57:47 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Sat, 13 Nov 2021 02:58:05 GMT
RUN adduser -D -H -g "" notary
# Sat, 13 Nov 2021 02:58:12 GMT
USER notary
# Sat, 13 Nov 2021 02:58:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 13 Nov 2021 02:58:25 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 13 Nov 2021 02:58:30 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:6729720a3e6b58511df148134bb67d786ad90f9fce1c02ba5bbfd31f33055fbe`  
		Last Modified: Fri, 12 Nov 2021 21:19:49 GMT  
		Size: 2.8 MB (2820517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a7806fed2d41d0755760e6717030f6aff9dc6d5c219ba7ea8e88bfeeb3104cb`  
		Last Modified: Sat, 13 Nov 2021 02:59:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17710bd31fffde751d347e6748a7dd6331b87678096d7c238c71873df8248dfe`  
		Last Modified: Sat, 13 Nov 2021 02:59:16 GMT  
		Size: 4.3 MB (4342905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8eb937120684e6a942598df616956feda3303abc0057aaf5a8d5eba3ed2fb3f`  
		Last Modified: Sat, 13 Nov 2021 02:59:15 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d6a82b8624c31634f38037f0a9d099bec7394379cb4d40a7cd1ca6ae8692bc`  
		Last Modified: Sat, 13 Nov 2021 02:59:15 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b175ad475b545323f1204fc8ad650e37b0fdfb2d3027b91bd6c54079dbf7bdf9`  
		Last Modified: Sat, 13 Nov 2021 02:59:15 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; s390x

```console
$ docker pull notary@sha256:e6f6947d924b122dcb51690332d26424ceda05418e10f3b803a30a275d9b197f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7327235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3761e07526b52455b9cffc179fcf7106a641d7c1384b87cf09ee1c53f329119b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:44 GMT
ADD file:637f327c9b07758709ef7dbc42eb472c888d221acde89b1c3775553864334d5c in / 
# Fri, 12 Nov 2021 16:41:44 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:28:05 GMT
ENV TAG=v0.6.1
# Fri, 12 Nov 2021 19:28:05 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Fri, 12 Nov 2021 19:28:25 GMT
ENV INSTALLDIR=/notary/signer
# Fri, 12 Nov 2021 19:28:25 GMT
EXPOSE 4444
# Fri, 12 Nov 2021 19:28:25 GMT
EXPOSE 7899
# Fri, 12 Nov 2021 19:28:25 GMT
WORKDIR /notary/signer
# Fri, 12 Nov 2021 19:28:35 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Fri, 12 Nov 2021 19:28:35 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Fri, 12 Nov 2021 19:28:36 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Fri, 12 Nov 2021 19:28:36 GMT
RUN adduser -D -H -g "" notary
# Fri, 12 Nov 2021 19:28:36 GMT
USER notary
# Fri, 12 Nov 2021 19:28:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Fri, 12 Nov 2021 19:28:36 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 12 Nov 2021 19:28:37 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:b872f056719bde6e6722091afb2a3376d720c69c142b91ac352050080dd79615`  
		Last Modified: Fri, 12 Nov 2021 16:42:54 GMT  
		Size: 2.6 MB (2611155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79567eeea74d41a59f001d5d151c4d04e765141889993d03e61de5e279c4c28c`  
		Last Modified: Fri, 12 Nov 2021 19:29:02 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9dec31adf090e3e1c49c2282770f8703464975f40a2f69c7bcb72afc984f794`  
		Last Modified: Fri, 12 Nov 2021 19:29:03 GMT  
		Size: 4.7 MB (4714020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9421ea8709971dd61a13b97364009d352ea9cd2e8152f451f7d89650e3a1cf`  
		Last Modified: Fri, 12 Nov 2021 19:29:02 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ae6189c031409f5ebd4c08d9285eeced61c89b885d30ce723fa22c3a32d5f0`  
		Last Modified: Fri, 12 Nov 2021 19:29:02 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83bcf41fcfe8e0486ace913fa3b816037305b13958b02a0a83f1149e3bb7795`  
		Last Modified: Fri, 12 Nov 2021 19:29:02 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
