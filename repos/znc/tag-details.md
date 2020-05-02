<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `znc`

-	[`znc:1.8`](#znc18)
-	[`znc:1.8.0`](#znc180)
-	[`znc:1.8.0-slim`](#znc180-slim)
-	[`znc:1.8-slim`](#znc18-slim)
-	[`znc:latest`](#znclatest)
-	[`znc:slim`](#zncslim)

## `znc:1.8`

```console
$ docker pull znc@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `znc:1.8.0`

```console
$ docker pull znc@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `znc:1.8.0-slim`

```console
$ docker pull znc@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `znc:1.8-slim`

```console
$ docker pull znc@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `znc:latest`

```console
$ docker pull znc@sha256:5998921e2ee9623dda3dab3a1418b1ac13a1e6b89f4637c3241c98424448cef2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:latest` - linux; amd64

```console
$ docker pull znc@sha256:33a0d224e9cfe670b31f2c984a9f1fd019cb5086073e99e0b1d4fdddf32cfb84
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.5 MB (140548151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5277a89190339af2aa249a091ab62b4b6098e4e8b39ccf0a683000c98572f1ce`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:08:05 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Fri, 24 Apr 2020 14:08:06 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Fri, 24 Apr 2020 14:08:06 GMT
ARG MAKEFLAGS=
# Fri, 24 Apr 2020 14:08:06 GMT
ENV ZNC_VERSION=1.7.5
# Fri, 24 Apr 2020 14:12:27 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Fri, 24 Apr 2020 14:12:28 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Fri, 24 Apr 2020 14:12:28 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Fri, 24 Apr 2020 14:12:28 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Fri, 24 Apr 2020 14:12:28 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Fri, 24 Apr 2020 14:12:29 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Fri, 24 Apr 2020 14:12:29 GMT
VOLUME [/znc-data]
# Fri, 24 Apr 2020 14:12:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 14:12:44 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Fri, 24 Apr 2020 14:12:45 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3dad0d167d56a6c0f5e900fe212c4c2fc030a9c8627c197282cbff6b8d7d83a`  
		Last Modified: Fri, 24 Apr 2020 14:13:04 GMT  
		Size: 56.7 MB (56722411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1528be50b48acfd802a5604448d706bb6d45b41062fb897624e7847f28ca08f0`  
		Last Modified: Fri, 24 Apr 2020 14:12:52 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875b5944a00c14e20001f5b6b9792969ae8d3c5f44d1b01bfc9b2c9e701edbca`  
		Last Modified: Fri, 24 Apr 2020 14:12:52 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789f4b6afd28ab7cb01995a1b9059f9d4fe14dfb805dac8172121ef5826b70c1`  
		Last Modified: Fri, 24 Apr 2020 14:12:53 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e3ed9b4a01e8e680c3807562f57cfccde6bf957da799d934eb8077d7d829bb`  
		Last Modified: Fri, 24 Apr 2020 14:12:52 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c04e71b40eb1eb58fc5f84e3018378afcf5200b90a4215849e48f98da050e20`  
		Last Modified: Fri, 24 Apr 2020 14:12:52 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3812e72cea42ce4e2bc15959bdfed2c35162cecb13837b4fbab474fed64b0a3d`  
		Last Modified: Fri, 24 Apr 2020 14:13:25 GMT  
		Size: 81.0 MB (81028431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d53197ac3f15f215c5c8c1cfb645c04614956d6f2d3666986f76711ab75ce0`  
		Last Modified: Fri, 24 Apr 2020 14:13:11 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:latest` - linux; arm variant v6

```console
$ docker pull znc@sha256:10478eb842ef1f650befc3ec32be7046f2c7906565166d3d24181c88c1e196a5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.3 MB (126346994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b6a1b3be181def7fbabcfa835d9a45fa22245e874c27ab5a24e878d120ac041`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:01:48 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 23 Apr 2020 17:01:49 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 23 Apr 2020 17:01:52 GMT
ARG MAKEFLAGS=
# Thu, 23 Apr 2020 17:01:54 GMT
ENV ZNC_VERSION=1.7.5
# Thu, 23 Apr 2020 17:10:26 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 23 Apr 2020 17:10:28 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 23 Apr 2020 17:10:29 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 23 Apr 2020 17:10:29 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 23 Apr 2020 17:10:30 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 23 Apr 2020 17:10:31 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 23 Apr 2020 17:10:32 GMT
VOLUME [/znc-data]
# Thu, 23 Apr 2020 17:10:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Apr 2020 17:11:00 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Thu, 23 Apr 2020 17:11:01 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d5ba8f4a101412d5741fcf7eb44349c05e37025703987b8832d99f01b9906e`  
		Last Modified: Thu, 23 Apr 2020 17:11:36 GMT  
		Size: 54.5 MB (54508143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336b6bd99272e92d94868313aa869deba03d316418e786e1fbcbb39326616f16`  
		Last Modified: Thu, 23 Apr 2020 17:11:14 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9742ab4a215dc41698a6270fc1e628e9ddfccf2a05a303c0231dc3efcd3977da`  
		Last Modified: Thu, 23 Apr 2020 17:11:15 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e157ecf8d5183fbf30493c110e2a2967358e32d98f22131d3325b1392610cf`  
		Last Modified: Thu, 23 Apr 2020 17:11:14 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e902be260a9e209e5ca7a15a30e53ed7b3d93630adc2c16177a01f8fd6e32bb`  
		Last Modified: Thu, 23 Apr 2020 17:11:14 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943faac87cfc340bf5979cc6811f71b80b02b0f6026b605d36fbab24a9d6a389`  
		Last Modified: Thu, 23 Apr 2020 17:11:14 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409604a860f30f63dcec7b44a0bf6db342e78eac8585988991e8023bf88fa6d0`  
		Last Modified: Thu, 23 Apr 2020 17:12:15 GMT  
		Size: 69.3 MB (69264581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25194f436db7fd03c45ce8ca33a17c8d75736e38899c33583c4b0f034e59c6db`  
		Last Modified: Thu, 23 Apr 2020 17:11:47 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:latest` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:5c80a894f404aef89f5e1ac22d001285e3b767d893cca887a63e5b1b72a5247b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.6 MB (132607770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:796e1bf6227acc6d0d0d8806b9b4bdf144087cc8075025e57da0e6a3b6b2596c`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:08:01 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Fri, 24 Apr 2020 09:08:01 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Fri, 24 Apr 2020 09:08:02 GMT
ARG MAKEFLAGS=
# Fri, 24 Apr 2020 09:08:03 GMT
ENV ZNC_VERSION=1.7.5
# Fri, 24 Apr 2020 09:16:37 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Fri, 24 Apr 2020 09:16:40 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Fri, 24 Apr 2020 09:16:41 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Fri, 24 Apr 2020 09:16:42 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Fri, 24 Apr 2020 09:16:42 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Fri, 24 Apr 2020 09:16:43 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Fri, 24 Apr 2020 09:16:44 GMT
VOLUME [/znc-data]
# Fri, 24 Apr 2020 09:16:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 09:17:09 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Fri, 24 Apr 2020 09:17:11 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b035ab36231c4d955a39ef3bd413d365f51688f5f3b2b8679ed316e3b3c24c`  
		Last Modified: Fri, 24 Apr 2020 09:17:42 GMT  
		Size: 56.7 MB (56711465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760889cb92fbe71f1cf7f577b2b70c383074f659247850d8851964f9a3d49f6c`  
		Last Modified: Fri, 24 Apr 2020 09:17:22 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10126c6822d6054799bddd5fdc67392c45d329f8e901729acc1843876c2144a9`  
		Last Modified: Fri, 24 Apr 2020 09:17:23 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803818fcf03e17847483742475dda1b8cb397dbfe0cc69d9b794c3f3eeb315c8`  
		Last Modified: Fri, 24 Apr 2020 09:17:22 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b12388b4c3bcc4dc5ad7f89185ac5581b13771280c956f8946ce5444d273c7`  
		Last Modified: Fri, 24 Apr 2020 09:17:22 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a55ad710465db5d6cc6d4dd5f8a8306fda039b75ee5dbec5f75f117592d3f7`  
		Last Modified: Fri, 24 Apr 2020 09:17:22 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:085c2f3db3b140ed9836dbd7f27885c47c669ca36549b4e1f80d2ed6937f2fc2`  
		Last Modified: Fri, 24 Apr 2020 09:18:20 GMT  
		Size: 73.2 MB (73175817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62005a15d72370ccedce3f6596de90142a43610e125d6ace39e5c8ad86009e81`  
		Last Modified: Fri, 24 Apr 2020 09:17:55 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:slim`

```console
$ docker pull znc@sha256:72dce40e5221d5f9a72e5a143c196a49af1b955f3ad442d170e9eb34f721c950
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:slim` - linux; amd64

```console
$ docker pull znc@sha256:274127c4173d07be36323b165435516afbfb9d3fee5d0d5666274aa34bace58e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59519389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:781e78c0401709999cde80e1ebe08a1f9141f2b522e7c775313af3933979f2cf`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:08:05 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Fri, 24 Apr 2020 14:08:06 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Fri, 24 Apr 2020 14:08:06 GMT
ARG MAKEFLAGS=
# Fri, 24 Apr 2020 14:08:06 GMT
ENV ZNC_VERSION=1.7.5
# Fri, 24 Apr 2020 14:12:27 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Fri, 24 Apr 2020 14:12:28 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Fri, 24 Apr 2020 14:12:28 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Fri, 24 Apr 2020 14:12:28 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Fri, 24 Apr 2020 14:12:28 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Fri, 24 Apr 2020 14:12:29 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Fri, 24 Apr 2020 14:12:29 GMT
VOLUME [/znc-data]
# Fri, 24 Apr 2020 14:12:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3dad0d167d56a6c0f5e900fe212c4c2fc030a9c8627c197282cbff6b8d7d83a`  
		Last Modified: Fri, 24 Apr 2020 14:13:04 GMT  
		Size: 56.7 MB (56722411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1528be50b48acfd802a5604448d706bb6d45b41062fb897624e7847f28ca08f0`  
		Last Modified: Fri, 24 Apr 2020 14:12:52 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875b5944a00c14e20001f5b6b9792969ae8d3c5f44d1b01bfc9b2c9e701edbca`  
		Last Modified: Fri, 24 Apr 2020 14:12:52 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789f4b6afd28ab7cb01995a1b9059f9d4fe14dfb805dac8172121ef5826b70c1`  
		Last Modified: Fri, 24 Apr 2020 14:12:53 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e3ed9b4a01e8e680c3807562f57cfccde6bf957da799d934eb8077d7d829bb`  
		Last Modified: Fri, 24 Apr 2020 14:12:52 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c04e71b40eb1eb58fc5f84e3018378afcf5200b90a4215849e48f98da050e20`  
		Last Modified: Fri, 24 Apr 2020 14:12:52 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:slim` - linux; arm variant v6

```console
$ docker pull znc@sha256:b7d09fa9d23bfac547c76ca4a45fa544ad6635151da789b06219be4eeabc2938
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57082081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5b107be44905c7426ebb6a118b6a54161048000752046858e5296e95973a75e`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:01:48 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 23 Apr 2020 17:01:49 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 23 Apr 2020 17:01:52 GMT
ARG MAKEFLAGS=
# Thu, 23 Apr 2020 17:01:54 GMT
ENV ZNC_VERSION=1.7.5
# Thu, 23 Apr 2020 17:10:26 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 23 Apr 2020 17:10:28 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 23 Apr 2020 17:10:29 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 23 Apr 2020 17:10:29 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 23 Apr 2020 17:10:30 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 23 Apr 2020 17:10:31 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 23 Apr 2020 17:10:32 GMT
VOLUME [/znc-data]
# Thu, 23 Apr 2020 17:10:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d5ba8f4a101412d5741fcf7eb44349c05e37025703987b8832d99f01b9906e`  
		Last Modified: Thu, 23 Apr 2020 17:11:36 GMT  
		Size: 54.5 MB (54508143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336b6bd99272e92d94868313aa869deba03d316418e786e1fbcbb39326616f16`  
		Last Modified: Thu, 23 Apr 2020 17:11:14 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9742ab4a215dc41698a6270fc1e628e9ddfccf2a05a303c0231dc3efcd3977da`  
		Last Modified: Thu, 23 Apr 2020 17:11:15 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e157ecf8d5183fbf30493c110e2a2967358e32d98f22131d3325b1392610cf`  
		Last Modified: Thu, 23 Apr 2020 17:11:14 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e902be260a9e209e5ca7a15a30e53ed7b3d93630adc2c16177a01f8fd6e32bb`  
		Last Modified: Thu, 23 Apr 2020 17:11:14 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943faac87cfc340bf5979cc6811f71b80b02b0f6026b605d36fbab24a9d6a389`  
		Last Modified: Thu, 23 Apr 2020 17:11:14 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:slim` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:e1baa681223a3a4525878b1759f5989cc7c3fa158878cbf962ea87f7f7b05a0c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59431622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a796aa0d6f01bb84d2fe012610c6b2367f841cc2a6b96ef5251af5db939a0e5`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:08:01 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Fri, 24 Apr 2020 09:08:01 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Fri, 24 Apr 2020 09:08:02 GMT
ARG MAKEFLAGS=
# Fri, 24 Apr 2020 09:08:03 GMT
ENV ZNC_VERSION=1.7.5
# Fri, 24 Apr 2020 09:16:37 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Fri, 24 Apr 2020 09:16:40 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Fri, 24 Apr 2020 09:16:41 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Fri, 24 Apr 2020 09:16:42 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Fri, 24 Apr 2020 09:16:42 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Fri, 24 Apr 2020 09:16:43 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Fri, 24 Apr 2020 09:16:44 GMT
VOLUME [/znc-data]
# Fri, 24 Apr 2020 09:16:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b035ab36231c4d955a39ef3bd413d365f51688f5f3b2b8679ed316e3b3c24c`  
		Last Modified: Fri, 24 Apr 2020 09:17:42 GMT  
		Size: 56.7 MB (56711465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760889cb92fbe71f1cf7f577b2b70c383074f659247850d8851964f9a3d49f6c`  
		Last Modified: Fri, 24 Apr 2020 09:17:22 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10126c6822d6054799bddd5fdc67392c45d329f8e901729acc1843876c2144a9`  
		Last Modified: Fri, 24 Apr 2020 09:17:23 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803818fcf03e17847483742475dda1b8cb397dbfe0cc69d9b794c3f3eeb315c8`  
		Last Modified: Fri, 24 Apr 2020 09:17:22 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b12388b4c3bcc4dc5ad7f89185ac5581b13771280c956f8946ce5444d273c7`  
		Last Modified: Fri, 24 Apr 2020 09:17:22 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a55ad710465db5d6cc6d4dd5f8a8306fda039b75ee5dbec5f75f117592d3f7`  
		Last Modified: Fri, 24 Apr 2020 09:17:22 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
