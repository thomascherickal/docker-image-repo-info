<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `znc`

-	[`znc:1.8`](#znc18)
-	[`znc:1.8.2`](#znc182)
-	[`znc:1.8.2-slim`](#znc182-slim)
-	[`znc:1.8-slim`](#znc18-slim)
-	[`znc:latest`](#znclatest)
-	[`znc:slim`](#zncslim)

## `znc:1.8`

```console
$ docker pull znc@sha256:5316ad98d0708ef3b93b911e2a98bd3b4de2206909aab37d987140f18301cf9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8` - linux; amd64

```console
$ docker pull znc@sha256:0fa3ea91829cc19a89db8568b5436e250f54d70a639af996ef5a28a69bade3ac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.6 MB (150607273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0073e8472cebc4ede105e2675f8bb492ea4ce59d134f44b1af1969aee4a890ca`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 06:05:00 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 22 Oct 2020 06:05:01 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 22 Oct 2020 06:05:01 GMT
ARG MAKEFLAGS=
# Thu, 22 Oct 2020 06:05:01 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 22 Oct 2020 06:11:10 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 22 Oct 2020 06:11:11 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 22 Oct 2020 06:11:11 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 22 Oct 2020 06:11:12 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 22 Oct 2020 06:11:12 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 22 Oct 2020 06:11:13 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 22 Oct 2020 06:11:13 GMT
VOLUME [/znc-data]
# Thu, 22 Oct 2020 06:11:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Oct 2020 06:11:35 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Thu, 22 Oct 2020 06:11:36 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0791fb9bd5d853a4620db9587acac4e5702d9fb63ef15123f885ea94159342c`  
		Last Modified: Thu, 22 Oct 2020 06:12:05 GMT  
		Size: 44.4 MB (44434892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c83b9beca5c9c26ebe0b2e287efc7a63b25cb16bdeaf1b54399b37f4e095665`  
		Last Modified: Thu, 22 Oct 2020 06:11:51 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47085387bf489e504bd8e581535a8dd00382a6775c461f57e48cd3ac45d7f4f9`  
		Last Modified: Thu, 22 Oct 2020 06:11:52 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8228de32d1fddd68f6bd466974b35c7e266629b74619c07a6191c86d6e12a54a`  
		Last Modified: Thu, 22 Oct 2020 06:11:51 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5da6e224361ae2d9a36212af67377a0d24bc4a86384fd32e165ae805d3e335`  
		Last Modified: Thu, 22 Oct 2020 06:11:52 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75b6faf1b171816e3706c54de9fd24fa7f6141f9081795dd0720e9fd20e655b`  
		Last Modified: Thu, 22 Oct 2020 06:11:52 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4724edc3b618a63c4e80fda513ad66a1be082731557dd815eebbdf5a752a1ac`  
		Last Modified: Thu, 22 Oct 2020 06:12:40 GMT  
		Size: 103.4 MB (103373793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99e5de9761ba1180d5357c2e9845b68f58bf534947d067f70afed65e7ec870f`  
		Last Modified: Thu, 22 Oct 2020 06:12:13 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8` - linux; arm variant v6

```console
$ docker pull znc@sha256:0282fcfdaa3fbea0a7af0dd8297a69f810c1799d390ecc5d53fde8c4024ccf88
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.3 MB (132306978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c80c86d2dfd752c2d69464c99940cc1205c98772848009f9ab3e6fdd299d7c8`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:43:44 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 22 Oct 2020 02:43:45 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 22 Oct 2020 02:43:47 GMT
ARG MAKEFLAGS=
# Thu, 22 Oct 2020 02:43:48 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 22 Oct 2020 02:52:04 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 22 Oct 2020 02:52:06 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 22 Oct 2020 02:52:07 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 22 Oct 2020 02:52:07 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 22 Oct 2020 02:52:08 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 22 Oct 2020 02:52:09 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 22 Oct 2020 02:52:11 GMT
VOLUME [/znc-data]
# Thu, 22 Oct 2020 02:52:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Oct 2020 02:52:38 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Thu, 22 Oct 2020 02:52:40 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f9828649f0a43abb2c7773562cb703c4174550ed46cd6873f1da33f8f7f7bc`  
		Last Modified: Thu, 22 Oct 2020 02:53:10 GMT  
		Size: 42.7 MB (42684189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce360030cd7eb3c6062ad0e8f22a430f6a7592052cbc442179f9facb20220dc`  
		Last Modified: Thu, 22 Oct 2020 02:52:52 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b59e17fda5a3bca1b5d7ef95539bd252efa4a18e7ea13f463181225a7860358`  
		Last Modified: Thu, 22 Oct 2020 02:52:53 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b016084e2f3ded73e2937734dadcb3e6d0564134e516a8d0ddced5867cde9990`  
		Last Modified: Thu, 22 Oct 2020 02:52:52 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02536655361cb4c04cc7c2f5600b73eabfb159ad3a6651859b239179d3fc2ad`  
		Last Modified: Thu, 22 Oct 2020 02:52:52 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14045112bb0830471184dcafe80013308ddc2e6625b319863e1f9fcc0ecb932d`  
		Last Modified: Thu, 22 Oct 2020 02:52:52 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed0305db86d902cf32741419da0708fb920bb1b33425b6a4f0eba4d7c86abbe`  
		Last Modified: Thu, 22 Oct 2020 02:53:50 GMT  
		Size: 87.0 MB (87019121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:332424b879c5d240e02e6a86013d7b0c33723f633e70a0eade0291a1d2984c68`  
		Last Modified: Thu, 22 Oct 2020 02:53:21 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:17ef337ea40f46e40752c71b78b7ae7a31d799b13ebaa935d4a2a2a6299a4bfc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.3 MB (138284755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8d8961c30f82318eecf820136c41f2ff442cf41312dafa07e7bf99c3a78cd24`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 08 Sep 2020 23:09:11 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 08 Sep 2020 23:09:16 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 08 Sep 2020 23:09:18 GMT
ARG MAKEFLAGS=
# Tue, 08 Sep 2020 23:09:18 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 08 Sep 2020 23:17:34 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 08 Sep 2020 23:17:36 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 08 Sep 2020 23:17:37 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Tue, 08 Sep 2020 23:17:38 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Tue, 08 Sep 2020 23:17:38 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Tue, 08 Sep 2020 23:17:39 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Tue, 08 Sep 2020 23:17:40 GMT
VOLUME [/znc-data]
# Tue, 08 Sep 2020 23:17:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Sep 2020 23:18:13 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Tue, 08 Sep 2020 23:18:16 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3af72c5f00c204d691f1d0ab9703f2a6c87908f0d8fdb3079b8098d3eb11a4`  
		Last Modified: Tue, 08 Sep 2020 23:18:48 GMT  
		Size: 44.8 MB (44801095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec466ff3936be03632f5727b3891f787daf4f8a061758cc90b25f594a36f7b0`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7d16865df27d4706a565442663d383cb2dd421e874156e381b56f3df7f3456`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c7803979df031fecc89a6999d0f0ef620c8ab57abdca3a16c7dd33be3637f3`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a735a2fee33451376f3325ba75ee6f13830d03360d7505d2ea55c5764f2c80be`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f750b1f7cb005497de29337ba7a060bdf3af650765cf6fd6b0cf1932ea056e3`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fec810c5f1dc79e90f36e7026499dd2a69dcca4ce91fde28308aceecd04c160`  
		Last Modified: Tue, 08 Sep 2020 23:19:24 GMT  
		Size: 90.8 MB (90773938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26564ba4ffa6428ea9687ca10c07aa71d8fab18067ae29af81e4f73f004c3c0`  
		Last Modified: Tue, 08 Sep 2020 23:18:57 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.8.2`

```console
$ docker pull znc@sha256:5316ad98d0708ef3b93b911e2a98bd3b4de2206909aab37d987140f18301cf9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8.2` - linux; amd64

```console
$ docker pull znc@sha256:0fa3ea91829cc19a89db8568b5436e250f54d70a639af996ef5a28a69bade3ac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.6 MB (150607273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0073e8472cebc4ede105e2675f8bb492ea4ce59d134f44b1af1969aee4a890ca`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 06:05:00 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 22 Oct 2020 06:05:01 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 22 Oct 2020 06:05:01 GMT
ARG MAKEFLAGS=
# Thu, 22 Oct 2020 06:05:01 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 22 Oct 2020 06:11:10 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 22 Oct 2020 06:11:11 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 22 Oct 2020 06:11:11 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 22 Oct 2020 06:11:12 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 22 Oct 2020 06:11:12 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 22 Oct 2020 06:11:13 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 22 Oct 2020 06:11:13 GMT
VOLUME [/znc-data]
# Thu, 22 Oct 2020 06:11:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Oct 2020 06:11:35 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Thu, 22 Oct 2020 06:11:36 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0791fb9bd5d853a4620db9587acac4e5702d9fb63ef15123f885ea94159342c`  
		Last Modified: Thu, 22 Oct 2020 06:12:05 GMT  
		Size: 44.4 MB (44434892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c83b9beca5c9c26ebe0b2e287efc7a63b25cb16bdeaf1b54399b37f4e095665`  
		Last Modified: Thu, 22 Oct 2020 06:11:51 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47085387bf489e504bd8e581535a8dd00382a6775c461f57e48cd3ac45d7f4f9`  
		Last Modified: Thu, 22 Oct 2020 06:11:52 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8228de32d1fddd68f6bd466974b35c7e266629b74619c07a6191c86d6e12a54a`  
		Last Modified: Thu, 22 Oct 2020 06:11:51 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5da6e224361ae2d9a36212af67377a0d24bc4a86384fd32e165ae805d3e335`  
		Last Modified: Thu, 22 Oct 2020 06:11:52 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75b6faf1b171816e3706c54de9fd24fa7f6141f9081795dd0720e9fd20e655b`  
		Last Modified: Thu, 22 Oct 2020 06:11:52 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4724edc3b618a63c4e80fda513ad66a1be082731557dd815eebbdf5a752a1ac`  
		Last Modified: Thu, 22 Oct 2020 06:12:40 GMT  
		Size: 103.4 MB (103373793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99e5de9761ba1180d5357c2e9845b68f58bf534947d067f70afed65e7ec870f`  
		Last Modified: Thu, 22 Oct 2020 06:12:13 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8.2` - linux; arm variant v6

```console
$ docker pull znc@sha256:0282fcfdaa3fbea0a7af0dd8297a69f810c1799d390ecc5d53fde8c4024ccf88
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.3 MB (132306978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c80c86d2dfd752c2d69464c99940cc1205c98772848009f9ab3e6fdd299d7c8`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:43:44 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 22 Oct 2020 02:43:45 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 22 Oct 2020 02:43:47 GMT
ARG MAKEFLAGS=
# Thu, 22 Oct 2020 02:43:48 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 22 Oct 2020 02:52:04 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 22 Oct 2020 02:52:06 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 22 Oct 2020 02:52:07 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 22 Oct 2020 02:52:07 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 22 Oct 2020 02:52:08 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 22 Oct 2020 02:52:09 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 22 Oct 2020 02:52:11 GMT
VOLUME [/znc-data]
# Thu, 22 Oct 2020 02:52:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Oct 2020 02:52:38 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Thu, 22 Oct 2020 02:52:40 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f9828649f0a43abb2c7773562cb703c4174550ed46cd6873f1da33f8f7f7bc`  
		Last Modified: Thu, 22 Oct 2020 02:53:10 GMT  
		Size: 42.7 MB (42684189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce360030cd7eb3c6062ad0e8f22a430f6a7592052cbc442179f9facb20220dc`  
		Last Modified: Thu, 22 Oct 2020 02:52:52 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b59e17fda5a3bca1b5d7ef95539bd252efa4a18e7ea13f463181225a7860358`  
		Last Modified: Thu, 22 Oct 2020 02:52:53 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b016084e2f3ded73e2937734dadcb3e6d0564134e516a8d0ddced5867cde9990`  
		Last Modified: Thu, 22 Oct 2020 02:52:52 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02536655361cb4c04cc7c2f5600b73eabfb159ad3a6651859b239179d3fc2ad`  
		Last Modified: Thu, 22 Oct 2020 02:52:52 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14045112bb0830471184dcafe80013308ddc2e6625b319863e1f9fcc0ecb932d`  
		Last Modified: Thu, 22 Oct 2020 02:52:52 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed0305db86d902cf32741419da0708fb920bb1b33425b6a4f0eba4d7c86abbe`  
		Last Modified: Thu, 22 Oct 2020 02:53:50 GMT  
		Size: 87.0 MB (87019121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:332424b879c5d240e02e6a86013d7b0c33723f633e70a0eade0291a1d2984c68`  
		Last Modified: Thu, 22 Oct 2020 02:53:21 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8.2` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:17ef337ea40f46e40752c71b78b7ae7a31d799b13ebaa935d4a2a2a6299a4bfc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.3 MB (138284755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8d8961c30f82318eecf820136c41f2ff442cf41312dafa07e7bf99c3a78cd24`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 08 Sep 2020 23:09:11 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 08 Sep 2020 23:09:16 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 08 Sep 2020 23:09:18 GMT
ARG MAKEFLAGS=
# Tue, 08 Sep 2020 23:09:18 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 08 Sep 2020 23:17:34 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 08 Sep 2020 23:17:36 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 08 Sep 2020 23:17:37 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Tue, 08 Sep 2020 23:17:38 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Tue, 08 Sep 2020 23:17:38 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Tue, 08 Sep 2020 23:17:39 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Tue, 08 Sep 2020 23:17:40 GMT
VOLUME [/znc-data]
# Tue, 08 Sep 2020 23:17:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Sep 2020 23:18:13 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Tue, 08 Sep 2020 23:18:16 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3af72c5f00c204d691f1d0ab9703f2a6c87908f0d8fdb3079b8098d3eb11a4`  
		Last Modified: Tue, 08 Sep 2020 23:18:48 GMT  
		Size: 44.8 MB (44801095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec466ff3936be03632f5727b3891f787daf4f8a061758cc90b25f594a36f7b0`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7d16865df27d4706a565442663d383cb2dd421e874156e381b56f3df7f3456`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c7803979df031fecc89a6999d0f0ef620c8ab57abdca3a16c7dd33be3637f3`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a735a2fee33451376f3325ba75ee6f13830d03360d7505d2ea55c5764f2c80be`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f750b1f7cb005497de29337ba7a060bdf3af650765cf6fd6b0cf1932ea056e3`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fec810c5f1dc79e90f36e7026499dd2a69dcca4ce91fde28308aceecd04c160`  
		Last Modified: Tue, 08 Sep 2020 23:19:24 GMT  
		Size: 90.8 MB (90773938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26564ba4ffa6428ea9687ca10c07aa71d8fab18067ae29af81e4f73f004c3c0`  
		Last Modified: Tue, 08 Sep 2020 23:18:57 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.8.2-slim`

```console
$ docker pull znc@sha256:f720165edcd939783306a7b9ca10e26f37ef8bd4a68048a5be14447c92604850
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8.2-slim` - linux; amd64

```console
$ docker pull znc@sha256:a773df7fd8dd5798dbcddae8843aca6e480065692efe6412cf98d8c957c407ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47233149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3be2cf2ae9dce24b718710e821f1fb04526bd15739edb47d405320c3f4dd2d0b`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 06:05:00 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 22 Oct 2020 06:05:01 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 22 Oct 2020 06:05:01 GMT
ARG MAKEFLAGS=
# Thu, 22 Oct 2020 06:05:01 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 22 Oct 2020 06:11:10 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 22 Oct 2020 06:11:11 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 22 Oct 2020 06:11:11 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 22 Oct 2020 06:11:12 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 22 Oct 2020 06:11:12 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 22 Oct 2020 06:11:13 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 22 Oct 2020 06:11:13 GMT
VOLUME [/znc-data]
# Thu, 22 Oct 2020 06:11:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0791fb9bd5d853a4620db9587acac4e5702d9fb63ef15123f885ea94159342c`  
		Last Modified: Thu, 22 Oct 2020 06:12:05 GMT  
		Size: 44.4 MB (44434892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c83b9beca5c9c26ebe0b2e287efc7a63b25cb16bdeaf1b54399b37f4e095665`  
		Last Modified: Thu, 22 Oct 2020 06:11:51 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47085387bf489e504bd8e581535a8dd00382a6775c461f57e48cd3ac45d7f4f9`  
		Last Modified: Thu, 22 Oct 2020 06:11:52 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8228de32d1fddd68f6bd466974b35c7e266629b74619c07a6191c86d6e12a54a`  
		Last Modified: Thu, 22 Oct 2020 06:11:51 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5da6e224361ae2d9a36212af67377a0d24bc4a86384fd32e165ae805d3e335`  
		Last Modified: Thu, 22 Oct 2020 06:11:52 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75b6faf1b171816e3706c54de9fd24fa7f6141f9081795dd0720e9fd20e655b`  
		Last Modified: Thu, 22 Oct 2020 06:11:52 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8.2-slim` - linux; arm variant v6

```console
$ docker pull znc@sha256:64a3b9b845547382135a5513135a1612de58aaa131c735e6ac1ef62fd8b789cd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.3 MB (45287525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f2c5e3b79c83b717704bef36d6ccad717a2b5225153873cb504d3613f89f3a`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:43:44 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 22 Oct 2020 02:43:45 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 22 Oct 2020 02:43:47 GMT
ARG MAKEFLAGS=
# Thu, 22 Oct 2020 02:43:48 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 22 Oct 2020 02:52:04 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 22 Oct 2020 02:52:06 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 22 Oct 2020 02:52:07 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 22 Oct 2020 02:52:07 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 22 Oct 2020 02:52:08 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 22 Oct 2020 02:52:09 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 22 Oct 2020 02:52:11 GMT
VOLUME [/znc-data]
# Thu, 22 Oct 2020 02:52:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f9828649f0a43abb2c7773562cb703c4174550ed46cd6873f1da33f8f7f7bc`  
		Last Modified: Thu, 22 Oct 2020 02:53:10 GMT  
		Size: 42.7 MB (42684189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce360030cd7eb3c6062ad0e8f22a430f6a7592052cbc442179f9facb20220dc`  
		Last Modified: Thu, 22 Oct 2020 02:52:52 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b59e17fda5a3bca1b5d7ef95539bd252efa4a18e7ea13f463181225a7860358`  
		Last Modified: Thu, 22 Oct 2020 02:52:53 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b016084e2f3ded73e2937734dadcb3e6d0564134e516a8d0ddced5867cde9990`  
		Last Modified: Thu, 22 Oct 2020 02:52:52 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02536655361cb4c04cc7c2f5600b73eabfb159ad3a6651859b239179d3fc2ad`  
		Last Modified: Thu, 22 Oct 2020 02:52:52 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14045112bb0830471184dcafe80013308ddc2e6625b319863e1f9fcc0ecb932d`  
		Last Modified: Thu, 22 Oct 2020 02:52:52 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8.2-slim` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:a7c2e95fddde0559e9537396f03bdcdc4000c2ff2bf6596352a589a65370e672
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.5 MB (47510487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05068a92fefa4483359efa9e88b75464de67a2e8ffebc5f3bb1ade5ef7b24999`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 08 Sep 2020 23:09:11 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 08 Sep 2020 23:09:16 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 08 Sep 2020 23:09:18 GMT
ARG MAKEFLAGS=
# Tue, 08 Sep 2020 23:09:18 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 08 Sep 2020 23:17:34 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 08 Sep 2020 23:17:36 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 08 Sep 2020 23:17:37 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Tue, 08 Sep 2020 23:17:38 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Tue, 08 Sep 2020 23:17:38 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Tue, 08 Sep 2020 23:17:39 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Tue, 08 Sep 2020 23:17:40 GMT
VOLUME [/znc-data]
# Tue, 08 Sep 2020 23:17:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3af72c5f00c204d691f1d0ab9703f2a6c87908f0d8fdb3079b8098d3eb11a4`  
		Last Modified: Tue, 08 Sep 2020 23:18:48 GMT  
		Size: 44.8 MB (44801095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec466ff3936be03632f5727b3891f787daf4f8a061758cc90b25f594a36f7b0`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7d16865df27d4706a565442663d383cb2dd421e874156e381b56f3df7f3456`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c7803979df031fecc89a6999d0f0ef620c8ab57abdca3a16c7dd33be3637f3`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a735a2fee33451376f3325ba75ee6f13830d03360d7505d2ea55c5764f2c80be`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f750b1f7cb005497de29337ba7a060bdf3af650765cf6fd6b0cf1932ea056e3`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.8-slim`

```console
$ docker pull znc@sha256:f720165edcd939783306a7b9ca10e26f37ef8bd4a68048a5be14447c92604850
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8-slim` - linux; amd64

```console
$ docker pull znc@sha256:a773df7fd8dd5798dbcddae8843aca6e480065692efe6412cf98d8c957c407ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47233149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3be2cf2ae9dce24b718710e821f1fb04526bd15739edb47d405320c3f4dd2d0b`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 06:05:00 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 22 Oct 2020 06:05:01 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 22 Oct 2020 06:05:01 GMT
ARG MAKEFLAGS=
# Thu, 22 Oct 2020 06:05:01 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 22 Oct 2020 06:11:10 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 22 Oct 2020 06:11:11 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 22 Oct 2020 06:11:11 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 22 Oct 2020 06:11:12 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 22 Oct 2020 06:11:12 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 22 Oct 2020 06:11:13 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 22 Oct 2020 06:11:13 GMT
VOLUME [/znc-data]
# Thu, 22 Oct 2020 06:11:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0791fb9bd5d853a4620db9587acac4e5702d9fb63ef15123f885ea94159342c`  
		Last Modified: Thu, 22 Oct 2020 06:12:05 GMT  
		Size: 44.4 MB (44434892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c83b9beca5c9c26ebe0b2e287efc7a63b25cb16bdeaf1b54399b37f4e095665`  
		Last Modified: Thu, 22 Oct 2020 06:11:51 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47085387bf489e504bd8e581535a8dd00382a6775c461f57e48cd3ac45d7f4f9`  
		Last Modified: Thu, 22 Oct 2020 06:11:52 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8228de32d1fddd68f6bd466974b35c7e266629b74619c07a6191c86d6e12a54a`  
		Last Modified: Thu, 22 Oct 2020 06:11:51 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5da6e224361ae2d9a36212af67377a0d24bc4a86384fd32e165ae805d3e335`  
		Last Modified: Thu, 22 Oct 2020 06:11:52 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75b6faf1b171816e3706c54de9fd24fa7f6141f9081795dd0720e9fd20e655b`  
		Last Modified: Thu, 22 Oct 2020 06:11:52 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8-slim` - linux; arm variant v6

```console
$ docker pull znc@sha256:64a3b9b845547382135a5513135a1612de58aaa131c735e6ac1ef62fd8b789cd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.3 MB (45287525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f2c5e3b79c83b717704bef36d6ccad717a2b5225153873cb504d3613f89f3a`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:43:44 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 22 Oct 2020 02:43:45 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 22 Oct 2020 02:43:47 GMT
ARG MAKEFLAGS=
# Thu, 22 Oct 2020 02:43:48 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 22 Oct 2020 02:52:04 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 22 Oct 2020 02:52:06 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 22 Oct 2020 02:52:07 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 22 Oct 2020 02:52:07 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 22 Oct 2020 02:52:08 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 22 Oct 2020 02:52:09 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 22 Oct 2020 02:52:11 GMT
VOLUME [/znc-data]
# Thu, 22 Oct 2020 02:52:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f9828649f0a43abb2c7773562cb703c4174550ed46cd6873f1da33f8f7f7bc`  
		Last Modified: Thu, 22 Oct 2020 02:53:10 GMT  
		Size: 42.7 MB (42684189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce360030cd7eb3c6062ad0e8f22a430f6a7592052cbc442179f9facb20220dc`  
		Last Modified: Thu, 22 Oct 2020 02:52:52 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b59e17fda5a3bca1b5d7ef95539bd252efa4a18e7ea13f463181225a7860358`  
		Last Modified: Thu, 22 Oct 2020 02:52:53 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b016084e2f3ded73e2937734dadcb3e6d0564134e516a8d0ddced5867cde9990`  
		Last Modified: Thu, 22 Oct 2020 02:52:52 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02536655361cb4c04cc7c2f5600b73eabfb159ad3a6651859b239179d3fc2ad`  
		Last Modified: Thu, 22 Oct 2020 02:52:52 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14045112bb0830471184dcafe80013308ddc2e6625b319863e1f9fcc0ecb932d`  
		Last Modified: Thu, 22 Oct 2020 02:52:52 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8-slim` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:a7c2e95fddde0559e9537396f03bdcdc4000c2ff2bf6596352a589a65370e672
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.5 MB (47510487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05068a92fefa4483359efa9e88b75464de67a2e8ffebc5f3bb1ade5ef7b24999`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 08 Sep 2020 23:09:11 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 08 Sep 2020 23:09:16 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 08 Sep 2020 23:09:18 GMT
ARG MAKEFLAGS=
# Tue, 08 Sep 2020 23:09:18 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 08 Sep 2020 23:17:34 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 08 Sep 2020 23:17:36 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 08 Sep 2020 23:17:37 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Tue, 08 Sep 2020 23:17:38 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Tue, 08 Sep 2020 23:17:38 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Tue, 08 Sep 2020 23:17:39 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Tue, 08 Sep 2020 23:17:40 GMT
VOLUME [/znc-data]
# Tue, 08 Sep 2020 23:17:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3af72c5f00c204d691f1d0ab9703f2a6c87908f0d8fdb3079b8098d3eb11a4`  
		Last Modified: Tue, 08 Sep 2020 23:18:48 GMT  
		Size: 44.8 MB (44801095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec466ff3936be03632f5727b3891f787daf4f8a061758cc90b25f594a36f7b0`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7d16865df27d4706a565442663d383cb2dd421e874156e381b56f3df7f3456`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c7803979df031fecc89a6999d0f0ef620c8ab57abdca3a16c7dd33be3637f3`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a735a2fee33451376f3325ba75ee6f13830d03360d7505d2ea55c5764f2c80be`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f750b1f7cb005497de29337ba7a060bdf3af650765cf6fd6b0cf1932ea056e3`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:latest`

```console
$ docker pull znc@sha256:5316ad98d0708ef3b93b911e2a98bd3b4de2206909aab37d987140f18301cf9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:latest` - linux; amd64

```console
$ docker pull znc@sha256:0fa3ea91829cc19a89db8568b5436e250f54d70a639af996ef5a28a69bade3ac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.6 MB (150607273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0073e8472cebc4ede105e2675f8bb492ea4ce59d134f44b1af1969aee4a890ca`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 06:05:00 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 22 Oct 2020 06:05:01 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 22 Oct 2020 06:05:01 GMT
ARG MAKEFLAGS=
# Thu, 22 Oct 2020 06:05:01 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 22 Oct 2020 06:11:10 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 22 Oct 2020 06:11:11 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 22 Oct 2020 06:11:11 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 22 Oct 2020 06:11:12 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 22 Oct 2020 06:11:12 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 22 Oct 2020 06:11:13 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 22 Oct 2020 06:11:13 GMT
VOLUME [/znc-data]
# Thu, 22 Oct 2020 06:11:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Oct 2020 06:11:35 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Thu, 22 Oct 2020 06:11:36 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0791fb9bd5d853a4620db9587acac4e5702d9fb63ef15123f885ea94159342c`  
		Last Modified: Thu, 22 Oct 2020 06:12:05 GMT  
		Size: 44.4 MB (44434892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c83b9beca5c9c26ebe0b2e287efc7a63b25cb16bdeaf1b54399b37f4e095665`  
		Last Modified: Thu, 22 Oct 2020 06:11:51 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47085387bf489e504bd8e581535a8dd00382a6775c461f57e48cd3ac45d7f4f9`  
		Last Modified: Thu, 22 Oct 2020 06:11:52 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8228de32d1fddd68f6bd466974b35c7e266629b74619c07a6191c86d6e12a54a`  
		Last Modified: Thu, 22 Oct 2020 06:11:51 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5da6e224361ae2d9a36212af67377a0d24bc4a86384fd32e165ae805d3e335`  
		Last Modified: Thu, 22 Oct 2020 06:11:52 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75b6faf1b171816e3706c54de9fd24fa7f6141f9081795dd0720e9fd20e655b`  
		Last Modified: Thu, 22 Oct 2020 06:11:52 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4724edc3b618a63c4e80fda513ad66a1be082731557dd815eebbdf5a752a1ac`  
		Last Modified: Thu, 22 Oct 2020 06:12:40 GMT  
		Size: 103.4 MB (103373793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99e5de9761ba1180d5357c2e9845b68f58bf534947d067f70afed65e7ec870f`  
		Last Modified: Thu, 22 Oct 2020 06:12:13 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:latest` - linux; arm variant v6

```console
$ docker pull znc@sha256:0282fcfdaa3fbea0a7af0dd8297a69f810c1799d390ecc5d53fde8c4024ccf88
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.3 MB (132306978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c80c86d2dfd752c2d69464c99940cc1205c98772848009f9ab3e6fdd299d7c8`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:43:44 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 22 Oct 2020 02:43:45 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 22 Oct 2020 02:43:47 GMT
ARG MAKEFLAGS=
# Thu, 22 Oct 2020 02:43:48 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 22 Oct 2020 02:52:04 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 22 Oct 2020 02:52:06 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 22 Oct 2020 02:52:07 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 22 Oct 2020 02:52:07 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 22 Oct 2020 02:52:08 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 22 Oct 2020 02:52:09 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 22 Oct 2020 02:52:11 GMT
VOLUME [/znc-data]
# Thu, 22 Oct 2020 02:52:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Oct 2020 02:52:38 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Thu, 22 Oct 2020 02:52:40 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f9828649f0a43abb2c7773562cb703c4174550ed46cd6873f1da33f8f7f7bc`  
		Last Modified: Thu, 22 Oct 2020 02:53:10 GMT  
		Size: 42.7 MB (42684189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce360030cd7eb3c6062ad0e8f22a430f6a7592052cbc442179f9facb20220dc`  
		Last Modified: Thu, 22 Oct 2020 02:52:52 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b59e17fda5a3bca1b5d7ef95539bd252efa4a18e7ea13f463181225a7860358`  
		Last Modified: Thu, 22 Oct 2020 02:52:53 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b016084e2f3ded73e2937734dadcb3e6d0564134e516a8d0ddced5867cde9990`  
		Last Modified: Thu, 22 Oct 2020 02:52:52 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02536655361cb4c04cc7c2f5600b73eabfb159ad3a6651859b239179d3fc2ad`  
		Last Modified: Thu, 22 Oct 2020 02:52:52 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14045112bb0830471184dcafe80013308ddc2e6625b319863e1f9fcc0ecb932d`  
		Last Modified: Thu, 22 Oct 2020 02:52:52 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed0305db86d902cf32741419da0708fb920bb1b33425b6a4f0eba4d7c86abbe`  
		Last Modified: Thu, 22 Oct 2020 02:53:50 GMT  
		Size: 87.0 MB (87019121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:332424b879c5d240e02e6a86013d7b0c33723f633e70a0eade0291a1d2984c68`  
		Last Modified: Thu, 22 Oct 2020 02:53:21 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:latest` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:17ef337ea40f46e40752c71b78b7ae7a31d799b13ebaa935d4a2a2a6299a4bfc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.3 MB (138284755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8d8961c30f82318eecf820136c41f2ff442cf41312dafa07e7bf99c3a78cd24`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 08 Sep 2020 23:09:11 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 08 Sep 2020 23:09:16 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 08 Sep 2020 23:09:18 GMT
ARG MAKEFLAGS=
# Tue, 08 Sep 2020 23:09:18 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 08 Sep 2020 23:17:34 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 08 Sep 2020 23:17:36 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 08 Sep 2020 23:17:37 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Tue, 08 Sep 2020 23:17:38 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Tue, 08 Sep 2020 23:17:38 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Tue, 08 Sep 2020 23:17:39 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Tue, 08 Sep 2020 23:17:40 GMT
VOLUME [/znc-data]
# Tue, 08 Sep 2020 23:17:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Sep 2020 23:18:13 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Tue, 08 Sep 2020 23:18:16 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3af72c5f00c204d691f1d0ab9703f2a6c87908f0d8fdb3079b8098d3eb11a4`  
		Last Modified: Tue, 08 Sep 2020 23:18:48 GMT  
		Size: 44.8 MB (44801095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec466ff3936be03632f5727b3891f787daf4f8a061758cc90b25f594a36f7b0`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7d16865df27d4706a565442663d383cb2dd421e874156e381b56f3df7f3456`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c7803979df031fecc89a6999d0f0ef620c8ab57abdca3a16c7dd33be3637f3`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a735a2fee33451376f3325ba75ee6f13830d03360d7505d2ea55c5764f2c80be`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f750b1f7cb005497de29337ba7a060bdf3af650765cf6fd6b0cf1932ea056e3`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fec810c5f1dc79e90f36e7026499dd2a69dcca4ce91fde28308aceecd04c160`  
		Last Modified: Tue, 08 Sep 2020 23:19:24 GMT  
		Size: 90.8 MB (90773938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26564ba4ffa6428ea9687ca10c07aa71d8fab18067ae29af81e4f73f004c3c0`  
		Last Modified: Tue, 08 Sep 2020 23:18:57 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:slim`

```console
$ docker pull znc@sha256:f720165edcd939783306a7b9ca10e26f37ef8bd4a68048a5be14447c92604850
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:slim` - linux; amd64

```console
$ docker pull znc@sha256:a773df7fd8dd5798dbcddae8843aca6e480065692efe6412cf98d8c957c407ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47233149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3be2cf2ae9dce24b718710e821f1fb04526bd15739edb47d405320c3f4dd2d0b`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 06:05:00 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 22 Oct 2020 06:05:01 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 22 Oct 2020 06:05:01 GMT
ARG MAKEFLAGS=
# Thu, 22 Oct 2020 06:05:01 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 22 Oct 2020 06:11:10 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 22 Oct 2020 06:11:11 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 22 Oct 2020 06:11:11 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 22 Oct 2020 06:11:12 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 22 Oct 2020 06:11:12 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 22 Oct 2020 06:11:13 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 22 Oct 2020 06:11:13 GMT
VOLUME [/znc-data]
# Thu, 22 Oct 2020 06:11:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0791fb9bd5d853a4620db9587acac4e5702d9fb63ef15123f885ea94159342c`  
		Last Modified: Thu, 22 Oct 2020 06:12:05 GMT  
		Size: 44.4 MB (44434892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c83b9beca5c9c26ebe0b2e287efc7a63b25cb16bdeaf1b54399b37f4e095665`  
		Last Modified: Thu, 22 Oct 2020 06:11:51 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47085387bf489e504bd8e581535a8dd00382a6775c461f57e48cd3ac45d7f4f9`  
		Last Modified: Thu, 22 Oct 2020 06:11:52 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8228de32d1fddd68f6bd466974b35c7e266629b74619c07a6191c86d6e12a54a`  
		Last Modified: Thu, 22 Oct 2020 06:11:51 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5da6e224361ae2d9a36212af67377a0d24bc4a86384fd32e165ae805d3e335`  
		Last Modified: Thu, 22 Oct 2020 06:11:52 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75b6faf1b171816e3706c54de9fd24fa7f6141f9081795dd0720e9fd20e655b`  
		Last Modified: Thu, 22 Oct 2020 06:11:52 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:slim` - linux; arm variant v6

```console
$ docker pull znc@sha256:64a3b9b845547382135a5513135a1612de58aaa131c735e6ac1ef62fd8b789cd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.3 MB (45287525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f2c5e3b79c83b717704bef36d6ccad717a2b5225153873cb504d3613f89f3a`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:43:44 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 22 Oct 2020 02:43:45 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 22 Oct 2020 02:43:47 GMT
ARG MAKEFLAGS=
# Thu, 22 Oct 2020 02:43:48 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 22 Oct 2020 02:52:04 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 22 Oct 2020 02:52:06 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 22 Oct 2020 02:52:07 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 22 Oct 2020 02:52:07 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 22 Oct 2020 02:52:08 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 22 Oct 2020 02:52:09 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 22 Oct 2020 02:52:11 GMT
VOLUME [/znc-data]
# Thu, 22 Oct 2020 02:52:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f9828649f0a43abb2c7773562cb703c4174550ed46cd6873f1da33f8f7f7bc`  
		Last Modified: Thu, 22 Oct 2020 02:53:10 GMT  
		Size: 42.7 MB (42684189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce360030cd7eb3c6062ad0e8f22a430f6a7592052cbc442179f9facb20220dc`  
		Last Modified: Thu, 22 Oct 2020 02:52:52 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b59e17fda5a3bca1b5d7ef95539bd252efa4a18e7ea13f463181225a7860358`  
		Last Modified: Thu, 22 Oct 2020 02:52:53 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b016084e2f3ded73e2937734dadcb3e6d0564134e516a8d0ddced5867cde9990`  
		Last Modified: Thu, 22 Oct 2020 02:52:52 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02536655361cb4c04cc7c2f5600b73eabfb159ad3a6651859b239179d3fc2ad`  
		Last Modified: Thu, 22 Oct 2020 02:52:52 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14045112bb0830471184dcafe80013308ddc2e6625b319863e1f9fcc0ecb932d`  
		Last Modified: Thu, 22 Oct 2020 02:52:52 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:slim` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:a7c2e95fddde0559e9537396f03bdcdc4000c2ff2bf6596352a589a65370e672
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.5 MB (47510487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05068a92fefa4483359efa9e88b75464de67a2e8ffebc5f3bb1ade5ef7b24999`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 08 Sep 2020 23:09:11 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 08 Sep 2020 23:09:16 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 08 Sep 2020 23:09:18 GMT
ARG MAKEFLAGS=
# Tue, 08 Sep 2020 23:09:18 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 08 Sep 2020 23:17:34 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 08 Sep 2020 23:17:36 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 08 Sep 2020 23:17:37 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Tue, 08 Sep 2020 23:17:38 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Tue, 08 Sep 2020 23:17:38 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Tue, 08 Sep 2020 23:17:39 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Tue, 08 Sep 2020 23:17:40 GMT
VOLUME [/znc-data]
# Tue, 08 Sep 2020 23:17:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3af72c5f00c204d691f1d0ab9703f2a6c87908f0d8fdb3079b8098d3eb11a4`  
		Last Modified: Tue, 08 Sep 2020 23:18:48 GMT  
		Size: 44.8 MB (44801095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec466ff3936be03632f5727b3891f787daf4f8a061758cc90b25f594a36f7b0`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7d16865df27d4706a565442663d383cb2dd421e874156e381b56f3df7f3456`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c7803979df031fecc89a6999d0f0ef620c8ab57abdca3a16c7dd33be3637f3`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a735a2fee33451376f3325ba75ee6f13830d03360d7505d2ea55c5764f2c80be`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f750b1f7cb005497de29337ba7a060bdf3af650765cf6fd6b0cf1932ea056e3`  
		Last Modified: Tue, 08 Sep 2020 23:18:28 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
