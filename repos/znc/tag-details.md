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
$ docker pull znc@sha256:c0b3be17fbbe55fcb601cb242d5c48974ee8bad5bd1b01462b772d2e16d15c7c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8` - linux; amd64

```console
$ docker pull znc@sha256:0f911a028bb64788063a525fd640c3bb1853ffadd8f8414252a7c9a9b7c09405
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.7 MB (146701569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f12f7b56ea76ed2177cf99599c15867fdcfa71e31dff72462391444851a846d`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 18:59:59 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 28 Jun 2021 18:59:59 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 28 Jun 2021 18:59:59 GMT
ARG MAKEFLAGS=
# Mon, 28 Jun 2021 18:59:59 GMT
ENV ZNC_VERSION=1.8.2
# Mon, 28 Jun 2021 19:04:14 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 28 Jun 2021 19:04:15 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 28 Jun 2021 19:04:15 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Mon, 28 Jun 2021 19:04:15 GMT
VOLUME [/znc-data]
# Mon, 28 Jun 2021 19:04:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 28 Jun 2021 19:04:32 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Mon, 28 Jun 2021 19:04:32 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff255ca4465dfd7d64f1026e4aba335f37ca89ccaedf2f2cd55a2fa892a7ded`  
		Last Modified: Mon, 28 Jun 2021 19:04:53 GMT  
		Size: 44.6 MB (44649978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1477044263d022284e2050fc9f82ba0751490b6e7df35bcd63f86b5e4dbd7fcd`  
		Last Modified: Mon, 28 Jun 2021 19:04:46 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b825a32f2536b44091a1c58a8b828b2a11a2ef56c0e3d20b7cee696113f1654`  
		Last Modified: Mon, 28 Jun 2021 19:04:45 GMT  
		Size: 779.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43134674caceac06229071edfc715ecf4c3a3b7001beff67b6b3ba8f00418176`  
		Last Modified: Mon, 28 Jun 2021 19:05:22 GMT  
		Size: 99.2 MB (99238340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe9fd463c2b59e47414d37cc5200789fe8d19598ae0b9031383162a4b0cbf0c`  
		Last Modified: Mon, 28 Jun 2021 19:05:06 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8` - linux; arm variant v6

```console
$ docker pull znc@sha256:be2fafa3ab9c4cb922a790726918444edb4a66225a4dcb0af9f0e71e8a65fd14
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129451613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6083062eb342c0a9abebb4b4500ca804b85eaa583483bbbd8ea69974c46cb19d`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 18:11:53 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 28 Jun 2021 18:11:53 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 28 Jun 2021 18:11:54 GMT
ARG MAKEFLAGS=
# Mon, 28 Jun 2021 18:11:54 GMT
ENV ZNC_VERSION=1.8.2
# Mon, 28 Jun 2021 18:23:31 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 28 Jun 2021 18:23:32 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 28 Jun 2021 18:23:32 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Mon, 28 Jun 2021 18:23:33 GMT
VOLUME [/znc-data]
# Mon, 28 Jun 2021 18:23:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 28 Jun 2021 18:24:06 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Mon, 28 Jun 2021 18:24:07 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944e320a77f3b6f2c1fbd46804b4fa4058896d08ab2707da5d917ae32d77b789`  
		Last Modified: Mon, 28 Jun 2021 18:25:19 GMT  
		Size: 42.8 MB (42832050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47608ed6582782255b0c9917f39f593f78399b7b42c2bc084c08f8b4c4494fc5`  
		Last Modified: Mon, 28 Jun 2021 18:24:47 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e77ec677df80b5e08009d4ba4ebd2ff639307cf0888d5e3325146fcbd31b50`  
		Last Modified: Mon, 28 Jun 2021 18:24:47 GMT  
		Size: 780.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a86d63a5747e5d199a47fbe397ad3147c50718ff8c86f4810ca3f17b2c6f94`  
		Last Modified: Mon, 28 Jun 2021 18:26:37 GMT  
		Size: 84.0 MB (83996148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb00c137240c181a6f956a841ebf14139e45902af131394baec6f16412b2d1c`  
		Last Modified: Mon, 28 Jun 2021 18:25:35 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:bb7b457d88e7997892b7794a2d9eb94c57f86f37c0c255292556d7df4a715e1a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137841271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d497269dbb116457df5b3e5e952d1669bf06ce67a1ed7b22da144f52657fdda`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 18:16:07 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 28 Jun 2021 18:16:07 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 28 Jun 2021 18:16:07 GMT
ARG MAKEFLAGS=
# Mon, 28 Jun 2021 18:16:08 GMT
ENV ZNC_VERSION=1.8.2
# Mon, 28 Jun 2021 18:21:00 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 28 Jun 2021 18:21:00 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 28 Jun 2021 18:21:01 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Mon, 28 Jun 2021 18:21:01 GMT
VOLUME [/znc-data]
# Mon, 28 Jun 2021 18:21:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 28 Jun 2021 18:21:12 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Mon, 28 Jun 2021 18:21:13 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98feef4a8cf58e3e072ba740a5ce2b7f1f2d5f59b5db8911f5458bd2c7fcc812`  
		Last Modified: Mon, 28 Jun 2021 18:21:43 GMT  
		Size: 44.5 MB (44508050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54025587be870eb934c2a5385656df29b12f72b4a818e0d6fef473af599eb46b`  
		Last Modified: Mon, 28 Jun 2021 18:21:35 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c425af5eab66d876d419f2733984ff569b524a80cae68eb394950a087a02f871`  
		Last Modified: Mon, 28 Jun 2021 18:21:35 GMT  
		Size: 779.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc4e82e456d6f722d653b5379d6e12186122d1ed0dbe3e5be650aeff3884f24`  
		Last Modified: Mon, 28 Jun 2021 18:22:19 GMT  
		Size: 90.6 MB (90619914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173d921cd186139b9f312a66117d175c99fb5cbb95b4c44ef2b7156e37ee5e72`  
		Last Modified: Mon, 28 Jun 2021 18:22:01 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.8-slim`

```console
$ docker pull znc@sha256:cabee54711095b058da8ed99dfce836ed3002b63bae0b4309769f25e0b5dcab7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8-slim` - linux; amd64

```console
$ docker pull znc@sha256:10037c21e7723b1ae48e6693153456cc289d73967fef030a7bd0e36acaf0394b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.5 MB (47462898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45a579bf68957eddacc056c42160e51684a43363a18ba98ea72e516e4a694a8a`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 18:59:59 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 28 Jun 2021 18:59:59 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 28 Jun 2021 18:59:59 GMT
ARG MAKEFLAGS=
# Mon, 28 Jun 2021 18:59:59 GMT
ENV ZNC_VERSION=1.8.2
# Mon, 28 Jun 2021 19:04:14 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 28 Jun 2021 19:04:15 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 28 Jun 2021 19:04:15 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Mon, 28 Jun 2021 19:04:15 GMT
VOLUME [/znc-data]
# Mon, 28 Jun 2021 19:04:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff255ca4465dfd7d64f1026e4aba335f37ca89ccaedf2f2cd55a2fa892a7ded`  
		Last Modified: Mon, 28 Jun 2021 19:04:53 GMT  
		Size: 44.6 MB (44649978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1477044263d022284e2050fc9f82ba0751490b6e7df35bcd63f86b5e4dbd7fcd`  
		Last Modified: Mon, 28 Jun 2021 19:04:46 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b825a32f2536b44091a1c58a8b828b2a11a2ef56c0e3d20b7cee696113f1654`  
		Last Modified: Mon, 28 Jun 2021 19:04:45 GMT  
		Size: 779.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8-slim` - linux; arm variant v6

```console
$ docker pull znc@sha256:8ca9c33c5ba7e56dd5fde8d73517a25eec7b54f55b54627860a9df291ce51685
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45455133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b06f44d7157fb476526b51dad12fccd1e465089139c9bcc38bca5fc25938551d`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 18:11:53 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 28 Jun 2021 18:11:53 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 28 Jun 2021 18:11:54 GMT
ARG MAKEFLAGS=
# Mon, 28 Jun 2021 18:11:54 GMT
ENV ZNC_VERSION=1.8.2
# Mon, 28 Jun 2021 18:23:31 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 28 Jun 2021 18:23:32 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 28 Jun 2021 18:23:32 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Mon, 28 Jun 2021 18:23:33 GMT
VOLUME [/znc-data]
# Mon, 28 Jun 2021 18:23:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944e320a77f3b6f2c1fbd46804b4fa4058896d08ab2707da5d917ae32d77b789`  
		Last Modified: Mon, 28 Jun 2021 18:25:19 GMT  
		Size: 42.8 MB (42832050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47608ed6582782255b0c9917f39f593f78399b7b42c2bc084c08f8b4c4494fc5`  
		Last Modified: Mon, 28 Jun 2021 18:24:47 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e77ec677df80b5e08009d4ba4ebd2ff639307cf0888d5e3325146fcbd31b50`  
		Last Modified: Mon, 28 Jun 2021 18:24:47 GMT  
		Size: 780.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8-slim` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:332fdcb980b88c2103e8fa4d03894d4b6c239035fba51770594397e9cec61d51
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47221026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c691cbf607aea787dfb30a9d98655fa9aafde54fb41e343d6401755283be872`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 18:16:07 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 28 Jun 2021 18:16:07 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 28 Jun 2021 18:16:07 GMT
ARG MAKEFLAGS=
# Mon, 28 Jun 2021 18:16:08 GMT
ENV ZNC_VERSION=1.8.2
# Mon, 28 Jun 2021 18:21:00 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 28 Jun 2021 18:21:00 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 28 Jun 2021 18:21:01 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Mon, 28 Jun 2021 18:21:01 GMT
VOLUME [/znc-data]
# Mon, 28 Jun 2021 18:21:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98feef4a8cf58e3e072ba740a5ce2b7f1f2d5f59b5db8911f5458bd2c7fcc812`  
		Last Modified: Mon, 28 Jun 2021 18:21:43 GMT  
		Size: 44.5 MB (44508050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54025587be870eb934c2a5385656df29b12f72b4a818e0d6fef473af599eb46b`  
		Last Modified: Mon, 28 Jun 2021 18:21:35 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c425af5eab66d876d419f2733984ff569b524a80cae68eb394950a087a02f871`  
		Last Modified: Mon, 28 Jun 2021 18:21:35 GMT  
		Size: 779.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.8.2`

```console
$ docker pull znc@sha256:c0b3be17fbbe55fcb601cb242d5c48974ee8bad5bd1b01462b772d2e16d15c7c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8.2` - linux; amd64

```console
$ docker pull znc@sha256:0f911a028bb64788063a525fd640c3bb1853ffadd8f8414252a7c9a9b7c09405
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.7 MB (146701569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f12f7b56ea76ed2177cf99599c15867fdcfa71e31dff72462391444851a846d`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 18:59:59 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 28 Jun 2021 18:59:59 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 28 Jun 2021 18:59:59 GMT
ARG MAKEFLAGS=
# Mon, 28 Jun 2021 18:59:59 GMT
ENV ZNC_VERSION=1.8.2
# Mon, 28 Jun 2021 19:04:14 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 28 Jun 2021 19:04:15 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 28 Jun 2021 19:04:15 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Mon, 28 Jun 2021 19:04:15 GMT
VOLUME [/znc-data]
# Mon, 28 Jun 2021 19:04:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 28 Jun 2021 19:04:32 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Mon, 28 Jun 2021 19:04:32 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff255ca4465dfd7d64f1026e4aba335f37ca89ccaedf2f2cd55a2fa892a7ded`  
		Last Modified: Mon, 28 Jun 2021 19:04:53 GMT  
		Size: 44.6 MB (44649978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1477044263d022284e2050fc9f82ba0751490b6e7df35bcd63f86b5e4dbd7fcd`  
		Last Modified: Mon, 28 Jun 2021 19:04:46 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b825a32f2536b44091a1c58a8b828b2a11a2ef56c0e3d20b7cee696113f1654`  
		Last Modified: Mon, 28 Jun 2021 19:04:45 GMT  
		Size: 779.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43134674caceac06229071edfc715ecf4c3a3b7001beff67b6b3ba8f00418176`  
		Last Modified: Mon, 28 Jun 2021 19:05:22 GMT  
		Size: 99.2 MB (99238340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe9fd463c2b59e47414d37cc5200789fe8d19598ae0b9031383162a4b0cbf0c`  
		Last Modified: Mon, 28 Jun 2021 19:05:06 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8.2` - linux; arm variant v6

```console
$ docker pull znc@sha256:be2fafa3ab9c4cb922a790726918444edb4a66225a4dcb0af9f0e71e8a65fd14
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129451613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6083062eb342c0a9abebb4b4500ca804b85eaa583483bbbd8ea69974c46cb19d`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 18:11:53 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 28 Jun 2021 18:11:53 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 28 Jun 2021 18:11:54 GMT
ARG MAKEFLAGS=
# Mon, 28 Jun 2021 18:11:54 GMT
ENV ZNC_VERSION=1.8.2
# Mon, 28 Jun 2021 18:23:31 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 28 Jun 2021 18:23:32 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 28 Jun 2021 18:23:32 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Mon, 28 Jun 2021 18:23:33 GMT
VOLUME [/znc-data]
# Mon, 28 Jun 2021 18:23:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 28 Jun 2021 18:24:06 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Mon, 28 Jun 2021 18:24:07 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944e320a77f3b6f2c1fbd46804b4fa4058896d08ab2707da5d917ae32d77b789`  
		Last Modified: Mon, 28 Jun 2021 18:25:19 GMT  
		Size: 42.8 MB (42832050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47608ed6582782255b0c9917f39f593f78399b7b42c2bc084c08f8b4c4494fc5`  
		Last Modified: Mon, 28 Jun 2021 18:24:47 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e77ec677df80b5e08009d4ba4ebd2ff639307cf0888d5e3325146fcbd31b50`  
		Last Modified: Mon, 28 Jun 2021 18:24:47 GMT  
		Size: 780.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a86d63a5747e5d199a47fbe397ad3147c50718ff8c86f4810ca3f17b2c6f94`  
		Last Modified: Mon, 28 Jun 2021 18:26:37 GMT  
		Size: 84.0 MB (83996148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb00c137240c181a6f956a841ebf14139e45902af131394baec6f16412b2d1c`  
		Last Modified: Mon, 28 Jun 2021 18:25:35 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8.2` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:bb7b457d88e7997892b7794a2d9eb94c57f86f37c0c255292556d7df4a715e1a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137841271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d497269dbb116457df5b3e5e952d1669bf06ce67a1ed7b22da144f52657fdda`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 18:16:07 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 28 Jun 2021 18:16:07 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 28 Jun 2021 18:16:07 GMT
ARG MAKEFLAGS=
# Mon, 28 Jun 2021 18:16:08 GMT
ENV ZNC_VERSION=1.8.2
# Mon, 28 Jun 2021 18:21:00 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 28 Jun 2021 18:21:00 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 28 Jun 2021 18:21:01 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Mon, 28 Jun 2021 18:21:01 GMT
VOLUME [/znc-data]
# Mon, 28 Jun 2021 18:21:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 28 Jun 2021 18:21:12 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Mon, 28 Jun 2021 18:21:13 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98feef4a8cf58e3e072ba740a5ce2b7f1f2d5f59b5db8911f5458bd2c7fcc812`  
		Last Modified: Mon, 28 Jun 2021 18:21:43 GMT  
		Size: 44.5 MB (44508050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54025587be870eb934c2a5385656df29b12f72b4a818e0d6fef473af599eb46b`  
		Last Modified: Mon, 28 Jun 2021 18:21:35 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c425af5eab66d876d419f2733984ff569b524a80cae68eb394950a087a02f871`  
		Last Modified: Mon, 28 Jun 2021 18:21:35 GMT  
		Size: 779.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc4e82e456d6f722d653b5379d6e12186122d1ed0dbe3e5be650aeff3884f24`  
		Last Modified: Mon, 28 Jun 2021 18:22:19 GMT  
		Size: 90.6 MB (90619914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173d921cd186139b9f312a66117d175c99fb5cbb95b4c44ef2b7156e37ee5e72`  
		Last Modified: Mon, 28 Jun 2021 18:22:01 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.8.2-slim`

```console
$ docker pull znc@sha256:cabee54711095b058da8ed99dfce836ed3002b63bae0b4309769f25e0b5dcab7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8.2-slim` - linux; amd64

```console
$ docker pull znc@sha256:10037c21e7723b1ae48e6693153456cc289d73967fef030a7bd0e36acaf0394b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.5 MB (47462898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45a579bf68957eddacc056c42160e51684a43363a18ba98ea72e516e4a694a8a`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 18:59:59 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 28 Jun 2021 18:59:59 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 28 Jun 2021 18:59:59 GMT
ARG MAKEFLAGS=
# Mon, 28 Jun 2021 18:59:59 GMT
ENV ZNC_VERSION=1.8.2
# Mon, 28 Jun 2021 19:04:14 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 28 Jun 2021 19:04:15 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 28 Jun 2021 19:04:15 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Mon, 28 Jun 2021 19:04:15 GMT
VOLUME [/znc-data]
# Mon, 28 Jun 2021 19:04:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff255ca4465dfd7d64f1026e4aba335f37ca89ccaedf2f2cd55a2fa892a7ded`  
		Last Modified: Mon, 28 Jun 2021 19:04:53 GMT  
		Size: 44.6 MB (44649978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1477044263d022284e2050fc9f82ba0751490b6e7df35bcd63f86b5e4dbd7fcd`  
		Last Modified: Mon, 28 Jun 2021 19:04:46 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b825a32f2536b44091a1c58a8b828b2a11a2ef56c0e3d20b7cee696113f1654`  
		Last Modified: Mon, 28 Jun 2021 19:04:45 GMT  
		Size: 779.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8.2-slim` - linux; arm variant v6

```console
$ docker pull znc@sha256:8ca9c33c5ba7e56dd5fde8d73517a25eec7b54f55b54627860a9df291ce51685
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45455133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b06f44d7157fb476526b51dad12fccd1e465089139c9bcc38bca5fc25938551d`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 18:11:53 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 28 Jun 2021 18:11:53 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 28 Jun 2021 18:11:54 GMT
ARG MAKEFLAGS=
# Mon, 28 Jun 2021 18:11:54 GMT
ENV ZNC_VERSION=1.8.2
# Mon, 28 Jun 2021 18:23:31 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 28 Jun 2021 18:23:32 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 28 Jun 2021 18:23:32 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Mon, 28 Jun 2021 18:23:33 GMT
VOLUME [/znc-data]
# Mon, 28 Jun 2021 18:23:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944e320a77f3b6f2c1fbd46804b4fa4058896d08ab2707da5d917ae32d77b789`  
		Last Modified: Mon, 28 Jun 2021 18:25:19 GMT  
		Size: 42.8 MB (42832050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47608ed6582782255b0c9917f39f593f78399b7b42c2bc084c08f8b4c4494fc5`  
		Last Modified: Mon, 28 Jun 2021 18:24:47 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e77ec677df80b5e08009d4ba4ebd2ff639307cf0888d5e3325146fcbd31b50`  
		Last Modified: Mon, 28 Jun 2021 18:24:47 GMT  
		Size: 780.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8.2-slim` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:332fdcb980b88c2103e8fa4d03894d4b6c239035fba51770594397e9cec61d51
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47221026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c691cbf607aea787dfb30a9d98655fa9aafde54fb41e343d6401755283be872`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 18:16:07 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 28 Jun 2021 18:16:07 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 28 Jun 2021 18:16:07 GMT
ARG MAKEFLAGS=
# Mon, 28 Jun 2021 18:16:08 GMT
ENV ZNC_VERSION=1.8.2
# Mon, 28 Jun 2021 18:21:00 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 28 Jun 2021 18:21:00 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 28 Jun 2021 18:21:01 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Mon, 28 Jun 2021 18:21:01 GMT
VOLUME [/znc-data]
# Mon, 28 Jun 2021 18:21:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98feef4a8cf58e3e072ba740a5ce2b7f1f2d5f59b5db8911f5458bd2c7fcc812`  
		Last Modified: Mon, 28 Jun 2021 18:21:43 GMT  
		Size: 44.5 MB (44508050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54025587be870eb934c2a5385656df29b12f72b4a818e0d6fef473af599eb46b`  
		Last Modified: Mon, 28 Jun 2021 18:21:35 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c425af5eab66d876d419f2733984ff569b524a80cae68eb394950a087a02f871`  
		Last Modified: Mon, 28 Jun 2021 18:21:35 GMT  
		Size: 779.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:latest`

```console
$ docker pull znc@sha256:c0b3be17fbbe55fcb601cb242d5c48974ee8bad5bd1b01462b772d2e16d15c7c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:latest` - linux; amd64

```console
$ docker pull znc@sha256:0f911a028bb64788063a525fd640c3bb1853ffadd8f8414252a7c9a9b7c09405
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.7 MB (146701569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f12f7b56ea76ed2177cf99599c15867fdcfa71e31dff72462391444851a846d`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 18:59:59 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 28 Jun 2021 18:59:59 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 28 Jun 2021 18:59:59 GMT
ARG MAKEFLAGS=
# Mon, 28 Jun 2021 18:59:59 GMT
ENV ZNC_VERSION=1.8.2
# Mon, 28 Jun 2021 19:04:14 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 28 Jun 2021 19:04:15 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 28 Jun 2021 19:04:15 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Mon, 28 Jun 2021 19:04:15 GMT
VOLUME [/znc-data]
# Mon, 28 Jun 2021 19:04:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 28 Jun 2021 19:04:32 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Mon, 28 Jun 2021 19:04:32 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff255ca4465dfd7d64f1026e4aba335f37ca89ccaedf2f2cd55a2fa892a7ded`  
		Last Modified: Mon, 28 Jun 2021 19:04:53 GMT  
		Size: 44.6 MB (44649978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1477044263d022284e2050fc9f82ba0751490b6e7df35bcd63f86b5e4dbd7fcd`  
		Last Modified: Mon, 28 Jun 2021 19:04:46 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b825a32f2536b44091a1c58a8b828b2a11a2ef56c0e3d20b7cee696113f1654`  
		Last Modified: Mon, 28 Jun 2021 19:04:45 GMT  
		Size: 779.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43134674caceac06229071edfc715ecf4c3a3b7001beff67b6b3ba8f00418176`  
		Last Modified: Mon, 28 Jun 2021 19:05:22 GMT  
		Size: 99.2 MB (99238340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe9fd463c2b59e47414d37cc5200789fe8d19598ae0b9031383162a4b0cbf0c`  
		Last Modified: Mon, 28 Jun 2021 19:05:06 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:latest` - linux; arm variant v6

```console
$ docker pull znc@sha256:be2fafa3ab9c4cb922a790726918444edb4a66225a4dcb0af9f0e71e8a65fd14
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129451613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6083062eb342c0a9abebb4b4500ca804b85eaa583483bbbd8ea69974c46cb19d`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 18:11:53 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 28 Jun 2021 18:11:53 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 28 Jun 2021 18:11:54 GMT
ARG MAKEFLAGS=
# Mon, 28 Jun 2021 18:11:54 GMT
ENV ZNC_VERSION=1.8.2
# Mon, 28 Jun 2021 18:23:31 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 28 Jun 2021 18:23:32 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 28 Jun 2021 18:23:32 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Mon, 28 Jun 2021 18:23:33 GMT
VOLUME [/znc-data]
# Mon, 28 Jun 2021 18:23:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 28 Jun 2021 18:24:06 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Mon, 28 Jun 2021 18:24:07 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944e320a77f3b6f2c1fbd46804b4fa4058896d08ab2707da5d917ae32d77b789`  
		Last Modified: Mon, 28 Jun 2021 18:25:19 GMT  
		Size: 42.8 MB (42832050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47608ed6582782255b0c9917f39f593f78399b7b42c2bc084c08f8b4c4494fc5`  
		Last Modified: Mon, 28 Jun 2021 18:24:47 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e77ec677df80b5e08009d4ba4ebd2ff639307cf0888d5e3325146fcbd31b50`  
		Last Modified: Mon, 28 Jun 2021 18:24:47 GMT  
		Size: 780.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a86d63a5747e5d199a47fbe397ad3147c50718ff8c86f4810ca3f17b2c6f94`  
		Last Modified: Mon, 28 Jun 2021 18:26:37 GMT  
		Size: 84.0 MB (83996148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb00c137240c181a6f956a841ebf14139e45902af131394baec6f16412b2d1c`  
		Last Modified: Mon, 28 Jun 2021 18:25:35 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:latest` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:bb7b457d88e7997892b7794a2d9eb94c57f86f37c0c255292556d7df4a715e1a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137841271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d497269dbb116457df5b3e5e952d1669bf06ce67a1ed7b22da144f52657fdda`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 18:16:07 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 28 Jun 2021 18:16:07 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 28 Jun 2021 18:16:07 GMT
ARG MAKEFLAGS=
# Mon, 28 Jun 2021 18:16:08 GMT
ENV ZNC_VERSION=1.8.2
# Mon, 28 Jun 2021 18:21:00 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 28 Jun 2021 18:21:00 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 28 Jun 2021 18:21:01 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Mon, 28 Jun 2021 18:21:01 GMT
VOLUME [/znc-data]
# Mon, 28 Jun 2021 18:21:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 28 Jun 2021 18:21:12 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Mon, 28 Jun 2021 18:21:13 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98feef4a8cf58e3e072ba740a5ce2b7f1f2d5f59b5db8911f5458bd2c7fcc812`  
		Last Modified: Mon, 28 Jun 2021 18:21:43 GMT  
		Size: 44.5 MB (44508050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54025587be870eb934c2a5385656df29b12f72b4a818e0d6fef473af599eb46b`  
		Last Modified: Mon, 28 Jun 2021 18:21:35 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c425af5eab66d876d419f2733984ff569b524a80cae68eb394950a087a02f871`  
		Last Modified: Mon, 28 Jun 2021 18:21:35 GMT  
		Size: 779.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc4e82e456d6f722d653b5379d6e12186122d1ed0dbe3e5be650aeff3884f24`  
		Last Modified: Mon, 28 Jun 2021 18:22:19 GMT  
		Size: 90.6 MB (90619914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173d921cd186139b9f312a66117d175c99fb5cbb95b4c44ef2b7156e37ee5e72`  
		Last Modified: Mon, 28 Jun 2021 18:22:01 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:slim`

```console
$ docker pull znc@sha256:cabee54711095b058da8ed99dfce836ed3002b63bae0b4309769f25e0b5dcab7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:slim` - linux; amd64

```console
$ docker pull znc@sha256:10037c21e7723b1ae48e6693153456cc289d73967fef030a7bd0e36acaf0394b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.5 MB (47462898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45a579bf68957eddacc056c42160e51684a43363a18ba98ea72e516e4a694a8a`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 18:59:59 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 28 Jun 2021 18:59:59 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 28 Jun 2021 18:59:59 GMT
ARG MAKEFLAGS=
# Mon, 28 Jun 2021 18:59:59 GMT
ENV ZNC_VERSION=1.8.2
# Mon, 28 Jun 2021 19:04:14 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 28 Jun 2021 19:04:15 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 28 Jun 2021 19:04:15 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Mon, 28 Jun 2021 19:04:15 GMT
VOLUME [/znc-data]
# Mon, 28 Jun 2021 19:04:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff255ca4465dfd7d64f1026e4aba335f37ca89ccaedf2f2cd55a2fa892a7ded`  
		Last Modified: Mon, 28 Jun 2021 19:04:53 GMT  
		Size: 44.6 MB (44649978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1477044263d022284e2050fc9f82ba0751490b6e7df35bcd63f86b5e4dbd7fcd`  
		Last Modified: Mon, 28 Jun 2021 19:04:46 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b825a32f2536b44091a1c58a8b828b2a11a2ef56c0e3d20b7cee696113f1654`  
		Last Modified: Mon, 28 Jun 2021 19:04:45 GMT  
		Size: 779.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:slim` - linux; arm variant v6

```console
$ docker pull znc@sha256:8ca9c33c5ba7e56dd5fde8d73517a25eec7b54f55b54627860a9df291ce51685
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45455133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b06f44d7157fb476526b51dad12fccd1e465089139c9bcc38bca5fc25938551d`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 18:11:53 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 28 Jun 2021 18:11:53 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 28 Jun 2021 18:11:54 GMT
ARG MAKEFLAGS=
# Mon, 28 Jun 2021 18:11:54 GMT
ENV ZNC_VERSION=1.8.2
# Mon, 28 Jun 2021 18:23:31 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 28 Jun 2021 18:23:32 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 28 Jun 2021 18:23:32 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Mon, 28 Jun 2021 18:23:33 GMT
VOLUME [/znc-data]
# Mon, 28 Jun 2021 18:23:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944e320a77f3b6f2c1fbd46804b4fa4058896d08ab2707da5d917ae32d77b789`  
		Last Modified: Mon, 28 Jun 2021 18:25:19 GMT  
		Size: 42.8 MB (42832050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47608ed6582782255b0c9917f39f593f78399b7b42c2bc084c08f8b4c4494fc5`  
		Last Modified: Mon, 28 Jun 2021 18:24:47 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e77ec677df80b5e08009d4ba4ebd2ff639307cf0888d5e3325146fcbd31b50`  
		Last Modified: Mon, 28 Jun 2021 18:24:47 GMT  
		Size: 780.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:slim` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:332fdcb980b88c2103e8fa4d03894d4b6c239035fba51770594397e9cec61d51
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47221026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c691cbf607aea787dfb30a9d98655fa9aafde54fb41e343d6401755283be872`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Mon, 28 Jun 2021 18:16:07 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 28 Jun 2021 18:16:07 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 28 Jun 2021 18:16:07 GMT
ARG MAKEFLAGS=
# Mon, 28 Jun 2021 18:16:08 GMT
ENV ZNC_VERSION=1.8.2
# Mon, 28 Jun 2021 18:21:00 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 28 Jun 2021 18:21:00 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 28 Jun 2021 18:21:01 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Mon, 28 Jun 2021 18:21:01 GMT
VOLUME [/znc-data]
# Mon, 28 Jun 2021 18:21:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98feef4a8cf58e3e072ba740a5ce2b7f1f2d5f59b5db8911f5458bd2c7fcc812`  
		Last Modified: Mon, 28 Jun 2021 18:21:43 GMT  
		Size: 44.5 MB (44508050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54025587be870eb934c2a5385656df29b12f72b4a818e0d6fef473af599eb46b`  
		Last Modified: Mon, 28 Jun 2021 18:21:35 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c425af5eab66d876d419f2733984ff569b524a80cae68eb394950a087a02f871`  
		Last Modified: Mon, 28 Jun 2021 18:21:35 GMT  
		Size: 779.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
