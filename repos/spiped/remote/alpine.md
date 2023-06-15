## `spiped:alpine`

```console
$ docker pull spiped@sha256:06f1af165905d00814f0b5fed901a955ee9301ab91374f1a3c2da3a0ce846af1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:alpine` - linux; amd64

```console
$ docker pull spiped@sha256:b30ffb11062d050f5e82aaf7d78c68bfba0145bcaf9d552e60e5d4a1ff989f01
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5080918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a22627799e7a16dc63c4a87f5a10aab25a0208b38b355991ec5c1746ba6e307f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 04:22:08 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 04:22:08 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 04:22:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 04:22:19 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 04:22:19 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 04:22:19 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 04:22:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 04:22:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 04:22:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7009e83c06c17eb996625171bf08b8b88dfc800b7110240cee783b8df3bdab`  
		Last Modified: Thu, 15 Jun 2023 04:22:35 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e968c07669fd5c8684973e30777b3d7aa561332751af2fbaa4d903a96942787f`  
		Last Modified: Thu, 15 Jun 2023 04:22:36 GMT  
		Size: 1.5 MB (1483166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb34038a914a6100cd46d4fc4ba06b2406f05cb528f07affe5cf1d0bcc3f012e`  
		Last Modified: Thu, 15 Jun 2023 04:22:35 GMT  
		Size: 221.3 KB (221304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3bb3dbe0ec4d1442cc10f5a9d0dfc971ced50a1b024748a0441f7717259a62`  
		Last Modified: Thu, 15 Jun 2023 04:22:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a865d54f1b59ecbcdd28db4a8ed51db52bced0b9103c08b4e3bd60d9ab5092ea`  
		Last Modified: Thu, 15 Jun 2023 04:22:36 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:06db8f6e615702076a78b5544ab4972b3d852851a43606bcff093be29bae66a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4558718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2acff564be060667f5e783e1a68645d35ad3986c948318d77a247b6669f8e22d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:25 GMT
ADD file:07e668ef139dce7f076143a30b89ff57885c8539d8b5764ac1bd5277d9936702 in / 
# Wed, 14 Jun 2023 18:49:25 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:21:32 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 06:21:34 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 06:21:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 06:21:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 06:21:43 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 06:21:43 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 06:21:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:21:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:21:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:33ec62e98ceea71d24212ee03e239c2d5538dbe7c98f41c42e8b2693fedf58fb`  
		Last Modified: Wed, 14 Jun 2023 18:50:00 GMT  
		Size: 3.1 MB (3110916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db263a5aca0de0797095f3bd22056067e9842fc931f78f7ae95d38a25236c185`  
		Last Modified: Thu, 15 Jun 2023 06:21:55 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec31a87286e0f4dd73f465a80b19111ac981d83ea1469375bd2531510958a9b9`  
		Last Modified: Thu, 15 Jun 2023 06:21:55 GMT  
		Size: 1.2 MB (1239671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cdb69483917a1a97a1e4517bf749631474cd4947b581bf545fc8ec922d82e3`  
		Last Modified: Thu, 15 Jun 2023 06:21:55 GMT  
		Size: 206.4 KB (206394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ffc82f232844968ce89b84e87c160a076403e5187688166db3012478b0ee8f`  
		Last Modified: Thu, 15 Jun 2023 06:21:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b99c8d7cfe4e601948b514fd305b8847633003b25cef4243a97e5e6349e033c`  
		Last Modified: Thu, 15 Jun 2023 06:21:55 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:69eaa2a0c21e8170650365f7d40d3a7c233b81d7661ece405dcca3b032e1bb77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7dde6285f1cdcbb4a49836abd7fa495595c255ae308325befc9aaee20f12ce9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:20 GMT
ADD file:5e92075a8d9a5898d661caf9c2be8a83fb25742251b4ebdc0c3d448a6dc58e4a in / 
# Wed, 14 Jun 2023 22:36:20 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 05:40:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 05:40:25 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 05:40:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 05:40:33 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 05:40:33 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 05:40:33 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 05:40:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 05:40:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 05:40:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f929d112168394cf1fbe294a86fbe5173dd92df4daac8cb09437b17dfc5df802`  
		Last Modified: Wed, 14 Jun 2023 22:37:01 GMT  
		Size: 2.9 MB (2868554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37196072c4a2a985d715b1ad2657cf1978ca9533fc1e523c12b328715e0b45d5`  
		Last Modified: Thu, 15 Jun 2023 05:40:45 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee5c46b5d561cfca9315d84fc298ad4d230bdc1a7cf8bd49a1249df54078185`  
		Last Modified: Thu, 15 Jun 2023 05:40:45 GMT  
		Size: 1.2 MB (1166836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eaf9facf339fdeab9ce293f598a0921e55287c3b97644313fe1f8cc691a0eda`  
		Last Modified: Thu, 15 Jun 2023 05:40:45 GMT  
		Size: 200.1 KB (200145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f49e7526be5915de8b82401cadb9a075e97c38dc51550ef1b5d3377544cb685`  
		Last Modified: Thu, 15 Jun 2023 05:40:45 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c7d118f25d5783b96754c98b6ec37c70b99f774f36ebf6beecdf0db3bfd9e0`  
		Last Modified: Thu, 15 Jun 2023 05:40:45 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b21f6104cf4f986ae42d2548c5a3e8edfeac1672739642c0051b1ce2e7ddc5dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4842828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:306f5b9d541620eedadaec0c057f09c6db34da10d9378cae2f5155b0081420a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:50:31 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 05:50:33 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 05:50:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 05:50:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 05:50:40 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 05:50:40 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 05:50:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 05:50:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 05:50:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a75b9333a53162c1a5789a4c7973a5cc525b738e1a394e58db69d0c32fa089`  
		Last Modified: Thu, 30 Mar 2023 05:50:49 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a905f71ab7e32bea70c662b413534aa7f764438f72937d84176a7b21115e19e`  
		Last Modified: Thu, 30 Mar 2023 05:50:50 GMT  
		Size: 1.4 MB (1363548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8364c9ed77705e5bab6f7d3ebcefe334f2401e4822779b17ceb1bb94d7510ce7`  
		Last Modified: Thu, 30 Mar 2023 05:50:50 GMT  
		Size: 215.7 KB (215692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a0bb75b3c36c6b1f0df28be9d91f3073dfcc4b0701cd2dffcafc2d8834c55`  
		Last Modified: Thu, 30 Mar 2023 05:50:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9fdfb5809799657c2cc38eac53edd7e1105371601d7e1c155b00bf07f8f3d0`  
		Last Modified: Thu, 30 Mar 2023 05:50:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:a0ef5e3831fe6edff2cbb0e86a938d1221c7cb3722165a2d84a75bb80c331700
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5131239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47bda906f8180f69c7a88e6bb9dd0306173696c2dfdb7ea927ee728006fc8806`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:26 GMT
ADD file:39180f040ebe17a01f8b9502d7b463edade8158d87fa99e47ac0b1f369e11a65 in / 
# Wed, 14 Jun 2023 22:33:26 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:19:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 15 Jun 2023 06:19:25 GMT
RUN apk add --no-cache libssl1.1
# Thu, 15 Jun 2023 06:19:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 15 Jun 2023 06:19:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 15 Jun 2023 06:19:36 GMT
VOLUME [/spiped]
# Thu, 15 Jun 2023 06:19:36 GMT
WORKDIR /spiped
# Thu, 15 Jun 2023 06:19:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:19:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:19:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:187bd96dd637d3adfc7a9b61a1e7465181bbfe90dbf7a2830dfba97e4e3243a4`  
		Last Modified: Wed, 14 Jun 2023 22:34:01 GMT  
		Size: 3.4 MB (3412675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6dc9f335c57afbc7b1e16495708b766aea73dd4a701c48f8224c9969059fe6`  
		Last Modified: Thu, 15 Jun 2023 06:19:46 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b173a46948db93064f235acd48f05a36d8367fddd933d24bd195f318e84c8e88`  
		Last Modified: Thu, 15 Jun 2023 06:19:50 GMT  
		Size: 1.5 MB (1485192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bf49c77ef03f39d9e293ebf197f230f3d09bd0dbcb18574059bfaa8a4e1023`  
		Last Modified: Thu, 15 Jun 2023 06:19:46 GMT  
		Size: 231.6 KB (231638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31434ea8ac7b673d5a898062b978fcf0b4eee889fe01aa4cdfc06a430063672d`  
		Last Modified: Thu, 15 Jun 2023 06:19:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bb416f535d69f288a9157a121afd70395a1694248283a278a68424ad083d83`  
		Last Modified: Thu, 15 Jun 2023 06:19:46 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:8b13ec4b458ac31fb096b22da921ddc5f982ca84907ae2ad42dfc9935e69a793
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5025754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70983caa08c37ccc9d7968473ced65e5b8ee6cc50feff3049de378aee313e62f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:27 GMT
ADD file:e95c1f256ba4bda85c5cbc0d8e84e6f329aa17c9dd2715b2da043e2139049124 in / 
# Wed, 29 Mar 2023 18:16:28 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:32:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 04:32:26 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 04:32:26 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 04:32:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 04:32:42 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 04:32:43 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 04:32:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 04:32:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 04:32:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1b7d25764eb3d3c55d73f5dfb9e3e9d75f3f39132e1b16142319de2a062dd673`  
		Last Modified: Wed, 29 Mar 2023 18:17:14 GMT  
		Size: 3.4 MB (3390935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abd914c752b02f6f79b7ef1571ed87d4130a25ed21a1d3892a23e3c2c1cfbec`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3cc8ae50d4833e170ee7dc2db705d37cc39c4e228e121c72a14cd9620b4847c`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 1.4 MB (1413051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac183c495785747e187a666506a1c63aeb182e3c511beaa79f82f4c86278a170`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 220.0 KB (220030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a70723c954d9ac5e16090c8b3aa6668bfab3384b6ce30cab8e10925bd1cd6c`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a4bf70a1b07cf55ae9e8498ca917bc7a43613629d823f0e1fa9b6c689b47b7`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:31fd069ea692240b5c5fc9e133487e244e6df34ce932c3470cad5763dffaa4c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 MB (6397813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f11cae2fc86cb997405cc5c3a4996740ff4651abe9f0e4af3b4f7ec8c89d5d31`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 03 May 2023 23:12:12 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 03 May 2023 23:12:13 GMT
RUN apk add --no-cache libssl1.1
# Wed, 03 May 2023 23:12:14 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 03 May 2023 23:12:20 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 03 May 2023 23:12:21 GMT
VOLUME [/spiped]
# Wed, 03 May 2023 23:12:21 GMT
WORKDIR /spiped
# Wed, 03 May 2023 23:12:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 03 May 2023 23:12:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 23:12:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8767d4ba6ffb04a8f593ae3a55b22eb4d0723a412c55cd55bca0f87af4ae7e71`  
		Last Modified: Wed, 03 May 2023 23:12:48 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d0ed4aa030d3cd667bab6930140621e2daf46573e404ec7feaa13530d59cf9`  
		Last Modified: Wed, 03 May 2023 23:12:49 GMT  
		Size: 1.2 MB (1223437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b0ffcfed6008438606174a08a596b98cdf875367dfaecebb1cb095f0fe00e1`  
		Last Modified: Wed, 03 May 2023 23:12:49 GMT  
		Size: 2.0 MB (1997449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af890e08dc1da930eb9bac534ec7ad96bd229fa34632688bb5a345a9044009c9`  
		Last Modified: Wed, 03 May 2023 23:12:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09f55129759a34f268901f558c8760261b43509b7900c8e66f5f6a447b2ef25`  
		Last Modified: Wed, 03 May 2023 23:12:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
