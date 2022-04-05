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
$ docker pull znc@sha256:c9cb2abb1cf5e4a56b84446103e17279d8b48f726914f5aeed41b5bb5c5e10c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8` - linux; amd64

```console
$ docker pull znc@sha256:965e6e4dd136d62907b87c35a0d89569cda4c697ec5db2666b50edf2fcacd9a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138531056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a06808447a2ce26d2325ad4970eb453f1da1f0cf393bb1e163c6465e2d370076`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:48:39 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 05 Apr 2022 09:48:39 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 05 Apr 2022 09:48:39 GMT
ARG MAKEFLAGS=
# Tue, 05 Apr 2022 09:48:39 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 05 Apr 2022 09:52:48 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 05 Apr 2022 09:52:48 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 05 Apr 2022 09:52:48 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 05 Apr 2022 09:52:48 GMT
VOLUME [/znc-data]
# Tue, 05 Apr 2022 09:52:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 09:53:08 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         openssl-dev         perl         python3
# Tue, 05 Apr 2022 09:53:08 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693ec67bc9a4a27a226ff63cd00eebfbc7e260c941b6398f57077617f8e18c90`  
		Last Modified: Tue, 05 Apr 2022 09:53:28 GMT  
		Size: 43.4 MB (43359682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8836528fad5890b023c4922fd7ebb55e54defd216ce7e4d065e735ed2e4b945b`  
		Last Modified: Tue, 05 Apr 2022 09:53:21 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47389a434a5f45e32c1b75051f48dc931a3787e607ea3478032e371bc2e3b4a`  
		Last Modified: Tue, 05 Apr 2022 09:53:21 GMT  
		Size: 779.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24aadd9789eb1a5c08f2a46b940b8e2434821b46a23ae93c5b2359ec9ef114b8`  
		Last Modified: Tue, 05 Apr 2022 09:53:55 GMT  
		Size: 92.4 MB (92350778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be21a2cd030e2f3b791bbf84f4435d7d3472c80073ea04cb7e9d8dd26e2f788`  
		Last Modified: Tue, 05 Apr 2022 09:53:41 GMT  
		Size: 332.0 B  
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
$ docker pull znc@sha256:c6d447bbea70f29ad2a600e3a8907716055eaa880427308021c52efa8e09d5b2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.8 MB (129834992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e473da2811571b93ddae9179ce428094469ebeb2fd648da249eba0c1f77bc2f`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:29:56 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 05 Apr 2022 07:29:57 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 05 Apr 2022 07:29:58 GMT
ARG MAKEFLAGS=
# Tue, 05 Apr 2022 07:29:59 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 05 Apr 2022 07:34:54 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 05 Apr 2022 07:34:55 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 05 Apr 2022 07:34:56 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 05 Apr 2022 07:34:56 GMT
VOLUME [/znc-data]
# Tue, 05 Apr 2022 07:34:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 07:35:15 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         openssl-dev         perl         python3
# Tue, 05 Apr 2022 07:35:16 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dade73c52ca649762693df12f39ec02756dee14e05c0864b24c4e97d97ad958d`  
		Last Modified: Tue, 05 Apr 2022 07:35:41 GMT  
		Size: 43.2 MB (43215389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bb3daa38da11139453d050715189241689eec49f348a62c35ef5c21cec730c`  
		Last Modified: Tue, 05 Apr 2022 07:35:35 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd345777189eda27551fcbf74799e48aeae6e50a81c2c18094733269e194b27f`  
		Last Modified: Tue, 05 Apr 2022 07:35:35 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0836f1c9f8e456a0a341ff8d4d1264de2900bc1d75304f4a82f982860106d4a`  
		Last Modified: Tue, 05 Apr 2022 07:36:08 GMT  
		Size: 83.9 MB (83897447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0017b43534c99c2fcda22306680b36735beae0ff8a5e5ff1395eeca4dfa7fce4`  
		Last Modified: Tue, 05 Apr 2022 07:35:55 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.8-slim`

```console
$ docker pull znc@sha256:fce567a092da99f64d0c6613c6bfdbcc11921625a075e9c326a75883e2ab8549
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8-slim` - linux; amd64

```console
$ docker pull znc@sha256:f0d779f1617c118f1d98575fb998679f3cd5901bd241c47aef4ef3ab31625f10
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46179946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea8f882dfd1f0cf37e6c3fb28c02976c45684c72e99747b19ebaff793138f59a`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:48:39 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 05 Apr 2022 09:48:39 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 05 Apr 2022 09:48:39 GMT
ARG MAKEFLAGS=
# Tue, 05 Apr 2022 09:48:39 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 05 Apr 2022 09:52:48 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 05 Apr 2022 09:52:48 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 05 Apr 2022 09:52:48 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 05 Apr 2022 09:52:48 GMT
VOLUME [/znc-data]
# Tue, 05 Apr 2022 09:52:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693ec67bc9a4a27a226ff63cd00eebfbc7e260c941b6398f57077617f8e18c90`  
		Last Modified: Tue, 05 Apr 2022 09:53:28 GMT  
		Size: 43.4 MB (43359682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8836528fad5890b023c4922fd7ebb55e54defd216ce7e4d065e735ed2e4b945b`  
		Last Modified: Tue, 05 Apr 2022 09:53:21 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47389a434a5f45e32c1b75051f48dc931a3787e607ea3478032e371bc2e3b4a`  
		Last Modified: Tue, 05 Apr 2022 09:53:21 GMT  
		Size: 779.0 B  
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
$ docker pull znc@sha256:af54eb8d2daf30393055c61060bc0bf7681e74efedb04d19c3bfe3c21fe295d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45937214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b780f2769519718faed55bc70d10abecc7ad3084e24e2527b6c1801a552d9e1b`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:29:56 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 05 Apr 2022 07:29:57 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 05 Apr 2022 07:29:58 GMT
ARG MAKEFLAGS=
# Tue, 05 Apr 2022 07:29:59 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 05 Apr 2022 07:34:54 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 05 Apr 2022 07:34:55 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 05 Apr 2022 07:34:56 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 05 Apr 2022 07:34:56 GMT
VOLUME [/znc-data]
# Tue, 05 Apr 2022 07:34:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dade73c52ca649762693df12f39ec02756dee14e05c0864b24c4e97d97ad958d`  
		Last Modified: Tue, 05 Apr 2022 07:35:41 GMT  
		Size: 43.2 MB (43215389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bb3daa38da11139453d050715189241689eec49f348a62c35ef5c21cec730c`  
		Last Modified: Tue, 05 Apr 2022 07:35:35 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd345777189eda27551fcbf74799e48aeae6e50a81c2c18094733269e194b27f`  
		Last Modified: Tue, 05 Apr 2022 07:35:35 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.8.2`

```console
$ docker pull znc@sha256:c9cb2abb1cf5e4a56b84446103e17279d8b48f726914f5aeed41b5bb5c5e10c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8.2` - linux; amd64

```console
$ docker pull znc@sha256:965e6e4dd136d62907b87c35a0d89569cda4c697ec5db2666b50edf2fcacd9a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138531056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a06808447a2ce26d2325ad4970eb453f1da1f0cf393bb1e163c6465e2d370076`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:48:39 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 05 Apr 2022 09:48:39 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 05 Apr 2022 09:48:39 GMT
ARG MAKEFLAGS=
# Tue, 05 Apr 2022 09:48:39 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 05 Apr 2022 09:52:48 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 05 Apr 2022 09:52:48 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 05 Apr 2022 09:52:48 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 05 Apr 2022 09:52:48 GMT
VOLUME [/znc-data]
# Tue, 05 Apr 2022 09:52:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 09:53:08 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         openssl-dev         perl         python3
# Tue, 05 Apr 2022 09:53:08 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693ec67bc9a4a27a226ff63cd00eebfbc7e260c941b6398f57077617f8e18c90`  
		Last Modified: Tue, 05 Apr 2022 09:53:28 GMT  
		Size: 43.4 MB (43359682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8836528fad5890b023c4922fd7ebb55e54defd216ce7e4d065e735ed2e4b945b`  
		Last Modified: Tue, 05 Apr 2022 09:53:21 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47389a434a5f45e32c1b75051f48dc931a3787e607ea3478032e371bc2e3b4a`  
		Last Modified: Tue, 05 Apr 2022 09:53:21 GMT  
		Size: 779.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24aadd9789eb1a5c08f2a46b940b8e2434821b46a23ae93c5b2359ec9ef114b8`  
		Last Modified: Tue, 05 Apr 2022 09:53:55 GMT  
		Size: 92.4 MB (92350778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be21a2cd030e2f3b791bbf84f4435d7d3472c80073ea04cb7e9d8dd26e2f788`  
		Last Modified: Tue, 05 Apr 2022 09:53:41 GMT  
		Size: 332.0 B  
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
$ docker pull znc@sha256:c6d447bbea70f29ad2a600e3a8907716055eaa880427308021c52efa8e09d5b2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.8 MB (129834992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e473da2811571b93ddae9179ce428094469ebeb2fd648da249eba0c1f77bc2f`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:29:56 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 05 Apr 2022 07:29:57 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 05 Apr 2022 07:29:58 GMT
ARG MAKEFLAGS=
# Tue, 05 Apr 2022 07:29:59 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 05 Apr 2022 07:34:54 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 05 Apr 2022 07:34:55 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 05 Apr 2022 07:34:56 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 05 Apr 2022 07:34:56 GMT
VOLUME [/znc-data]
# Tue, 05 Apr 2022 07:34:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 07:35:15 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         openssl-dev         perl         python3
# Tue, 05 Apr 2022 07:35:16 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dade73c52ca649762693df12f39ec02756dee14e05c0864b24c4e97d97ad958d`  
		Last Modified: Tue, 05 Apr 2022 07:35:41 GMT  
		Size: 43.2 MB (43215389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bb3daa38da11139453d050715189241689eec49f348a62c35ef5c21cec730c`  
		Last Modified: Tue, 05 Apr 2022 07:35:35 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd345777189eda27551fcbf74799e48aeae6e50a81c2c18094733269e194b27f`  
		Last Modified: Tue, 05 Apr 2022 07:35:35 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0836f1c9f8e456a0a341ff8d4d1264de2900bc1d75304f4a82f982860106d4a`  
		Last Modified: Tue, 05 Apr 2022 07:36:08 GMT  
		Size: 83.9 MB (83897447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0017b43534c99c2fcda22306680b36735beae0ff8a5e5ff1395eeca4dfa7fce4`  
		Last Modified: Tue, 05 Apr 2022 07:35:55 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.8.2-slim`

```console
$ docker pull znc@sha256:fce567a092da99f64d0c6613c6bfdbcc11921625a075e9c326a75883e2ab8549
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8.2-slim` - linux; amd64

```console
$ docker pull znc@sha256:f0d779f1617c118f1d98575fb998679f3cd5901bd241c47aef4ef3ab31625f10
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46179946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea8f882dfd1f0cf37e6c3fb28c02976c45684c72e99747b19ebaff793138f59a`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:48:39 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 05 Apr 2022 09:48:39 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 05 Apr 2022 09:48:39 GMT
ARG MAKEFLAGS=
# Tue, 05 Apr 2022 09:48:39 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 05 Apr 2022 09:52:48 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 05 Apr 2022 09:52:48 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 05 Apr 2022 09:52:48 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 05 Apr 2022 09:52:48 GMT
VOLUME [/znc-data]
# Tue, 05 Apr 2022 09:52:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693ec67bc9a4a27a226ff63cd00eebfbc7e260c941b6398f57077617f8e18c90`  
		Last Modified: Tue, 05 Apr 2022 09:53:28 GMT  
		Size: 43.4 MB (43359682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8836528fad5890b023c4922fd7ebb55e54defd216ce7e4d065e735ed2e4b945b`  
		Last Modified: Tue, 05 Apr 2022 09:53:21 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47389a434a5f45e32c1b75051f48dc931a3787e607ea3478032e371bc2e3b4a`  
		Last Modified: Tue, 05 Apr 2022 09:53:21 GMT  
		Size: 779.0 B  
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
$ docker pull znc@sha256:af54eb8d2daf30393055c61060bc0bf7681e74efedb04d19c3bfe3c21fe295d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45937214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b780f2769519718faed55bc70d10abecc7ad3084e24e2527b6c1801a552d9e1b`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:29:56 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 05 Apr 2022 07:29:57 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 05 Apr 2022 07:29:58 GMT
ARG MAKEFLAGS=
# Tue, 05 Apr 2022 07:29:59 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 05 Apr 2022 07:34:54 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 05 Apr 2022 07:34:55 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 05 Apr 2022 07:34:56 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 05 Apr 2022 07:34:56 GMT
VOLUME [/znc-data]
# Tue, 05 Apr 2022 07:34:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dade73c52ca649762693df12f39ec02756dee14e05c0864b24c4e97d97ad958d`  
		Last Modified: Tue, 05 Apr 2022 07:35:41 GMT  
		Size: 43.2 MB (43215389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bb3daa38da11139453d050715189241689eec49f348a62c35ef5c21cec730c`  
		Last Modified: Tue, 05 Apr 2022 07:35:35 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd345777189eda27551fcbf74799e48aeae6e50a81c2c18094733269e194b27f`  
		Last Modified: Tue, 05 Apr 2022 07:35:35 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:latest`

```console
$ docker pull znc@sha256:c9cb2abb1cf5e4a56b84446103e17279d8b48f726914f5aeed41b5bb5c5e10c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:latest` - linux; amd64

```console
$ docker pull znc@sha256:965e6e4dd136d62907b87c35a0d89569cda4c697ec5db2666b50edf2fcacd9a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138531056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a06808447a2ce26d2325ad4970eb453f1da1f0cf393bb1e163c6465e2d370076`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:48:39 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 05 Apr 2022 09:48:39 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 05 Apr 2022 09:48:39 GMT
ARG MAKEFLAGS=
# Tue, 05 Apr 2022 09:48:39 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 05 Apr 2022 09:52:48 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 05 Apr 2022 09:52:48 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 05 Apr 2022 09:52:48 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 05 Apr 2022 09:52:48 GMT
VOLUME [/znc-data]
# Tue, 05 Apr 2022 09:52:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 09:53:08 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         openssl-dev         perl         python3
# Tue, 05 Apr 2022 09:53:08 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693ec67bc9a4a27a226ff63cd00eebfbc7e260c941b6398f57077617f8e18c90`  
		Last Modified: Tue, 05 Apr 2022 09:53:28 GMT  
		Size: 43.4 MB (43359682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8836528fad5890b023c4922fd7ebb55e54defd216ce7e4d065e735ed2e4b945b`  
		Last Modified: Tue, 05 Apr 2022 09:53:21 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47389a434a5f45e32c1b75051f48dc931a3787e607ea3478032e371bc2e3b4a`  
		Last Modified: Tue, 05 Apr 2022 09:53:21 GMT  
		Size: 779.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24aadd9789eb1a5c08f2a46b940b8e2434821b46a23ae93c5b2359ec9ef114b8`  
		Last Modified: Tue, 05 Apr 2022 09:53:55 GMT  
		Size: 92.4 MB (92350778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be21a2cd030e2f3b791bbf84f4435d7d3472c80073ea04cb7e9d8dd26e2f788`  
		Last Modified: Tue, 05 Apr 2022 09:53:41 GMT  
		Size: 332.0 B  
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
$ docker pull znc@sha256:c6d447bbea70f29ad2a600e3a8907716055eaa880427308021c52efa8e09d5b2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.8 MB (129834992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e473da2811571b93ddae9179ce428094469ebeb2fd648da249eba0c1f77bc2f`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:29:56 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 05 Apr 2022 07:29:57 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 05 Apr 2022 07:29:58 GMT
ARG MAKEFLAGS=
# Tue, 05 Apr 2022 07:29:59 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 05 Apr 2022 07:34:54 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 05 Apr 2022 07:34:55 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 05 Apr 2022 07:34:56 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 05 Apr 2022 07:34:56 GMT
VOLUME [/znc-data]
# Tue, 05 Apr 2022 07:34:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 07:35:15 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         openssl-dev         perl         python3
# Tue, 05 Apr 2022 07:35:16 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dade73c52ca649762693df12f39ec02756dee14e05c0864b24c4e97d97ad958d`  
		Last Modified: Tue, 05 Apr 2022 07:35:41 GMT  
		Size: 43.2 MB (43215389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bb3daa38da11139453d050715189241689eec49f348a62c35ef5c21cec730c`  
		Last Modified: Tue, 05 Apr 2022 07:35:35 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd345777189eda27551fcbf74799e48aeae6e50a81c2c18094733269e194b27f`  
		Last Modified: Tue, 05 Apr 2022 07:35:35 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0836f1c9f8e456a0a341ff8d4d1264de2900bc1d75304f4a82f982860106d4a`  
		Last Modified: Tue, 05 Apr 2022 07:36:08 GMT  
		Size: 83.9 MB (83897447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0017b43534c99c2fcda22306680b36735beae0ff8a5e5ff1395eeca4dfa7fce4`  
		Last Modified: Tue, 05 Apr 2022 07:35:55 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:slim`

```console
$ docker pull znc@sha256:fce567a092da99f64d0c6613c6bfdbcc11921625a075e9c326a75883e2ab8549
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:slim` - linux; amd64

```console
$ docker pull znc@sha256:f0d779f1617c118f1d98575fb998679f3cd5901bd241c47aef4ef3ab31625f10
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46179946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea8f882dfd1f0cf37e6c3fb28c02976c45684c72e99747b19ebaff793138f59a`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:48:39 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 05 Apr 2022 09:48:39 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 05 Apr 2022 09:48:39 GMT
ARG MAKEFLAGS=
# Tue, 05 Apr 2022 09:48:39 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 05 Apr 2022 09:52:48 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 05 Apr 2022 09:52:48 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 05 Apr 2022 09:52:48 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 05 Apr 2022 09:52:48 GMT
VOLUME [/znc-data]
# Tue, 05 Apr 2022 09:52:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693ec67bc9a4a27a226ff63cd00eebfbc7e260c941b6398f57077617f8e18c90`  
		Last Modified: Tue, 05 Apr 2022 09:53:28 GMT  
		Size: 43.4 MB (43359682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8836528fad5890b023c4922fd7ebb55e54defd216ce7e4d065e735ed2e4b945b`  
		Last Modified: Tue, 05 Apr 2022 09:53:21 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47389a434a5f45e32c1b75051f48dc931a3787e607ea3478032e371bc2e3b4a`  
		Last Modified: Tue, 05 Apr 2022 09:53:21 GMT  
		Size: 779.0 B  
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
$ docker pull znc@sha256:af54eb8d2daf30393055c61060bc0bf7681e74efedb04d19c3bfe3c21fe295d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45937214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b780f2769519718faed55bc70d10abecc7ad3084e24e2527b6c1801a552d9e1b`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:29:56 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Tue, 05 Apr 2022 07:29:57 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Tue, 05 Apr 2022 07:29:58 GMT
ARG MAKEFLAGS=
# Tue, 05 Apr 2022 07:29:59 GMT
ENV ZNC_VERSION=1.8.2
# Tue, 05 Apr 2022 07:34:54 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Tue, 05 Apr 2022 07:34:55 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Tue, 05 Apr 2022 07:34:56 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Tue, 05 Apr 2022 07:34:56 GMT
VOLUME [/znc-data]
# Tue, 05 Apr 2022 07:34:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dade73c52ca649762693df12f39ec02756dee14e05c0864b24c4e97d97ad958d`  
		Last Modified: Tue, 05 Apr 2022 07:35:41 GMT  
		Size: 43.2 MB (43215389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bb3daa38da11139453d050715189241689eec49f348a62c35ef5c21cec730c`  
		Last Modified: Tue, 05 Apr 2022 07:35:35 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd345777189eda27551fcbf74799e48aeae6e50a81c2c18094733269e194b27f`  
		Last Modified: Tue, 05 Apr 2022 07:35:35 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
