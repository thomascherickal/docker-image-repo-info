## `znc:latest`

```console
$ docker pull znc@sha256:88c4c21d82b8ed3d4aff704477bcacda4206fb5f4c5ad265276d7f139e370a2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `znc:latest` - linux; amd64

```console
$ docker pull znc@sha256:fb9db2b2e43fa981716f9db6f046887e9a440098e0eb33df66c3e69c2d0c02e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138528701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea19fa174c286d3e8ab8a24365df4f2d9fe6a228e4d1abda45a39c993b3f3911`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:36 GMT
ADD file:51c08645923aa2d3513f66571f0c598a727dd5805e4f2bb87fb660b2f789348d in / 
# Thu, 17 Mar 2022 15:19:36 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 16:00:08 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 17 Mar 2022 16:00:08 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 17 Mar 2022 16:00:08 GMT
ARG MAKEFLAGS=
# Thu, 17 Mar 2022 16:00:08 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 17 Mar 2022 16:07:42 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 17 Mar 2022 16:07:43 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 17 Mar 2022 16:07:43 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Thu, 17 Mar 2022 16:07:43 GMT
VOLUME [/znc-data]
# Thu, 17 Mar 2022 16:07:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 16:07:59 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         openssl-dev         perl         python3
# Thu, 17 Mar 2022 16:08:00 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:e1096b72685a2366348e697f5b57e3b8feb41660e3dbe68447e168381515111a`  
		Last Modified: Thu, 17 Mar 2022 15:20:24 GMT  
		Size: 2.8 MB (2817181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67a28a4b9ceca6cc104a16de89d5ef95974afbb8a2e122b58fd86e661657847`  
		Last Modified: Thu, 17 Mar 2022 16:08:29 GMT  
		Size: 43.4 MB (43359474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b59b22213054b16fd1299e23fc7a5feeec2f73254543c1a2371156b58b91911`  
		Last Modified: Thu, 17 Mar 2022 16:08:18 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e0931023ccafc5987c147f725d43ffb5eacef2588352038ad747cb2f173570d`  
		Last Modified: Thu, 17 Mar 2022 16:08:18 GMT  
		Size: 781.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7b012d222e96e263abdccd4132be9b9fb542cb68a703bc69934e1516f654f4`  
		Last Modified: Thu, 17 Mar 2022 16:09:03 GMT  
		Size: 92.4 MB (92350762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa67de5fe8be36e646082f84fc43a8f3bfaaad6ac4c5defd52fce241c8dc0a09`  
		Last Modified: Thu, 17 Mar 2022 16:08:41 GMT  
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
$ docker pull znc@sha256:70a11507447aaeaee609db6cb856a724e450914060bb7ee9e1a0988a64727bc8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.8 MB (129833537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65b015d835374542799967b43265c97cdd734040ee169cba2ccd40a0149dd824`
-	Entrypoint: `["\/entrypoint.sh"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:19 GMT
ADD file:0bbbf3ca52651bbef2547689474beafcef779899da63743efd8166a01d9f3f7a in / 
# Thu, 17 Mar 2022 18:43:20 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 21:24:14 GMT
ENV GPG_KEY=D5823CACB477191CAC0075555AE420CC0209989E
# Thu, 17 Mar 2022 21:24:15 GMT
ARG CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES
# Thu, 17 Mar 2022 21:24:16 GMT
ARG MAKEFLAGS=
# Thu, 17 Mar 2022 21:24:17 GMT
ENV ZNC_VERSION=1.8.2
# Thu, 17 Mar 2022 21:29:47 GMT
# ARGS: CMAKEFLAGS=-DCMAKE_INSTALL_PREFIX=/opt/znc -DWANT_CYRUS=YES -DWANT_PERL=YES -DWANT_PYTHON=YES MAKEFLAGS=
RUN set -x     && adduser -S znc     && addgroup -S znc     && apk add --no-cache --virtual runtime-dependencies         boost         ca-certificates         cyrus-sasl         icu         openssl         su-exec         tini         tzdata     && apk add --no-cache --virtual build-dependencies         boost-dev         build-base         cmake         curl         cyrus-sasl-dev         gettext         gnupg         icu-dev         openssl-dev         perl-dev         python3-dev     && mkdir /znc-src && cd /znc-src     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz" -o znc.tgz     && curl -fsSL "https://znc.in/releases/archive/znc-${ZNC_VERSION}.tar.gz.sig" -o znc.tgz.sig     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${GPG_KEY}"     && gpg --batch --verify znc.tgz.sig znc.tgz     && rm -rf "$GNUPGHOME"     && tar -zxf znc.tgz --strip-components=1     && mkdir build && cd build     && cmake .. ${CMAKEFLAGS}     && make $MAKEFLAGS     && make install     && apk del build-dependencies     && cd / && rm -rf /znc-src
# Thu, 17 Mar 2022 21:29:48 GMT
COPY file:15e47c9cc6835e0818d6896aa6537a8adda40ff814c287685183c73fa9df4713 in / 
# Thu, 17 Mar 2022 21:29:49 GMT
COPY dir:4684da7bbf1d77862fa1a1b074543f975eb608cc0b6b1951ff5c5b58959d0faa in /startup-sequence/ 
# Thu, 17 Mar 2022 21:29:49 GMT
VOLUME [/znc-data]
# Thu, 17 Mar 2022 21:29:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 21:30:04 GMT
RUN set -x     && apk add --no-cache         build-base         cmake         icu-dev         openssl-dev         perl         python3
# Thu, 17 Mar 2022 21:30:05 GMT
COPY file:765473e154cb7674cba99ed8ee42b51feda01581be870e3d1e7e4930b82a0f37 in /startup-sequence/ 
```

-	Layers:
	-	`sha256:6b5c040bf1f18956758f68628afdc8e179044ac75bcd411134da39a661a772e0`  
		Last Modified: Thu, 17 Mar 2022 18:44:11 GMT  
		Size: 2.7 MB (2719134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b30df6f49001636caf347a9397cb3b309e4b5c7883ff08eba15a35e4cbe24d`  
		Last Modified: Thu, 17 Mar 2022 21:30:32 GMT  
		Size: 43.2 MB (43215727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5245881b4efd818a982356de01d2753252dff511cccbaa4a1eb5a7ae643bba7c`  
		Last Modified: Thu, 17 Mar 2022 21:30:25 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6d5c181a221e96597ccb12324dbdf05ee2b9bc3621297a14fb4e556ce0b8ff`  
		Last Modified: Thu, 17 Mar 2022 21:30:25 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e841340454e42ea0a3eff767d4fe9f18750a3042705117111016f74d1e7e1c`  
		Last Modified: Thu, 17 Mar 2022 21:31:00 GMT  
		Size: 83.9 MB (83897417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75711cc3b16e5ab0a1d384e261fe2d8a7440e469198a4237acb0df748d9d4bec`  
		Last Modified: Thu, 17 Mar 2022 21:30:46 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
