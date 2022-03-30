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
$ docker pull znc@sha256:946f0db0026a108be8798820546a9daad9225600578aba7bb400551a9b929b2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8` - linux; amd64

```console
$ docker pull znc@sha256:5348de9df3651481cf62a0f5d977933cd3cea7f2a2d623c849355aa71323a25d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138530986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e47cb054e40ad76dadb212c37f572341c36bca4732271f9f258aa77ba3cd33c1`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:46 GMT
ADD file:a2ef39a587aac85256b55bee81f17d73aaa7154b2a32a31527c7803fb889f2e7 in / 
# Tue, 29 Mar 2022 00:19:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 16:07:58 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 29 Mar 2022 16:07:58 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 29 Mar 2022 16:07:58 GMT
ARG MAKEFLAGS=
# Tue, 29 Mar 2022 16:07:58 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 29 Mar 2022 16:12:13 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 29 Mar 2022 16:12:14 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 29 Mar 2022 16:12:14 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 29 Mar 2022 16:12:14 GMT
VOLUME [/znc-data]
# Tue, 29 Mar 2022 16:12:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 16:12:27 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         openssl-dev         perl         python3
# Tue, 29 Mar 2022 16:12:28 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:b9c05db88786fd3c89b78787631257301391f898c03ba50553b556630046a741`  
		Last Modified: Tue, 29 Mar 2022 00:20:43 GMT  
		Size: 2.8 MB (2819223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f828069458554a26d8b7395651e4a55e5f48af3b81b37fc6092491aea430405`  
		Last Modified: Tue, 29 Mar 2022 16:12:47 GMT  
		Size: 43.4 MB (43359890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee677992da18b636e970f4253d80d3a318b2e3555ce8cea335338d84cfd152fa`  
		Last Modified: Tue, 29 Mar 2022 16:12:44 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893204669ae7612ae82d0ae4f26c5514eebede3b62d4ff38d233ea85ece5f761`  
		Last Modified: Tue, 29 Mar 2022 16:12:40 GMT  
		Size: 780.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37fab8128192bae0458d3a7e3a6246b47f7e204e5eef1fdfe9b04f0ac8e211e7`  
		Last Modified: Tue, 29 Mar 2022 16:13:14 GMT  
		Size: 92.4 MB (92350590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea665336f33cc9974ba0398e37daa4971aaf021d268e7a09c7594517f4a52434`  
		Last Modified: Tue, 29 Mar 2022 16:13:00 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8` - linux; arm variant v6

```console
$ docker pull znc@sha256:d0af1b1e4cbb5ee5cbbf62aaaf9e9a6838379d727f799ae2e188c4df4487a37e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122174529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc9ad2fdf124d1915fadea022a203f09aae0bb603c94590f86f4c2e0d1c0414c`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:56 GMT
ADD file:23d913551f75313e359a4e93592ea0a9655e1a7c2bec5fddd210717d70c3114b in / 
# Tue, 29 Mar 2022 00:49:57 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 14:00:29 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 29 Mar 2022 14:00:29 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 29 Mar 2022 14:00:29 GMT
ARG MAKEFLAGS=
# Tue, 29 Mar 2022 14:00:30 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 29 Mar 2022 14:12:16 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 29 Mar 2022 14:12:17 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 29 Mar 2022 14:12:17 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 29 Mar 2022 14:12:18 GMT
VOLUME [/znc-data]
# Tue, 29 Mar 2022 14:12:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 14:12:50 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         openssl-dev         perl         python3
# Tue, 29 Mar 2022 14:12:52 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:eba0847afba90891ea7dae672f5dadfa405a822df0bc9c00b9e3328fd5fd889c`  
		Last Modified: Tue, 29 Mar 2022 00:51:57 GMT  
		Size: 2.6 MB (2625139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617d2651b3585383f243ada330f7b3fffce991c6f06ca6cdf2b8b76cd08987c8`  
		Last Modified: Tue, 29 Mar 2022 14:13:59 GMT  
		Size: 41.6 MB (41648111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab681de6259659ebd0dfdf3086f6b323437acbaf7a1ec6aa4afe9b66c8015e4`  
		Last Modified: Tue, 29 Mar 2022 14:13:30 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa3f3eae0ba9559c3b27561249e2ca0e713501a0cedba262a9b37c0b64a2108`  
		Last Modified: Tue, 29 Mar 2022 14:13:30 GMT  
		Size: 780.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bdca122f2e7669d641475c4c366fd47cc3a507698d53893acfc4f99faf060d`  
		Last Modified: Tue, 29 Mar 2022 14:15:07 GMT  
		Size: 77.9 MB (77899997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be475792ab0f9a38c5250c50c63396c8421ba1278888d09e9b26cdf500208603`  
		Last Modified: Tue, 29 Mar 2022 14:14:14 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:afa3fbb8af8ced8fd1efdce3fca62d80480db10c990d68a1204e9f9e87ee865f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.8 MB (129834581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a09a33e1e703d52997d47e2abaa82b2acc565496bdf935982be0ff309f87be8`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:18 GMT
ADD file:3b8e0dac20ca40faf2aaf084b69476a222952f177c0e6ec90804a10c91a51feb in / 
# Tue, 29 Mar 2022 00:40:19 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 19:18:28 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 29 Mar 2022 19:18:29 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 29 Mar 2022 19:18:30 GMT
ARG MAKEFLAGS=
# Tue, 29 Mar 2022 19:18:31 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 29 Mar 2022 19:25:25 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 29 Mar 2022 19:25:26 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 29 Mar 2022 19:25:27 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 29 Mar 2022 19:25:27 GMT
VOLUME [/znc-data]
# Tue, 29 Mar 2022 19:25:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 19:25:48 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         openssl-dev         perl         python3
# Tue, 29 Mar 2022 19:25:49 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:4e7dd0becbc2dc968b69cba46c81a25fa500c88a644832ce17a5bb090925fa79`  
		Last Modified: Tue, 29 Mar 2022 00:41:37 GMT  
		Size: 2.7 MB (2720845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5070d58019f3fbd98dfb0d64dfb89857cf102a882a0e662a978de4f58f09c81`  
		Last Modified: Tue, 29 Mar 2022 19:26:17 GMT  
		Size: 43.2 MB (43215473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df106e1faca283318264b35af87e0d5c0cd998d951c136d824245d2a0a1b8d4f`  
		Last Modified: Tue, 29 Mar 2022 19:26:10 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985a79206f205a0b4852f8fa5063e4cf47106b5d2bf7efa3afbd692afdd3628d`  
		Last Modified: Tue, 29 Mar 2022 19:26:10 GMT  
		Size: 755.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d144af141dce589245355fea5aa1204e67814ba8ddddaa1db69d95267770f7e9`  
		Last Modified: Tue, 29 Mar 2022 19:26:45 GMT  
		Size: 83.9 MB (83897003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c07affa0a705b835a1e82b88b7e38b24c9aca493031410658c3601b229f4f70`  
		Last Modified: Tue, 29 Mar 2022 19:26:31 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.8-slim`

```console
$ docker pull znc@sha256:f771ba4cc42a6043a7ded9821187c8e07ed29f6019140e861cea7e889dfa1fea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8-slim` - linux; amd64

```console
$ docker pull znc@sha256:029d8b1041c4ed3490d443119e01ee3cd89be3b67a12fe71cb4dcb37f2ba7c1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46180066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1c4d26fc232011047921515efc69b4157bbc180ee38e0aac737271ecfb56909`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:46 GMT
ADD file:a2ef39a587aac85256b55bee81f17d73aaa7154b2a32a31527c7803fb889f2e7 in / 
# Tue, 29 Mar 2022 00:19:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 16:07:58 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 29 Mar 2022 16:07:58 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 29 Mar 2022 16:07:58 GMT
ARG MAKEFLAGS=
# Tue, 29 Mar 2022 16:07:58 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 29 Mar 2022 16:12:13 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 29 Mar 2022 16:12:14 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 29 Mar 2022 16:12:14 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 29 Mar 2022 16:12:14 GMT
VOLUME [/znc-data]
# Tue, 29 Mar 2022 16:12:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:b9c05db88786fd3c89b78787631257301391f898c03ba50553b556630046a741`  
		Last Modified: Tue, 29 Mar 2022 00:20:43 GMT  
		Size: 2.8 MB (2819223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f828069458554a26d8b7395651e4a55e5f48af3b81b37fc6092491aea430405`  
		Last Modified: Tue, 29 Mar 2022 16:12:47 GMT  
		Size: 43.4 MB (43359890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee677992da18b636e970f4253d80d3a318b2e3555ce8cea335338d84cfd152fa`  
		Last Modified: Tue, 29 Mar 2022 16:12:44 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893204669ae7612ae82d0ae4f26c5514eebede3b62d4ff38d233ea85ece5f761`  
		Last Modified: Tue, 29 Mar 2022 16:12:40 GMT  
		Size: 780.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8-slim` - linux; arm variant v6

```console
$ docker pull znc@sha256:7aa6152330dfbc7b9966895ad20f960f9b8373d2eefac1659592dcd85ac40b94
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44274202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4b49b5c07147d7bb98e6dc1eec8dd1d26b27f11102a9275a00e947fe408c14c`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:56 GMT
ADD file:23d913551f75313e359a4e93592ea0a9655e1a7c2bec5fddd210717d70c3114b in / 
# Tue, 29 Mar 2022 00:49:57 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 14:00:29 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 29 Mar 2022 14:00:29 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 29 Mar 2022 14:00:29 GMT
ARG MAKEFLAGS=
# Tue, 29 Mar 2022 14:00:30 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 29 Mar 2022 14:12:16 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 29 Mar 2022 14:12:17 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 29 Mar 2022 14:12:17 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 29 Mar 2022 14:12:18 GMT
VOLUME [/znc-data]
# Tue, 29 Mar 2022 14:12:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:eba0847afba90891ea7dae672f5dadfa405a822df0bc9c00b9e3328fd5fd889c`  
		Last Modified: Tue, 29 Mar 2022 00:51:57 GMT  
		Size: 2.6 MB (2625139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617d2651b3585383f243ada330f7b3fffce991c6f06ca6cdf2b8b76cd08987c8`  
		Last Modified: Tue, 29 Mar 2022 14:13:59 GMT  
		Size: 41.6 MB (41648111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab681de6259659ebd0dfdf3086f6b323437acbaf7a1ec6aa4afe9b66c8015e4`  
		Last Modified: Tue, 29 Mar 2022 14:13:30 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa3f3eae0ba9559c3b27561249e2ca0e713501a0cedba262a9b37c0b64a2108`  
		Last Modified: Tue, 29 Mar 2022 14:13:30 GMT  
		Size: 780.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8-slim` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:15925a7c7db76a8ffa6f0db05e18413ce24c256f87c14a7545994247ae50f506
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45937246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc76b9c8d156dee5d05166bc2e52acb6002c1703db08879784266bde6de8319`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:18 GMT
ADD file:3b8e0dac20ca40faf2aaf084b69476a222952f177c0e6ec90804a10c91a51feb in / 
# Tue, 29 Mar 2022 00:40:19 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 19:18:28 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 29 Mar 2022 19:18:29 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 29 Mar 2022 19:18:30 GMT
ARG MAKEFLAGS=
# Tue, 29 Mar 2022 19:18:31 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 29 Mar 2022 19:25:25 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 29 Mar 2022 19:25:26 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 29 Mar 2022 19:25:27 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 29 Mar 2022 19:25:27 GMT
VOLUME [/znc-data]
# Tue, 29 Mar 2022 19:25:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:4e7dd0becbc2dc968b69cba46c81a25fa500c88a644832ce17a5bb090925fa79`  
		Last Modified: Tue, 29 Mar 2022 00:41:37 GMT  
		Size: 2.7 MB (2720845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5070d58019f3fbd98dfb0d64dfb89857cf102a882a0e662a978de4f58f09c81`  
		Last Modified: Tue, 29 Mar 2022 19:26:17 GMT  
		Size: 43.2 MB (43215473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df106e1faca283318264b35af87e0d5c0cd998d951c136d824245d2a0a1b8d4f`  
		Last Modified: Tue, 29 Mar 2022 19:26:10 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985a79206f205a0b4852f8fa5063e4cf47106b5d2bf7efa3afbd692afdd3628d`  
		Last Modified: Tue, 29 Mar 2022 19:26:10 GMT  
		Size: 755.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.8.2`

```console
$ docker pull znc@sha256:946f0db0026a108be8798820546a9daad9225600578aba7bb400551a9b929b2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8.2` - linux; amd64

```console
$ docker pull znc@sha256:5348de9df3651481cf62a0f5d977933cd3cea7f2a2d623c849355aa71323a25d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138530986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e47cb054e40ad76dadb212c37f572341c36bca4732271f9f258aa77ba3cd33c1`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:46 GMT
ADD file:a2ef39a587aac85256b55bee81f17d73aaa7154b2a32a31527c7803fb889f2e7 in / 
# Tue, 29 Mar 2022 00:19:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 16:07:58 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 29 Mar 2022 16:07:58 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 29 Mar 2022 16:07:58 GMT
ARG MAKEFLAGS=
# Tue, 29 Mar 2022 16:07:58 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 29 Mar 2022 16:12:13 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 29 Mar 2022 16:12:14 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 29 Mar 2022 16:12:14 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 29 Mar 2022 16:12:14 GMT
VOLUME [/znc-data]
# Tue, 29 Mar 2022 16:12:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 16:12:27 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         openssl-dev         perl         python3
# Tue, 29 Mar 2022 16:12:28 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:b9c05db88786fd3c89b78787631257301391f898c03ba50553b556630046a741`  
		Last Modified: Tue, 29 Mar 2022 00:20:43 GMT  
		Size: 2.8 MB (2819223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f828069458554a26d8b7395651e4a55e5f48af3b81b37fc6092491aea430405`  
		Last Modified: Tue, 29 Mar 2022 16:12:47 GMT  
		Size: 43.4 MB (43359890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee677992da18b636e970f4253d80d3a318b2e3555ce8cea335338d84cfd152fa`  
		Last Modified: Tue, 29 Mar 2022 16:12:44 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893204669ae7612ae82d0ae4f26c5514eebede3b62d4ff38d233ea85ece5f761`  
		Last Modified: Tue, 29 Mar 2022 16:12:40 GMT  
		Size: 780.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37fab8128192bae0458d3a7e3a6246b47f7e204e5eef1fdfe9b04f0ac8e211e7`  
		Last Modified: Tue, 29 Mar 2022 16:13:14 GMT  
		Size: 92.4 MB (92350590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea665336f33cc9974ba0398e37daa4971aaf021d268e7a09c7594517f4a52434`  
		Last Modified: Tue, 29 Mar 2022 16:13:00 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8.2` - linux; arm variant v6

```console
$ docker pull znc@sha256:d0af1b1e4cbb5ee5cbbf62aaaf9e9a6838379d727f799ae2e188c4df4487a37e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122174529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc9ad2fdf124d1915fadea022a203f09aae0bb603c94590f86f4c2e0d1c0414c`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:56 GMT
ADD file:23d913551f75313e359a4e93592ea0a9655e1a7c2bec5fddd210717d70c3114b in / 
# Tue, 29 Mar 2022 00:49:57 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 14:00:29 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 29 Mar 2022 14:00:29 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 29 Mar 2022 14:00:29 GMT
ARG MAKEFLAGS=
# Tue, 29 Mar 2022 14:00:30 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 29 Mar 2022 14:12:16 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 29 Mar 2022 14:12:17 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 29 Mar 2022 14:12:17 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 29 Mar 2022 14:12:18 GMT
VOLUME [/znc-data]
# Tue, 29 Mar 2022 14:12:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 14:12:50 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         openssl-dev         perl         python3
# Tue, 29 Mar 2022 14:12:52 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:eba0847afba90891ea7dae672f5dadfa405a822df0bc9c00b9e3328fd5fd889c`  
		Last Modified: Tue, 29 Mar 2022 00:51:57 GMT  
		Size: 2.6 MB (2625139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617d2651b3585383f243ada330f7b3fffce991c6f06ca6cdf2b8b76cd08987c8`  
		Last Modified: Tue, 29 Mar 2022 14:13:59 GMT  
		Size: 41.6 MB (41648111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab681de6259659ebd0dfdf3086f6b323437acbaf7a1ec6aa4afe9b66c8015e4`  
		Last Modified: Tue, 29 Mar 2022 14:13:30 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa3f3eae0ba9559c3b27561249e2ca0e713501a0cedba262a9b37c0b64a2108`  
		Last Modified: Tue, 29 Mar 2022 14:13:30 GMT  
		Size: 780.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bdca122f2e7669d641475c4c366fd47cc3a507698d53893acfc4f99faf060d`  
		Last Modified: Tue, 29 Mar 2022 14:15:07 GMT  
		Size: 77.9 MB (77899997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be475792ab0f9a38c5250c50c63396c8421ba1278888d09e9b26cdf500208603`  
		Last Modified: Tue, 29 Mar 2022 14:14:14 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8.2` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:afa3fbb8af8ced8fd1efdce3fca62d80480db10c990d68a1204e9f9e87ee865f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.8 MB (129834581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a09a33e1e703d52997d47e2abaa82b2acc565496bdf935982be0ff309f87be8`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:18 GMT
ADD file:3b8e0dac20ca40faf2aaf084b69476a222952f177c0e6ec90804a10c91a51feb in / 
# Tue, 29 Mar 2022 00:40:19 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 19:18:28 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 29 Mar 2022 19:18:29 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 29 Mar 2022 19:18:30 GMT
ARG MAKEFLAGS=
# Tue, 29 Mar 2022 19:18:31 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 29 Mar 2022 19:25:25 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 29 Mar 2022 19:25:26 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 29 Mar 2022 19:25:27 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 29 Mar 2022 19:25:27 GMT
VOLUME [/znc-data]
# Tue, 29 Mar 2022 19:25:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 19:25:48 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         openssl-dev         perl         python3
# Tue, 29 Mar 2022 19:25:49 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:4e7dd0becbc2dc968b69cba46c81a25fa500c88a644832ce17a5bb090925fa79`  
		Last Modified: Tue, 29 Mar 2022 00:41:37 GMT  
		Size: 2.7 MB (2720845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5070d58019f3fbd98dfb0d64dfb89857cf102a882a0e662a978de4f58f09c81`  
		Last Modified: Tue, 29 Mar 2022 19:26:17 GMT  
		Size: 43.2 MB (43215473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df106e1faca283318264b35af87e0d5c0cd998d951c136d824245d2a0a1b8d4f`  
		Last Modified: Tue, 29 Mar 2022 19:26:10 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985a79206f205a0b4852f8fa5063e4cf47106b5d2bf7efa3afbd692afdd3628d`  
		Last Modified: Tue, 29 Mar 2022 19:26:10 GMT  
		Size: 755.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d144af141dce589245355fea5aa1204e67814ba8ddddaa1db69d95267770f7e9`  
		Last Modified: Tue, 29 Mar 2022 19:26:45 GMT  
		Size: 83.9 MB (83897003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c07affa0a705b835a1e82b88b7e38b24c9aca493031410658c3601b229f4f70`  
		Last Modified: Tue, 29 Mar 2022 19:26:31 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.8.2-slim`

```console
$ docker pull znc@sha256:f771ba4cc42a6043a7ded9821187c8e07ed29f6019140e861cea7e889dfa1fea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8.2-slim` - linux; amd64

```console
$ docker pull znc@sha256:029d8b1041c4ed3490d443119e01ee3cd89be3b67a12fe71cb4dcb37f2ba7c1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46180066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1c4d26fc232011047921515efc69b4157bbc180ee38e0aac737271ecfb56909`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:46 GMT
ADD file:a2ef39a587aac85256b55bee81f17d73aaa7154b2a32a31527c7803fb889f2e7 in / 
# Tue, 29 Mar 2022 00:19:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 16:07:58 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 29 Mar 2022 16:07:58 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 29 Mar 2022 16:07:58 GMT
ARG MAKEFLAGS=
# Tue, 29 Mar 2022 16:07:58 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 29 Mar 2022 16:12:13 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 29 Mar 2022 16:12:14 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 29 Mar 2022 16:12:14 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 29 Mar 2022 16:12:14 GMT
VOLUME [/znc-data]
# Tue, 29 Mar 2022 16:12:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:b9c05db88786fd3c89b78787631257301391f898c03ba50553b556630046a741`  
		Last Modified: Tue, 29 Mar 2022 00:20:43 GMT  
		Size: 2.8 MB (2819223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f828069458554a26d8b7395651e4a55e5f48af3b81b37fc6092491aea430405`  
		Last Modified: Tue, 29 Mar 2022 16:12:47 GMT  
		Size: 43.4 MB (43359890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee677992da18b636e970f4253d80d3a318b2e3555ce8cea335338d84cfd152fa`  
		Last Modified: Tue, 29 Mar 2022 16:12:44 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893204669ae7612ae82d0ae4f26c5514eebede3b62d4ff38d233ea85ece5f761`  
		Last Modified: Tue, 29 Mar 2022 16:12:40 GMT  
		Size: 780.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8.2-slim` - linux; arm variant v6

```console
$ docker pull znc@sha256:7aa6152330dfbc7b9966895ad20f960f9b8373d2eefac1659592dcd85ac40b94
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44274202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4b49b5c07147d7bb98e6dc1eec8dd1d26b27f11102a9275a00e947fe408c14c`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:56 GMT
ADD file:23d913551f75313e359a4e93592ea0a9655e1a7c2bec5fddd210717d70c3114b in / 
# Tue, 29 Mar 2022 00:49:57 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 14:00:29 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 29 Mar 2022 14:00:29 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 29 Mar 2022 14:00:29 GMT
ARG MAKEFLAGS=
# Tue, 29 Mar 2022 14:00:30 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 29 Mar 2022 14:12:16 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 29 Mar 2022 14:12:17 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 29 Mar 2022 14:12:17 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 29 Mar 2022 14:12:18 GMT
VOLUME [/znc-data]
# Tue, 29 Mar 2022 14:12:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:eba0847afba90891ea7dae672f5dadfa405a822df0bc9c00b9e3328fd5fd889c`  
		Last Modified: Tue, 29 Mar 2022 00:51:57 GMT  
		Size: 2.6 MB (2625139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617d2651b3585383f243ada330f7b3fffce991c6f06ca6cdf2b8b76cd08987c8`  
		Last Modified: Tue, 29 Mar 2022 14:13:59 GMT  
		Size: 41.6 MB (41648111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab681de6259659ebd0dfdf3086f6b323437acbaf7a1ec6aa4afe9b66c8015e4`  
		Last Modified: Tue, 29 Mar 2022 14:13:30 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa3f3eae0ba9559c3b27561249e2ca0e713501a0cedba262a9b37c0b64a2108`  
		Last Modified: Tue, 29 Mar 2022 14:13:30 GMT  
		Size: 780.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8.2-slim` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:15925a7c7db76a8ffa6f0db05e18413ce24c256f87c14a7545994247ae50f506
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45937246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc76b9c8d156dee5d05166bc2e52acb6002c1703db08879784266bde6de8319`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:18 GMT
ADD file:3b8e0dac20ca40faf2aaf084b69476a222952f177c0e6ec90804a10c91a51feb in / 
# Tue, 29 Mar 2022 00:40:19 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 19:18:28 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 29 Mar 2022 19:18:29 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 29 Mar 2022 19:18:30 GMT
ARG MAKEFLAGS=
# Tue, 29 Mar 2022 19:18:31 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 29 Mar 2022 19:25:25 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 29 Mar 2022 19:25:26 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 29 Mar 2022 19:25:27 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 29 Mar 2022 19:25:27 GMT
VOLUME [/znc-data]
# Tue, 29 Mar 2022 19:25:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:4e7dd0becbc2dc968b69cba46c81a25fa500c88a644832ce17a5bb090925fa79`  
		Last Modified: Tue, 29 Mar 2022 00:41:37 GMT  
		Size: 2.7 MB (2720845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5070d58019f3fbd98dfb0d64dfb89857cf102a882a0e662a978de4f58f09c81`  
		Last Modified: Tue, 29 Mar 2022 19:26:17 GMT  
		Size: 43.2 MB (43215473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df106e1faca283318264b35af87e0d5c0cd998d951c136d824245d2a0a1b8d4f`  
		Last Modified: Tue, 29 Mar 2022 19:26:10 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985a79206f205a0b4852f8fa5063e4cf47106b5d2bf7efa3afbd692afdd3628d`  
		Last Modified: Tue, 29 Mar 2022 19:26:10 GMT  
		Size: 755.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:latest`

```console
$ docker pull znc@sha256:946f0db0026a108be8798820546a9daad9225600578aba7bb400551a9b929b2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:latest` - linux; amd64

```console
$ docker pull znc@sha256:5348de9df3651481cf62a0f5d977933cd3cea7f2a2d623c849355aa71323a25d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138530986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e47cb054e40ad76dadb212c37f572341c36bca4732271f9f258aa77ba3cd33c1`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:46 GMT
ADD file:a2ef39a587aac85256b55bee81f17d73aaa7154b2a32a31527c7803fb889f2e7 in / 
# Tue, 29 Mar 2022 00:19:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 16:07:58 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 29 Mar 2022 16:07:58 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 29 Mar 2022 16:07:58 GMT
ARG MAKEFLAGS=
# Tue, 29 Mar 2022 16:07:58 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 29 Mar 2022 16:12:13 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 29 Mar 2022 16:12:14 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 29 Mar 2022 16:12:14 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 29 Mar 2022 16:12:14 GMT
VOLUME [/znc-data]
# Tue, 29 Mar 2022 16:12:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 16:12:27 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         openssl-dev         perl         python3
# Tue, 29 Mar 2022 16:12:28 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:b9c05db88786fd3c89b78787631257301391f898c03ba50553b556630046a741`  
		Last Modified: Tue, 29 Mar 2022 00:20:43 GMT  
		Size: 2.8 MB (2819223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f828069458554a26d8b7395651e4a55e5f48af3b81b37fc6092491aea430405`  
		Last Modified: Tue, 29 Mar 2022 16:12:47 GMT  
		Size: 43.4 MB (43359890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee677992da18b636e970f4253d80d3a318b2e3555ce8cea335338d84cfd152fa`  
		Last Modified: Tue, 29 Mar 2022 16:12:44 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893204669ae7612ae82d0ae4f26c5514eebede3b62d4ff38d233ea85ece5f761`  
		Last Modified: Tue, 29 Mar 2022 16:12:40 GMT  
		Size: 780.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37fab8128192bae0458d3a7e3a6246b47f7e204e5eef1fdfe9b04f0ac8e211e7`  
		Last Modified: Tue, 29 Mar 2022 16:13:14 GMT  
		Size: 92.4 MB (92350590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea665336f33cc9974ba0398e37daa4971aaf021d268e7a09c7594517f4a52434`  
		Last Modified: Tue, 29 Mar 2022 16:13:00 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:latest` - linux; arm variant v6

```console
$ docker pull znc@sha256:d0af1b1e4cbb5ee5cbbf62aaaf9e9a6838379d727f799ae2e188c4df4487a37e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122174529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc9ad2fdf124d1915fadea022a203f09aae0bb603c94590f86f4c2e0d1c0414c`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:56 GMT
ADD file:23d913551f75313e359a4e93592ea0a9655e1a7c2bec5fddd210717d70c3114b in / 
# Tue, 29 Mar 2022 00:49:57 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 14:00:29 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 29 Mar 2022 14:00:29 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 29 Mar 2022 14:00:29 GMT
ARG MAKEFLAGS=
# Tue, 29 Mar 2022 14:00:30 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 29 Mar 2022 14:12:16 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 29 Mar 2022 14:12:17 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 29 Mar 2022 14:12:17 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 29 Mar 2022 14:12:18 GMT
VOLUME [/znc-data]
# Tue, 29 Mar 2022 14:12:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 14:12:50 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         openssl-dev         perl         python3
# Tue, 29 Mar 2022 14:12:52 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:eba0847afba90891ea7dae672f5dadfa405a822df0bc9c00b9e3328fd5fd889c`  
		Last Modified: Tue, 29 Mar 2022 00:51:57 GMT  
		Size: 2.6 MB (2625139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617d2651b3585383f243ada330f7b3fffce991c6f06ca6cdf2b8b76cd08987c8`  
		Last Modified: Tue, 29 Mar 2022 14:13:59 GMT  
		Size: 41.6 MB (41648111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab681de6259659ebd0dfdf3086f6b323437acbaf7a1ec6aa4afe9b66c8015e4`  
		Last Modified: Tue, 29 Mar 2022 14:13:30 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa3f3eae0ba9559c3b27561249e2ca0e713501a0cedba262a9b37c0b64a2108`  
		Last Modified: Tue, 29 Mar 2022 14:13:30 GMT  
		Size: 780.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bdca122f2e7669d641475c4c366fd47cc3a507698d53893acfc4f99faf060d`  
		Last Modified: Tue, 29 Mar 2022 14:15:07 GMT  
		Size: 77.9 MB (77899997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be475792ab0f9a38c5250c50c63396c8421ba1278888d09e9b26cdf500208603`  
		Last Modified: Tue, 29 Mar 2022 14:14:14 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:latest` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:afa3fbb8af8ced8fd1efdce3fca62d80480db10c990d68a1204e9f9e87ee865f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.8 MB (129834581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a09a33e1e703d52997d47e2abaa82b2acc565496bdf935982be0ff309f87be8`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:18 GMT
ADD file:3b8e0dac20ca40faf2aaf084b69476a222952f177c0e6ec90804a10c91a51feb in / 
# Tue, 29 Mar 2022 00:40:19 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 19:18:28 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 29 Mar 2022 19:18:29 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 29 Mar 2022 19:18:30 GMT
ARG MAKEFLAGS=
# Tue, 29 Mar 2022 19:18:31 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 29 Mar 2022 19:25:25 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 29 Mar 2022 19:25:26 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 29 Mar 2022 19:25:27 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 29 Mar 2022 19:25:27 GMT
VOLUME [/znc-data]
# Tue, 29 Mar 2022 19:25:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 19:25:48 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         openssl-dev         perl         python3
# Tue, 29 Mar 2022 19:25:49 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:4e7dd0becbc2dc968b69cba46c81a25fa500c88a644832ce17a5bb090925fa79`  
		Last Modified: Tue, 29 Mar 2022 00:41:37 GMT  
		Size: 2.7 MB (2720845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5070d58019f3fbd98dfb0d64dfb89857cf102a882a0e662a978de4f58f09c81`  
		Last Modified: Tue, 29 Mar 2022 19:26:17 GMT  
		Size: 43.2 MB (43215473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df106e1faca283318264b35af87e0d5c0cd998d951c136d824245d2a0a1b8d4f`  
		Last Modified: Tue, 29 Mar 2022 19:26:10 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985a79206f205a0b4852f8fa5063e4cf47106b5d2bf7efa3afbd692afdd3628d`  
		Last Modified: Tue, 29 Mar 2022 19:26:10 GMT  
		Size: 755.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d144af141dce589245355fea5aa1204e67814ba8ddddaa1db69d95267770f7e9`  
		Last Modified: Tue, 29 Mar 2022 19:26:45 GMT  
		Size: 83.9 MB (83897003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c07affa0a705b835a1e82b88b7e38b24c9aca493031410658c3601b229f4f70`  
		Last Modified: Tue, 29 Mar 2022 19:26:31 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:slim`

```console
$ docker pull znc@sha256:f771ba4cc42a6043a7ded9821187c8e07ed29f6019140e861cea7e889dfa1fea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:slim` - linux; amd64

```console
$ docker pull znc@sha256:029d8b1041c4ed3490d443119e01ee3cd89be3b67a12fe71cb4dcb37f2ba7c1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46180066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1c4d26fc232011047921515efc69b4157bbc180ee38e0aac737271ecfb56909`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:46 GMT
ADD file:a2ef39a587aac85256b55bee81f17d73aaa7154b2a32a31527c7803fb889f2e7 in / 
# Tue, 29 Mar 2022 00:19:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 16:07:58 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 29 Mar 2022 16:07:58 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 29 Mar 2022 16:07:58 GMT
ARG MAKEFLAGS=
# Tue, 29 Mar 2022 16:07:58 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 29 Mar 2022 16:12:13 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 29 Mar 2022 16:12:14 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 29 Mar 2022 16:12:14 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 29 Mar 2022 16:12:14 GMT
VOLUME [/znc-data]
# Tue, 29 Mar 2022 16:12:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:b9c05db88786fd3c89b78787631257301391f898c03ba50553b556630046a741`  
		Last Modified: Tue, 29 Mar 2022 00:20:43 GMT  
		Size: 2.8 MB (2819223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f828069458554a26d8b7395651e4a55e5f48af3b81b37fc6092491aea430405`  
		Last Modified: Tue, 29 Mar 2022 16:12:47 GMT  
		Size: 43.4 MB (43359890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee677992da18b636e970f4253d80d3a318b2e3555ce8cea335338d84cfd152fa`  
		Last Modified: Tue, 29 Mar 2022 16:12:44 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893204669ae7612ae82d0ae4f26c5514eebede3b62d4ff38d233ea85ece5f761`  
		Last Modified: Tue, 29 Mar 2022 16:12:40 GMT  
		Size: 780.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:slim` - linux; arm variant v6

```console
$ docker pull znc@sha256:7aa6152330dfbc7b9966895ad20f960f9b8373d2eefac1659592dcd85ac40b94
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44274202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4b49b5c07147d7bb98e6dc1eec8dd1d26b27f11102a9275a00e947fe408c14c`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:56 GMT
ADD file:23d913551f75313e359a4e93592ea0a9655e1a7c2bec5fddd210717d70c3114b in / 
# Tue, 29 Mar 2022 00:49:57 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 14:00:29 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 29 Mar 2022 14:00:29 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 29 Mar 2022 14:00:29 GMT
ARG MAKEFLAGS=
# Tue, 29 Mar 2022 14:00:30 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 29 Mar 2022 14:12:16 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 29 Mar 2022 14:12:17 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 29 Mar 2022 14:12:17 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 29 Mar 2022 14:12:18 GMT
VOLUME [/znc-data]
# Tue, 29 Mar 2022 14:12:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:eba0847afba90891ea7dae672f5dadfa405a822df0bc9c00b9e3328fd5fd889c`  
		Last Modified: Tue, 29 Mar 2022 00:51:57 GMT  
		Size: 2.6 MB (2625139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617d2651b3585383f243ada330f7b3fffce991c6f06ca6cdf2b8b76cd08987c8`  
		Last Modified: Tue, 29 Mar 2022 14:13:59 GMT  
		Size: 41.6 MB (41648111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab681de6259659ebd0dfdf3086f6b323437acbaf7a1ec6aa4afe9b66c8015e4`  
		Last Modified: Tue, 29 Mar 2022 14:13:30 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa3f3eae0ba9559c3b27561249e2ca0e713501a0cedba262a9b37c0b64a2108`  
		Last Modified: Tue, 29 Mar 2022 14:13:30 GMT  
		Size: 780.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:slim` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:15925a7c7db76a8ffa6f0db05e18413ce24c256f87c14a7545994247ae50f506
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45937246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc76b9c8d156dee5d05166bc2e52acb6002c1703db08879784266bde6de8319`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:18 GMT
ADD file:3b8e0dac20ca40faf2aaf084b69476a222952f177c0e6ec90804a10c91a51feb in / 
# Tue, 29 Mar 2022 00:40:19 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 19:18:28 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 29 Mar 2022 19:18:29 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 29 Mar 2022 19:18:30 GMT
ARG MAKEFLAGS=
# Tue, 29 Mar 2022 19:18:31 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 29 Mar 2022 19:25:25 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 29 Mar 2022 19:25:26 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 29 Mar 2022 19:25:27 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 29 Mar 2022 19:25:27 GMT
VOLUME [/znc-data]
# Tue, 29 Mar 2022 19:25:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:4e7dd0becbc2dc968b69cba46c81a25fa500c88a644832ce17a5bb090925fa79`  
		Last Modified: Tue, 29 Mar 2022 00:41:37 GMT  
		Size: 2.7 MB (2720845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5070d58019f3fbd98dfb0d64dfb89857cf102a882a0e662a978de4f58f09c81`  
		Last Modified: Tue, 29 Mar 2022 19:26:17 GMT  
		Size: 43.2 MB (43215473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df106e1faca283318264b35af87e0d5c0cd998d951c136d824245d2a0a1b8d4f`  
		Last Modified: Tue, 29 Mar 2022 19:26:10 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985a79206f205a0b4852f8fa5063e4cf47106b5d2bf7efa3afbd692afdd3628d`  
		Last Modified: Tue, 29 Mar 2022 19:26:10 GMT  
		Size: 755.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
