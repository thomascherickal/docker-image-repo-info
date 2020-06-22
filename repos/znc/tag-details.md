<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `znc`

-	[`znc:1.8`](#znc18)
-	[`znc:1.8.0`](#znc180)
-	[`znc:1.8.0-slim`](#znc180-slim)
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

## `znc:1.8.0`

```console
$ docker pull znc@sha256:45e798f4b292b6f84bae6751a44c996bf5244261e726782aa81f3207a4271e7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8.0` - linux; amd64

```console
$ docker pull znc@sha256:57cb594bd7577d8482d20b3c5d1999de70020ed953b4e84e9fde0574d1c804e7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.5 MB (145471759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cda26be0c4e56c60166f4b4c9399567bc1714d2e9e7ec135898cd393f0a047f`
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
# Mon, 22 Jun 2020 20:11:15 GMT
ENV ZNC_VERSION=1.8.0
# Mon, 22 Jun 2020 20:15:58 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 22 Jun 2020 20:15:59 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 22 Jun 2020 20:15:59 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Mon, 22 Jun 2020 20:15:59 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Mon, 22 Jun 2020 20:15:59 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Mon, 22 Jun 2020 20:16:00 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Mon, 22 Jun 2020 20:16:00 GMT
VOLUME [/znc-data]
# Mon, 22 Jun 2020 20:16:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 22 Jun 2020 20:16:13 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Mon, 22 Jun 2020 20:16:13 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80a37b098b791d6cbfd504a9bd14105450d2e0fe9930c00f3da861518f5a457`  
		Last Modified: Mon, 22 Jun 2020 20:17:15 GMT  
		Size: 57.4 MB (57402593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42852651439ba22c07fe3c13feb6bbf757e268fa8c00fd444f30e8731ecf3ce8`  
		Last Modified: Mon, 22 Jun 2020 20:17:03 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911fcab858cab4f6a89547d119106c35faa872f479bec7f559fe0c457fd3f78a`  
		Last Modified: Mon, 22 Jun 2020 20:17:03 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:175415dc90749eebcf888c9afdc0ee2755e3257fdc95a1582a396a603b2c2a01`  
		Last Modified: Mon, 22 Jun 2020 20:17:03 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad955c351439b934f8f7df383e93df3c6315b3df8e5db4c96d11b6e358e1c3`  
		Last Modified: Mon, 22 Jun 2020 20:17:03 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1a3ec5847d7bc342b50c6dfc16e3369b91b3bfc29aba88f5f38d3bd856d875`  
		Last Modified: Mon, 22 Jun 2020 20:17:03 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf6d9857ae4369c4288a0617beeb715043cf0f4ebfd68a132542e8d3c91a76e`  
		Last Modified: Mon, 22 Jun 2020 20:17:41 GMT  
		Size: 85.3 MB (85254123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8bdaa02d0ee1b51452b37651cec7e1eb429e9c1424f30f361fcffd439a5c0d4`  
		Last Modified: Mon, 22 Jun 2020 20:17:25 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8.0` - linux; arm variant v6

```console
$ docker pull znc@sha256:ebf5be574d491f348d9374455a0d40e9b9e9c072d389439f032fd520ec37c03e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.7 MB (129679097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c00cfa91cde2c1ff3ff0a00f687d75cb1f62528717564a04ef32d7ca06f6c0f4`
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
# Mon, 22 Jun 2020 19:58:28 GMT
ENV ZNC_VERSION=1.8.0
# Mon, 22 Jun 2020 20:07:00 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 22 Jun 2020 20:07:02 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 22 Jun 2020 20:07:03 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Mon, 22 Jun 2020 20:07:04 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Mon, 22 Jun 2020 20:07:05 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Mon, 22 Jun 2020 20:07:06 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Mon, 22 Jun 2020 20:07:06 GMT
VOLUME [/znc-data]
# Mon, 22 Jun 2020 20:07:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 22 Jun 2020 20:09:41 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Mon, 22 Jun 2020 20:09:43 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32be418f97ac2724863e41eb651bf88b761e189cafce23669ff82ffa2d756f30`  
		Last Modified: Mon, 22 Jun 2020 20:07:59 GMT  
		Size: 55.6 MB (55625248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab81b90c966872b207d1e1ea0906d1d875385c59a1d785525773f324f5d4a49`  
		Last Modified: Mon, 22 Jun 2020 20:07:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2b2c9b220d1f3d7cd52d1849acfeaafb4985614a01e5ca4942d5688a71de90`  
		Last Modified: Mon, 22 Jun 2020 20:07:36 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaeffdf11d315412cc3738dab6f15b0d1008de7ab11466432f191ad9ca777448`  
		Last Modified: Mon, 22 Jun 2020 20:07:36 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2fa7ca90a2094192d65c4f40a29aa35aa0cf62116b8ef766d8786b9fb0b619`  
		Last Modified: Mon, 22 Jun 2020 20:07:37 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cc62dca2f62d979909d9250ba4ca79d87050d4941eb8e926c0c63f1f4871bd`  
		Last Modified: Mon, 22 Jun 2020 20:07:36 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb65dbe1b979d830a2a7fb90758c58362e833f29372f19089c03d43de96a6d96`  
		Last Modified: Mon, 22 Jun 2020 20:10:53 GMT  
		Size: 71.4 MB (71432155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d5cd9d8bc3cf78d60e060f80584935e3b6d39f5ce66c9ea6d0266333f9f17c`  
		Last Modified: Mon, 22 Jun 2020 20:10:27 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8.0` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:81d0da9a7c9da40f36d808c262ff710b29540e64e26f0bab948358a339606d89
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.3 MB (135290115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbe18e81225b1945c68b2efeb4390db98dfdb8b4a7ff8c23e581269d8c465471`
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
# Mon, 22 Jun 2020 20:17:18 GMT
ENV ZNC_VERSION=1.8.0
# Mon, 22 Jun 2020 20:25:33 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 22 Jun 2020 20:25:35 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 22 Jun 2020 20:25:36 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Mon, 22 Jun 2020 20:25:36 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Mon, 22 Jun 2020 20:25:37 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Mon, 22 Jun 2020 20:25:38 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Mon, 22 Jun 2020 20:25:39 GMT
VOLUME [/znc-data]
# Mon, 22 Jun 2020 20:25:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 22 Jun 2020 20:26:26 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Mon, 22 Jun 2020 20:26:28 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7352680d5cd22c41eac086061e32981e4f200bf334b213e9dc8cdb2c4bc1b0`  
		Last Modified: Mon, 22 Jun 2020 20:26:32 GMT  
		Size: 57.3 MB (57311349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363ad5b01303682e36a5ec85dcf5ceaa2cb889c99bc524a444b6056b2d3c96c5`  
		Last Modified: Mon, 22 Jun 2020 20:26:13 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f71af5ae69a891cf8be326f91a6d0ba38f6c685edc2f277e1c2f0610bb71480`  
		Last Modified: Mon, 22 Jun 2020 20:26:12 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c08c1543827cca47f621d1cd75b0fb2e787b03c018d5e87713c8afa49a099be`  
		Last Modified: Mon, 22 Jun 2020 20:26:12 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefbf406ac2b1ccebe953e77cb16a449c811dfc95282df4dd169dd0980bc29ad`  
		Last Modified: Mon, 22 Jun 2020 20:26:11 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f8f2d78248a91552e7408dbfe884ecaeda778e35a381cb7bf7e36cfa488f14`  
		Last Modified: Mon, 22 Jun 2020 20:26:11 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b16b8bf24bcc55a3247da46c209091f19bd06911737837b2d8b449635b2b35b`  
		Last Modified: Mon, 22 Jun 2020 20:27:27 GMT  
		Size: 75.3 MB (75252587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4e1d0f1c322837cf0878d282aced7adcb3b63a2ac111562d493ff6a026b4ea`  
		Last Modified: Mon, 22 Jun 2020 20:27:02 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.8.0-slim`

```console
$ docker pull znc@sha256:d1d731f180a57bece271b0c06bb630d1e2163b59b86d3cf7a1ad55509584cc23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8.0-slim` - linux; amd64

```console
$ docker pull znc@sha256:71f6b3fa0531162741ae8349ff6707c7ab6bb5289a5416ae4cc7ca69ca6b63f0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.2 MB (60217306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f12bb6bae1a7e77af814a900a528b9d9648a244ebc35f6ccff779a886ad9094`
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
# Mon, 22 Jun 2020 20:11:15 GMT
ENV ZNC_VERSION=1.8.0
# Mon, 22 Jun 2020 20:15:58 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 22 Jun 2020 20:15:59 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 22 Jun 2020 20:15:59 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Mon, 22 Jun 2020 20:15:59 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Mon, 22 Jun 2020 20:15:59 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Mon, 22 Jun 2020 20:16:00 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Mon, 22 Jun 2020 20:16:00 GMT
VOLUME [/znc-data]
# Mon, 22 Jun 2020 20:16:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80a37b098b791d6cbfd504a9bd14105450d2e0fe9930c00f3da861518f5a457`  
		Last Modified: Mon, 22 Jun 2020 20:17:15 GMT  
		Size: 57.4 MB (57402593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42852651439ba22c07fe3c13feb6bbf757e268fa8c00fd444f30e8731ecf3ce8`  
		Last Modified: Mon, 22 Jun 2020 20:17:03 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911fcab858cab4f6a89547d119106c35faa872f479bec7f559fe0c457fd3f78a`  
		Last Modified: Mon, 22 Jun 2020 20:17:03 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:175415dc90749eebcf888c9afdc0ee2755e3257fdc95a1582a396a603b2c2a01`  
		Last Modified: Mon, 22 Jun 2020 20:17:03 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad955c351439b934f8f7df383e93df3c6315b3df8e5db4c96d11b6e358e1c3`  
		Last Modified: Mon, 22 Jun 2020 20:17:03 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1a3ec5847d7bc342b50c6dfc16e3369b91b3bfc29aba88f5f38d3bd856d875`  
		Last Modified: Mon, 22 Jun 2020 20:17:03 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8.0-slim` - linux; arm variant v6

```console
$ docker pull znc@sha256:bad920760d8d3c4f958c916e02150fd4a4c180022e3ff906d298e61a7a701e91
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58246607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7d3f90cff2b83cc1bf08f2efb7f1f4c45fa1eb150b31a63f36469131f81fc4d`
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
# Mon, 22 Jun 2020 19:58:28 GMT
ENV ZNC_VERSION=1.8.0
# Mon, 22 Jun 2020 20:07:00 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 22 Jun 2020 20:07:02 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 22 Jun 2020 20:07:03 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Mon, 22 Jun 2020 20:07:04 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Mon, 22 Jun 2020 20:07:05 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Mon, 22 Jun 2020 20:07:06 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Mon, 22 Jun 2020 20:07:06 GMT
VOLUME [/znc-data]
# Mon, 22 Jun 2020 20:07:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32be418f97ac2724863e41eb651bf88b761e189cafce23669ff82ffa2d756f30`  
		Last Modified: Mon, 22 Jun 2020 20:07:59 GMT  
		Size: 55.6 MB (55625248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab81b90c966872b207d1e1ea0906d1d875385c59a1d785525773f324f5d4a49`  
		Last Modified: Mon, 22 Jun 2020 20:07:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2b2c9b220d1f3d7cd52d1849acfeaafb4985614a01e5ca4942d5688a71de90`  
		Last Modified: Mon, 22 Jun 2020 20:07:36 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaeffdf11d315412cc3738dab6f15b0d1008de7ab11466432f191ad9ca777448`  
		Last Modified: Mon, 22 Jun 2020 20:07:36 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2fa7ca90a2094192d65c4f40a29aa35aa0cf62116b8ef766d8786b9fb0b619`  
		Last Modified: Mon, 22 Jun 2020 20:07:37 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cc62dca2f62d979909d9250ba4ca79d87050d4941eb8e926c0c63f1f4871bd`  
		Last Modified: Mon, 22 Jun 2020 20:07:36 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:1.8.0-slim` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:7d4a43ee00e9ee24bbb742b8ae55b86a2f1f4d106cf56252e45e04f6d9f68f3d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.0 MB (60037196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4dcf8c435d56e1a44a278284bc93d85afc7816dc8600880280f5404e50986fb`
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
# Mon, 22 Jun 2020 20:17:18 GMT
ENV ZNC_VERSION=1.8.0
# Mon, 22 Jun 2020 20:25:33 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Mon, 22 Jun 2020 20:25:35 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Mon, 22 Jun 2020 20:25:36 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Mon, 22 Jun 2020 20:25:36 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Mon, 22 Jun 2020 20:25:37 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Mon, 22 Jun 2020 20:25:38 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Mon, 22 Jun 2020 20:25:39 GMT
VOLUME [/znc-data]
# Mon, 22 Jun 2020 20:25:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7352680d5cd22c41eac086061e32981e4f200bf334b213e9dc8cdb2c4bc1b0`  
		Last Modified: Mon, 22 Jun 2020 20:26:32 GMT  
		Size: 57.3 MB (57311349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363ad5b01303682e36a5ec85dcf5ceaa2cb889c99bc524a444b6056b2d3c96c5`  
		Last Modified: Mon, 22 Jun 2020 20:26:13 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f71af5ae69a891cf8be326f91a6d0ba38f6c685edc2f277e1c2f0610bb71480`  
		Last Modified: Mon, 22 Jun 2020 20:26:12 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c08c1543827cca47f621d1cd75b0fb2e787b03c018d5e87713c8afa49a099be`  
		Last Modified: Mon, 22 Jun 2020 20:26:12 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefbf406ac2b1ccebe953e77cb16a449c811dfc95282df4dd169dd0980bc29ad`  
		Last Modified: Mon, 22 Jun 2020 20:26:11 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f8f2d78248a91552e7408dbfe884ecaeda778e35a381cb7bf7e36cfa488f14`  
		Last Modified: Mon, 22 Jun 2020 20:26:11 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `znc:1.8.1`

```console
$ docker pull znc@sha256:654eccd63c1f57638acc488c46a42cd9c51a253b142541479563d39d444b3d23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8.1` - linux; amd64

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

### `znc:1.8.1` - linux; arm64 variant v8

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

## `znc:1.8.1-slim`

```console
$ docker pull znc@sha256:aa772be85911a449dbfa316bd19347b378679d0e99dc4c9b55696d217ba15fc0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:1.8.1-slim` - linux; amd64

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

### `znc:1.8.1-slim` - linux; arm64 variant v8

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
