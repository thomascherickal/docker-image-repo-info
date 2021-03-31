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
$ docker pull znc@sha256:8e87441cd12b57fc0f3c2b4febef884e56f28c76670a6b440c55c940cac7c20f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8` - linux; amd64

```console
$ docker pull znc@sha256:06f36fd86b43a8e7734f8170934e9d4fa5bbc6a94ce90f965882edf9f6f0f20d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (150968904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c803978ff1716d522e2dbb48cf667a2933030683dec6170898f8ea135ffb72e`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:49:36 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Fri, 26 Mar 2021 02:49:37 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Fri, 26 Mar 2021 02:49:37 GMT
ARG MAKEFLAGS=
# Fri, 26 Mar 2021 02:49:37 GMT
ENV ZNC_VERSION=1.8.2
# Fri, 26 Mar 2021 02:55:28 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Fri, 26 Mar 2021 02:55:28 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Fri, 26 Mar 2021 02:55:28 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Fri, 26 Mar 2021 02:55:29 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Fri, 26 Mar 2021 02:55:29 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Fri, 26 Mar 2021 02:55:29 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Fri, 26 Mar 2021 02:55:29 GMT
VOLUME [/znc-data]
# Fri, 26 Mar 2021 02:55:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 02:55:39 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Fri, 26 Mar 2021 02:55:39 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef753c00beaf06a3ee7647f2da37af968d3c33b9655927a8d6aca2d1d995e28c`  
		Last Modified: Fri, 26 Mar 2021 02:56:04 GMT  
		Size: 44.8 MB (44790585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9739f8a41ed5c01a8660fa107743ba3fb79709cdf9fd584ea4298252afa54a14`  
		Last Modified: Fri, 26 Mar 2021 02:55:52 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f021d06d531c1dbf7b87991e227094bb17ed380b2aeac36c819c64fad6cf9cc`  
		Last Modified: Fri, 26 Mar 2021 02:55:53 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db01e30df5558a3c24faf6d409e32758133a06c2e2145417d83e1cbeb3e4aee`  
		Last Modified: Fri, 26 Mar 2021 02:55:52 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afac7b001b7aa8a0b0dbd7c72ca4b057cf50099234a4751ab06b4e33b5a17f10`  
		Last Modified: Fri, 26 Mar 2021 02:55:52 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee18e3181ce87afeaaadc596532013194e9cc8132f0c58f8d235f7f9295e734`  
		Last Modified: Fri, 26 Mar 2021 02:55:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7585d98d7ae0ca7844e2d481de40ee8bfee40e04d9afa6d3c57a664165d40cc0`  
		Last Modified: Fri, 26 Mar 2021 02:56:35 GMT  
		Size: 103.4 MB (103376800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3bd687d2611b904fa018ddbec55747e33a4ef0747e568c2976c11c595859cc`  
		Last Modified: Fri, 26 Mar 2021 02:56:17 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8` - linux; arm variant v6

```console
$ docker pull znc@sha256:ddfe1fadb406db1a004fd488cfa47e05b22955988f435694c59ed8d77d27b92a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.7 MB (132673455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a143fe9f167782342008d41db959f61417cefaa723821899dc578a2dffb49d7`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 17:42:11 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Wed, 31 Mar 2021 17:42:11 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Wed, 31 Mar 2021 17:42:12 GMT
ARG MAKEFLAGS=
# Wed, 31 Mar 2021 17:42:13 GMT
ENV ZNC_VERSION=1.8.2
# Wed, 31 Mar 2021 17:50:40 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Wed, 31 Mar 2021 17:50:42 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Wed, 31 Mar 2021 17:50:44 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Wed, 31 Mar 2021 17:50:45 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Wed, 31 Mar 2021 17:50:46 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Wed, 31 Mar 2021 17:50:48 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Wed, 31 Mar 2021 17:50:50 GMT
VOLUME [/znc-data]
# Wed, 31 Mar 2021 17:50:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 17:51:26 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Wed, 31 Mar 2021 17:51:32 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3886333d907bad3825a1872f1dbbf1c596896930531994f4e86cb28dc6fceb`  
		Last Modified: Wed, 31 Mar 2021 17:52:08 GMT  
		Size: 43.0 MB (43047554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7c0b696ec30f6f96326d09b075904580a56314f80f8f15c22f3397f0f810e8`  
		Last Modified: Wed, 31 Mar 2021 17:51:49 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59da53be9c7202b665f6fd3eea5a7c06f3ca767a7dece9a6c1092194822b3909`  
		Last Modified: Wed, 31 Mar 2021 17:51:50 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef8b9c711055b45c44d93df2261200fd9bbdb82408ed9dc6f026c5e0710f676`  
		Last Modified: Wed, 31 Mar 2021 17:51:48 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03332397d4ff777be8babfbcb868c559cfd0af48c32d76b938831b58de40dc21`  
		Last Modified: Wed, 31 Mar 2021 17:51:48 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42892a8210a35ab55795ec9e555d8ba18c17480ee1129833d4d31f42b50d3bf2`  
		Last Modified: Wed, 31 Mar 2021 17:51:48 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff41a0b34e55fd23b33184337e9fd3644cbd0bfa22bf94d1dea99c83c16d8cb`  
		Last Modified: Wed, 31 Mar 2021 17:52:48 GMT  
		Size: 87.0 MB (87019485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a571a5e7d8add8b875bc4c7a372a14b3fad2ed1053925c76ac9cfe9dc8dfb5`  
		Last Modified: Wed, 31 Mar 2021 17:52:21 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:867d8008e3c661f2f36ae5de43c0d8761c09394f6efa432fb9755f41388ad2de
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.1 MB (138119258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae9dbdb0d56d42b79e772164b24015a6b6eb5f3df3a9d7c74e803e51ce2f1f2e`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:00 GMT
ADD file:97aac29a9ffbba2c76441891035010395614dc3115c4710d58932205b604308f in / 
# Thu, 25 Mar 2021 22:41:10 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 08:50:00 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Fri, 26 Mar 2021 08:50:01 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Fri, 26 Mar 2021 08:50:01 GMT
ARG MAKEFLAGS=
# Fri, 26 Mar 2021 08:50:02 GMT
ENV ZNC_VERSION=1.8.2
# Fri, 26 Mar 2021 08:58:39 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Fri, 26 Mar 2021 08:58:40 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Fri, 26 Mar 2021 08:58:41 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Fri, 26 Mar 2021 08:58:43 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Fri, 26 Mar 2021 08:58:44 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Fri, 26 Mar 2021 08:58:45 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Fri, 26 Mar 2021 08:58:46 GMT
VOLUME [/znc-data]
# Fri, 26 Mar 2021 08:58:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 08:59:09 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Fri, 26 Mar 2021 08:59:12 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:95dec6db372224fc1909f0d0c0a9a9d5767ec6b78d066ff6a7d5723160037828`  
		Last Modified: Thu, 25 Mar 2021 22:45:23 GMT  
		Size: 2.7 MB (2709692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261b1493d1cb2458295caac1ef25dd52633a9918efc444ba17cc51219d26a8d9`  
		Last Modified: Fri, 26 Mar 2021 08:59:40 GMT  
		Size: 44.6 MB (44634463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2281c6206ad9e01aeba3f087c93c093edf03b65b013c1e5f30f1c1cc74e9d4d`  
		Last Modified: Fri, 26 Mar 2021 08:59:27 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6757db4ee2933909c092344b92ea6da1ae5f0cb9dc22909417c149a6c7230e6`  
		Last Modified: Fri, 26 Mar 2021 08:59:27 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1812d97bc4f8773fb4157ee1040400c92ba44a0f4cb42ee1d3968738f711d30`  
		Last Modified: Fri, 26 Mar 2021 08:59:26 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083ed828033ac4f4536b200687724afd662cadc3cadab7be191836076e23b0a8`  
		Last Modified: Fri, 26 Mar 2021 08:59:26 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5351579885da0be0c3e00c76b547db0e55bdeeba9d93a2a5bc221e79e44d1cdb`  
		Last Modified: Fri, 26 Mar 2021 08:59:26 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2c89f681197b95d37c9eca50392af5784da5bba01a0b5b061626be357271a1`  
		Last Modified: Fri, 26 Mar 2021 09:00:18 GMT  
		Size: 90.8 MB (90773349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6446c82cbc42091f0d17d84181f2a84c5a3c8a6fbba3169b39554bb92d3241`  
		Last Modified: Fri, 26 Mar 2021 08:59:52 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.8-slim`

```console
$ docker pull znc@sha256:8dce50f00d936dc872148c4a981cf34116f85bfbd433fb6778627e13b13bedaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8-slim` - linux; amd64

```console
$ docker pull znc@sha256:4303ffe84845e4386c18f084a7100f391b9e71311400d623391d17e7195ddb29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47591773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01f27eae3fac4ef84586b44f4ca6e780dafaae50dbe4bf6c460ec7125dedcdf3`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:49:36 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Fri, 26 Mar 2021 02:49:37 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Fri, 26 Mar 2021 02:49:37 GMT
ARG MAKEFLAGS=
# Fri, 26 Mar 2021 02:49:37 GMT
ENV ZNC_VERSION=1.8.2
# Fri, 26 Mar 2021 02:55:28 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Fri, 26 Mar 2021 02:55:28 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Fri, 26 Mar 2021 02:55:28 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Fri, 26 Mar 2021 02:55:29 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Fri, 26 Mar 2021 02:55:29 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Fri, 26 Mar 2021 02:55:29 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Fri, 26 Mar 2021 02:55:29 GMT
VOLUME [/znc-data]
# Fri, 26 Mar 2021 02:55:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef753c00beaf06a3ee7647f2da37af968d3c33b9655927a8d6aca2d1d995e28c`  
		Last Modified: Fri, 26 Mar 2021 02:56:04 GMT  
		Size: 44.8 MB (44790585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9739f8a41ed5c01a8660fa107743ba3fb79709cdf9fd584ea4298252afa54a14`  
		Last Modified: Fri, 26 Mar 2021 02:55:52 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f021d06d531c1dbf7b87991e227094bb17ed380b2aeac36c819c64fad6cf9cc`  
		Last Modified: Fri, 26 Mar 2021 02:55:53 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db01e30df5558a3c24faf6d409e32758133a06c2e2145417d83e1cbeb3e4aee`  
		Last Modified: Fri, 26 Mar 2021 02:55:52 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afac7b001b7aa8a0b0dbd7c72ca4b057cf50099234a4751ab06b4e33b5a17f10`  
		Last Modified: Fri, 26 Mar 2021 02:55:52 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee18e3181ce87afeaaadc596532013194e9cc8132f0c58f8d235f7f9295e734`  
		Last Modified: Fri, 26 Mar 2021 02:55:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8-slim` - linux; arm variant v6

```console
$ docker pull znc@sha256:2a68259503ed3ebd996393ec515c599f698c273ca940409118ede2f1fc74994a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45653638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5e52705c8ce39b70c2d5c380db1f9ff6798526b9d1687c361dfe68e148217fe`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 17:42:11 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Wed, 31 Mar 2021 17:42:11 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Wed, 31 Mar 2021 17:42:12 GMT
ARG MAKEFLAGS=
# Wed, 31 Mar 2021 17:42:13 GMT
ENV ZNC_VERSION=1.8.2
# Wed, 31 Mar 2021 17:50:40 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Wed, 31 Mar 2021 17:50:42 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Wed, 31 Mar 2021 17:50:44 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Wed, 31 Mar 2021 17:50:45 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Wed, 31 Mar 2021 17:50:46 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Wed, 31 Mar 2021 17:50:48 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Wed, 31 Mar 2021 17:50:50 GMT
VOLUME [/znc-data]
# Wed, 31 Mar 2021 17:50:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3886333d907bad3825a1872f1dbbf1c596896930531994f4e86cb28dc6fceb`  
		Last Modified: Wed, 31 Mar 2021 17:52:08 GMT  
		Size: 43.0 MB (43047554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7c0b696ec30f6f96326d09b075904580a56314f80f8f15c22f3397f0f810e8`  
		Last Modified: Wed, 31 Mar 2021 17:51:49 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59da53be9c7202b665f6fd3eea5a7c06f3ca767a7dece9a6c1092194822b3909`  
		Last Modified: Wed, 31 Mar 2021 17:51:50 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef8b9c711055b45c44d93df2261200fd9bbdb82408ed9dc6f026c5e0710f676`  
		Last Modified: Wed, 31 Mar 2021 17:51:48 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03332397d4ff777be8babfbcb868c559cfd0af48c32d76b938831b58de40dc21`  
		Last Modified: Wed, 31 Mar 2021 17:51:48 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42892a8210a35ab55795ec9e555d8ba18c17480ee1129833d4d31f42b50d3bf2`  
		Last Modified: Wed, 31 Mar 2021 17:51:48 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8-slim` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:b2c8bb3fb1e9afe5258235cc3c9d3f4d6901d1252257dd61ebd2d03621344885
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.3 MB (47345578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a9b88dc147bf333fbb832cb8f42a88497233062db2848c50687f14fe28d1180`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:00 GMT
ADD file:97aac29a9ffbba2c76441891035010395614dc3115c4710d58932205b604308f in / 
# Thu, 25 Mar 2021 22:41:10 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 08:50:00 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Fri, 26 Mar 2021 08:50:01 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Fri, 26 Mar 2021 08:50:01 GMT
ARG MAKEFLAGS=
# Fri, 26 Mar 2021 08:50:02 GMT
ENV ZNC_VERSION=1.8.2
# Fri, 26 Mar 2021 08:58:39 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Fri, 26 Mar 2021 08:58:40 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Fri, 26 Mar 2021 08:58:41 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Fri, 26 Mar 2021 08:58:43 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Fri, 26 Mar 2021 08:58:44 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Fri, 26 Mar 2021 08:58:45 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Fri, 26 Mar 2021 08:58:46 GMT
VOLUME [/znc-data]
# Fri, 26 Mar 2021 08:58:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:95dec6db372224fc1909f0d0c0a9a9d5767ec6b78d066ff6a7d5723160037828`  
		Last Modified: Thu, 25 Mar 2021 22:45:23 GMT  
		Size: 2.7 MB (2709692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261b1493d1cb2458295caac1ef25dd52633a9918efc444ba17cc51219d26a8d9`  
		Last Modified: Fri, 26 Mar 2021 08:59:40 GMT  
		Size: 44.6 MB (44634463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2281c6206ad9e01aeba3f087c93c093edf03b65b013c1e5f30f1c1cc74e9d4d`  
		Last Modified: Fri, 26 Mar 2021 08:59:27 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6757db4ee2933909c092344b92ea6da1ae5f0cb9dc22909417c149a6c7230e6`  
		Last Modified: Fri, 26 Mar 2021 08:59:27 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1812d97bc4f8773fb4157ee1040400c92ba44a0f4cb42ee1d3968738f711d30`  
		Last Modified: Fri, 26 Mar 2021 08:59:26 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083ed828033ac4f4536b200687724afd662cadc3cadab7be191836076e23b0a8`  
		Last Modified: Fri, 26 Mar 2021 08:59:26 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5351579885da0be0c3e00c76b547db0e55bdeeba9d93a2a5bc221e79e44d1cdb`  
		Last Modified: Fri, 26 Mar 2021 08:59:26 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.8.2`

```console
$ docker pull znc@sha256:8e87441cd12b57fc0f3c2b4febef884e56f28c76670a6b440c55c940cac7c20f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8.2` - linux; amd64

```console
$ docker pull znc@sha256:06f36fd86b43a8e7734f8170934e9d4fa5bbc6a94ce90f965882edf9f6f0f20d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (150968904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c803978ff1716d522e2dbb48cf667a2933030683dec6170898f8ea135ffb72e`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:49:36 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Fri, 26 Mar 2021 02:49:37 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Fri, 26 Mar 2021 02:49:37 GMT
ARG MAKEFLAGS=
# Fri, 26 Mar 2021 02:49:37 GMT
ENV ZNC_VERSION=1.8.2
# Fri, 26 Mar 2021 02:55:28 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Fri, 26 Mar 2021 02:55:28 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Fri, 26 Mar 2021 02:55:28 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Fri, 26 Mar 2021 02:55:29 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Fri, 26 Mar 2021 02:55:29 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Fri, 26 Mar 2021 02:55:29 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Fri, 26 Mar 2021 02:55:29 GMT
VOLUME [/znc-data]
# Fri, 26 Mar 2021 02:55:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 02:55:39 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Fri, 26 Mar 2021 02:55:39 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef753c00beaf06a3ee7647f2da37af968d3c33b9655927a8d6aca2d1d995e28c`  
		Last Modified: Fri, 26 Mar 2021 02:56:04 GMT  
		Size: 44.8 MB (44790585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9739f8a41ed5c01a8660fa107743ba3fb79709cdf9fd584ea4298252afa54a14`  
		Last Modified: Fri, 26 Mar 2021 02:55:52 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f021d06d531c1dbf7b87991e227094bb17ed380b2aeac36c819c64fad6cf9cc`  
		Last Modified: Fri, 26 Mar 2021 02:55:53 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db01e30df5558a3c24faf6d409e32758133a06c2e2145417d83e1cbeb3e4aee`  
		Last Modified: Fri, 26 Mar 2021 02:55:52 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afac7b001b7aa8a0b0dbd7c72ca4b057cf50099234a4751ab06b4e33b5a17f10`  
		Last Modified: Fri, 26 Mar 2021 02:55:52 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee18e3181ce87afeaaadc596532013194e9cc8132f0c58f8d235f7f9295e734`  
		Last Modified: Fri, 26 Mar 2021 02:55:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7585d98d7ae0ca7844e2d481de40ee8bfee40e04d9afa6d3c57a664165d40cc0`  
		Last Modified: Fri, 26 Mar 2021 02:56:35 GMT  
		Size: 103.4 MB (103376800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3bd687d2611b904fa018ddbec55747e33a4ef0747e568c2976c11c595859cc`  
		Last Modified: Fri, 26 Mar 2021 02:56:17 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8.2` - linux; arm variant v6

```console
$ docker pull znc@sha256:ddfe1fadb406db1a004fd488cfa47e05b22955988f435694c59ed8d77d27b92a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.7 MB (132673455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a143fe9f167782342008d41db959f61417cefaa723821899dc578a2dffb49d7`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 17:42:11 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Wed, 31 Mar 2021 17:42:11 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Wed, 31 Mar 2021 17:42:12 GMT
ARG MAKEFLAGS=
# Wed, 31 Mar 2021 17:42:13 GMT
ENV ZNC_VERSION=1.8.2
# Wed, 31 Mar 2021 17:50:40 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Wed, 31 Mar 2021 17:50:42 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Wed, 31 Mar 2021 17:50:44 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Wed, 31 Mar 2021 17:50:45 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Wed, 31 Mar 2021 17:50:46 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Wed, 31 Mar 2021 17:50:48 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Wed, 31 Mar 2021 17:50:50 GMT
VOLUME [/znc-data]
# Wed, 31 Mar 2021 17:50:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 17:51:26 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Wed, 31 Mar 2021 17:51:32 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3886333d907bad3825a1872f1dbbf1c596896930531994f4e86cb28dc6fceb`  
		Last Modified: Wed, 31 Mar 2021 17:52:08 GMT  
		Size: 43.0 MB (43047554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7c0b696ec30f6f96326d09b075904580a56314f80f8f15c22f3397f0f810e8`  
		Last Modified: Wed, 31 Mar 2021 17:51:49 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59da53be9c7202b665f6fd3eea5a7c06f3ca767a7dece9a6c1092194822b3909`  
		Last Modified: Wed, 31 Mar 2021 17:51:50 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef8b9c711055b45c44d93df2261200fd9bbdb82408ed9dc6f026c5e0710f676`  
		Last Modified: Wed, 31 Mar 2021 17:51:48 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03332397d4ff777be8babfbcb868c559cfd0af48c32d76b938831b58de40dc21`  
		Last Modified: Wed, 31 Mar 2021 17:51:48 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42892a8210a35ab55795ec9e555d8ba18c17480ee1129833d4d31f42b50d3bf2`  
		Last Modified: Wed, 31 Mar 2021 17:51:48 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff41a0b34e55fd23b33184337e9fd3644cbd0bfa22bf94d1dea99c83c16d8cb`  
		Last Modified: Wed, 31 Mar 2021 17:52:48 GMT  
		Size: 87.0 MB (87019485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a571a5e7d8add8b875bc4c7a372a14b3fad2ed1053925c76ac9cfe9dc8dfb5`  
		Last Modified: Wed, 31 Mar 2021 17:52:21 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8.2` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:867d8008e3c661f2f36ae5de43c0d8761c09394f6efa432fb9755f41388ad2de
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.1 MB (138119258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae9dbdb0d56d42b79e772164b24015a6b6eb5f3df3a9d7c74e803e51ce2f1f2e`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:00 GMT
ADD file:97aac29a9ffbba2c76441891035010395614dc3115c4710d58932205b604308f in / 
# Thu, 25 Mar 2021 22:41:10 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 08:50:00 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Fri, 26 Mar 2021 08:50:01 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Fri, 26 Mar 2021 08:50:01 GMT
ARG MAKEFLAGS=
# Fri, 26 Mar 2021 08:50:02 GMT
ENV ZNC_VERSION=1.8.2
# Fri, 26 Mar 2021 08:58:39 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Fri, 26 Mar 2021 08:58:40 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Fri, 26 Mar 2021 08:58:41 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Fri, 26 Mar 2021 08:58:43 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Fri, 26 Mar 2021 08:58:44 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Fri, 26 Mar 2021 08:58:45 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Fri, 26 Mar 2021 08:58:46 GMT
VOLUME [/znc-data]
# Fri, 26 Mar 2021 08:58:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 08:59:09 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Fri, 26 Mar 2021 08:59:12 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:95dec6db372224fc1909f0d0c0a9a9d5767ec6b78d066ff6a7d5723160037828`  
		Last Modified: Thu, 25 Mar 2021 22:45:23 GMT  
		Size: 2.7 MB (2709692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261b1493d1cb2458295caac1ef25dd52633a9918efc444ba17cc51219d26a8d9`  
		Last Modified: Fri, 26 Mar 2021 08:59:40 GMT  
		Size: 44.6 MB (44634463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2281c6206ad9e01aeba3f087c93c093edf03b65b013c1e5f30f1c1cc74e9d4d`  
		Last Modified: Fri, 26 Mar 2021 08:59:27 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6757db4ee2933909c092344b92ea6da1ae5f0cb9dc22909417c149a6c7230e6`  
		Last Modified: Fri, 26 Mar 2021 08:59:27 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1812d97bc4f8773fb4157ee1040400c92ba44a0f4cb42ee1d3968738f711d30`  
		Last Modified: Fri, 26 Mar 2021 08:59:26 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083ed828033ac4f4536b200687724afd662cadc3cadab7be191836076e23b0a8`  
		Last Modified: Fri, 26 Mar 2021 08:59:26 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5351579885da0be0c3e00c76b547db0e55bdeeba9d93a2a5bc221e79e44d1cdb`  
		Last Modified: Fri, 26 Mar 2021 08:59:26 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2c89f681197b95d37c9eca50392af5784da5bba01a0b5b061626be357271a1`  
		Last Modified: Fri, 26 Mar 2021 09:00:18 GMT  
		Size: 90.8 MB (90773349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6446c82cbc42091f0d17d84181f2a84c5a3c8a6fbba3169b39554bb92d3241`  
		Last Modified: Fri, 26 Mar 2021 08:59:52 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.8.2-slim`

```console
$ docker pull znc@sha256:8dce50f00d936dc872148c4a981cf34116f85bfbd433fb6778627e13b13bedaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8.2-slim` - linux; amd64

```console
$ docker pull znc@sha256:4303ffe84845e4386c18f084a7100f391b9e71311400d623391d17e7195ddb29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47591773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01f27eae3fac4ef84586b44f4ca6e780dafaae50dbe4bf6c460ec7125dedcdf3`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:49:36 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Fri, 26 Mar 2021 02:49:37 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Fri, 26 Mar 2021 02:49:37 GMT
ARG MAKEFLAGS=
# Fri, 26 Mar 2021 02:49:37 GMT
ENV ZNC_VERSION=1.8.2
# Fri, 26 Mar 2021 02:55:28 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Fri, 26 Mar 2021 02:55:28 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Fri, 26 Mar 2021 02:55:28 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Fri, 26 Mar 2021 02:55:29 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Fri, 26 Mar 2021 02:55:29 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Fri, 26 Mar 2021 02:55:29 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Fri, 26 Mar 2021 02:55:29 GMT
VOLUME [/znc-data]
# Fri, 26 Mar 2021 02:55:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef753c00beaf06a3ee7647f2da37af968d3c33b9655927a8d6aca2d1d995e28c`  
		Last Modified: Fri, 26 Mar 2021 02:56:04 GMT  
		Size: 44.8 MB (44790585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9739f8a41ed5c01a8660fa107743ba3fb79709cdf9fd584ea4298252afa54a14`  
		Last Modified: Fri, 26 Mar 2021 02:55:52 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f021d06d531c1dbf7b87991e227094bb17ed380b2aeac36c819c64fad6cf9cc`  
		Last Modified: Fri, 26 Mar 2021 02:55:53 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db01e30df5558a3c24faf6d409e32758133a06c2e2145417d83e1cbeb3e4aee`  
		Last Modified: Fri, 26 Mar 2021 02:55:52 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afac7b001b7aa8a0b0dbd7c72ca4b057cf50099234a4751ab06b4e33b5a17f10`  
		Last Modified: Fri, 26 Mar 2021 02:55:52 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee18e3181ce87afeaaadc596532013194e9cc8132f0c58f8d235f7f9295e734`  
		Last Modified: Fri, 26 Mar 2021 02:55:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8.2-slim` - linux; arm variant v6

```console
$ docker pull znc@sha256:2a68259503ed3ebd996393ec515c599f698c273ca940409118ede2f1fc74994a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45653638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5e52705c8ce39b70c2d5c380db1f9ff6798526b9d1687c361dfe68e148217fe`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 17:42:11 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Wed, 31 Mar 2021 17:42:11 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Wed, 31 Mar 2021 17:42:12 GMT
ARG MAKEFLAGS=
# Wed, 31 Mar 2021 17:42:13 GMT
ENV ZNC_VERSION=1.8.2
# Wed, 31 Mar 2021 17:50:40 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Wed, 31 Mar 2021 17:50:42 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Wed, 31 Mar 2021 17:50:44 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Wed, 31 Mar 2021 17:50:45 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Wed, 31 Mar 2021 17:50:46 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Wed, 31 Mar 2021 17:50:48 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Wed, 31 Mar 2021 17:50:50 GMT
VOLUME [/znc-data]
# Wed, 31 Mar 2021 17:50:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3886333d907bad3825a1872f1dbbf1c596896930531994f4e86cb28dc6fceb`  
		Last Modified: Wed, 31 Mar 2021 17:52:08 GMT  
		Size: 43.0 MB (43047554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7c0b696ec30f6f96326d09b075904580a56314f80f8f15c22f3397f0f810e8`  
		Last Modified: Wed, 31 Mar 2021 17:51:49 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59da53be9c7202b665f6fd3eea5a7c06f3ca767a7dece9a6c1092194822b3909`  
		Last Modified: Wed, 31 Mar 2021 17:51:50 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef8b9c711055b45c44d93df2261200fd9bbdb82408ed9dc6f026c5e0710f676`  
		Last Modified: Wed, 31 Mar 2021 17:51:48 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03332397d4ff777be8babfbcb868c559cfd0af48c32d76b938831b58de40dc21`  
		Last Modified: Wed, 31 Mar 2021 17:51:48 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42892a8210a35ab55795ec9e555d8ba18c17480ee1129833d4d31f42b50d3bf2`  
		Last Modified: Wed, 31 Mar 2021 17:51:48 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8.2-slim` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:b2c8bb3fb1e9afe5258235cc3c9d3f4d6901d1252257dd61ebd2d03621344885
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.3 MB (47345578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a9b88dc147bf333fbb832cb8f42a88497233062db2848c50687f14fe28d1180`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:00 GMT
ADD file:97aac29a9ffbba2c76441891035010395614dc3115c4710d58932205b604308f in / 
# Thu, 25 Mar 2021 22:41:10 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 08:50:00 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Fri, 26 Mar 2021 08:50:01 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Fri, 26 Mar 2021 08:50:01 GMT
ARG MAKEFLAGS=
# Fri, 26 Mar 2021 08:50:02 GMT
ENV ZNC_VERSION=1.8.2
# Fri, 26 Mar 2021 08:58:39 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Fri, 26 Mar 2021 08:58:40 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Fri, 26 Mar 2021 08:58:41 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Fri, 26 Mar 2021 08:58:43 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Fri, 26 Mar 2021 08:58:44 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Fri, 26 Mar 2021 08:58:45 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Fri, 26 Mar 2021 08:58:46 GMT
VOLUME [/znc-data]
# Fri, 26 Mar 2021 08:58:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:95dec6db372224fc1909f0d0c0a9a9d5767ec6b78d066ff6a7d5723160037828`  
		Last Modified: Thu, 25 Mar 2021 22:45:23 GMT  
		Size: 2.7 MB (2709692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261b1493d1cb2458295caac1ef25dd52633a9918efc444ba17cc51219d26a8d9`  
		Last Modified: Fri, 26 Mar 2021 08:59:40 GMT  
		Size: 44.6 MB (44634463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2281c6206ad9e01aeba3f087c93c093edf03b65b013c1e5f30f1c1cc74e9d4d`  
		Last Modified: Fri, 26 Mar 2021 08:59:27 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6757db4ee2933909c092344b92ea6da1ae5f0cb9dc22909417c149a6c7230e6`  
		Last Modified: Fri, 26 Mar 2021 08:59:27 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1812d97bc4f8773fb4157ee1040400c92ba44a0f4cb42ee1d3968738f711d30`  
		Last Modified: Fri, 26 Mar 2021 08:59:26 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083ed828033ac4f4536b200687724afd662cadc3cadab7be191836076e23b0a8`  
		Last Modified: Fri, 26 Mar 2021 08:59:26 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5351579885da0be0c3e00c76b547db0e55bdeeba9d93a2a5bc221e79e44d1cdb`  
		Last Modified: Fri, 26 Mar 2021 08:59:26 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:latest`

```console
$ docker pull znc@sha256:8e87441cd12b57fc0f3c2b4febef884e56f28c76670a6b440c55c940cac7c20f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:latest` - linux; amd64

```console
$ docker pull znc@sha256:06f36fd86b43a8e7734f8170934e9d4fa5bbc6a94ce90f965882edf9f6f0f20d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (150968904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c803978ff1716d522e2dbb48cf667a2933030683dec6170898f8ea135ffb72e`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:49:36 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Fri, 26 Mar 2021 02:49:37 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Fri, 26 Mar 2021 02:49:37 GMT
ARG MAKEFLAGS=
# Fri, 26 Mar 2021 02:49:37 GMT
ENV ZNC_VERSION=1.8.2
# Fri, 26 Mar 2021 02:55:28 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Fri, 26 Mar 2021 02:55:28 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Fri, 26 Mar 2021 02:55:28 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Fri, 26 Mar 2021 02:55:29 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Fri, 26 Mar 2021 02:55:29 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Fri, 26 Mar 2021 02:55:29 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Fri, 26 Mar 2021 02:55:29 GMT
VOLUME [/znc-data]
# Fri, 26 Mar 2021 02:55:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 02:55:39 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Fri, 26 Mar 2021 02:55:39 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef753c00beaf06a3ee7647f2da37af968d3c33b9655927a8d6aca2d1d995e28c`  
		Last Modified: Fri, 26 Mar 2021 02:56:04 GMT  
		Size: 44.8 MB (44790585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9739f8a41ed5c01a8660fa107743ba3fb79709cdf9fd584ea4298252afa54a14`  
		Last Modified: Fri, 26 Mar 2021 02:55:52 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f021d06d531c1dbf7b87991e227094bb17ed380b2aeac36c819c64fad6cf9cc`  
		Last Modified: Fri, 26 Mar 2021 02:55:53 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db01e30df5558a3c24faf6d409e32758133a06c2e2145417d83e1cbeb3e4aee`  
		Last Modified: Fri, 26 Mar 2021 02:55:52 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afac7b001b7aa8a0b0dbd7c72ca4b057cf50099234a4751ab06b4e33b5a17f10`  
		Last Modified: Fri, 26 Mar 2021 02:55:52 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee18e3181ce87afeaaadc596532013194e9cc8132f0c58f8d235f7f9295e734`  
		Last Modified: Fri, 26 Mar 2021 02:55:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7585d98d7ae0ca7844e2d481de40ee8bfee40e04d9afa6d3c57a664165d40cc0`  
		Last Modified: Fri, 26 Mar 2021 02:56:35 GMT  
		Size: 103.4 MB (103376800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3bd687d2611b904fa018ddbec55747e33a4ef0747e568c2976c11c595859cc`  
		Last Modified: Fri, 26 Mar 2021 02:56:17 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:latest` - linux; arm variant v6

```console
$ docker pull znc@sha256:ddfe1fadb406db1a004fd488cfa47e05b22955988f435694c59ed8d77d27b92a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.7 MB (132673455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a143fe9f167782342008d41db959f61417cefaa723821899dc578a2dffb49d7`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 17:42:11 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Wed, 31 Mar 2021 17:42:11 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Wed, 31 Mar 2021 17:42:12 GMT
ARG MAKEFLAGS=
# Wed, 31 Mar 2021 17:42:13 GMT
ENV ZNC_VERSION=1.8.2
# Wed, 31 Mar 2021 17:50:40 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Wed, 31 Mar 2021 17:50:42 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Wed, 31 Mar 2021 17:50:44 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Wed, 31 Mar 2021 17:50:45 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Wed, 31 Mar 2021 17:50:46 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Wed, 31 Mar 2021 17:50:48 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Wed, 31 Mar 2021 17:50:50 GMT
VOLUME [/znc-data]
# Wed, 31 Mar 2021 17:50:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 17:51:26 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Wed, 31 Mar 2021 17:51:32 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3886333d907bad3825a1872f1dbbf1c596896930531994f4e86cb28dc6fceb`  
		Last Modified: Wed, 31 Mar 2021 17:52:08 GMT  
		Size: 43.0 MB (43047554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7c0b696ec30f6f96326d09b075904580a56314f80f8f15c22f3397f0f810e8`  
		Last Modified: Wed, 31 Mar 2021 17:51:49 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59da53be9c7202b665f6fd3eea5a7c06f3ca767a7dece9a6c1092194822b3909`  
		Last Modified: Wed, 31 Mar 2021 17:51:50 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef8b9c711055b45c44d93df2261200fd9bbdb82408ed9dc6f026c5e0710f676`  
		Last Modified: Wed, 31 Mar 2021 17:51:48 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03332397d4ff777be8babfbcb868c559cfd0af48c32d76b938831b58de40dc21`  
		Last Modified: Wed, 31 Mar 2021 17:51:48 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42892a8210a35ab55795ec9e555d8ba18c17480ee1129833d4d31f42b50d3bf2`  
		Last Modified: Wed, 31 Mar 2021 17:51:48 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff41a0b34e55fd23b33184337e9fd3644cbd0bfa22bf94d1dea99c83c16d8cb`  
		Last Modified: Wed, 31 Mar 2021 17:52:48 GMT  
		Size: 87.0 MB (87019485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a571a5e7d8add8b875bc4c7a372a14b3fad2ed1053925c76ac9cfe9dc8dfb5`  
		Last Modified: Wed, 31 Mar 2021 17:52:21 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:latest` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:867d8008e3c661f2f36ae5de43c0d8761c09394f6efa432fb9755f41388ad2de
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.1 MB (138119258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae9dbdb0d56d42b79e772164b24015a6b6eb5f3df3a9d7c74e803e51ce2f1f2e`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:00 GMT
ADD file:97aac29a9ffbba2c76441891035010395614dc3115c4710d58932205b604308f in / 
# Thu, 25 Mar 2021 22:41:10 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 08:50:00 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Fri, 26 Mar 2021 08:50:01 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Fri, 26 Mar 2021 08:50:01 GMT
ARG MAKEFLAGS=
# Fri, 26 Mar 2021 08:50:02 GMT
ENV ZNC_VERSION=1.8.2
# Fri, 26 Mar 2021 08:58:39 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Fri, 26 Mar 2021 08:58:40 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Fri, 26 Mar 2021 08:58:41 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Fri, 26 Mar 2021 08:58:43 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Fri, 26 Mar 2021 08:58:44 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Fri, 26 Mar 2021 08:58:45 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Fri, 26 Mar 2021 08:58:46 GMT
VOLUME [/znc-data]
# Fri, 26 Mar 2021 08:58:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 08:59:09 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Fri, 26 Mar 2021 08:59:12 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:95dec6db372224fc1909f0d0c0a9a9d5767ec6b78d066ff6a7d5723160037828`  
		Last Modified: Thu, 25 Mar 2021 22:45:23 GMT  
		Size: 2.7 MB (2709692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261b1493d1cb2458295caac1ef25dd52633a9918efc444ba17cc51219d26a8d9`  
		Last Modified: Fri, 26 Mar 2021 08:59:40 GMT  
		Size: 44.6 MB (44634463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2281c6206ad9e01aeba3f087c93c093edf03b65b013c1e5f30f1c1cc74e9d4d`  
		Last Modified: Fri, 26 Mar 2021 08:59:27 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6757db4ee2933909c092344b92ea6da1ae5f0cb9dc22909417c149a6c7230e6`  
		Last Modified: Fri, 26 Mar 2021 08:59:27 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1812d97bc4f8773fb4157ee1040400c92ba44a0f4cb42ee1d3968738f711d30`  
		Last Modified: Fri, 26 Mar 2021 08:59:26 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083ed828033ac4f4536b200687724afd662cadc3cadab7be191836076e23b0a8`  
		Last Modified: Fri, 26 Mar 2021 08:59:26 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5351579885da0be0c3e00c76b547db0e55bdeeba9d93a2a5bc221e79e44d1cdb`  
		Last Modified: Fri, 26 Mar 2021 08:59:26 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2c89f681197b95d37c9eca50392af5784da5bba01a0b5b061626be357271a1`  
		Last Modified: Fri, 26 Mar 2021 09:00:18 GMT  
		Size: 90.8 MB (90773349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6446c82cbc42091f0d17d84181f2a84c5a3c8a6fbba3169b39554bb92d3241`  
		Last Modified: Fri, 26 Mar 2021 08:59:52 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:slim`

```console
$ docker pull znc@sha256:8dce50f00d936dc872148c4a981cf34116f85bfbd433fb6778627e13b13bedaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:slim` - linux; amd64

```console
$ docker pull znc@sha256:4303ffe84845e4386c18f084a7100f391b9e71311400d623391d17e7195ddb29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47591773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01f27eae3fac4ef84586b44f4ca6e780dafaae50dbe4bf6c460ec7125dedcdf3`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:49:36 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Fri, 26 Mar 2021 02:49:37 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Fri, 26 Mar 2021 02:49:37 GMT
ARG MAKEFLAGS=
# Fri, 26 Mar 2021 02:49:37 GMT
ENV ZNC_VERSION=1.8.2
# Fri, 26 Mar 2021 02:55:28 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Fri, 26 Mar 2021 02:55:28 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Fri, 26 Mar 2021 02:55:28 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Fri, 26 Mar 2021 02:55:29 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Fri, 26 Mar 2021 02:55:29 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Fri, 26 Mar 2021 02:55:29 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Fri, 26 Mar 2021 02:55:29 GMT
VOLUME [/znc-data]
# Fri, 26 Mar 2021 02:55:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef753c00beaf06a3ee7647f2da37af968d3c33b9655927a8d6aca2d1d995e28c`  
		Last Modified: Fri, 26 Mar 2021 02:56:04 GMT  
		Size: 44.8 MB (44790585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9739f8a41ed5c01a8660fa107743ba3fb79709cdf9fd584ea4298252afa54a14`  
		Last Modified: Fri, 26 Mar 2021 02:55:52 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f021d06d531c1dbf7b87991e227094bb17ed380b2aeac36c819c64fad6cf9cc`  
		Last Modified: Fri, 26 Mar 2021 02:55:53 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db01e30df5558a3c24faf6d409e32758133a06c2e2145417d83e1cbeb3e4aee`  
		Last Modified: Fri, 26 Mar 2021 02:55:52 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afac7b001b7aa8a0b0dbd7c72ca4b057cf50099234a4751ab06b4e33b5a17f10`  
		Last Modified: Fri, 26 Mar 2021 02:55:52 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee18e3181ce87afeaaadc596532013194e9cc8132f0c58f8d235f7f9295e734`  
		Last Modified: Fri, 26 Mar 2021 02:55:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:slim` - linux; arm variant v6

```console
$ docker pull znc@sha256:2a68259503ed3ebd996393ec515c599f698c273ca940409118ede2f1fc74994a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45653638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5e52705c8ce39b70c2d5c380db1f9ff6798526b9d1687c361dfe68e148217fe`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 17:42:11 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Wed, 31 Mar 2021 17:42:11 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Wed, 31 Mar 2021 17:42:12 GMT
ARG MAKEFLAGS=
# Wed, 31 Mar 2021 17:42:13 GMT
ENV ZNC_VERSION=1.8.2
# Wed, 31 Mar 2021 17:50:40 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Wed, 31 Mar 2021 17:50:42 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Wed, 31 Mar 2021 17:50:44 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Wed, 31 Mar 2021 17:50:45 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Wed, 31 Mar 2021 17:50:46 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Wed, 31 Mar 2021 17:50:48 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Wed, 31 Mar 2021 17:50:50 GMT
VOLUME [/znc-data]
# Wed, 31 Mar 2021 17:50:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3886333d907bad3825a1872f1dbbf1c596896930531994f4e86cb28dc6fceb`  
		Last Modified: Wed, 31 Mar 2021 17:52:08 GMT  
		Size: 43.0 MB (43047554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7c0b696ec30f6f96326d09b075904580a56314f80f8f15c22f3397f0f810e8`  
		Last Modified: Wed, 31 Mar 2021 17:51:49 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59da53be9c7202b665f6fd3eea5a7c06f3ca767a7dece9a6c1092194822b3909`  
		Last Modified: Wed, 31 Mar 2021 17:51:50 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef8b9c711055b45c44d93df2261200fd9bbdb82408ed9dc6f026c5e0710f676`  
		Last Modified: Wed, 31 Mar 2021 17:51:48 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03332397d4ff777be8babfbcb868c559cfd0af48c32d76b938831b58de40dc21`  
		Last Modified: Wed, 31 Mar 2021 17:51:48 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42892a8210a35ab55795ec9e555d8ba18c17480ee1129833d4d31f42b50d3bf2`  
		Last Modified: Wed, 31 Mar 2021 17:51:48 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:slim` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:b2c8bb3fb1e9afe5258235cc3c9d3f4d6901d1252257dd61ebd2d03621344885
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.3 MB (47345578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a9b88dc147bf333fbb832cb8f42a88497233062db2848c50687f14fe28d1180`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:00 GMT
ADD file:97aac29a9ffbba2c76441891035010395614dc3115c4710d58932205b604308f in / 
# Thu, 25 Mar 2021 22:41:10 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 08:50:00 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Fri, 26 Mar 2021 08:50:01 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Fri, 26 Mar 2021 08:50:01 GMT
ARG MAKEFLAGS=
# Fri, 26 Mar 2021 08:50:02 GMT
ENV ZNC_VERSION=1.8.2
# Fri, 26 Mar 2021 08:58:39 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Fri, 26 Mar 2021 08:58:40 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Fri, 26 Mar 2021 08:58:41 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Fri, 26 Mar 2021 08:58:43 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Fri, 26 Mar 2021 08:58:44 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Fri, 26 Mar 2021 08:58:45 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Fri, 26 Mar 2021 08:58:46 GMT
VOLUME [/znc-data]
# Fri, 26 Mar 2021 08:58:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:95dec6db372224fc1909f0d0c0a9a9d5767ec6b78d066ff6a7d5723160037828`  
		Last Modified: Thu, 25 Mar 2021 22:45:23 GMT  
		Size: 2.7 MB (2709692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261b1493d1cb2458295caac1ef25dd52633a9918efc444ba17cc51219d26a8d9`  
		Last Modified: Fri, 26 Mar 2021 08:59:40 GMT  
		Size: 44.6 MB (44634463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2281c6206ad9e01aeba3f087c93c093edf03b65b013c1e5f30f1c1cc74e9d4d`  
		Last Modified: Fri, 26 Mar 2021 08:59:27 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6757db4ee2933909c092344b92ea6da1ae5f0cb9dc22909417c149a6c7230e6`  
		Last Modified: Fri, 26 Mar 2021 08:59:27 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1812d97bc4f8773fb4157ee1040400c92ba44a0f4cb42ee1d3968738f711d30`  
		Last Modified: Fri, 26 Mar 2021 08:59:26 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083ed828033ac4f4536b200687724afd662cadc3cadab7be191836076e23b0a8`  
		Last Modified: Fri, 26 Mar 2021 08:59:26 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5351579885da0be0c3e00c76b547db0e55bdeeba9d93a2a5bc221e79e44d1cdb`  
		Last Modified: Fri, 26 Mar 2021 08:59:26 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
