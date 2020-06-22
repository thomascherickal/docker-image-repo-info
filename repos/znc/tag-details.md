<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `znc`

-	[`znc:1.8`](#znc18)
-	[`znc:1.8.1`](#znc181)
-	[`znc:1.8.1-slim`](#znc181-slim)
-	[`znc:1.8-slim`](#znc18-slim)
-	[`znc:latest`](#znclatest)
-	[`znc:slim`](#zncslim)

## `znc:1.8`

```console
$ docker pull znc@sha256:654eccd63c1f57638acc488c46a42cd9c51a253b142541479563d39d444b3d23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8` - linux; amd64

```console
$ docker pull znc@sha256:f05fa99cf91c247467afad3c0ad3fd262a6f8f27fccc36a8446837db52f3e6c0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.5 MB (145467376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:296c6bf2e7b733563835673ce63565322b6186e1049e6634d8dbc0f3f8df1f86`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Mon, 04 May 2020 19:22:11 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 04 May 2020 19:22:11 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 04 May 2020 19:22:11 GMT
ARG MAKEFLAGS=
# Mon, 08 Jun 2020 18:25:56 GMT
ENV ZNC_VERSION=1.8.1
# Mon, 08 Jun 2020 18:30:18 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 08 Jun 2020 18:30:18 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 08 Jun 2020 18:30:18 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:30:19 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:30:19 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Mon, 08 Jun 2020 18:30:19 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:30:19 GMT
VOLUME [/znc-data]
# Mon, 08 Jun 2020 18:30:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 08 Jun 2020 18:30:35 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Mon, 08 Jun 2020 18:30:35 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5a1332069b5686f2953370c761c60ad203b22a4b5d907cddabd5e3766aa49b`  
		Last Modified: Mon, 08 Jun 2020 18:30:56 GMT  
		Size: 57.4 MB (57402945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a3efef78d5bed01124912e52f0e3a0779a6345f5b42c17788d65c978ea7bb7`  
		Last Modified: Mon, 08 Jun 2020 18:30:43 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c3f10758cc9042e43fb6abf244903f8ba5a9dc2a669a9a30b95dc589d21087`  
		Last Modified: Mon, 08 Jun 2020 18:30:43 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83dd650d49b861285b5f22ebeb69e7cf2ef5c693e0648c22b4b78d960a91a9dc`  
		Last Modified: Mon, 08 Jun 2020 18:30:43 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee9947bd59b5d71c18d40c71849c7ed7540188da416129ac186d78cd18b0714`  
		Last Modified: Mon, 08 Jun 2020 18:30:43 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ec4d8b8066c8edda8b14884cea78384b3245fc8ff088524fee89c3409d3389`  
		Last Modified: Mon, 08 Jun 2020 18:30:43 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7115798da545f00a3b605b09ecee681bab84bb9f2a5aa910306504c5fcdf758c`  
		Last Modified: Mon, 08 Jun 2020 18:31:16 GMT  
		Size: 85.2 MB (85249387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82542bfc7155c7556a2ef1fc164c34f30eaf31d36613e32107c0fd122756a45c`  
		Last Modified: Mon, 08 Jun 2020 18:31:01 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8` - linux; arm variant v6

```console
$ docker pull znc@sha256:b26ae39f9e9f766b5a8409c6b6d134768efcbb3af5f0ab213ba6e77b5c57e919
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.7 MB (129651275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04f545fe3110a0e848021c888168cfbb111b180097caa391fbea942918da9ec9`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Mon, 04 May 2020 19:49:36 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 04 May 2020 19:49:37 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 04 May 2020 19:49:37 GMT
ARG MAKEFLAGS=
# Mon, 08 Jun 2020 18:50:17 GMT
ENV ZNC_VERSION=1.8.1
# Mon, 08 Jun 2020 18:58:16 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 08 Jun 2020 18:58:18 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 08 Jun 2020 18:58:18 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:58:19 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:58:19 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Mon, 08 Jun 2020 18:58:20 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:58:21 GMT
VOLUME [/znc-data]
# Mon, 08 Jun 2020 18:58:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 08 Jun 2020 18:58:41 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Mon, 08 Jun 2020 18:58:42 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5067ba1e39510a319c267902927feeafa6f8c29fd0fbdcf9c30e2230193ed28e`  
		Last Modified: Mon, 08 Jun 2020 18:59:19 GMT  
		Size: 55.6 MB (55601921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5056ada25c94f1e4dd89a015938c8f21f1365a00cd8c8ec6c7df3012fd0b67bc`  
		Last Modified: Mon, 08 Jun 2020 18:58:55 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b059d59ed64226cf083795c86c10c7635dd24e9da2e853c94731df2af4109ba2`  
		Last Modified: Mon, 08 Jun 2020 18:58:55 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78722115536a71822036c201fdc9154eb83f6586e2c8a3063e1c85e61fd3fba5`  
		Last Modified: Mon, 08 Jun 2020 18:58:56 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25bed4e5ddb5882411590ad8171ecf4985c51b870de8b03bcd8da08cddf269`  
		Last Modified: Mon, 08 Jun 2020 18:58:55 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4edc595142bdcfec0a054fb6a5263c506bda09c5c140f05bb78dc8c5f0b65c`  
		Last Modified: Mon, 08 Jun 2020 18:58:55 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832d3cbaa1292db4d7d405992435af4c58b11de75cb71fdd696e2aedc557248a`  
		Last Modified: Mon, 08 Jun 2020 18:59:54 GMT  
		Size: 71.4 MB (71427663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62123481f7168fb21c2c5ba4758f4c0070685f1fd24858f7b17e82b323ef0900`  
		Last Modified: Mon, 08 Jun 2020 18:59:27 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:9b1369022519d39413ce456ee0368eaa3a8b6720ba32d9beee434c0bb8ac5c4e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.3 MB (135289590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:036305fce5a5341a326034ee6b3a8938105ea4cde69ada975d1206a5660a4158`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Mon, 04 May 2020 19:40:23 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 04 May 2020 19:40:23 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 04 May 2020 19:40:24 GMT
ARG MAKEFLAGS=
# Mon, 08 Jun 2020 18:44:15 GMT
ENV ZNC_VERSION=1.8.1
# Mon, 08 Jun 2020 18:52:37 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 08 Jun 2020 18:52:40 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 08 Jun 2020 18:52:41 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:52:42 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:52:42 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Mon, 08 Jun 2020 18:52:43 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:52:43 GMT
VOLUME [/znc-data]
# Mon, 08 Jun 2020 18:52:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 08 Jun 2020 18:53:06 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Mon, 08 Jun 2020 18:53:09 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3887515d24b1515c28be3aeca64919edc9acbcff3321a497ba03a160633368`  
		Last Modified: Mon, 08 Jun 2020 18:53:38 GMT  
		Size: 57.3 MB (57312408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79050300cb2ffb98537cb2cfa0f82a803c51cc89a4d952679aed84418b9efdc2`  
		Last Modified: Mon, 08 Jun 2020 18:53:20 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4a6462efa842040fc02cfab1ac30d09819cf8a70034bda884df08f50ff60e6`  
		Last Modified: Mon, 08 Jun 2020 18:53:20 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbdbcc0a36123d143db9ab73ea2025356b52af8c3f872e1e2778fba03fb46ff6`  
		Last Modified: Mon, 08 Jun 2020 18:53:20 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deeec6fca5fad8f785f3307d8fbc2886d7c9f565801eded4da2da998260812e2`  
		Last Modified: Mon, 08 Jun 2020 18:53:20 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7add17715b9f9b7f4adf7b91582039d04239311f783b7b1c8be8e52c60a97a41`  
		Last Modified: Mon, 08 Jun 2020 18:53:20 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db4a3dd149ce5b911704202d9dfa809d57303fd48fc45762642eb9d121bfc64`  
		Last Modified: Mon, 08 Jun 2020 18:54:32 GMT  
		Size: 75.3 MB (75251002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdd51f2fb833202202ffebf7fc1a469502a05c393d501702c9ea804ef2aa456`  
		Last Modified: Mon, 08 Jun 2020 18:53:47 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.8.1`

```console
$ docker pull znc@sha256:535bf20b57a614e9bd2a9c2eccc2af016844af0d48c7dd1fb2e5140037772ddd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6

### `znc:1.8.1` - linux; arm variant v6

```console
$ docker pull znc@sha256:b26ae39f9e9f766b5a8409c6b6d134768efcbb3af5f0ab213ba6e77b5c57e919
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.7 MB (129651275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04f545fe3110a0e848021c888168cfbb111b180097caa391fbea942918da9ec9`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Mon, 04 May 2020 19:49:36 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 04 May 2020 19:49:37 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 04 May 2020 19:49:37 GMT
ARG MAKEFLAGS=
# Mon, 08 Jun 2020 18:50:17 GMT
ENV ZNC_VERSION=1.8.1
# Mon, 08 Jun 2020 18:58:16 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 08 Jun 2020 18:58:18 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 08 Jun 2020 18:58:18 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:58:19 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:58:19 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Mon, 08 Jun 2020 18:58:20 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:58:21 GMT
VOLUME [/znc-data]
# Mon, 08 Jun 2020 18:58:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 08 Jun 2020 18:58:41 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Mon, 08 Jun 2020 18:58:42 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5067ba1e39510a319c267902927feeafa6f8c29fd0fbdcf9c30e2230193ed28e`  
		Last Modified: Mon, 08 Jun 2020 18:59:19 GMT  
		Size: 55.6 MB (55601921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5056ada25c94f1e4dd89a015938c8f21f1365a00cd8c8ec6c7df3012fd0b67bc`  
		Last Modified: Mon, 08 Jun 2020 18:58:55 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b059d59ed64226cf083795c86c10c7635dd24e9da2e853c94731df2af4109ba2`  
		Last Modified: Mon, 08 Jun 2020 18:58:55 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78722115536a71822036c201fdc9154eb83f6586e2c8a3063e1c85e61fd3fba5`  
		Last Modified: Mon, 08 Jun 2020 18:58:56 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25bed4e5ddb5882411590ad8171ecf4985c51b870de8b03bcd8da08cddf269`  
		Last Modified: Mon, 08 Jun 2020 18:58:55 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4edc595142bdcfec0a054fb6a5263c506bda09c5c140f05bb78dc8c5f0b65c`  
		Last Modified: Mon, 08 Jun 2020 18:58:55 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832d3cbaa1292db4d7d405992435af4c58b11de75cb71fdd696e2aedc557248a`  
		Last Modified: Mon, 08 Jun 2020 18:59:54 GMT  
		Size: 71.4 MB (71427663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62123481f7168fb21c2c5ba4758f4c0070685f1fd24858f7b17e82b323ef0900`  
		Last Modified: Mon, 08 Jun 2020 18:59:27 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.8.1-slim`

```console
$ docker pull znc@sha256:1d63f5d8ed073d1369be00da9c81f4c87fb5148ea91a4e2f9ea8ca0ffb6980bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6

### `znc:1.8.1-slim` - linux; arm variant v6

```console
$ docker pull znc@sha256:d3c7b98cfcba827ef928f67d651ae54d93f37e5ec1f4aa8da129a605ea887138
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58223280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f38881c3c3a93aa029a3112ef2c695550c6c4492b7448dc6fb745262a39ebe07`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Mon, 04 May 2020 19:49:36 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 04 May 2020 19:49:37 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 04 May 2020 19:49:37 GMT
ARG MAKEFLAGS=
# Mon, 08 Jun 2020 18:50:17 GMT
ENV ZNC_VERSION=1.8.1
# Mon, 08 Jun 2020 18:58:16 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 08 Jun 2020 18:58:18 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 08 Jun 2020 18:58:18 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:58:19 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:58:19 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Mon, 08 Jun 2020 18:58:20 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:58:21 GMT
VOLUME [/znc-data]
# Mon, 08 Jun 2020 18:58:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5067ba1e39510a319c267902927feeafa6f8c29fd0fbdcf9c30e2230193ed28e`  
		Last Modified: Mon, 08 Jun 2020 18:59:19 GMT  
		Size: 55.6 MB (55601921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5056ada25c94f1e4dd89a015938c8f21f1365a00cd8c8ec6c7df3012fd0b67bc`  
		Last Modified: Mon, 08 Jun 2020 18:58:55 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b059d59ed64226cf083795c86c10c7635dd24e9da2e853c94731df2af4109ba2`  
		Last Modified: Mon, 08 Jun 2020 18:58:55 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78722115536a71822036c201fdc9154eb83f6586e2c8a3063e1c85e61fd3fba5`  
		Last Modified: Mon, 08 Jun 2020 18:58:56 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25bed4e5ddb5882411590ad8171ecf4985c51b870de8b03bcd8da08cddf269`  
		Last Modified: Mon, 08 Jun 2020 18:58:55 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4edc595142bdcfec0a054fb6a5263c506bda09c5c140f05bb78dc8c5f0b65c`  
		Last Modified: Mon, 08 Jun 2020 18:58:55 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.8-slim`

```console
$ docker pull znc@sha256:aa772be85911a449dbfa316bd19347b378679d0e99dc4c9b55696d217ba15fc0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8-slim` - linux; amd64

```console
$ docker pull znc@sha256:befd9ba6f2781b5a6afcc0360dbc8ddaee995cbafa48e642b85e111f235425c4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.2 MB (60217659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ad09677c3e952082f8efcdf8f65d8136caefe9e75a481efefe6d5d81de6e21`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Mon, 04 May 2020 19:22:11 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 04 May 2020 19:22:11 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 04 May 2020 19:22:11 GMT
ARG MAKEFLAGS=
# Mon, 08 Jun 2020 18:25:56 GMT
ENV ZNC_VERSION=1.8.1
# Mon, 08 Jun 2020 18:30:18 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 08 Jun 2020 18:30:18 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 08 Jun 2020 18:30:18 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:30:19 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:30:19 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Mon, 08 Jun 2020 18:30:19 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:30:19 GMT
VOLUME [/znc-data]
# Mon, 08 Jun 2020 18:30:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5a1332069b5686f2953370c761c60ad203b22a4b5d907cddabd5e3766aa49b`  
		Last Modified: Mon, 08 Jun 2020 18:30:56 GMT  
		Size: 57.4 MB (57402945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a3efef78d5bed01124912e52f0e3a0779a6345f5b42c17788d65c978ea7bb7`  
		Last Modified: Mon, 08 Jun 2020 18:30:43 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c3f10758cc9042e43fb6abf244903f8ba5a9dc2a669a9a30b95dc589d21087`  
		Last Modified: Mon, 08 Jun 2020 18:30:43 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83dd650d49b861285b5f22ebeb69e7cf2ef5c693e0648c22b4b78d960a91a9dc`  
		Last Modified: Mon, 08 Jun 2020 18:30:43 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee9947bd59b5d71c18d40c71849c7ed7540188da416129ac186d78cd18b0714`  
		Last Modified: Mon, 08 Jun 2020 18:30:43 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ec4d8b8066c8edda8b14884cea78384b3245fc8ff088524fee89c3409d3389`  
		Last Modified: Mon, 08 Jun 2020 18:30:43 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8-slim` - linux; arm variant v6

```console
$ docker pull znc@sha256:d3c7b98cfcba827ef928f67d651ae54d93f37e5ec1f4aa8da129a605ea887138
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58223280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f38881c3c3a93aa029a3112ef2c695550c6c4492b7448dc6fb745262a39ebe07`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Mon, 04 May 2020 19:49:36 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 04 May 2020 19:49:37 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 04 May 2020 19:49:37 GMT
ARG MAKEFLAGS=
# Mon, 08 Jun 2020 18:50:17 GMT
ENV ZNC_VERSION=1.8.1
# Mon, 08 Jun 2020 18:58:16 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 08 Jun 2020 18:58:18 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 08 Jun 2020 18:58:18 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:58:19 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:58:19 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Mon, 08 Jun 2020 18:58:20 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:58:21 GMT
VOLUME [/znc-data]
# Mon, 08 Jun 2020 18:58:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5067ba1e39510a319c267902927feeafa6f8c29fd0fbdcf9c30e2230193ed28e`  
		Last Modified: Mon, 08 Jun 2020 18:59:19 GMT  
		Size: 55.6 MB (55601921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5056ada25c94f1e4dd89a015938c8f21f1365a00cd8c8ec6c7df3012fd0b67bc`  
		Last Modified: Mon, 08 Jun 2020 18:58:55 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b059d59ed64226cf083795c86c10c7635dd24e9da2e853c94731df2af4109ba2`  
		Last Modified: Mon, 08 Jun 2020 18:58:55 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78722115536a71822036c201fdc9154eb83f6586e2c8a3063e1c85e61fd3fba5`  
		Last Modified: Mon, 08 Jun 2020 18:58:56 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25bed4e5ddb5882411590ad8171ecf4985c51b870de8b03bcd8da08cddf269`  
		Last Modified: Mon, 08 Jun 2020 18:58:55 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4edc595142bdcfec0a054fb6a5263c506bda09c5c140f05bb78dc8c5f0b65c`  
		Last Modified: Mon, 08 Jun 2020 18:58:55 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8-slim` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:45db8a930c474ec1b471d330f0d7837817781f442781660d54b83c957d3913d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.0 MB (60038258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6493addde7db3714dc117a9bd647ff1ba622a8bdb5dbceb68954dc4d43a562d7`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Mon, 04 May 2020 19:40:23 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 04 May 2020 19:40:23 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 04 May 2020 19:40:24 GMT
ARG MAKEFLAGS=
# Mon, 08 Jun 2020 18:44:15 GMT
ENV ZNC_VERSION=1.8.1
# Mon, 08 Jun 2020 18:52:37 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 08 Jun 2020 18:52:40 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 08 Jun 2020 18:52:41 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:52:42 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:52:42 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Mon, 08 Jun 2020 18:52:43 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:52:43 GMT
VOLUME [/znc-data]
# Mon, 08 Jun 2020 18:52:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3887515d24b1515c28be3aeca64919edc9acbcff3321a497ba03a160633368`  
		Last Modified: Mon, 08 Jun 2020 18:53:38 GMT  
		Size: 57.3 MB (57312408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79050300cb2ffb98537cb2cfa0f82a803c51cc89a4d952679aed84418b9efdc2`  
		Last Modified: Mon, 08 Jun 2020 18:53:20 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4a6462efa842040fc02cfab1ac30d09819cf8a70034bda884df08f50ff60e6`  
		Last Modified: Mon, 08 Jun 2020 18:53:20 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbdbcc0a36123d143db9ab73ea2025356b52af8c3f872e1e2778fba03fb46ff6`  
		Last Modified: Mon, 08 Jun 2020 18:53:20 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deeec6fca5fad8f785f3307d8fbc2886d7c9f565801eded4da2da998260812e2`  
		Last Modified: Mon, 08 Jun 2020 18:53:20 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7add17715b9f9b7f4adf7b91582039d04239311f783b7b1c8be8e52c60a97a41`  
		Last Modified: Mon, 08 Jun 2020 18:53:20 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:latest`

```console
$ docker pull znc@sha256:654eccd63c1f57638acc488c46a42cd9c51a253b142541479563d39d444b3d23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:latest` - linux; amd64

```console
$ docker pull znc@sha256:f05fa99cf91c247467afad3c0ad3fd262a6f8f27fccc36a8446837db52f3e6c0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.5 MB (145467376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:296c6bf2e7b733563835673ce63565322b6186e1049e6634d8dbc0f3f8df1f86`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Mon, 04 May 2020 19:22:11 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 04 May 2020 19:22:11 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 04 May 2020 19:22:11 GMT
ARG MAKEFLAGS=
# Mon, 08 Jun 2020 18:25:56 GMT
ENV ZNC_VERSION=1.8.1
# Mon, 08 Jun 2020 18:30:18 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 08 Jun 2020 18:30:18 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 08 Jun 2020 18:30:18 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:30:19 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:30:19 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Mon, 08 Jun 2020 18:30:19 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:30:19 GMT
VOLUME [/znc-data]
# Mon, 08 Jun 2020 18:30:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 08 Jun 2020 18:30:35 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Mon, 08 Jun 2020 18:30:35 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5a1332069b5686f2953370c761c60ad203b22a4b5d907cddabd5e3766aa49b`  
		Last Modified: Mon, 08 Jun 2020 18:30:56 GMT  
		Size: 57.4 MB (57402945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a3efef78d5bed01124912e52f0e3a0779a6345f5b42c17788d65c978ea7bb7`  
		Last Modified: Mon, 08 Jun 2020 18:30:43 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c3f10758cc9042e43fb6abf244903f8ba5a9dc2a669a9a30b95dc589d21087`  
		Last Modified: Mon, 08 Jun 2020 18:30:43 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83dd650d49b861285b5f22ebeb69e7cf2ef5c693e0648c22b4b78d960a91a9dc`  
		Last Modified: Mon, 08 Jun 2020 18:30:43 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee9947bd59b5d71c18d40c71849c7ed7540188da416129ac186d78cd18b0714`  
		Last Modified: Mon, 08 Jun 2020 18:30:43 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ec4d8b8066c8edda8b14884cea78384b3245fc8ff088524fee89c3409d3389`  
		Last Modified: Mon, 08 Jun 2020 18:30:43 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7115798da545f00a3b605b09ecee681bab84bb9f2a5aa910306504c5fcdf758c`  
		Last Modified: Mon, 08 Jun 2020 18:31:16 GMT  
		Size: 85.2 MB (85249387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82542bfc7155c7556a2ef1fc164c34f30eaf31d36613e32107c0fd122756a45c`  
		Last Modified: Mon, 08 Jun 2020 18:31:01 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:latest` - linux; arm variant v6

```console
$ docker pull znc@sha256:b26ae39f9e9f766b5a8409c6b6d134768efcbb3af5f0ab213ba6e77b5c57e919
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.7 MB (129651275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04f545fe3110a0e848021c888168cfbb111b180097caa391fbea942918da9ec9`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Mon, 04 May 2020 19:49:36 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 04 May 2020 19:49:37 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 04 May 2020 19:49:37 GMT
ARG MAKEFLAGS=
# Mon, 08 Jun 2020 18:50:17 GMT
ENV ZNC_VERSION=1.8.1
# Mon, 08 Jun 2020 18:58:16 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 08 Jun 2020 18:58:18 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 08 Jun 2020 18:58:18 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:58:19 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:58:19 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Mon, 08 Jun 2020 18:58:20 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:58:21 GMT
VOLUME [/znc-data]
# Mon, 08 Jun 2020 18:58:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 08 Jun 2020 18:58:41 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Mon, 08 Jun 2020 18:58:42 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5067ba1e39510a319c267902927feeafa6f8c29fd0fbdcf9c30e2230193ed28e`  
		Last Modified: Mon, 08 Jun 2020 18:59:19 GMT  
		Size: 55.6 MB (55601921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5056ada25c94f1e4dd89a015938c8f21f1365a00cd8c8ec6c7df3012fd0b67bc`  
		Last Modified: Mon, 08 Jun 2020 18:58:55 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b059d59ed64226cf083795c86c10c7635dd24e9da2e853c94731df2af4109ba2`  
		Last Modified: Mon, 08 Jun 2020 18:58:55 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78722115536a71822036c201fdc9154eb83f6586e2c8a3063e1c85e61fd3fba5`  
		Last Modified: Mon, 08 Jun 2020 18:58:56 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25bed4e5ddb5882411590ad8171ecf4985c51b870de8b03bcd8da08cddf269`  
		Last Modified: Mon, 08 Jun 2020 18:58:55 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4edc595142bdcfec0a054fb6a5263c506bda09c5c140f05bb78dc8c5f0b65c`  
		Last Modified: Mon, 08 Jun 2020 18:58:55 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832d3cbaa1292db4d7d405992435af4c58b11de75cb71fdd696e2aedc557248a`  
		Last Modified: Mon, 08 Jun 2020 18:59:54 GMT  
		Size: 71.4 MB (71427663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62123481f7168fb21c2c5ba4758f4c0070685f1fd24858f7b17e82b323ef0900`  
		Last Modified: Mon, 08 Jun 2020 18:59:27 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:latest` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:9b1369022519d39413ce456ee0368eaa3a8b6720ba32d9beee434c0bb8ac5c4e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.3 MB (135289590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:036305fce5a5341a326034ee6b3a8938105ea4cde69ada975d1206a5660a4158`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Mon, 04 May 2020 19:40:23 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 04 May 2020 19:40:23 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 04 May 2020 19:40:24 GMT
ARG MAKEFLAGS=
# Mon, 08 Jun 2020 18:44:15 GMT
ENV ZNC_VERSION=1.8.1
# Mon, 08 Jun 2020 18:52:37 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 08 Jun 2020 18:52:40 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 08 Jun 2020 18:52:41 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:52:42 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:52:42 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Mon, 08 Jun 2020 18:52:43 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:52:43 GMT
VOLUME [/znc-data]
# Mon, 08 Jun 2020 18:52:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 08 Jun 2020 18:53:06 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Mon, 08 Jun 2020 18:53:09 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3887515d24b1515c28be3aeca64919edc9acbcff3321a497ba03a160633368`  
		Last Modified: Mon, 08 Jun 2020 18:53:38 GMT  
		Size: 57.3 MB (57312408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79050300cb2ffb98537cb2cfa0f82a803c51cc89a4d952679aed84418b9efdc2`  
		Last Modified: Mon, 08 Jun 2020 18:53:20 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4a6462efa842040fc02cfab1ac30d09819cf8a70034bda884df08f50ff60e6`  
		Last Modified: Mon, 08 Jun 2020 18:53:20 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbdbcc0a36123d143db9ab73ea2025356b52af8c3f872e1e2778fba03fb46ff6`  
		Last Modified: Mon, 08 Jun 2020 18:53:20 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deeec6fca5fad8f785f3307d8fbc2886d7c9f565801eded4da2da998260812e2`  
		Last Modified: Mon, 08 Jun 2020 18:53:20 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7add17715b9f9b7f4adf7b91582039d04239311f783b7b1c8be8e52c60a97a41`  
		Last Modified: Mon, 08 Jun 2020 18:53:20 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db4a3dd149ce5b911704202d9dfa809d57303fd48fc45762642eb9d121bfc64`  
		Last Modified: Mon, 08 Jun 2020 18:54:32 GMT  
		Size: 75.3 MB (75251002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdd51f2fb833202202ffebf7fc1a469502a05c393d501702c9ea804ef2aa456`  
		Last Modified: Mon, 08 Jun 2020 18:53:47 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:slim`

```console
$ docker pull znc@sha256:aa772be85911a449dbfa316bd19347b378679d0e99dc4c9b55696d217ba15fc0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:slim` - linux; amd64

```console
$ docker pull znc@sha256:befd9ba6f2781b5a6afcc0360dbc8ddaee995cbafa48e642b85e111f235425c4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.2 MB (60217659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ad09677c3e952082f8efcdf8f65d8136caefe9e75a481efefe6d5d81de6e21`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Mon, 04 May 2020 19:22:11 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 04 May 2020 19:22:11 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 04 May 2020 19:22:11 GMT
ARG MAKEFLAGS=
# Mon, 08 Jun 2020 18:25:56 GMT
ENV ZNC_VERSION=1.8.1
# Mon, 08 Jun 2020 18:30:18 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 08 Jun 2020 18:30:18 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 08 Jun 2020 18:30:18 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:30:19 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:30:19 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Mon, 08 Jun 2020 18:30:19 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:30:19 GMT
VOLUME [/znc-data]
# Mon, 08 Jun 2020 18:30:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5a1332069b5686f2953370c761c60ad203b22a4b5d907cddabd5e3766aa49b`  
		Last Modified: Mon, 08 Jun 2020 18:30:56 GMT  
		Size: 57.4 MB (57402945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a3efef78d5bed01124912e52f0e3a0779a6345f5b42c17788d65c978ea7bb7`  
		Last Modified: Mon, 08 Jun 2020 18:30:43 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c3f10758cc9042e43fb6abf244903f8ba5a9dc2a669a9a30b95dc589d21087`  
		Last Modified: Mon, 08 Jun 2020 18:30:43 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83dd650d49b861285b5f22ebeb69e7cf2ef5c693e0648c22b4b78d960a91a9dc`  
		Last Modified: Mon, 08 Jun 2020 18:30:43 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee9947bd59b5d71c18d40c71849c7ed7540188da416129ac186d78cd18b0714`  
		Last Modified: Mon, 08 Jun 2020 18:30:43 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ec4d8b8066c8edda8b14884cea78384b3245fc8ff088524fee89c3409d3389`  
		Last Modified: Mon, 08 Jun 2020 18:30:43 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:slim` - linux; arm variant v6

```console
$ docker pull znc@sha256:d3c7b98cfcba827ef928f67d651ae54d93f37e5ec1f4aa8da129a605ea887138
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58223280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f38881c3c3a93aa029a3112ef2c695550c6c4492b7448dc6fb745262a39ebe07`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Mon, 04 May 2020 19:49:36 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 04 May 2020 19:49:37 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 04 May 2020 19:49:37 GMT
ARG MAKEFLAGS=
# Mon, 08 Jun 2020 18:50:17 GMT
ENV ZNC_VERSION=1.8.1
# Mon, 08 Jun 2020 18:58:16 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 08 Jun 2020 18:58:18 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 08 Jun 2020 18:58:18 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:58:19 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:58:19 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Mon, 08 Jun 2020 18:58:20 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:58:21 GMT
VOLUME [/znc-data]
# Mon, 08 Jun 2020 18:58:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5067ba1e39510a319c267902927feeafa6f8c29fd0fbdcf9c30e2230193ed28e`  
		Last Modified: Mon, 08 Jun 2020 18:59:19 GMT  
		Size: 55.6 MB (55601921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5056ada25c94f1e4dd89a015938c8f21f1365a00cd8c8ec6c7df3012fd0b67bc`  
		Last Modified: Mon, 08 Jun 2020 18:58:55 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b059d59ed64226cf083795c86c10c7635dd24e9da2e853c94731df2af4109ba2`  
		Last Modified: Mon, 08 Jun 2020 18:58:55 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78722115536a71822036c201fdc9154eb83f6586e2c8a3063e1c85e61fd3fba5`  
		Last Modified: Mon, 08 Jun 2020 18:58:56 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25bed4e5ddb5882411590ad8171ecf4985c51b870de8b03bcd8da08cddf269`  
		Last Modified: Mon, 08 Jun 2020 18:58:55 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4edc595142bdcfec0a054fb6a5263c506bda09c5c140f05bb78dc8c5f0b65c`  
		Last Modified: Mon, 08 Jun 2020 18:58:55 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:slim` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:45db8a930c474ec1b471d330f0d7837817781f442781660d54b83c957d3913d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.0 MB (60038258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6493addde7db3714dc117a9bd647ff1ba622a8bdb5dbceb68954dc4d43a562d7`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Mon, 04 May 2020 19:40:23 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Mon, 04 May 2020 19:40:23 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Mon, 04 May 2020 19:40:24 GMT
ARG MAKEFLAGS=
# Mon, 08 Jun 2020 18:44:15 GMT
ENV ZNC_VERSION=1.8.1
# Mon, 08 Jun 2020 18:52:37 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 08 Jun 2020 18:52:40 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 08 Jun 2020 18:52:41 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:52:42 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:52:42 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Mon, 08 Jun 2020 18:52:43 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Mon, 08 Jun 2020 18:52:43 GMT
VOLUME [/znc-data]
# Mon, 08 Jun 2020 18:52:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3887515d24b1515c28be3aeca64919edc9acbcff3321a497ba03a160633368`  
		Last Modified: Mon, 08 Jun 2020 18:53:38 GMT  
		Size: 57.3 MB (57312408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79050300cb2ffb98537cb2cfa0f82a803c51cc89a4d952679aed84418b9efdc2`  
		Last Modified: Mon, 08 Jun 2020 18:53:20 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4a6462efa842040fc02cfab1ac30d09819cf8a70034bda884df08f50ff60e6`  
		Last Modified: Mon, 08 Jun 2020 18:53:20 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbdbcc0a36123d143db9ab73ea2025356b52af8c3f872e1e2778fba03fb46ff6`  
		Last Modified: Mon, 08 Jun 2020 18:53:20 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deeec6fca5fad8f785f3307d8fbc2886d7c9f565801eded4da2da998260812e2`  
		Last Modified: Mon, 08 Jun 2020 18:53:20 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7add17715b9f9b7f4adf7b91582039d04239311f783b7b1c8be8e52c60a97a41`  
		Last Modified: Mon, 08 Jun 2020 18:53:20 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
