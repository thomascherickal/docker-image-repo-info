## `znc:slim`

```console
$ docker pull znc@sha256:52e07ca0862f8fd55e39f5fc7395cbfa6a8dff7490eacbf998d81d0dccc90452
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:slim` - linux; amd64

```console
$ docker pull znc@sha256:c12357aecba5946a940b0400d3e85b165577338129935f9438ae0669ee34c7db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 MB (49963679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6484e9ae2e785fa00c021966e812a4efcb51cf81aedb7caea8edb047c545d50`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:35:25 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Wed, 29 Mar 2023 22:35:26 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Wed, 29 Mar 2023 22:35:26 GMT
ARG MAKEFLAGS=
# Wed, 29 Mar 2023 22:35:26 GMT
ENV ZNC_VERSION=1.8.2
# Wed, 29 Mar 2023 22:39:14 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         icu-data-full         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Wed, 29 Mar 2023 22:39:14 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Wed, 29 Mar 2023 22:39:14 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Wed, 29 Mar 2023 22:39:14 GMT
VOLUME [/znc-data]
# Wed, 29 Mar 2023 22:39:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628065eebc464c3ea58f2a84ab6829bc61fcdf4253d83f2200c4491d21d43b12`  
		Last Modified: Wed, 29 Mar 2023 22:39:42 GMT  
		Size: 46.6 MB (46588163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b301ae97cf7ee40ac648d3a2974f1ceec1d513ffb9c0ff84b7fb9cf63810bcaf`  
		Last Modified: Wed, 29 Mar 2023 22:39:35 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc4ac561604775023835601922cc9b88329f54d01c718015aae294511e45739`  
		Last Modified: Wed, 29 Mar 2023 22:39:35 GMT  
		Size: 781.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:slim` - linux; arm variant v6

```console
$ docker pull znc@sha256:6a62024f976032ef25b99c985c962aa7815aa590c268c54cac39433e608d4ad9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47904227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:515d7d0524a8a21480728df9ec048fa1297ddd12c26e6b7636b9ba2925d87554`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:44 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Mon, 13 Mar 2023 16:12:44 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:34:46 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 14 Mar 2023 01:34:46 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 14 Mar 2023 01:34:46 GMT
ARG MAKEFLAGS=
# Tue, 14 Mar 2023 01:34:47 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 14 Mar 2023 01:38:44 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         icu-data-full         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 14 Mar 2023 01:38:45 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 14 Mar 2023 01:38:45 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 14 Mar 2023 01:38:45 GMT
VOLUME [/znc-data]
# Tue, 14 Mar 2023 01:38:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42933172301fd2be0ab8950f19f61b3602c33c7746f4dcd26f941df0b0cb95ef`  
		Last Modified: Tue, 14 Mar 2023 01:39:34 GMT  
		Size: 44.8 MB (44792390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2561f3efb45bbafc3772ac345422b9e80205b08cf90db50b7c7e6cb4e2ed2418`  
		Last Modified: Tue, 14 Mar 2023 01:39:27 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:babbea5e4b86a37bfc8067420a81a37e8369c626b6d2a5c4750d3b6d8cdc2533`  
		Last Modified: Tue, 14 Mar 2023 01:39:27 GMT  
		Size: 781.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:slim` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:969ce53adb4b341534ab59d9372abcd94cc2f179b084630c48cef4149f038ab4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49435467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3149d1da08678ca71c50e2f6270616a6a3f6aaab348ec6117b00ea9e79a71747`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:30:31 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 30 Mar 2023 03:30:31 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 30 Mar 2023 03:30:31 GMT
ARG MAKEFLAGS=
# Thu, 30 Mar 2023 03:30:31 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 30 Mar 2023 03:33:49 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         icu-data-full         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 30 Mar 2023 03:33:49 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 30 Mar 2023 03:33:49 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Thu, 30 Mar 2023 03:33:49 GMT
VOLUME [/znc-data]
# Thu, 30 Mar 2023 03:33:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d424ead6aed8c838c75f48c27cf2be9fdd5b1dc10176fa85b64d8d22027e914`  
		Last Modified: Thu, 30 Mar 2023 03:34:14 GMT  
		Size: 46.2 MB (46172660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afc8953072a44d8b42dd597abe4f4871637b5c1824e511a0a95e640be0a4da0`  
		Last Modified: Thu, 30 Mar 2023 03:34:08 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f06664a2ffd9112eed232444e1a0e47374c8cc80680eaef898556a5da68a1d1`  
		Last Modified: Thu, 30 Mar 2023 03:34:08 GMT  
		Size: 780.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
