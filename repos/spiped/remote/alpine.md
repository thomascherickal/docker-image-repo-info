## `spiped:alpine`

```console
$ docker pull spiped@sha256:c6ea8390da034fda56d586cb2dc256b994d9051decc4f0db828959d6e856a050
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
$ docker pull spiped@sha256:77bb7048879f502a0be6947d6ded556dedd56bfbd65846f202ddbae6c0220f84
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecec5286e75ac64570dd86ae159bec30df6ff4bb0ecc79f42dd8a5c7126be6eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 18:41:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 18:41:21 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 18:41:21 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 19:03:03 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 19:03:03 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 19:03:03 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 19:03:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:03:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:03:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc49c1d100974d70cd457c65f0e781af958b9d07a56e03267424f0d11990712`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f3e43d8c62d03bca76a106e58c3099bd76fb7fbad003082a81a3670c07ba69`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 7.3 KB (7282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcdfa185ef47533e780a1502b6ecf0f1486cc0955b4930432fdfdc77813e9d50`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 212.6 KB (212559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241cc499201ce5b553c5be7e1b77bfddb66137711a90180f2e25689109405751`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179d6882fdc5e95f3b1481ffb5d149c0fda3dc71d8fa51eba15edc3be50dc54c`  
		Last Modified: Fri, 25 Jun 2021 19:03:21 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:b758b42acbf998e5a39dc12204e0be903d69a2af37753e5d2133b5df87b06523
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2835923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae8ff3806515f364a387402ad57b51af1f948f849240b2e704a6de2c048ada9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Tue, 22 Jun 2021 00:21:07 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 22 Jun 2021 00:21:09 GMT
RUN apk add --no-cache libssl1.1
# Tue, 22 Jun 2021 00:21:10 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 19:38:07 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 19:38:07 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 19:38:08 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 19:38:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:38:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:38:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9e2daf3ec825cb3613604aa1365dbe414dc4e91784135871c1b1dfc68db23d`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6101fbc0ffdf60230b896427f198bc223946522d7d1f77e2275181837980568d`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 7.3 KB (7308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296999154521c5c6c6c67a405f842cacada3793a86c889ce922a114bae5354a6`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 202.5 KB (202495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22c40bed8d80ea82bb949a3747badad3421eb16ea2e2440962324c9d79ab00b`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd55faef8cc92525b1be13e1e39b9ee16e5caaf2df3e0db276ed2683a509da9`  
		Last Modified: Fri, 25 Jun 2021 19:38:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:57f8db33a0eec466bfc76dd17cee895a03a3789dbd31bd89ef2e8dc7da3455e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2632718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:676e5f41ec430a6e87108a46dd408d068f0e501170755f72925c7a760ed458ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Thu, 24 Jun 2021 07:25:48 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 24 Jun 2021 07:25:50 GMT
RUN apk add --no-cache libssl1.1
# Thu, 24 Jun 2021 07:25:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 19:17:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 19:17:30 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 19:17:30 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 19:17:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 19:17:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 19:17:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c429d40f3f855015d365208d1b968cd8f34de9ccedd71360b7f05eab24ddd1`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4522338918253627f69a56835ddb741f10f29e2de17157de4ca03a12561d3e05`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 7.3 KB (7296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58f4ce029c4b37ef76a46da093755b9e24c2d0765592fd00547e013edf3479c`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 195.8 KB (195767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10cb1e83ae0b13c5adcff700076e63bf3322c49067170f59c7ec0c9d6f0698f`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e1913bac6b271f9c4b484fad7338dcbc98a4526b6e48bf1f6a8ccb3fa3b9a`  
		Last Modified: Fri, 25 Jun 2021 19:18:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:40541478eb401d67036d56bbd4cfd5933f148ce155f8e3292a4d083fbb62ba19
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2923277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a02b54f6f7a1b548ed3db2fc33cafcbb8ef9b27d6ae45811deeb5ecf484a3d75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 18:40:49 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 18:40:50 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 18:40:51 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 18:54:08 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 18:54:08 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 18:54:08 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 18:54:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 18:54:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 18:54:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48a6e447f49f6576247dd515ff88f610088fde09c8c378492a19009d6f6fd3b`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05549f8a714910bf1ba795919183eda4ed8c6c1dacd25e27d16f60e584efd239`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 7.3 KB (7295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b70a09132ff271f43729154235e305beed323f6f44bb8f91d3f71be66c9f58`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 204.6 KB (204616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf3cdb40c67131120870a15e3902a71c8b1db82a03999be16d35d7d6ae59309`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb17f3d198dd5104ea91d70276d05d71182af08cf309adc75a3b64bd770c1699`  
		Last Modified: Fri, 25 Jun 2021 18:54:38 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:041a4401f89326839b354e7fb7aeb38b07f545fab3de4c84dc0c8f9cebefacca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f94b397232ecc82d13aa208dbbe6e5a315e7a44a1d284fc0089f766e22aea2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 18:40:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 16 Jun 2021 18:40:32 GMT
RUN apk add --no-cache libssl1.1
# Wed, 16 Jun 2021 18:40:33 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 25 Jun 2021 18:55:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 25 Jun 2021 18:55:36 GMT
VOLUME [/spiped]
# Fri, 25 Jun 2021 18:55:37 GMT
WORKDIR /spiped
# Fri, 25 Jun 2021 18:55:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 25 Jun 2021 18:55:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 18:55:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8a1adc7e61a91c39fcba896b070192f506dd419fc77a733ce377c563448785`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982f88ff86958b26737edc45adbf2bf850db25cdc970e348723b0d305f5f6db2`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 7.3 KB (7296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24fe46b36c0cdba759eaf8ea030281f67337289db167fb4d8d3b7da3e191680`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 223.4 KB (223438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7eb79119bc0cf80b5d4a32e3035a171c2c43177ce8bd6cf5f6ad53da848ae22`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1027751b1d208d42e1c73a3526f36a885067bd323348563fb1186928a536a01a`  
		Last Modified: Fri, 25 Jun 2021 18:56:08 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:4ac4db371098fa15cc8c0963c8f7408d1cfe32a0963ff0387e06e855f74f0b70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3040763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deb52dde65aeb803d22820dd79678d168c7f81757563e087913ae87794f4c710`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 30 Jul 2021 17:24:32 GMT
ADD file:0075aad7a94f0496483442bb2d9fdaa13e9c23087b90638d014b4bc263aa3861 in / 
# Fri, 30 Jul 2021 17:24:37 GMT
CMD ["/bin/sh"]
# Sat, 31 Jul 2021 00:40:03 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 31 Jul 2021 00:40:12 GMT
RUN apk add --no-cache libssl1.1
# Sat, 31 Jul 2021 00:40:17 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 31 Jul 2021 00:40:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 31 Jul 2021 00:40:46 GMT
VOLUME [/spiped]
# Sat, 31 Jul 2021 00:40:52 GMT
WORKDIR /spiped
# Sat, 31 Jul 2021 00:40:54 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 31 Jul 2021 00:40:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 31 Jul 2021 00:41:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:baf144cfb66ebe9df1969f3b90f1c448beff98edc84de1ccb5d6346195a070d4`  
		Last Modified: Tue, 15 Jun 2021 22:27:38 GMT  
		Size: 2.8 MB (2810478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54ddec4b7614399b7b4b38d2736b0a41ebabd1502632967abe1ebea6084f967`  
		Last Modified: Sat, 31 Jul 2021 00:41:32 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb9d6e78bdf90d8864e90e2013112ffb2081dfc00b405b7147d885e8543ae96`  
		Last Modified: Sat, 31 Jul 2021 00:41:31 GMT  
		Size: 7.3 KB (7299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0490d0b1065581892a2225a0292c69269fe912e4ba59724df02bafe686e8440`  
		Last Modified: Sat, 31 Jul 2021 00:41:32 GMT  
		Size: 221.2 KB (221246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271e5d7f0b4d6bd57eabcff98334c4669cf1af150ff233a9b8c59abc3500bb66`  
		Last Modified: Sat, 31 Jul 2021 00:41:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dcb128806b493c1ee2a046a629ded343bea04ac1bc240aa0b35a48ad8954754`  
		Last Modified: Sat, 31 Jul 2021 00:41:31 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:6ec14094d3594e86c89a330bd9ac7db9109578591c71a7fc895ef583f56a0ebc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2816473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8e10c73436dfd94b9788c63d5d89c26217f62795e62170bfee7bb5fddea096c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:06:26 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 14 Apr 2021 20:06:27 GMT
RUN apk add --no-cache libssl1.1
# Wed, 14 Apr 2021 20:06:27 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 14 Apr 2021 20:06:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Wed, 14 Apr 2021 20:06:37 GMT
VOLUME [/spiped]
# Wed, 14 Apr 2021 20:06:37 GMT
WORKDIR /spiped
# Wed, 14 Apr 2021 20:06:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:06:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:06:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64390452532879e125a5bb8a9120ef0206a6ffed9b7b45143408593823449b69`  
		Last Modified: Wed, 14 Apr 2021 20:06:56 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe161c1af56f1ac1b902a43d31cc07ce45e66ce5deaae0c37c972f8d4d505530`  
		Last Modified: Wed, 14 Apr 2021 20:06:59 GMT  
		Size: 7.1 KB (7054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62195a09ae764bb27e5a0afa4b95616824bbb859a891aaf48c9f5979d1482176`  
		Last Modified: Wed, 14 Apr 2021 20:06:55 GMT  
		Size: 205.0 KB (205043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c57dc974a3fd6357043b304379826936777167d99e198e01a3341c951c15b9`  
		Last Modified: Wed, 14 Apr 2021 20:06:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113c0808aca0ef9883bd02b957ed90398dbfabff1dcf1d5e822af51ba8e53d69`  
		Last Modified: Wed, 14 Apr 2021 20:06:56 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
