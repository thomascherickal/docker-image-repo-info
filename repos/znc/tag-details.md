<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `znc`

-	[`znc:1.7`](#znc17)
-	[`znc:1.7.5`](#znc175)
-	[`znc:1.7.5-slim`](#znc175-slim)
-	[`znc:1.7-slim`](#znc17-slim)
-	[`znc:latest`](#znclatest)
-	[`znc:slim`](#zncslim)

## `znc:1.7`

```console
$ docker pull znc@sha256:4414e15dd4519327fe1d80eaf046ccfaec7c0d52a5700013449d755348978c6d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.7` - linux; amd64

```console
$ docker pull znc@sha256:792086307563b65168174df9db9fc1248ca342439a1f2c2e558d3cddc7793d59
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.0 MB (141035369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9846126f9a1644eac75ca66a376fceb1ed1cd2907da04d5b026fd27a62f8df2`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 06:03:41 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Fri, 24 Jan 2020 06:03:42 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Fri, 24 Jan 2020 06:03:42 GMT
ARG MAKEFLAGS=
# Fri, 24 Jan 2020 06:03:42 GMT
ENV ZNC_VERSION=1.7.5
# Fri, 24 Jan 2020 06:09:40 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Fri, 24 Jan 2020 06:09:42 GMT
VOLUME [/znc-data]
# Fri, 24 Jan 2020 06:09:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Jan 2020 06:10:09 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Fri, 24 Jan 2020 06:10:09 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d431a7a850a5f025178c3f777f5088d9b146ee379cb5d825a5c8a9f60fa33f3`  
		Last Modified: Fri, 24 Jan 2020 06:10:58 GMT  
		Size: 57.2 MB (57150897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeac081eeec39f38f5555ba19b6e37545ee73d545b5c130b85958178481d75e3`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ce8bd72a7bafeeb0c4f3d839bd97e139d9dae2d46aa7457128c81ad9ee8f5c`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77728f03247ad0f4eda096aafd7cebfbf697a71fbb345f46f2023acdf6b3b885`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3946d71a165cf02480f9040255c376da9a9f1df968ca958886bd6f57edb318`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21228b04c92627db7b8d28dfc3932db82bddb24cdf469656de9412d4383012c`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f3fbaa1b2909e9c3f05cd072414687b6fa6fe3b00cc8eacc2b75d702519ade`  
		Last Modified: Fri, 24 Jan 2020 06:11:27 GMT  
		Size: 81.1 MB (81095782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1c012f32f3cc925b0da06af80edb5df381684225b31882305cb5807e608b80`  
		Last Modified: Fri, 24 Jan 2020 06:11:04 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.7` - linux; arm variant v6

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

### `znc:1.7` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:8497a8aeeda6b0730266cdbcfc425424353908d3d0ce163e402d647c8fd6b6b7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133123411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcdc8b15ffcba76c2fe2f09927b76a88c106b03ce2b3807982f8ad61379190f7`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 23:29:58 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 23 Jan 2020 23:29:59 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 23 Jan 2020 23:30:00 GMT
ARG MAKEFLAGS=
# Thu, 23 Jan 2020 23:30:01 GMT
ENV ZNC_VERSION=1.7.5
# Thu, 23 Jan 2020 23:39:17 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 23 Jan 2020 23:39:20 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 23 Jan 2020 23:39:21 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 23 Jan 2020 23:39:21 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 23 Jan 2020 23:39:22 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 23 Jan 2020 23:39:22 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 23 Jan 2020 23:39:23 GMT
VOLUME [/znc-data]
# Thu, 23 Jan 2020 23:39:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jan 2020 23:39:48 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Thu, 23 Jan 2020 23:39:50 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3b47418bf3a6e5d2778b748061c50a7518c6554c0d3ec81d6d608530d78679`  
		Last Modified: Thu, 23 Jan 2020 23:40:25 GMT  
		Size: 57.1 MB (57144077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f98e527749796085630187d3f964dd3718db09ff97587fdc5195f68795e9b92`  
		Last Modified: Thu, 23 Jan 2020 23:40:00 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d580c323b6dee1733c0c7210d8e203b178782bf67bea74d779ce609e775b6d6a`  
		Last Modified: Thu, 23 Jan 2020 23:40:01 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8d290025141c446610989abd8ac637f56cf93cba54a50b4b2b2d37c7588afc`  
		Last Modified: Thu, 23 Jan 2020 23:40:01 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bb431ea14ba15dbea9a83c016a06a3c001c14bd48b3fd4c90e1cbbb5d81706`  
		Last Modified: Thu, 23 Jan 2020 23:40:01 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd070f6b75d343824eaf1daec8e97b268c4b16280c69285af0b51915186d4c0c`  
		Last Modified: Thu, 23 Jan 2020 23:40:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ae45375592048973050782ae12ab1805b934022f9a7fb0724f538120da267c`  
		Last Modified: Thu, 23 Jan 2020 23:40:58 GMT  
		Size: 73.3 MB (73259842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e84c297ba8f182bce571f9b95d0bf3f39844cee063d6f2f5b0ae82703005a1`  
		Last Modified: Thu, 23 Jan 2020 23:40:33 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.7.5`

```console
$ docker pull znc@sha256:4414e15dd4519327fe1d80eaf046ccfaec7c0d52a5700013449d755348978c6d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.7.5` - linux; amd64

```console
$ docker pull znc@sha256:792086307563b65168174df9db9fc1248ca342439a1f2c2e558d3cddc7793d59
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.0 MB (141035369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9846126f9a1644eac75ca66a376fceb1ed1cd2907da04d5b026fd27a62f8df2`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 06:03:41 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Fri, 24 Jan 2020 06:03:42 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Fri, 24 Jan 2020 06:03:42 GMT
ARG MAKEFLAGS=
# Fri, 24 Jan 2020 06:03:42 GMT
ENV ZNC_VERSION=1.7.5
# Fri, 24 Jan 2020 06:09:40 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Fri, 24 Jan 2020 06:09:42 GMT
VOLUME [/znc-data]
# Fri, 24 Jan 2020 06:09:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Jan 2020 06:10:09 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Fri, 24 Jan 2020 06:10:09 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d431a7a850a5f025178c3f777f5088d9b146ee379cb5d825a5c8a9f60fa33f3`  
		Last Modified: Fri, 24 Jan 2020 06:10:58 GMT  
		Size: 57.2 MB (57150897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeac081eeec39f38f5555ba19b6e37545ee73d545b5c130b85958178481d75e3`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ce8bd72a7bafeeb0c4f3d839bd97e139d9dae2d46aa7457128c81ad9ee8f5c`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77728f03247ad0f4eda096aafd7cebfbf697a71fbb345f46f2023acdf6b3b885`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3946d71a165cf02480f9040255c376da9a9f1df968ca958886bd6f57edb318`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21228b04c92627db7b8d28dfc3932db82bddb24cdf469656de9412d4383012c`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f3fbaa1b2909e9c3f05cd072414687b6fa6fe3b00cc8eacc2b75d702519ade`  
		Last Modified: Fri, 24 Jan 2020 06:11:27 GMT  
		Size: 81.1 MB (81095782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1c012f32f3cc925b0da06af80edb5df381684225b31882305cb5807e608b80`  
		Last Modified: Fri, 24 Jan 2020 06:11:04 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.7.5` - linux; arm variant v6

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

### `znc:1.7.5` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:8497a8aeeda6b0730266cdbcfc425424353908d3d0ce163e402d647c8fd6b6b7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133123411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcdc8b15ffcba76c2fe2f09927b76a88c106b03ce2b3807982f8ad61379190f7`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 23:29:58 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 23 Jan 2020 23:29:59 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 23 Jan 2020 23:30:00 GMT
ARG MAKEFLAGS=
# Thu, 23 Jan 2020 23:30:01 GMT
ENV ZNC_VERSION=1.7.5
# Thu, 23 Jan 2020 23:39:17 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 23 Jan 2020 23:39:20 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 23 Jan 2020 23:39:21 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 23 Jan 2020 23:39:21 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 23 Jan 2020 23:39:22 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 23 Jan 2020 23:39:22 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 23 Jan 2020 23:39:23 GMT
VOLUME [/znc-data]
# Thu, 23 Jan 2020 23:39:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jan 2020 23:39:48 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Thu, 23 Jan 2020 23:39:50 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3b47418bf3a6e5d2778b748061c50a7518c6554c0d3ec81d6d608530d78679`  
		Last Modified: Thu, 23 Jan 2020 23:40:25 GMT  
		Size: 57.1 MB (57144077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f98e527749796085630187d3f964dd3718db09ff97587fdc5195f68795e9b92`  
		Last Modified: Thu, 23 Jan 2020 23:40:00 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d580c323b6dee1733c0c7210d8e203b178782bf67bea74d779ce609e775b6d6a`  
		Last Modified: Thu, 23 Jan 2020 23:40:01 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8d290025141c446610989abd8ac637f56cf93cba54a50b4b2b2d37c7588afc`  
		Last Modified: Thu, 23 Jan 2020 23:40:01 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bb431ea14ba15dbea9a83c016a06a3c001c14bd48b3fd4c90e1cbbb5d81706`  
		Last Modified: Thu, 23 Jan 2020 23:40:01 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd070f6b75d343824eaf1daec8e97b268c4b16280c69285af0b51915186d4c0c`  
		Last Modified: Thu, 23 Jan 2020 23:40:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ae45375592048973050782ae12ab1805b934022f9a7fb0724f538120da267c`  
		Last Modified: Thu, 23 Jan 2020 23:40:58 GMT  
		Size: 73.3 MB (73259842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e84c297ba8f182bce571f9b95d0bf3f39844cee063d6f2f5b0ae82703005a1`  
		Last Modified: Thu, 23 Jan 2020 23:40:33 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.7.5-slim`

```console
$ docker pull znc@sha256:6109e72e9a5b7305401f3ffdb4b373908370cf8768d7e1902bc3fb621e3dfceb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.7.5-slim` - linux; amd64

```console
$ docker pull znc@sha256:3c2cbac1a82f36f276f3ccc843d0cbc1fe16fb5ce0194a9347ee7a14fa60607b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.9 MB (59939255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:420c0449430d73bd88c79ff68ee3131d81e8d0d785adb5f9dd6ad8499f8b4770`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 06:03:41 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Fri, 24 Jan 2020 06:03:42 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Fri, 24 Jan 2020 06:03:42 GMT
ARG MAKEFLAGS=
# Fri, 24 Jan 2020 06:03:42 GMT
ENV ZNC_VERSION=1.7.5
# Fri, 24 Jan 2020 06:09:40 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Fri, 24 Jan 2020 06:09:42 GMT
VOLUME [/znc-data]
# Fri, 24 Jan 2020 06:09:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d431a7a850a5f025178c3f777f5088d9b146ee379cb5d825a5c8a9f60fa33f3`  
		Last Modified: Fri, 24 Jan 2020 06:10:58 GMT  
		Size: 57.2 MB (57150897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeac081eeec39f38f5555ba19b6e37545ee73d545b5c130b85958178481d75e3`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ce8bd72a7bafeeb0c4f3d839bd97e139d9dae2d46aa7457128c81ad9ee8f5c`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77728f03247ad0f4eda096aafd7cebfbf697a71fbb345f46f2023acdf6b3b885`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3946d71a165cf02480f9040255c376da9a9f1df968ca958886bd6f57edb318`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21228b04c92627db7b8d28dfc3932db82bddb24cdf469656de9412d4383012c`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.7.5-slim` - linux; arm variant v6

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

### `znc:1.7.5-slim` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:2d791daf77b0ec3743ae12731cb423aba4c48e7743481bc12b21b34c2776facc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.9 MB (59863236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0e7494f9262f95486f18b0ab94683bc768e380ede8e1983de45c4136feb024c`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 23:29:58 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 23 Jan 2020 23:29:59 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 23 Jan 2020 23:30:00 GMT
ARG MAKEFLAGS=
# Thu, 23 Jan 2020 23:30:01 GMT
ENV ZNC_VERSION=1.7.5
# Thu, 23 Jan 2020 23:39:17 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 23 Jan 2020 23:39:20 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 23 Jan 2020 23:39:21 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 23 Jan 2020 23:39:21 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 23 Jan 2020 23:39:22 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 23 Jan 2020 23:39:22 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 23 Jan 2020 23:39:23 GMT
VOLUME [/znc-data]
# Thu, 23 Jan 2020 23:39:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3b47418bf3a6e5d2778b748061c50a7518c6554c0d3ec81d6d608530d78679`  
		Last Modified: Thu, 23 Jan 2020 23:40:25 GMT  
		Size: 57.1 MB (57144077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f98e527749796085630187d3f964dd3718db09ff97587fdc5195f68795e9b92`  
		Last Modified: Thu, 23 Jan 2020 23:40:00 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d580c323b6dee1733c0c7210d8e203b178782bf67bea74d779ce609e775b6d6a`  
		Last Modified: Thu, 23 Jan 2020 23:40:01 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8d290025141c446610989abd8ac637f56cf93cba54a50b4b2b2d37c7588afc`  
		Last Modified: Thu, 23 Jan 2020 23:40:01 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bb431ea14ba15dbea9a83c016a06a3c001c14bd48b3fd4c90e1cbbb5d81706`  
		Last Modified: Thu, 23 Jan 2020 23:40:01 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd070f6b75d343824eaf1daec8e97b268c4b16280c69285af0b51915186d4c0c`  
		Last Modified: Thu, 23 Jan 2020 23:40:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.7-slim`

```console
$ docker pull znc@sha256:6109e72e9a5b7305401f3ffdb4b373908370cf8768d7e1902bc3fb621e3dfceb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.7-slim` - linux; amd64

```console
$ docker pull znc@sha256:3c2cbac1a82f36f276f3ccc843d0cbc1fe16fb5ce0194a9347ee7a14fa60607b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.9 MB (59939255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:420c0449430d73bd88c79ff68ee3131d81e8d0d785adb5f9dd6ad8499f8b4770`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 06:03:41 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Fri, 24 Jan 2020 06:03:42 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Fri, 24 Jan 2020 06:03:42 GMT
ARG MAKEFLAGS=
# Fri, 24 Jan 2020 06:03:42 GMT
ENV ZNC_VERSION=1.7.5
# Fri, 24 Jan 2020 06:09:40 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Fri, 24 Jan 2020 06:09:42 GMT
VOLUME [/znc-data]
# Fri, 24 Jan 2020 06:09:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d431a7a850a5f025178c3f777f5088d9b146ee379cb5d825a5c8a9f60fa33f3`  
		Last Modified: Fri, 24 Jan 2020 06:10:58 GMT  
		Size: 57.2 MB (57150897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeac081eeec39f38f5555ba19b6e37545ee73d545b5c130b85958178481d75e3`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ce8bd72a7bafeeb0c4f3d839bd97e139d9dae2d46aa7457128c81ad9ee8f5c`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77728f03247ad0f4eda096aafd7cebfbf697a71fbb345f46f2023acdf6b3b885`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3946d71a165cf02480f9040255c376da9a9f1df968ca958886bd6f57edb318`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21228b04c92627db7b8d28dfc3932db82bddb24cdf469656de9412d4383012c`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.7-slim` - linux; arm variant v6

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

### `znc:1.7-slim` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:2d791daf77b0ec3743ae12731cb423aba4c48e7743481bc12b21b34c2776facc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.9 MB (59863236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0e7494f9262f95486f18b0ab94683bc768e380ede8e1983de45c4136feb024c`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 23:29:58 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 23 Jan 2020 23:29:59 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 23 Jan 2020 23:30:00 GMT
ARG MAKEFLAGS=
# Thu, 23 Jan 2020 23:30:01 GMT
ENV ZNC_VERSION=1.7.5
# Thu, 23 Jan 2020 23:39:17 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 23 Jan 2020 23:39:20 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 23 Jan 2020 23:39:21 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 23 Jan 2020 23:39:21 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 23 Jan 2020 23:39:22 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 23 Jan 2020 23:39:22 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 23 Jan 2020 23:39:23 GMT
VOLUME [/znc-data]
# Thu, 23 Jan 2020 23:39:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3b47418bf3a6e5d2778b748061c50a7518c6554c0d3ec81d6d608530d78679`  
		Last Modified: Thu, 23 Jan 2020 23:40:25 GMT  
		Size: 57.1 MB (57144077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f98e527749796085630187d3f964dd3718db09ff97587fdc5195f68795e9b92`  
		Last Modified: Thu, 23 Jan 2020 23:40:00 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d580c323b6dee1733c0c7210d8e203b178782bf67bea74d779ce609e775b6d6a`  
		Last Modified: Thu, 23 Jan 2020 23:40:01 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8d290025141c446610989abd8ac637f56cf93cba54a50b4b2b2d37c7588afc`  
		Last Modified: Thu, 23 Jan 2020 23:40:01 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bb431ea14ba15dbea9a83c016a06a3c001c14bd48b3fd4c90e1cbbb5d81706`  
		Last Modified: Thu, 23 Jan 2020 23:40:01 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd070f6b75d343824eaf1daec8e97b268c4b16280c69285af0b51915186d4c0c`  
		Last Modified: Thu, 23 Jan 2020 23:40:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:latest`

```console
$ docker pull znc@sha256:4414e15dd4519327fe1d80eaf046ccfaec7c0d52a5700013449d755348978c6d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:latest` - linux; amd64

```console
$ docker pull znc@sha256:792086307563b65168174df9db9fc1248ca342439a1f2c2e558d3cddc7793d59
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.0 MB (141035369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9846126f9a1644eac75ca66a376fceb1ed1cd2907da04d5b026fd27a62f8df2`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 06:03:41 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Fri, 24 Jan 2020 06:03:42 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Fri, 24 Jan 2020 06:03:42 GMT
ARG MAKEFLAGS=
# Fri, 24 Jan 2020 06:03:42 GMT
ENV ZNC_VERSION=1.7.5
# Fri, 24 Jan 2020 06:09:40 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Fri, 24 Jan 2020 06:09:42 GMT
VOLUME [/znc-data]
# Fri, 24 Jan 2020 06:09:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Jan 2020 06:10:09 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Fri, 24 Jan 2020 06:10:09 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d431a7a850a5f025178c3f777f5088d9b146ee379cb5d825a5c8a9f60fa33f3`  
		Last Modified: Fri, 24 Jan 2020 06:10:58 GMT  
		Size: 57.2 MB (57150897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeac081eeec39f38f5555ba19b6e37545ee73d545b5c130b85958178481d75e3`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ce8bd72a7bafeeb0c4f3d839bd97e139d9dae2d46aa7457128c81ad9ee8f5c`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77728f03247ad0f4eda096aafd7cebfbf697a71fbb345f46f2023acdf6b3b885`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3946d71a165cf02480f9040255c376da9a9f1df968ca958886bd6f57edb318`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21228b04c92627db7b8d28dfc3932db82bddb24cdf469656de9412d4383012c`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f3fbaa1b2909e9c3f05cd072414687b6fa6fe3b00cc8eacc2b75d702519ade`  
		Last Modified: Fri, 24 Jan 2020 06:11:27 GMT  
		Size: 81.1 MB (81095782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1c012f32f3cc925b0da06af80edb5df381684225b31882305cb5807e608b80`  
		Last Modified: Fri, 24 Jan 2020 06:11:04 GMT  
		Size: 332.0 B  
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
$ docker pull znc@sha256:8497a8aeeda6b0730266cdbcfc425424353908d3d0ce163e402d647c8fd6b6b7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133123411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcdc8b15ffcba76c2fe2f09927b76a88c106b03ce2b3807982f8ad61379190f7`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 23:29:58 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 23 Jan 2020 23:29:59 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 23 Jan 2020 23:30:00 GMT
ARG MAKEFLAGS=
# Thu, 23 Jan 2020 23:30:01 GMT
ENV ZNC_VERSION=1.7.5
# Thu, 23 Jan 2020 23:39:17 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 23 Jan 2020 23:39:20 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 23 Jan 2020 23:39:21 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 23 Jan 2020 23:39:21 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 23 Jan 2020 23:39:22 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 23 Jan 2020 23:39:22 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 23 Jan 2020 23:39:23 GMT
VOLUME [/znc-data]
# Thu, 23 Jan 2020 23:39:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jan 2020 23:39:48 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Thu, 23 Jan 2020 23:39:50 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3b47418bf3a6e5d2778b748061c50a7518c6554c0d3ec81d6d608530d78679`  
		Last Modified: Thu, 23 Jan 2020 23:40:25 GMT  
		Size: 57.1 MB (57144077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f98e527749796085630187d3f964dd3718db09ff97587fdc5195f68795e9b92`  
		Last Modified: Thu, 23 Jan 2020 23:40:00 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d580c323b6dee1733c0c7210d8e203b178782bf67bea74d779ce609e775b6d6a`  
		Last Modified: Thu, 23 Jan 2020 23:40:01 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8d290025141c446610989abd8ac637f56cf93cba54a50b4b2b2d37c7588afc`  
		Last Modified: Thu, 23 Jan 2020 23:40:01 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bb431ea14ba15dbea9a83c016a06a3c001c14bd48b3fd4c90e1cbbb5d81706`  
		Last Modified: Thu, 23 Jan 2020 23:40:01 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd070f6b75d343824eaf1daec8e97b268c4b16280c69285af0b51915186d4c0c`  
		Last Modified: Thu, 23 Jan 2020 23:40:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ae45375592048973050782ae12ab1805b934022f9a7fb0724f538120da267c`  
		Last Modified: Thu, 23 Jan 2020 23:40:58 GMT  
		Size: 73.3 MB (73259842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e84c297ba8f182bce571f9b95d0bf3f39844cee063d6f2f5b0ae82703005a1`  
		Last Modified: Thu, 23 Jan 2020 23:40:33 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:slim`

```console
$ docker pull znc@sha256:6109e72e9a5b7305401f3ffdb4b373908370cf8768d7e1902bc3fb621e3dfceb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:slim` - linux; amd64

```console
$ docker pull znc@sha256:3c2cbac1a82f36f276f3ccc843d0cbc1fe16fb5ce0194a9347ee7a14fa60607b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.9 MB (59939255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:420c0449430d73bd88c79ff68ee3131d81e8d0d785adb5f9dd6ad8499f8b4770`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 06:03:41 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Fri, 24 Jan 2020 06:03:42 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Fri, 24 Jan 2020 06:03:42 GMT
ARG MAKEFLAGS=
# Fri, 24 Jan 2020 06:03:42 GMT
ENV ZNC_VERSION=1.7.5
# Fri, 24 Jan 2020 06:09:40 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Fri, 24 Jan 2020 06:09:41 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Fri, 24 Jan 2020 06:09:42 GMT
VOLUME [/znc-data]
# Fri, 24 Jan 2020 06:09:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d431a7a850a5f025178c3f777f5088d9b146ee379cb5d825a5c8a9f60fa33f3`  
		Last Modified: Fri, 24 Jan 2020 06:10:58 GMT  
		Size: 57.2 MB (57150897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeac081eeec39f38f5555ba19b6e37545ee73d545b5c130b85958178481d75e3`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ce8bd72a7bafeeb0c4f3d839bd97e139d9dae2d46aa7457128c81ad9ee8f5c`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77728f03247ad0f4eda096aafd7cebfbf697a71fbb345f46f2023acdf6b3b885`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3946d71a165cf02480f9040255c376da9a9f1df968ca958886bd6f57edb318`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21228b04c92627db7b8d28dfc3932db82bddb24cdf469656de9412d4383012c`  
		Last Modified: Fri, 24 Jan 2020 06:10:20 GMT  
		Size: 339.0 B  
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
$ docker pull znc@sha256:2d791daf77b0ec3743ae12731cb423aba4c48e7743481bc12b21b34c2776facc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.9 MB (59863236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0e7494f9262f95486f18b0ab94683bc768e380ede8e1983de45c4136feb024c`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 23:29:58 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 23 Jan 2020 23:29:59 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 23 Jan 2020 23:30:00 GMT
ARG MAKEFLAGS=
# Thu, 23 Jan 2020 23:30:01 GMT
ENV ZNC_VERSION=1.7.5
# Thu, 23 Jan 2020 23:39:17 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 23 Jan 2020 23:39:20 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 23 Jan 2020 23:39:21 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 23 Jan 2020 23:39:21 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 23 Jan 2020 23:39:22 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 23 Jan 2020 23:39:22 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 23 Jan 2020 23:39:23 GMT
VOLUME [/znc-data]
# Thu, 23 Jan 2020 23:39:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3b47418bf3a6e5d2778b748061c50a7518c6554c0d3ec81d6d608530d78679`  
		Last Modified: Thu, 23 Jan 2020 23:40:25 GMT  
		Size: 57.1 MB (57144077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f98e527749796085630187d3f964dd3718db09ff97587fdc5195f68795e9b92`  
		Last Modified: Thu, 23 Jan 2020 23:40:00 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d580c323b6dee1733c0c7210d8e203b178782bf67bea74d779ce609e775b6d6a`  
		Last Modified: Thu, 23 Jan 2020 23:40:01 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8d290025141c446610989abd8ac637f56cf93cba54a50b4b2b2d37c7588afc`  
		Last Modified: Thu, 23 Jan 2020 23:40:01 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bb431ea14ba15dbea9a83c016a06a3c001c14bd48b3fd4c90e1cbbb5d81706`  
		Last Modified: Thu, 23 Jan 2020 23:40:01 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd070f6b75d343824eaf1daec8e97b268c4b16280c69285af0b51915186d4c0c`  
		Last Modified: Thu, 23 Jan 2020 23:40:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
