## `znc:latest`

```console
$ docker pull znc@sha256:567140da1342b13427a78d2b4acf86eb7148259c7374939e3ee08bde3be8f366
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:latest` - linux; amd64

```console
$ docker pull znc@sha256:f39e663707ac914f5d268c94debe0aafca48463433ca81f46749a00f6217d2f3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.1 MB (151128570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a3686951e6b39e68a291c0b4b83a72a2ea4970e181b1c1bf06fbe9a98e9e0d7`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Wed, 09 Sep 2020 00:19:23 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Wed, 09 Sep 2020 00:19:23 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Wed, 09 Sep 2020 00:19:23 GMT
ARG MAKEFLAGS=
# Wed, 09 Sep 2020 00:19:23 GMT
ENV ZNC_VERSION=1.8.2
# Wed, 09 Sep 2020 00:23:42 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Wed, 09 Sep 2020 00:23:42 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Wed, 09 Sep 2020 00:23:42 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Wed, 09 Sep 2020 00:23:42 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Wed, 09 Sep 2020 00:23:43 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Wed, 09 Sep 2020 00:23:43 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Wed, 09 Sep 2020 00:23:43 GMT
VOLUME [/znc-data]
# Wed, 09 Sep 2020 00:23:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Sep 2020 00:24:03 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Wed, 09 Sep 2020 00:24:03 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03cbd9e5076625b6bc9c281d96c12c30b447add2ba1be651ae0ae4a6a5a4a068`  
		Last Modified: Wed, 09 Sep 2020 00:24:20 GMT  
		Size: 45.0 MB (44954895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e9d6d7bb84742dc473e3a84f3a72eebb081a75d63147b05079e96d82f010aea`  
		Last Modified: Wed, 09 Sep 2020 00:24:11 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3e859a427884566b791a46ba46e263a8dccde6ca27dad0b2c83b0bb3e5a839`  
		Last Modified: Wed, 09 Sep 2020 00:24:12 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0bcd676ed587c65b67a1051e826d026ca96fee08eb817754575eb8614409602`  
		Last Modified: Wed, 09 Sep 2020 00:24:11 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aeda33c4af5d65f0bc4d726c760c724a9a28c764ce062522c27955c7142b523`  
		Last Modified: Wed, 09 Sep 2020 00:24:11 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cb2060dcdbc5a1850562b19ffed28ba2b8b5cf05214bb524f6b4aae76704eb`  
		Last Modified: Wed, 09 Sep 2020 00:24:11 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ffcda97f1ef96bde0bf637b63f0e5da95e93845173282123e724f39596f6de`  
		Last Modified: Wed, 09 Sep 2020 00:24:43 GMT  
		Size: 103.4 MB (103374405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9964ec853c8fa0fff14d98f13d57074554d92e59e1f6532e52a09a5a5ee5ac`  
		Last Modified: Wed, 09 Sep 2020 00:24:25 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:latest` - linux; arm variant v6

```console
$ docker pull znc@sha256:47740b4e5a6c020aada41ac19c1931c360b7d129267b271ce5f06d67b426e831
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.8 MB (132809194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed893f3b3eb5611fc653b2c70c796c00e2190e482db23d758ce36325b39c39f0`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Tue, 08 Sep 2020 22:04:03 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 08 Sep 2020 22:04:10 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 08 Sep 2020 22:04:19 GMT
ARG MAKEFLAGS=
# Tue, 08 Sep 2020 22:04:27 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 08 Sep 2020 22:13:28 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 08 Sep 2020 22:13:41 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 08 Sep 2020 22:13:57 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Tue, 08 Sep 2020 22:14:11 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Tue, 08 Sep 2020 22:14:25 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Tue, 08 Sep 2020 22:14:40 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Tue, 08 Sep 2020 22:14:51 GMT
VOLUME [/znc-data]
# Tue, 08 Sep 2020 22:15:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Sep 2020 22:16:05 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Tue, 08 Sep 2020 22:16:20 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82217ea964091f8c190214bd997420f9132e906b89fed351d36269f6152d586e`  
		Last Modified: Tue, 08 Sep 2020 22:16:54 GMT  
		Size: 43.2 MB (43184125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8954ac8421360fdd845e73456cca768d6e6063c0a97b158edecdd95f999965b7`  
		Last Modified: Tue, 08 Sep 2020 22:16:39 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523acf9284a5c22a3148b30bdca3b5c4f5fe55e1ae8586a8e282235cc56a4f7c`  
		Last Modified: Tue, 08 Sep 2020 22:16:39 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aba0fda97135a4280a08db5555814f2b04ae0ffc032f48d47b47a98d6783c15`  
		Last Modified: Tue, 08 Sep 2020 22:16:39 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd444df6d3a77099159e06342ba5bca06b8dca6d054d79165cabbfa044b5c7f`  
		Last Modified: Tue, 08 Sep 2020 22:16:39 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766280c07d141fab7909b7e07cbd0a3373166a404354be8fdb200285c9a813d4`  
		Last Modified: Tue, 08 Sep 2020 22:16:39 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275a81cb106f91a9cc396b3ff0d4d472115391735da996d949d4e960100219c8`  
		Last Modified: Tue, 08 Sep 2020 22:17:34 GMT  
		Size: 87.0 MB (87020019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f02b101b1cfe888ef641b0875361f3640ac62ce395366cb86645a78c69e6a7`  
		Last Modified: Tue, 08 Sep 2020 22:17:07 GMT  
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
