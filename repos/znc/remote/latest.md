## `znc:latest`

```console
$ docker pull znc@sha256:fd7ff651c236b5a284476b3fab5f0e839607f38d345599e49b95e7b64cad6d7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:latest` - linux; amd64

```console
$ docker pull znc@sha256:6d405b394978ad3a15fe95f0e6672e1f49336332ddfe5bf005385bd0ac7998f2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.7 MB (150734139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ae7fb19c6f259433762f5f330bcb068df121b268e1a38e960fb0e14eff0b49b`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:58:41 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Fri, 11 Dec 2020 02:58:41 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Fri, 11 Dec 2020 02:58:41 GMT
ARG MAKEFLAGS=
# Fri, 11 Dec 2020 02:58:41 GMT
ENV ZNC_VERSION=1.8.2
# Fri, 11 Dec 2020 03:04:58 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Fri, 11 Dec 2020 03:04:59 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Fri, 11 Dec 2020 03:04:59 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Fri, 11 Dec 2020 03:05:00 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Fri, 11 Dec 2020 03:05:00 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Fri, 11 Dec 2020 03:05:00 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Fri, 11 Dec 2020 03:05:00 GMT
VOLUME [/znc-data]
# Fri, 11 Dec 2020 03:05:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Dec 2020 03:05:28 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Fri, 11 Dec 2020 03:05:29 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c57e0a0d721075aff41f2227ea83044ddda0b4afaaa8dd922e0b12d10c85f5ca`  
		Last Modified: Fri, 11 Dec 2020 03:05:55 GMT  
		Size: 44.6 MB (44561100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2073b962af9cd96c54f17d308f1c4a67b8ccb872a8a033b7d1e9b4ae748e6f30`  
		Last Modified: Fri, 11 Dec 2020 03:05:43 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba3b9973333fd68f4e0e03509daef45327575a0ecf60989b47b0fda013bcb87`  
		Last Modified: Fri, 11 Dec 2020 03:05:42 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993dfe378ea75a077d968f140037ac8fb081756951374e81f9f80f44905644ef`  
		Last Modified: Fri, 11 Dec 2020 03:05:42 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ab289eda1213c4054cef7dda7c63a605d2f1d2241f6def781bfd203ddd522b`  
		Last Modified: Fri, 11 Dec 2020 03:05:42 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c0ab7ef77192afe5ae14e997d6c64551a7a94251c93cb8c8c015f22cf8bfe4`  
		Last Modified: Fri, 11 Dec 2020 03:05:43 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb82933df45b3a70a07326a3e38638377d627bb2426777a881cc3b961be61564`  
		Last Modified: Fri, 11 Dec 2020 03:06:29 GMT  
		Size: 103.4 MB (103374368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8d9db27c7e9e57348cafbe55750396c651e494a4517522fc146ada295c8fbf`  
		Last Modified: Fri, 11 Dec 2020 03:06:04 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:latest` - linux; arm variant v6

```console
$ docker pull znc@sha256:4d9052d7fb8b5661cdff55a11b8e37b0cfac9fa9712b78d7b048c6e9564cb40d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.4 MB (132435843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf9434f5f5e45128b6ce719a8028d0ec28c1527f6814524d8bbb6f45a808d6dc`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:00:55 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 17 Dec 2020 01:00:56 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 17 Dec 2020 01:00:57 GMT
ARG MAKEFLAGS=
# Thu, 17 Dec 2020 01:00:59 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 17 Dec 2020 01:09:12 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 17 Dec 2020 01:09:14 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 17 Dec 2020 01:09:14 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 17 Dec 2020 01:09:15 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 17 Dec 2020 01:09:16 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 17 Dec 2020 01:09:17 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 17 Dec 2020 01:09:18 GMT
VOLUME [/znc-data]
# Thu, 17 Dec 2020 01:09:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 01:09:53 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Thu, 17 Dec 2020 01:10:03 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2661c80b7141d305dd17dea87550c3f6d61839f7bba2c560ec767f5c1c71a24`  
		Last Modified: Thu, 17 Dec 2020 01:10:44 GMT  
		Size: 42.8 MB (42810103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f5b774fd47ed78219c699c0afb4dadd2621783e956616723978ccb49bbd728`  
		Last Modified: Thu, 17 Dec 2020 01:10:25 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e775f21a73c3edebadd78773262e2377f931bf671e56cabb73ae27ba611f2b0b`  
		Last Modified: Thu, 17 Dec 2020 01:10:25 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4278650e0b3317e95eb455cfb4fa9389b86e96db441d5e30b4f52464c6d26d8`  
		Last Modified: Thu, 17 Dec 2020 01:10:25 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba055919132f30bfc88ad7d9328fda6135f551ae22ccfc575c3f39c0584d9916`  
		Last Modified: Thu, 17 Dec 2020 01:10:25 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb9b0b9197351a79caeab46ae19c8d836cd60757ed263e265c8052e9b988365`  
		Last Modified: Thu, 17 Dec 2020 01:10:25 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec9be463df837575defd778ced800b8c078212c10e2200ba5fd3813b6f0db7c`  
		Last Modified: Thu, 17 Dec 2020 01:11:27 GMT  
		Size: 87.0 MB (87019820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de5fe456af340607307da0f38d93aa3783f554815d2be4403f26aa8e5ad2a87`  
		Last Modified: Thu, 17 Dec 2020 01:10:57 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `znc:latest` - linux; arm64 variant v8

```console
$ docker pull znc@sha256:6b5f6c0fc9aaa4f6c3b5888f50bc4614697c4972fea45d9c7ccb222ca1e72fe4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.9 MB (137893594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:295b544dab63a7732baea1693e70dcd11aa608834b3c4b8c61653b4fe0a3e689`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 07:16:55 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 17 Dec 2020 07:16:55 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 17 Dec 2020 07:16:56 GMT
ARG MAKEFLAGS=
# Thu, 17 Dec 2020 07:16:57 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 17 Dec 2020 07:25:18 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         libressl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         libressl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 17 Dec 2020 07:25:20 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 17 Dec 2020 07:25:21 GMT
COPY file:dfda6761eff5635f2f7a6c1d540b2b14ea67514867578d12226629a780844185 in /startup-sequence/ 
# Thu, 17 Dec 2020 07:25:22 GMT
COPY file:809dccdc6a2a9f5e2a058644d9f71b2f167ab0f237913902896fef13b6315814 in /startup-sequence/ 
# Thu, 17 Dec 2020 07:25:23 GMT
COPY file:84986dd2ebc690804b4c47eb72d1af3a52ba257c76202478879604756431ff5c in /startup-sequence/ 
# Thu, 17 Dec 2020 07:25:24 GMT
COPY file:50e035ea8915a4bc88fd57c8f79152224f23e0c4c4b68ea8469294aedbddd039 in /startup-sequence/ 
# Thu, 17 Dec 2020 07:25:25 GMT
VOLUME [/znc-data]
# Thu, 17 Dec 2020 07:25:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 07:26:03 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         libressl-dev         perl         python3
# Thu, 17 Dec 2020 07:26:08 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c96944a822ccd3332cf814b043fa0552e60645694e203bbe8c03ab9f0e38e9f`  
		Last Modified: Thu, 17 Dec 2020 07:26:39 GMT  
		Size: 44.4 MB (44409239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4277f89796cac247420c68a0ef2f274b54c4b9be90fea7e1164668a23894a38d`  
		Last Modified: Thu, 17 Dec 2020 07:26:24 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858bc81db26160a8c8494cc3be8a5a82242950d011ffbfb3214e4601b7470eb6`  
		Last Modified: Thu, 17 Dec 2020 07:26:25 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250e6d26a37c84cdd1b38feeef67925bd6f6d3a1144e44d68c1e9626a6b52e09`  
		Last Modified: Thu, 17 Dec 2020 07:26:24 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68614fba9fb5e54cdfbd361234ade58c5341af1e779e99170f221073243a2768`  
		Last Modified: Thu, 17 Dec 2020 07:26:24 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a62466e101590e5f41bb75144628545232e4b3f46f6889f796105ce362a990b`  
		Last Modified: Thu, 17 Dec 2020 07:26:24 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8db0d18c5ced70203daba9b0a3ff326b7f39fc8abf0e29cfe3c85737218537`  
		Last Modified: Thu, 17 Dec 2020 07:27:15 GMT  
		Size: 90.8 MB (90773546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ad9c6525d9d3c4c619873d03c1ea5559adb8f106b71b4a73df06f645da002b`  
		Last Modified: Thu, 17 Dec 2020 07:26:52 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
