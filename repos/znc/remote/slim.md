## `znc:slim`

```console
$ docker pull znc@sha256:e87e750ebed5390fa4b59e3deec590753ed2f71964cd2c3d7a34feb39f13aee7
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
$ docker pull znc@sha256:f7001156dd9eb18eac1a4f8264e3f882d0b9f9c6ab61fa3aee37fb1ce54c59fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47397065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdd8bc94cd59a4d36dd7b1376ef413baf66ba37fadf7613d226434e996b651d3`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:09 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Tue, 15 Jun 2021 21:45:09 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:24:57 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Wed, 16 Jun 2021 11:24:58 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Wed, 16 Jun 2021 11:24:58 GMT
ARG MAKEFLAGS=
# Wed, 16 Jun 2021 11:24:58 GMT
ENV ZNC_VERSION=1.8.2
# Wed, 16 Jun 2021 11:29:25 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Wed, 16 Jun 2021 11:29:26 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Wed, 16 Jun 2021 11:29:26 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Wed, 16 Jun 2021 11:29:26 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Wed, 16 Jun 2021 11:29:27 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Wed, 16 Jun 2021 11:29:27 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Wed, 16 Jun 2021 11:29:27 GMT
VOLUME [/znc-data]
# Wed, 16 Jun 2021 11:29:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad34e1a951e15db912aec3b8a89b72cec244f7da06cee8602496bee1b6c4b380`  
		Last Modified: Wed, 16 Jun 2021 11:30:19 GMT  
		Size: 44.7 MB (44684943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5aaa05046f2cbd4af59682c3b708c54e6e2d3073f4aa6d7f6b374845de0875`  
		Last Modified: Wed, 16 Jun 2021 11:30:08 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3aa030dadd6b84941525f666882ece3060bd10f3959ad50c3fc21e67ff4ac4d`  
		Last Modified: Wed, 16 Jun 2021 11:30:08 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3acb452f5fd5a281ff8b9de1e94ecdb9b23e494ef016030dba61c53fc4df657e`  
		Last Modified: Wed, 16 Jun 2021 11:30:08 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fe5f1b898af137c34519aa601733c57cf5cfddbcfa76a4e7756b373425777c`  
		Last Modified: Wed, 16 Jun 2021 11:30:08 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7499d75d656abef6f0af344cda7e65d5e00451adc9a1b7d15cec8571592b6210`  
		Last Modified: Wed, 16 Jun 2021 11:30:08 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
