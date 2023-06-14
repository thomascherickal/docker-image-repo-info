<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `znc`

-	[`znc:1.8`](#znc18)
-	[`znc:1.8-slim`](#znc18-slim)
-	[`znc:1.8.2`](#znc182)
-	[`znc:1.8.2-slim`](#znc182-slim)
-	[`znc:latest`](#znclatest)
-	[`znc:slim`](#zncslim)

## `znc:1.8`

```console
$ docker pull znc@sha256:97841a0bd8a110b7bb4b72a30c00c4562e5d62badbcb7672b8a4bc06cc8d6ee8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8` - linux; amd64

```console
$ docker pull znc@sha256:401cb95c4aa225d135be4749d69ecf291af765986bf82c7bfe06773963ee2f30
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.5 MB (164466362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eadd4b911a28ef8c706b44eecf7edbedd1253e79c63b1090e652d0b546c8c190`
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
# Wed, 29 Mar 2023 22:39:25 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         openssl-dev         perl         python3
# Wed, 29 Mar 2023 22:39:25 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
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
	-	`sha256:9c690252585c12a33ecc76ebbffd0b2c343350ee43a728936a4a3236f8168a92`  
		Last Modified: Wed, 29 Mar 2023 22:40:08 GMT  
		Size: 114.5 MB (114502351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266e650d642f6de9e3bbd0bbe9e585b28e27326ff09dca74f42da43c89139876`  
		Last Modified: Wed, 29 Mar 2023 22:39:52 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8` - linux; arm variant v6

```console
$ docker pull znc@sha256:07d5c7e072255c6717aa361d3c3819b6a21acec27a29077237642227ddeb4737
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.1 MB (144064646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f8c5d262311959a6046b24fc7fb644d8e6abd3959319adac0d766e785fb7bb6`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:25 GMT
ADD file:07e668ef139dce7f076143a30b89ff57885c8539d8b5764ac1bd5277d9936702 in / 
# Wed, 14 Jun 2023 18:49:25 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:13:55 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Wed, 14 Jun 2023 20:13:55 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Wed, 14 Jun 2023 20:13:56 GMT
ARG MAKEFLAGS=
# Wed, 14 Jun 2023 20:13:56 GMT
ENV ZNC_VERSION=1.8.2
# Wed, 14 Jun 2023 20:18:04 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         icu-data-full         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Wed, 14 Jun 2023 20:18:04 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Wed, 14 Jun 2023 20:18:04 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Wed, 14 Jun 2023 20:18:05 GMT
VOLUME [/znc-data]
# Wed, 14 Jun 2023 20:18:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 20:18:30 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         openssl-dev         perl         python3
# Wed, 14 Jun 2023 20:18:33 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:33ec62e98ceea71d24212ee03e239c2d5538dbe7c98f41c42e8b2693fedf58fb`  
		Last Modified: Wed, 14 Jun 2023 18:50:00 GMT  
		Size: 3.1 MB (3110916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33307be6b66090bf65bdab1d1a56dfa125ac4a3a18db9adc8156e2b6e8a185ac`  
		Last Modified: Wed, 14 Jun 2023 20:18:52 GMT  
		Size: 44.8 MB (44792156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2186893ac1c9522ac10185266cda9406e7a492404936d0811f1150d749ca1ab2`  
		Last Modified: Wed, 14 Jun 2023 20:18:43 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6302be92bb802d0679620711eecf7d91604f2c4556cfc77e5f6b01b8bf44d4bc`  
		Last Modified: Wed, 14 Jun 2023 20:18:43 GMT  
		Size: 782.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89c890c8235198d9c0a89d5a6438cbdaa69a411243d2876b34d61fa5a37ebe7`  
		Last Modified: Wed, 14 Jun 2023 20:19:20 GMT  
		Size: 96.2 MB (96160290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ac9f384cae3b6e9433b9ac16f6a9d0849b35bdf733c340f5657a2d3d890d79`  
		Last Modified: Wed, 14 Jun 2023 20:19:01 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:d84c3f4fb78d6ce56ec712f6584277560cf66a3bbe6eeffef71ac3f72910754e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.4 MB (153351216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68453737876ef4dbc504f0b08fff3d71e9c90305a13903b7a3f2a2a9388daa77`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 23:17:52 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Wed, 14 Jun 2023 23:17:52 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Wed, 14 Jun 2023 23:17:52 GMT
ARG MAKEFLAGS=
# Wed, 14 Jun 2023 23:17:52 GMT
ENV ZNC_VERSION=1.8.2
# Wed, 14 Jun 2023 23:21:11 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         icu-data-full         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Wed, 14 Jun 2023 23:21:11 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Wed, 14 Jun 2023 23:21:11 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Wed, 14 Jun 2023 23:21:11 GMT
VOLUME [/znc-data]
# Wed, 14 Jun 2023 23:21:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 23:21:21 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         openssl-dev         perl         python3
# Wed, 14 Jun 2023 23:21:22 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea2d5dae4844b5e0888bf91da15915273f907c297e917dcdcca8dad25945e53`  
		Last Modified: Wed, 14 Jun 2023 23:21:37 GMT  
		Size: 46.2 MB (46189731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a15b36520b6aab8222d6b5143826eee590bb0f74bbfd7478315b0fcc822126`  
		Last Modified: Wed, 14 Jun 2023 23:21:31 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307a032731516a64d1b6860da8a0b1f7df436d013d655d58096a3d8fb320a7c0`  
		Last Modified: Wed, 14 Jun 2023 23:21:32 GMT  
		Size: 779.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13743297593f220c5d8cdd463b456d362bc2ae50b7babca64d5e6081897fabdd`  
		Last Modified: Wed, 14 Jun 2023 23:21:58 GMT  
		Size: 103.9 MB (103899063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f473c2df4eaad7b91c91e1de5b1a03ddbbb61b154d0646eb0359bc003a641e`  
		Last Modified: Wed, 14 Jun 2023 23:21:47 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.8-slim`

```console
$ docker pull znc@sha256:ec95cb5b222af919f5c9b0629889350245a7ab4779a6a8856c2decc1c2e3b73a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8-slim` - linux; amd64

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

### `znc:1.8-slim` - linux; arm variant v6

```console
$ docker pull znc@sha256:0ae2308bc3bea8e11d1f7eec71b3bc4f1968662f865b47abe2d80c24ea515b7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47904025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9609cd9c2fecde2134aca5f4728d25e7d832701897fd4416ec98d3592ced1b61`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:25 GMT
ADD file:07e668ef139dce7f076143a30b89ff57885c8539d8b5764ac1bd5277d9936702 in / 
# Wed, 14 Jun 2023 18:49:25 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:13:55 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Wed, 14 Jun 2023 20:13:55 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Wed, 14 Jun 2023 20:13:56 GMT
ARG MAKEFLAGS=
# Wed, 14 Jun 2023 20:13:56 GMT
ENV ZNC_VERSION=1.8.2
# Wed, 14 Jun 2023 20:18:04 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         icu-data-full         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Wed, 14 Jun 2023 20:18:04 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Wed, 14 Jun 2023 20:18:04 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Wed, 14 Jun 2023 20:18:05 GMT
VOLUME [/znc-data]
# Wed, 14 Jun 2023 20:18:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:33ec62e98ceea71d24212ee03e239c2d5538dbe7c98f41c42e8b2693fedf58fb`  
		Last Modified: Wed, 14 Jun 2023 18:50:00 GMT  
		Size: 3.1 MB (3110916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33307be6b66090bf65bdab1d1a56dfa125ac4a3a18db9adc8156e2b6e8a185ac`  
		Last Modified: Wed, 14 Jun 2023 20:18:52 GMT  
		Size: 44.8 MB (44792156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2186893ac1c9522ac10185266cda9406e7a492404936d0811f1150d749ca1ab2`  
		Last Modified: Wed, 14 Jun 2023 20:18:43 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6302be92bb802d0679620711eecf7d91604f2c4556cfc77e5f6b01b8bf44d4bc`  
		Last Modified: Wed, 14 Jun 2023 20:18:43 GMT  
		Size: 782.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8-slim` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:c37c7c923a0d73111e400880d124ff42d8df6f31266f34f15ac06684f33d0ae5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49451821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4e88e2d6739bc5de25f7cf776662f830db0e37ddece1dc76480854888ced5d1`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 23:17:52 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Wed, 14 Jun 2023 23:17:52 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Wed, 14 Jun 2023 23:17:52 GMT
ARG MAKEFLAGS=
# Wed, 14 Jun 2023 23:17:52 GMT
ENV ZNC_VERSION=1.8.2
# Wed, 14 Jun 2023 23:21:11 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         icu-data-full         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Wed, 14 Jun 2023 23:21:11 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Wed, 14 Jun 2023 23:21:11 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Wed, 14 Jun 2023 23:21:11 GMT
VOLUME [/znc-data]
# Wed, 14 Jun 2023 23:21:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea2d5dae4844b5e0888bf91da15915273f907c297e917dcdcca8dad25945e53`  
		Last Modified: Wed, 14 Jun 2023 23:21:37 GMT  
		Size: 46.2 MB (46189731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a15b36520b6aab8222d6b5143826eee590bb0f74bbfd7478315b0fcc822126`  
		Last Modified: Wed, 14 Jun 2023 23:21:31 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307a032731516a64d1b6860da8a0b1f7df436d013d655d58096a3d8fb320a7c0`  
		Last Modified: Wed, 14 Jun 2023 23:21:32 GMT  
		Size: 779.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.8.2`

```console
$ docker pull znc@sha256:97841a0bd8a110b7bb4b72a30c00c4562e5d62badbcb7672b8a4bc06cc8d6ee8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8.2` - linux; amd64

```console
$ docker pull znc@sha256:401cb95c4aa225d135be4749d69ecf291af765986bf82c7bfe06773963ee2f30
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.5 MB (164466362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eadd4b911a28ef8c706b44eecf7edbedd1253e79c63b1090e652d0b546c8c190`
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
# Wed, 29 Mar 2023 22:39:25 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         openssl-dev         perl         python3
# Wed, 29 Mar 2023 22:39:25 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
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
	-	`sha256:9c690252585c12a33ecc76ebbffd0b2c343350ee43a728936a4a3236f8168a92`  
		Last Modified: Wed, 29 Mar 2023 22:40:08 GMT  
		Size: 114.5 MB (114502351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266e650d642f6de9e3bbd0bbe9e585b28e27326ff09dca74f42da43c89139876`  
		Last Modified: Wed, 29 Mar 2023 22:39:52 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8.2` - linux; arm variant v6

```console
$ docker pull znc@sha256:07d5c7e072255c6717aa361d3c3819b6a21acec27a29077237642227ddeb4737
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.1 MB (144064646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f8c5d262311959a6046b24fc7fb644d8e6abd3959319adac0d766e785fb7bb6`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:25 GMT
ADD file:07e668ef139dce7f076143a30b89ff57885c8539d8b5764ac1bd5277d9936702 in / 
# Wed, 14 Jun 2023 18:49:25 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:13:55 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Wed, 14 Jun 2023 20:13:55 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Wed, 14 Jun 2023 20:13:56 GMT
ARG MAKEFLAGS=
# Wed, 14 Jun 2023 20:13:56 GMT
ENV ZNC_VERSION=1.8.2
# Wed, 14 Jun 2023 20:18:04 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         icu-data-full         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Wed, 14 Jun 2023 20:18:04 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Wed, 14 Jun 2023 20:18:04 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Wed, 14 Jun 2023 20:18:05 GMT
VOLUME [/znc-data]
# Wed, 14 Jun 2023 20:18:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 20:18:30 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         openssl-dev         perl         python3
# Wed, 14 Jun 2023 20:18:33 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:33ec62e98ceea71d24212ee03e239c2d5538dbe7c98f41c42e8b2693fedf58fb`  
		Last Modified: Wed, 14 Jun 2023 18:50:00 GMT  
		Size: 3.1 MB (3110916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33307be6b66090bf65bdab1d1a56dfa125ac4a3a18db9adc8156e2b6e8a185ac`  
		Last Modified: Wed, 14 Jun 2023 20:18:52 GMT  
		Size: 44.8 MB (44792156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2186893ac1c9522ac10185266cda9406e7a492404936d0811f1150d749ca1ab2`  
		Last Modified: Wed, 14 Jun 2023 20:18:43 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6302be92bb802d0679620711eecf7d91604f2c4556cfc77e5f6b01b8bf44d4bc`  
		Last Modified: Wed, 14 Jun 2023 20:18:43 GMT  
		Size: 782.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89c890c8235198d9c0a89d5a6438cbdaa69a411243d2876b34d61fa5a37ebe7`  
		Last Modified: Wed, 14 Jun 2023 20:19:20 GMT  
		Size: 96.2 MB (96160290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ac9f384cae3b6e9433b9ac16f6a9d0849b35bdf733c340f5657a2d3d890d79`  
		Last Modified: Wed, 14 Jun 2023 20:19:01 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8.2` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:d84c3f4fb78d6ce56ec712f6584277560cf66a3bbe6eeffef71ac3f72910754e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.4 MB (153351216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68453737876ef4dbc504f0b08fff3d71e9c90305a13903b7a3f2a2a9388daa77`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 23:17:52 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Wed, 14 Jun 2023 23:17:52 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Wed, 14 Jun 2023 23:17:52 GMT
ARG MAKEFLAGS=
# Wed, 14 Jun 2023 23:17:52 GMT
ENV ZNC_VERSION=1.8.2
# Wed, 14 Jun 2023 23:21:11 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         icu-data-full         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Wed, 14 Jun 2023 23:21:11 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Wed, 14 Jun 2023 23:21:11 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Wed, 14 Jun 2023 23:21:11 GMT
VOLUME [/znc-data]
# Wed, 14 Jun 2023 23:21:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 23:21:21 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         openssl-dev         perl         python3
# Wed, 14 Jun 2023 23:21:22 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea2d5dae4844b5e0888bf91da15915273f907c297e917dcdcca8dad25945e53`  
		Last Modified: Wed, 14 Jun 2023 23:21:37 GMT  
		Size: 46.2 MB (46189731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a15b36520b6aab8222d6b5143826eee590bb0f74bbfd7478315b0fcc822126`  
		Last Modified: Wed, 14 Jun 2023 23:21:31 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307a032731516a64d1b6860da8a0b1f7df436d013d655d58096a3d8fb320a7c0`  
		Last Modified: Wed, 14 Jun 2023 23:21:32 GMT  
		Size: 779.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13743297593f220c5d8cdd463b456d362bc2ae50b7babca64d5e6081897fabdd`  
		Last Modified: Wed, 14 Jun 2023 23:21:58 GMT  
		Size: 103.9 MB (103899063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f473c2df4eaad7b91c91e1de5b1a03ddbbb61b154d0646eb0359bc003a641e`  
		Last Modified: Wed, 14 Jun 2023 23:21:47 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.8.2-slim`

```console
$ docker pull znc@sha256:ec95cb5b222af919f5c9b0629889350245a7ab4779a6a8856c2decc1c2e3b73a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8.2-slim` - linux; amd64

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

### `znc:1.8.2-slim` - linux; arm variant v6

```console
$ docker pull znc@sha256:0ae2308bc3bea8e11d1f7eec71b3bc4f1968662f865b47abe2d80c24ea515b7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47904025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9609cd9c2fecde2134aca5f4728d25e7d832701897fd4416ec98d3592ced1b61`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:25 GMT
ADD file:07e668ef139dce7f076143a30b89ff57885c8539d8b5764ac1bd5277d9936702 in / 
# Wed, 14 Jun 2023 18:49:25 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:13:55 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Wed, 14 Jun 2023 20:13:55 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Wed, 14 Jun 2023 20:13:56 GMT
ARG MAKEFLAGS=
# Wed, 14 Jun 2023 20:13:56 GMT
ENV ZNC_VERSION=1.8.2
# Wed, 14 Jun 2023 20:18:04 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         icu-data-full         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Wed, 14 Jun 2023 20:18:04 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Wed, 14 Jun 2023 20:18:04 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Wed, 14 Jun 2023 20:18:05 GMT
VOLUME [/znc-data]
# Wed, 14 Jun 2023 20:18:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:33ec62e98ceea71d24212ee03e239c2d5538dbe7c98f41c42e8b2693fedf58fb`  
		Last Modified: Wed, 14 Jun 2023 18:50:00 GMT  
		Size: 3.1 MB (3110916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33307be6b66090bf65bdab1d1a56dfa125ac4a3a18db9adc8156e2b6e8a185ac`  
		Last Modified: Wed, 14 Jun 2023 20:18:52 GMT  
		Size: 44.8 MB (44792156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2186893ac1c9522ac10185266cda9406e7a492404936d0811f1150d749ca1ab2`  
		Last Modified: Wed, 14 Jun 2023 20:18:43 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6302be92bb802d0679620711eecf7d91604f2c4556cfc77e5f6b01b8bf44d4bc`  
		Last Modified: Wed, 14 Jun 2023 20:18:43 GMT  
		Size: 782.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8.2-slim` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:c37c7c923a0d73111e400880d124ff42d8df6f31266f34f15ac06684f33d0ae5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49451821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4e88e2d6739bc5de25f7cf776662f830db0e37ddece1dc76480854888ced5d1`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 23:17:52 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Wed, 14 Jun 2023 23:17:52 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Wed, 14 Jun 2023 23:17:52 GMT
ARG MAKEFLAGS=
# Wed, 14 Jun 2023 23:17:52 GMT
ENV ZNC_VERSION=1.8.2
# Wed, 14 Jun 2023 23:21:11 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         icu-data-full         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Wed, 14 Jun 2023 23:21:11 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Wed, 14 Jun 2023 23:21:11 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Wed, 14 Jun 2023 23:21:11 GMT
VOLUME [/znc-data]
# Wed, 14 Jun 2023 23:21:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea2d5dae4844b5e0888bf91da15915273f907c297e917dcdcca8dad25945e53`  
		Last Modified: Wed, 14 Jun 2023 23:21:37 GMT  
		Size: 46.2 MB (46189731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a15b36520b6aab8222d6b5143826eee590bb0f74bbfd7478315b0fcc822126`  
		Last Modified: Wed, 14 Jun 2023 23:21:31 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307a032731516a64d1b6860da8a0b1f7df436d013d655d58096a3d8fb320a7c0`  
		Last Modified: Wed, 14 Jun 2023 23:21:32 GMT  
		Size: 779.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:latest`

```console
$ docker pull znc@sha256:97841a0bd8a110b7bb4b72a30c00c4562e5d62badbcb7672b8a4bc06cc8d6ee8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:latest` - linux; amd64

```console
$ docker pull znc@sha256:401cb95c4aa225d135be4749d69ecf291af765986bf82c7bfe06773963ee2f30
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.5 MB (164466362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eadd4b911a28ef8c706b44eecf7edbedd1253e79c63b1090e652d0b546c8c190`
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
# Wed, 29 Mar 2023 22:39:25 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         openssl-dev         perl         python3
# Wed, 29 Mar 2023 22:39:25 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
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
	-	`sha256:9c690252585c12a33ecc76ebbffd0b2c343350ee43a728936a4a3236f8168a92`  
		Last Modified: Wed, 29 Mar 2023 22:40:08 GMT  
		Size: 114.5 MB (114502351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266e650d642f6de9e3bbd0bbe9e585b28e27326ff09dca74f42da43c89139876`  
		Last Modified: Wed, 29 Mar 2023 22:39:52 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:latest` - linux; arm variant v6

```console
$ docker pull znc@sha256:07d5c7e072255c6717aa361d3c3819b6a21acec27a29077237642227ddeb4737
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.1 MB (144064646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f8c5d262311959a6046b24fc7fb644d8e6abd3959319adac0d766e785fb7bb6`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:25 GMT
ADD file:07e668ef139dce7f076143a30b89ff57885c8539d8b5764ac1bd5277d9936702 in / 
# Wed, 14 Jun 2023 18:49:25 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:13:55 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Wed, 14 Jun 2023 20:13:55 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Wed, 14 Jun 2023 20:13:56 GMT
ARG MAKEFLAGS=
# Wed, 14 Jun 2023 20:13:56 GMT
ENV ZNC_VERSION=1.8.2
# Wed, 14 Jun 2023 20:18:04 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         icu-data-full         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Wed, 14 Jun 2023 20:18:04 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Wed, 14 Jun 2023 20:18:04 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Wed, 14 Jun 2023 20:18:05 GMT
VOLUME [/znc-data]
# Wed, 14 Jun 2023 20:18:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 20:18:30 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         openssl-dev         perl         python3
# Wed, 14 Jun 2023 20:18:33 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:33ec62e98ceea71d24212ee03e239c2d5538dbe7c98f41c42e8b2693fedf58fb`  
		Last Modified: Wed, 14 Jun 2023 18:50:00 GMT  
		Size: 3.1 MB (3110916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33307be6b66090bf65bdab1d1a56dfa125ac4a3a18db9adc8156e2b6e8a185ac`  
		Last Modified: Wed, 14 Jun 2023 20:18:52 GMT  
		Size: 44.8 MB (44792156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2186893ac1c9522ac10185266cda9406e7a492404936d0811f1150d749ca1ab2`  
		Last Modified: Wed, 14 Jun 2023 20:18:43 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6302be92bb802d0679620711eecf7d91604f2c4556cfc77e5f6b01b8bf44d4bc`  
		Last Modified: Wed, 14 Jun 2023 20:18:43 GMT  
		Size: 782.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89c890c8235198d9c0a89d5a6438cbdaa69a411243d2876b34d61fa5a37ebe7`  
		Last Modified: Wed, 14 Jun 2023 20:19:20 GMT  
		Size: 96.2 MB (96160290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ac9f384cae3b6e9433b9ac16f6a9d0849b35bdf733c340f5657a2d3d890d79`  
		Last Modified: Wed, 14 Jun 2023 20:19:01 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:latest` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:d84c3f4fb78d6ce56ec712f6584277560cf66a3bbe6eeffef71ac3f72910754e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.4 MB (153351216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68453737876ef4dbc504f0b08fff3d71e9c90305a13903b7a3f2a2a9388daa77`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 23:17:52 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Wed, 14 Jun 2023 23:17:52 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Wed, 14 Jun 2023 23:17:52 GMT
ARG MAKEFLAGS=
# Wed, 14 Jun 2023 23:17:52 GMT
ENV ZNC_VERSION=1.8.2
# Wed, 14 Jun 2023 23:21:11 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         icu-data-full         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Wed, 14 Jun 2023 23:21:11 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Wed, 14 Jun 2023 23:21:11 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Wed, 14 Jun 2023 23:21:11 GMT
VOLUME [/znc-data]
# Wed, 14 Jun 2023 23:21:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 23:21:21 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         openssl-dev         perl         python3
# Wed, 14 Jun 2023 23:21:22 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea2d5dae4844b5e0888bf91da15915273f907c297e917dcdcca8dad25945e53`  
		Last Modified: Wed, 14 Jun 2023 23:21:37 GMT  
		Size: 46.2 MB (46189731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a15b36520b6aab8222d6b5143826eee590bb0f74bbfd7478315b0fcc822126`  
		Last Modified: Wed, 14 Jun 2023 23:21:31 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307a032731516a64d1b6860da8a0b1f7df436d013d655d58096a3d8fb320a7c0`  
		Last Modified: Wed, 14 Jun 2023 23:21:32 GMT  
		Size: 779.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13743297593f220c5d8cdd463b456d362bc2ae50b7babca64d5e6081897fabdd`  
		Last Modified: Wed, 14 Jun 2023 23:21:58 GMT  
		Size: 103.9 MB (103899063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f473c2df4eaad7b91c91e1de5b1a03ddbbb61b154d0646eb0359bc003a641e`  
		Last Modified: Wed, 14 Jun 2023 23:21:47 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:slim`

```console
$ docker pull znc@sha256:ec95cb5b222af919f5c9b0629889350245a7ab4779a6a8856c2decc1c2e3b73a
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
$ docker pull znc@sha256:0ae2308bc3bea8e11d1f7eec71b3bc4f1968662f865b47abe2d80c24ea515b7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47904025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9609cd9c2fecde2134aca5f4728d25e7d832701897fd4416ec98d3592ced1b61`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:25 GMT
ADD file:07e668ef139dce7f076143a30b89ff57885c8539d8b5764ac1bd5277d9936702 in / 
# Wed, 14 Jun 2023 18:49:25 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:13:55 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Wed, 14 Jun 2023 20:13:55 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Wed, 14 Jun 2023 20:13:56 GMT
ARG MAKEFLAGS=
# Wed, 14 Jun 2023 20:13:56 GMT
ENV ZNC_VERSION=1.8.2
# Wed, 14 Jun 2023 20:18:04 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         icu-data-full         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Wed, 14 Jun 2023 20:18:04 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Wed, 14 Jun 2023 20:18:04 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Wed, 14 Jun 2023 20:18:05 GMT
VOLUME [/znc-data]
# Wed, 14 Jun 2023 20:18:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:33ec62e98ceea71d24212ee03e239c2d5538dbe7c98f41c42e8b2693fedf58fb`  
		Last Modified: Wed, 14 Jun 2023 18:50:00 GMT  
		Size: 3.1 MB (3110916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33307be6b66090bf65bdab1d1a56dfa125ac4a3a18db9adc8156e2b6e8a185ac`  
		Last Modified: Wed, 14 Jun 2023 20:18:52 GMT  
		Size: 44.8 MB (44792156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2186893ac1c9522ac10185266cda9406e7a492404936d0811f1150d749ca1ab2`  
		Last Modified: Wed, 14 Jun 2023 20:18:43 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6302be92bb802d0679620711eecf7d91604f2c4556cfc77e5f6b01b8bf44d4bc`  
		Last Modified: Wed, 14 Jun 2023 20:18:43 GMT  
		Size: 782.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:slim` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:c37c7c923a0d73111e400880d124ff42d8df6f31266f34f15ac06684f33d0ae5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49451821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4e88e2d6739bc5de25f7cf776662f830db0e37ddece1dc76480854888ced5d1`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 23:17:52 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Wed, 14 Jun 2023 23:17:52 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Wed, 14 Jun 2023 23:17:52 GMT
ARG MAKEFLAGS=
# Wed, 14 Jun 2023 23:17:52 GMT
ENV ZNC_VERSION=1.8.2
# Wed, 14 Jun 2023 23:21:11 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         icu-data-full         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Wed, 14 Jun 2023 23:21:11 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Wed, 14 Jun 2023 23:21:11 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Wed, 14 Jun 2023 23:21:11 GMT
VOLUME [/znc-data]
# Wed, 14 Jun 2023 23:21:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea2d5dae4844b5e0888bf91da15915273f907c297e917dcdcca8dad25945e53`  
		Last Modified: Wed, 14 Jun 2023 23:21:37 GMT  
		Size: 46.2 MB (46189731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a15b36520b6aab8222d6b5143826eee590bb0f74bbfd7478315b0fcc822126`  
		Last Modified: Wed, 14 Jun 2023 23:21:31 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307a032731516a64d1b6860da8a0b1f7df436d013d655d58096a3d8fb320a7c0`  
		Last Modified: Wed, 14 Jun 2023 23:21:32 GMT  
		Size: 779.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
