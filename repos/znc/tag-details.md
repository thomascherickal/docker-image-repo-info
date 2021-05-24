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
$ docker pull znc@sha256:d150a0131945a0703c58a3029c15967564481594cfdfe49ed8b192c2787bc2d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8` - linux; amd64

```console
$ docker pull znc@sha256:2b472aa12e1e6df0af93d7d0fbcdc76c43f13b5f25366695d58e5012624fea77
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (150976169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a504340efb3ee87ba29443a5a485e2ef4001245a9c52aeb7abd49e71f9ce7c0f`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 08:49:29 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 15 Apr 2021 08:49:29 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 15 Apr 2021 08:49:29 GMT
ARG MAKEFLAGS=
# Thu, 15 Apr 2021 08:49:29 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 15 Apr 2021 08:53:11 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 15 Apr 2021 08:53:11 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 15 Apr 2021 08:53:11 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:53:12 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:53:12 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 15 Apr 2021 08:53:12 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:53:12 GMT
VOLUME [/znc-data]
# Thu, 15 Apr 2021 08:53:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Apr 2021 08:53:32 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Thu, 15 Apr 2021 08:53:32 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb2e5913ac4c145e00a1896b6ca33dd769f1ae89d094e1036fea9158e697255`  
		Last Modified: Thu, 15 Apr 2021 08:53:56 GMT  
		Size: 44.8 MB (44791665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5baa3714b7588148fea833496685a7c3ae7f7594155bccfbce829a2dcc181bab`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9df6d19694e9b31214bcb2e58eff4ec7c1edf95604c4bc082ce254cabc8f376`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 303.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7461218a0b487e65c95477eb8af45c79a19f76a36c2849efbc880fad8f09bd8`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01964acb966afc4e11e5072b630ce334c9a3755fc140c33ea7794295940a6de`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3925cb8dc6060e3a0ed0da6f992cbe4968b1da9fdce9748a194d87292e0e30d0`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be684e19e6c893922d2bda3ce925dcd04b60b7bfd9b23b0b353a749989ea762a`  
		Last Modified: Thu, 15 Apr 2021 08:54:27 GMT  
		Size: 103.4 MB (103382183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a13707e68ab73cd2b6ca6fb7f5e20034a14f59f8b138f5dded3a47b0b25015`  
		Last Modified: Thu, 15 Apr 2021 08:54:10 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8` - linux; arm variant v6

```console
$ docker pull znc@sha256:637262cf7726596493c9e1b36319cadee4df531ad169e2ab193bfa5c793c606a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.7 MB (132687454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db254ececf401d0f7db47f515c435b080eeccf382db2085cedd9b4df8336259c`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:06:24 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Wed, 14 Apr 2021 19:06:25 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Wed, 14 Apr 2021 19:06:26 GMT
ARG MAKEFLAGS=
# Wed, 14 Apr 2021 19:06:27 GMT
ENV ZNC_VERSION=1.8.2
# Wed, 14 Apr 2021 19:14:38 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Wed, 14 Apr 2021 19:14:40 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Wed, 14 Apr 2021 19:14:41 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Wed, 14 Apr 2021 19:14:42 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Wed, 14 Apr 2021 19:14:43 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Wed, 14 Apr 2021 19:14:44 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Wed, 14 Apr 2021 19:14:45 GMT
VOLUME [/znc-data]
# Wed, 14 Apr 2021 19:14:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 19:15:07 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Wed, 14 Apr 2021 19:15:10 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a7c2bb5435b1fa5a12ae177d982fedb637c06223b2c701cb90ecd09de64929`  
		Last Modified: Wed, 14 Apr 2021 19:15:45 GMT  
		Size: 43.0 MB (43047705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174b893fee9110b0d361ce6ac762b55def7e783e102df78cfa7de76273c474c2`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cd01900ad296ad09f6b29dc0dbf821432761b6b9771daddbe9077e2ac7bede`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4852ba58f3351dc50f648ff54754f3143c4bc73aff353c8fc44f1ca4b2727e1b`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e2bd3ffa516127012f7dd673a572cff0cc0b3a53555d987507a3f0e697e70d`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc133d3eda0b1cbf3ee429aa42a8babe168097f3490aff7e11bf216e2200ff9`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6f9dc0fc71449c9d6aa086257cdeeccd8c2b27bc1d0912041ec74b9acd1e76`  
		Last Modified: Wed, 14 Apr 2021 19:16:23 GMT  
		Size: 87.0 MB (87032736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773f8f7b9621c6f9898eccd6e54c2229ef68db2240332907412d1c0e7a7bb167`  
		Last Modified: Wed, 14 Apr 2021 19:15:56 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:29d98eabc792795f96284e8e5035370c2050827723614beadc05c997c3bd70b1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.1 MB (138149484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6989fa92e7955f83225a6b4c06e8424a0423ac758dbe6fd3b746d6d5e2e2b722`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 08:12:40 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 15 Apr 2021 08:12:41 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 15 Apr 2021 08:12:43 GMT
ARG MAKEFLAGS=
# Thu, 15 Apr 2021 08:12:44 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 15 Apr 2021 08:21:02 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 15 Apr 2021 08:21:03 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 15 Apr 2021 08:21:05 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:21:06 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:21:07 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 15 Apr 2021 08:21:08 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:21:09 GMT
VOLUME [/znc-data]
# Thu, 15 Apr 2021 08:21:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Apr 2021 08:21:32 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Thu, 15 Apr 2021 08:21:34 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b3d8e65d0874b1cc53dbb44a2e82d655e8190289913fab876cd4a5b436bcf1`  
		Last Modified: Thu, 15 Apr 2021 08:22:05 GMT  
		Size: 44.6 MB (44634519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d035de95c553cb3f7613ba60b02fbdef7bd797abc283c6f50c0d6e9cc4c98816`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71254d8296a59ad61bd4ad74ff217b2c47ed1a5cdd1b76e68021626df65bdd57`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168537d99c9d6d4daa6bc6ed86109da65add907c96c77c2e34eee0e0a42edccb`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d66e70ca1fcef2fdccee60836c00ebb782d33fc344be33f26cea26cb56b7d20`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0d8f2e63bb260ced0b1c2fde1f39c5b7c65e177825c5f5d50d99cbccc16e24`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000a6a235692a3416c03c800f989cfb587885d6703b14fac566e1d99cb13226e`  
		Last Modified: Thu, 15 Apr 2021 08:22:38 GMT  
		Size: 90.8 MB (90802510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8955ad239f51ee3c4b20437a4d49828decee2ddec1dd66b42927d14032ebdb86`  
		Last Modified: Thu, 15 Apr 2021 08:22:17 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.8.2`

```console
$ docker pull znc@sha256:d150a0131945a0703c58a3029c15967564481594cfdfe49ed8b192c2787bc2d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8.2` - linux; amd64

```console
$ docker pull znc@sha256:2b472aa12e1e6df0af93d7d0fbcdc76c43f13b5f25366695d58e5012624fea77
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (150976169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a504340efb3ee87ba29443a5a485e2ef4001245a9c52aeb7abd49e71f9ce7c0f`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 08:49:29 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 15 Apr 2021 08:49:29 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 15 Apr 2021 08:49:29 GMT
ARG MAKEFLAGS=
# Thu, 15 Apr 2021 08:49:29 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 15 Apr 2021 08:53:11 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 15 Apr 2021 08:53:11 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 15 Apr 2021 08:53:11 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:53:12 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:53:12 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 15 Apr 2021 08:53:12 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:53:12 GMT
VOLUME [/znc-data]
# Thu, 15 Apr 2021 08:53:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Apr 2021 08:53:32 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Thu, 15 Apr 2021 08:53:32 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb2e5913ac4c145e00a1896b6ca33dd769f1ae89d094e1036fea9158e697255`  
		Last Modified: Thu, 15 Apr 2021 08:53:56 GMT  
		Size: 44.8 MB (44791665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5baa3714b7588148fea833496685a7c3ae7f7594155bccfbce829a2dcc181bab`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9df6d19694e9b31214bcb2e58eff4ec7c1edf95604c4bc082ce254cabc8f376`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 303.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7461218a0b487e65c95477eb8af45c79a19f76a36c2849efbc880fad8f09bd8`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01964acb966afc4e11e5072b630ce334c9a3755fc140c33ea7794295940a6de`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3925cb8dc6060e3a0ed0da6f992cbe4968b1da9fdce9748a194d87292e0e30d0`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be684e19e6c893922d2bda3ce925dcd04b60b7bfd9b23b0b353a749989ea762a`  
		Last Modified: Thu, 15 Apr 2021 08:54:27 GMT  
		Size: 103.4 MB (103382183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a13707e68ab73cd2b6ca6fb7f5e20034a14f59f8b138f5dded3a47b0b25015`  
		Last Modified: Thu, 15 Apr 2021 08:54:10 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8.2` - linux; arm variant v6

```console
$ docker pull znc@sha256:637262cf7726596493c9e1b36319cadee4df531ad169e2ab193bfa5c793c606a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.7 MB (132687454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db254ececf401d0f7db47f515c435b080eeccf382db2085cedd9b4df8336259c`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:06:24 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Wed, 14 Apr 2021 19:06:25 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Wed, 14 Apr 2021 19:06:26 GMT
ARG MAKEFLAGS=
# Wed, 14 Apr 2021 19:06:27 GMT
ENV ZNC_VERSION=1.8.2
# Wed, 14 Apr 2021 19:14:38 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Wed, 14 Apr 2021 19:14:40 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Wed, 14 Apr 2021 19:14:41 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Wed, 14 Apr 2021 19:14:42 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Wed, 14 Apr 2021 19:14:43 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Wed, 14 Apr 2021 19:14:44 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Wed, 14 Apr 2021 19:14:45 GMT
VOLUME [/znc-data]
# Wed, 14 Apr 2021 19:14:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 19:15:07 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Wed, 14 Apr 2021 19:15:10 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a7c2bb5435b1fa5a12ae177d982fedb637c06223b2c701cb90ecd09de64929`  
		Last Modified: Wed, 14 Apr 2021 19:15:45 GMT  
		Size: 43.0 MB (43047705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174b893fee9110b0d361ce6ac762b55def7e783e102df78cfa7de76273c474c2`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cd01900ad296ad09f6b29dc0dbf821432761b6b9771daddbe9077e2ac7bede`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4852ba58f3351dc50f648ff54754f3143c4bc73aff353c8fc44f1ca4b2727e1b`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e2bd3ffa516127012f7dd673a572cff0cc0b3a53555d987507a3f0e697e70d`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc133d3eda0b1cbf3ee429aa42a8babe168097f3490aff7e11bf216e2200ff9`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6f9dc0fc71449c9d6aa086257cdeeccd8c2b27bc1d0912041ec74b9acd1e76`  
		Last Modified: Wed, 14 Apr 2021 19:16:23 GMT  
		Size: 87.0 MB (87032736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773f8f7b9621c6f9898eccd6e54c2229ef68db2240332907412d1c0e7a7bb167`  
		Last Modified: Wed, 14 Apr 2021 19:15:56 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8.2` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:29d98eabc792795f96284e8e5035370c2050827723614beadc05c997c3bd70b1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.1 MB (138149484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6989fa92e7955f83225a6b4c06e8424a0423ac758dbe6fd3b746d6d5e2e2b722`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 08:12:40 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 15 Apr 2021 08:12:41 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 15 Apr 2021 08:12:43 GMT
ARG MAKEFLAGS=
# Thu, 15 Apr 2021 08:12:44 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 15 Apr 2021 08:21:02 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 15 Apr 2021 08:21:03 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 15 Apr 2021 08:21:05 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:21:06 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:21:07 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 15 Apr 2021 08:21:08 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:21:09 GMT
VOLUME [/znc-data]
# Thu, 15 Apr 2021 08:21:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Apr 2021 08:21:32 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Thu, 15 Apr 2021 08:21:34 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b3d8e65d0874b1cc53dbb44a2e82d655e8190289913fab876cd4a5b436bcf1`  
		Last Modified: Thu, 15 Apr 2021 08:22:05 GMT  
		Size: 44.6 MB (44634519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d035de95c553cb3f7613ba60b02fbdef7bd797abc283c6f50c0d6e9cc4c98816`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71254d8296a59ad61bd4ad74ff217b2c47ed1a5cdd1b76e68021626df65bdd57`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168537d99c9d6d4daa6bc6ed86109da65add907c96c77c2e34eee0e0a42edccb`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d66e70ca1fcef2fdccee60836c00ebb782d33fc344be33f26cea26cb56b7d20`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0d8f2e63bb260ced0b1c2fde1f39c5b7c65e177825c5f5d50d99cbccc16e24`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000a6a235692a3416c03c800f989cfb587885d6703b14fac566e1d99cb13226e`  
		Last Modified: Thu, 15 Apr 2021 08:22:38 GMT  
		Size: 90.8 MB (90802510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8955ad239f51ee3c4b20437a4d49828decee2ddec1dd66b42927d14032ebdb86`  
		Last Modified: Thu, 15 Apr 2021 08:22:17 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.8.2-slim`

```console
$ docker pull znc@sha256:5515dc9456b053f1ae3f00ff7d6426f231fdd145cd0888e2ce20df3372b87dbb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8.2-slim` - linux; amd64

```console
$ docker pull znc@sha256:7c20dea07cb246d3bee4c887ccbd5a3affd84810f2fc65edb9e2e284681ac339
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47593655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65fb140272cb5e4984ce9eac1a9086ce06ccc5c5b7d6eb1b0cf43cb40507f152`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 08:49:29 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 15 Apr 2021 08:49:29 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 15 Apr 2021 08:49:29 GMT
ARG MAKEFLAGS=
# Thu, 15 Apr 2021 08:49:29 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 15 Apr 2021 08:53:11 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 15 Apr 2021 08:53:11 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 15 Apr 2021 08:53:11 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:53:12 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:53:12 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 15 Apr 2021 08:53:12 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:53:12 GMT
VOLUME [/znc-data]
# Thu, 15 Apr 2021 08:53:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb2e5913ac4c145e00a1896b6ca33dd769f1ae89d094e1036fea9158e697255`  
		Last Modified: Thu, 15 Apr 2021 08:53:56 GMT  
		Size: 44.8 MB (44791665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5baa3714b7588148fea833496685a7c3ae7f7594155bccfbce829a2dcc181bab`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9df6d19694e9b31214bcb2e58eff4ec7c1edf95604c4bc082ce254cabc8f376`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 303.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7461218a0b487e65c95477eb8af45c79a19f76a36c2849efbc880fad8f09bd8`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01964acb966afc4e11e5072b630ce334c9a3755fc140c33ea7794295940a6de`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3925cb8dc6060e3a0ed0da6f992cbe4968b1da9fdce9748a194d87292e0e30d0`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8.2-slim` - linux; arm variant v6

```console
$ docker pull znc@sha256:9b761b1992bdda212d16af7b3b2d0d468764d161c88035178ac474f7537a0eb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45654386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d2ff69e5ce11a914848b667be0bf0a31b595738cc67565d230d38f15915d641`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:06:24 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Wed, 14 Apr 2021 19:06:25 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Wed, 14 Apr 2021 19:06:26 GMT
ARG MAKEFLAGS=
# Wed, 14 Apr 2021 19:06:27 GMT
ENV ZNC_VERSION=1.8.2
# Wed, 14 Apr 2021 19:14:38 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Wed, 14 Apr 2021 19:14:40 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Wed, 14 Apr 2021 19:14:41 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Wed, 14 Apr 2021 19:14:42 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Wed, 14 Apr 2021 19:14:43 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Wed, 14 Apr 2021 19:14:44 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Wed, 14 Apr 2021 19:14:45 GMT
VOLUME [/znc-data]
# Wed, 14 Apr 2021 19:14:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a7c2bb5435b1fa5a12ae177d982fedb637c06223b2c701cb90ecd09de64929`  
		Last Modified: Wed, 14 Apr 2021 19:15:45 GMT  
		Size: 43.0 MB (43047705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174b893fee9110b0d361ce6ac762b55def7e783e102df78cfa7de76273c474c2`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cd01900ad296ad09f6b29dc0dbf821432761b6b9771daddbe9077e2ac7bede`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4852ba58f3351dc50f648ff54754f3143c4bc73aff353c8fc44f1ca4b2727e1b`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e2bd3ffa516127012f7dd673a572cff0cc0b3a53555d987507a3f0e697e70d`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc133d3eda0b1cbf3ee429aa42a8babe168097f3490aff7e11bf216e2200ff9`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8.2-slim` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:8502fe47bdebeb45769bb56cf91662c958cd676886e9f035121b775585038af6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.3 MB (47346641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:802414287d6aab3ba0157371e0a749c55d2a4e90e4b65367b3a170ad1ab6b71f`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 08:12:40 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 15 Apr 2021 08:12:41 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 15 Apr 2021 08:12:43 GMT
ARG MAKEFLAGS=
# Thu, 15 Apr 2021 08:12:44 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 15 Apr 2021 08:21:02 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 15 Apr 2021 08:21:03 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 15 Apr 2021 08:21:05 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:21:06 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:21:07 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 15 Apr 2021 08:21:08 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:21:09 GMT
VOLUME [/znc-data]
# Thu, 15 Apr 2021 08:21:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b3d8e65d0874b1cc53dbb44a2e82d655e8190289913fab876cd4a5b436bcf1`  
		Last Modified: Thu, 15 Apr 2021 08:22:05 GMT  
		Size: 44.6 MB (44634519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d035de95c553cb3f7613ba60b02fbdef7bd797abc283c6f50c0d6e9cc4c98816`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71254d8296a59ad61bd4ad74ff217b2c47ed1a5cdd1b76e68021626df65bdd57`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168537d99c9d6d4daa6bc6ed86109da65add907c96c77c2e34eee0e0a42edccb`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d66e70ca1fcef2fdccee60836c00ebb782d33fc344be33f26cea26cb56b7d20`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0d8f2e63bb260ced0b1c2fde1f39c5b7c65e177825c5f5d50d99cbccc16e24`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.8-slim`

```console
$ docker pull znc@sha256:5515dc9456b053f1ae3f00ff7d6426f231fdd145cd0888e2ce20df3372b87dbb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8-slim` - linux; amd64

```console
$ docker pull znc@sha256:7c20dea07cb246d3bee4c887ccbd5a3affd84810f2fc65edb9e2e284681ac339
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47593655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65fb140272cb5e4984ce9eac1a9086ce06ccc5c5b7d6eb1b0cf43cb40507f152`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 08:49:29 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 15 Apr 2021 08:49:29 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 15 Apr 2021 08:49:29 GMT
ARG MAKEFLAGS=
# Thu, 15 Apr 2021 08:49:29 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 15 Apr 2021 08:53:11 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 15 Apr 2021 08:53:11 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 15 Apr 2021 08:53:11 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:53:12 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:53:12 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 15 Apr 2021 08:53:12 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:53:12 GMT
VOLUME [/znc-data]
# Thu, 15 Apr 2021 08:53:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb2e5913ac4c145e00a1896b6ca33dd769f1ae89d094e1036fea9158e697255`  
		Last Modified: Thu, 15 Apr 2021 08:53:56 GMT  
		Size: 44.8 MB (44791665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5baa3714b7588148fea833496685a7c3ae7f7594155bccfbce829a2dcc181bab`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9df6d19694e9b31214bcb2e58eff4ec7c1edf95604c4bc082ce254cabc8f376`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 303.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7461218a0b487e65c95477eb8af45c79a19f76a36c2849efbc880fad8f09bd8`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01964acb966afc4e11e5072b630ce334c9a3755fc140c33ea7794295940a6de`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3925cb8dc6060e3a0ed0da6f992cbe4968b1da9fdce9748a194d87292e0e30d0`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8-slim` - linux; arm variant v6

```console
$ docker pull znc@sha256:9b761b1992bdda212d16af7b3b2d0d468764d161c88035178ac474f7537a0eb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45654386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d2ff69e5ce11a914848b667be0bf0a31b595738cc67565d230d38f15915d641`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:06:24 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Wed, 14 Apr 2021 19:06:25 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Wed, 14 Apr 2021 19:06:26 GMT
ARG MAKEFLAGS=
# Wed, 14 Apr 2021 19:06:27 GMT
ENV ZNC_VERSION=1.8.2
# Wed, 14 Apr 2021 19:14:38 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Wed, 14 Apr 2021 19:14:40 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Wed, 14 Apr 2021 19:14:41 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Wed, 14 Apr 2021 19:14:42 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Wed, 14 Apr 2021 19:14:43 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Wed, 14 Apr 2021 19:14:44 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Wed, 14 Apr 2021 19:14:45 GMT
VOLUME [/znc-data]
# Wed, 14 Apr 2021 19:14:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a7c2bb5435b1fa5a12ae177d982fedb637c06223b2c701cb90ecd09de64929`  
		Last Modified: Wed, 14 Apr 2021 19:15:45 GMT  
		Size: 43.0 MB (43047705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174b893fee9110b0d361ce6ac762b55def7e783e102df78cfa7de76273c474c2`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cd01900ad296ad09f6b29dc0dbf821432761b6b9771daddbe9077e2ac7bede`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4852ba58f3351dc50f648ff54754f3143c4bc73aff353c8fc44f1ca4b2727e1b`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e2bd3ffa516127012f7dd673a572cff0cc0b3a53555d987507a3f0e697e70d`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc133d3eda0b1cbf3ee429aa42a8babe168097f3490aff7e11bf216e2200ff9`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8-slim` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:8502fe47bdebeb45769bb56cf91662c958cd676886e9f035121b775585038af6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.3 MB (47346641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:802414287d6aab3ba0157371e0a749c55d2a4e90e4b65367b3a170ad1ab6b71f`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 08:12:40 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 15 Apr 2021 08:12:41 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 15 Apr 2021 08:12:43 GMT
ARG MAKEFLAGS=
# Thu, 15 Apr 2021 08:12:44 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 15 Apr 2021 08:21:02 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 15 Apr 2021 08:21:03 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 15 Apr 2021 08:21:05 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:21:06 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:21:07 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 15 Apr 2021 08:21:08 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:21:09 GMT
VOLUME [/znc-data]
# Thu, 15 Apr 2021 08:21:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b3d8e65d0874b1cc53dbb44a2e82d655e8190289913fab876cd4a5b436bcf1`  
		Last Modified: Thu, 15 Apr 2021 08:22:05 GMT  
		Size: 44.6 MB (44634519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d035de95c553cb3f7613ba60b02fbdef7bd797abc283c6f50c0d6e9cc4c98816`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71254d8296a59ad61bd4ad74ff217b2c47ed1a5cdd1b76e68021626df65bdd57`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168537d99c9d6d4daa6bc6ed86109da65add907c96c77c2e34eee0e0a42edccb`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d66e70ca1fcef2fdccee60836c00ebb782d33fc344be33f26cea26cb56b7d20`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0d8f2e63bb260ced0b1c2fde1f39c5b7c65e177825c5f5d50d99cbccc16e24`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:latest`

```console
$ docker pull znc@sha256:d150a0131945a0703c58a3029c15967564481594cfdfe49ed8b192c2787bc2d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:latest` - linux; amd64

```console
$ docker pull znc@sha256:2b472aa12e1e6df0af93d7d0fbcdc76c43f13b5f25366695d58e5012624fea77
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (150976169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a504340efb3ee87ba29443a5a485e2ef4001245a9c52aeb7abd49e71f9ce7c0f`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 08:49:29 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 15 Apr 2021 08:49:29 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 15 Apr 2021 08:49:29 GMT
ARG MAKEFLAGS=
# Thu, 15 Apr 2021 08:49:29 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 15 Apr 2021 08:53:11 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 15 Apr 2021 08:53:11 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 15 Apr 2021 08:53:11 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:53:12 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:53:12 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 15 Apr 2021 08:53:12 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:53:12 GMT
VOLUME [/znc-data]
# Thu, 15 Apr 2021 08:53:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Apr 2021 08:53:32 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Thu, 15 Apr 2021 08:53:32 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb2e5913ac4c145e00a1896b6ca33dd769f1ae89d094e1036fea9158e697255`  
		Last Modified: Thu, 15 Apr 2021 08:53:56 GMT  
		Size: 44.8 MB (44791665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5baa3714b7588148fea833496685a7c3ae7f7594155bccfbce829a2dcc181bab`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9df6d19694e9b31214bcb2e58eff4ec7c1edf95604c4bc082ce254cabc8f376`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 303.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7461218a0b487e65c95477eb8af45c79a19f76a36c2849efbc880fad8f09bd8`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01964acb966afc4e11e5072b630ce334c9a3755fc140c33ea7794295940a6de`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3925cb8dc6060e3a0ed0da6f992cbe4968b1da9fdce9748a194d87292e0e30d0`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be684e19e6c893922d2bda3ce925dcd04b60b7bfd9b23b0b353a749989ea762a`  
		Last Modified: Thu, 15 Apr 2021 08:54:27 GMT  
		Size: 103.4 MB (103382183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a13707e68ab73cd2b6ca6fb7f5e20034a14f59f8b138f5dded3a47b0b25015`  
		Last Modified: Thu, 15 Apr 2021 08:54:10 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:latest` - linux; arm variant v6

```console
$ docker pull znc@sha256:637262cf7726596493c9e1b36319cadee4df531ad169e2ab193bfa5c793c606a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.7 MB (132687454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db254ececf401d0f7db47f515c435b080eeccf382db2085cedd9b4df8336259c`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:06:24 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Wed, 14 Apr 2021 19:06:25 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Wed, 14 Apr 2021 19:06:26 GMT
ARG MAKEFLAGS=
# Wed, 14 Apr 2021 19:06:27 GMT
ENV ZNC_VERSION=1.8.2
# Wed, 14 Apr 2021 19:14:38 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Wed, 14 Apr 2021 19:14:40 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Wed, 14 Apr 2021 19:14:41 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Wed, 14 Apr 2021 19:14:42 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Wed, 14 Apr 2021 19:14:43 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Wed, 14 Apr 2021 19:14:44 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Wed, 14 Apr 2021 19:14:45 GMT
VOLUME [/znc-data]
# Wed, 14 Apr 2021 19:14:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 19:15:07 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Wed, 14 Apr 2021 19:15:10 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a7c2bb5435b1fa5a12ae177d982fedb637c06223b2c701cb90ecd09de64929`  
		Last Modified: Wed, 14 Apr 2021 19:15:45 GMT  
		Size: 43.0 MB (43047705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174b893fee9110b0d361ce6ac762b55def7e783e102df78cfa7de76273c474c2`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cd01900ad296ad09f6b29dc0dbf821432761b6b9771daddbe9077e2ac7bede`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4852ba58f3351dc50f648ff54754f3143c4bc73aff353c8fc44f1ca4b2727e1b`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e2bd3ffa516127012f7dd673a572cff0cc0b3a53555d987507a3f0e697e70d`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc133d3eda0b1cbf3ee429aa42a8babe168097f3490aff7e11bf216e2200ff9`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6f9dc0fc71449c9d6aa086257cdeeccd8c2b27bc1d0912041ec74b9acd1e76`  
		Last Modified: Wed, 14 Apr 2021 19:16:23 GMT  
		Size: 87.0 MB (87032736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773f8f7b9621c6f9898eccd6e54c2229ef68db2240332907412d1c0e7a7bb167`  
		Last Modified: Wed, 14 Apr 2021 19:15:56 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:latest` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:29d98eabc792795f96284e8e5035370c2050827723614beadc05c997c3bd70b1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.1 MB (138149484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6989fa92e7955f83225a6b4c06e8424a0423ac758dbe6fd3b746d6d5e2e2b722`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 08:12:40 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 15 Apr 2021 08:12:41 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 15 Apr 2021 08:12:43 GMT
ARG MAKEFLAGS=
# Thu, 15 Apr 2021 08:12:44 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 15 Apr 2021 08:21:02 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 15 Apr 2021 08:21:03 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 15 Apr 2021 08:21:05 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:21:06 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:21:07 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 15 Apr 2021 08:21:08 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:21:09 GMT
VOLUME [/znc-data]
# Thu, 15 Apr 2021 08:21:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Apr 2021 08:21:32 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Thu, 15 Apr 2021 08:21:34 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b3d8e65d0874b1cc53dbb44a2e82d655e8190289913fab876cd4a5b436bcf1`  
		Last Modified: Thu, 15 Apr 2021 08:22:05 GMT  
		Size: 44.6 MB (44634519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d035de95c553cb3f7613ba60b02fbdef7bd797abc283c6f50c0d6e9cc4c98816`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71254d8296a59ad61bd4ad74ff217b2c47ed1a5cdd1b76e68021626df65bdd57`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168537d99c9d6d4daa6bc6ed86109da65add907c96c77c2e34eee0e0a42edccb`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d66e70ca1fcef2fdccee60836c00ebb782d33fc344be33f26cea26cb56b7d20`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0d8f2e63bb260ced0b1c2fde1f39c5b7c65e177825c5f5d50d99cbccc16e24`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000a6a235692a3416c03c800f989cfb587885d6703b14fac566e1d99cb13226e`  
		Last Modified: Thu, 15 Apr 2021 08:22:38 GMT  
		Size: 90.8 MB (90802510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8955ad239f51ee3c4b20437a4d49828decee2ddec1dd66b42927d14032ebdb86`  
		Last Modified: Thu, 15 Apr 2021 08:22:17 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:slim`

```console
$ docker pull znc@sha256:5515dc9456b053f1ae3f00ff7d6426f231fdd145cd0888e2ce20df3372b87dbb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:slim` - linux; amd64

```console
$ docker pull znc@sha256:7c20dea07cb246d3bee4c887ccbd5a3affd84810f2fc65edb9e2e284681ac339
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47593655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65fb140272cb5e4984ce9eac1a9086ce06ccc5c5b7d6eb1b0cf43cb40507f152`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 08:49:29 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 15 Apr 2021 08:49:29 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 15 Apr 2021 08:49:29 GMT
ARG MAKEFLAGS=
# Thu, 15 Apr 2021 08:49:29 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 15 Apr 2021 08:53:11 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 15 Apr 2021 08:53:11 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 15 Apr 2021 08:53:11 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:53:12 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:53:12 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 15 Apr 2021 08:53:12 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:53:12 GMT
VOLUME [/znc-data]
# Thu, 15 Apr 2021 08:53:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb2e5913ac4c145e00a1896b6ca33dd769f1ae89d094e1036fea9158e697255`  
		Last Modified: Thu, 15 Apr 2021 08:53:56 GMT  
		Size: 44.8 MB (44791665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5baa3714b7588148fea833496685a7c3ae7f7594155bccfbce829a2dcc181bab`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9df6d19694e9b31214bcb2e58eff4ec7c1edf95604c4bc082ce254cabc8f376`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 303.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7461218a0b487e65c95477eb8af45c79a19f76a36c2849efbc880fad8f09bd8`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01964acb966afc4e11e5072b630ce334c9a3755fc140c33ea7794295940a6de`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3925cb8dc6060e3a0ed0da6f992cbe4968b1da9fdce9748a194d87292e0e30d0`  
		Last Modified: Thu, 15 Apr 2021 08:53:45 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:slim` - linux; arm variant v6

```console
$ docker pull znc@sha256:9b761b1992bdda212d16af7b3b2d0d468764d161c88035178ac474f7537a0eb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45654386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d2ff69e5ce11a914848b667be0bf0a31b595738cc67565d230d38f15915d641`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:06:24 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Wed, 14 Apr 2021 19:06:25 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Wed, 14 Apr 2021 19:06:26 GMT
ARG MAKEFLAGS=
# Wed, 14 Apr 2021 19:06:27 GMT
ENV ZNC_VERSION=1.8.2
# Wed, 14 Apr 2021 19:14:38 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Wed, 14 Apr 2021 19:14:40 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Wed, 14 Apr 2021 19:14:41 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Wed, 14 Apr 2021 19:14:42 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Wed, 14 Apr 2021 19:14:43 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Wed, 14 Apr 2021 19:14:44 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Wed, 14 Apr 2021 19:14:45 GMT
VOLUME [/znc-data]
# Wed, 14 Apr 2021 19:14:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a7c2bb5435b1fa5a12ae177d982fedb637c06223b2c701cb90ecd09de64929`  
		Last Modified: Wed, 14 Apr 2021 19:15:45 GMT  
		Size: 43.0 MB (43047705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174b893fee9110b0d361ce6ac762b55def7e783e102df78cfa7de76273c474c2`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cd01900ad296ad09f6b29dc0dbf821432761b6b9771daddbe9077e2ac7bede`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4852ba58f3351dc50f648ff54754f3143c4bc73aff353c8fc44f1ca4b2727e1b`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e2bd3ffa516127012f7dd673a572cff0cc0b3a53555d987507a3f0e697e70d`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc133d3eda0b1cbf3ee429aa42a8babe168097f3490aff7e11bf216e2200ff9`  
		Last Modified: Wed, 14 Apr 2021 19:15:28 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:slim` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:8502fe47bdebeb45769bb56cf91662c958cd676886e9f035121b775585038af6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.3 MB (47346641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:802414287d6aab3ba0157371e0a749c55d2a4e90e4b65367b3a170ad1ab6b71f`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 08:12:40 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 15 Apr 2021 08:12:41 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 15 Apr 2021 08:12:43 GMT
ARG MAKEFLAGS=
# Thu, 15 Apr 2021 08:12:44 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 15 Apr 2021 08:21:02 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 15 Apr 2021 08:21:03 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 15 Apr 2021 08:21:05 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:21:06 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:21:07 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 15 Apr 2021 08:21:08 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 15 Apr 2021 08:21:09 GMT
VOLUME [/znc-data]
# Thu, 15 Apr 2021 08:21:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b3d8e65d0874b1cc53dbb44a2e82d655e8190289913fab876cd4a5b436bcf1`  
		Last Modified: Thu, 15 Apr 2021 08:22:05 GMT  
		Size: 44.6 MB (44634519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d035de95c553cb3f7613ba60b02fbdef7bd797abc283c6f50c0d6e9cc4c98816`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71254d8296a59ad61bd4ad74ff217b2c47ed1a5cdd1b76e68021626df65bdd57`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168537d99c9d6d4daa6bc6ed86109da65add907c96c77c2e34eee0e0a42edccb`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d66e70ca1fcef2fdccee60836c00ebb782d33fc344be33f26cea26cb56b7d20`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0d8f2e63bb260ced0b1c2fde1f39c5b7c65e177825c5f5d50d99cbccc16e24`  
		Last Modified: Thu, 15 Apr 2021 08:21:51 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
