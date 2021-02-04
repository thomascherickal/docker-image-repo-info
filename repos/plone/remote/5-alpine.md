## `plone:5-alpine`

```console
$ docker pull plone@sha256:907474984a1d8a002e720ba99584a7d9d5950bfa58d6c5c22522da25ff64c646
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `plone:5-alpine` - linux; amd64

```console
$ docker pull plone@sha256:055eedcd4949d81b907572446524ae8e81f78b28fca12bd39f0494bab6fc614d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.2 MB (137223750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26e03456c8a80d325a3ba39997d59f6b9d58b1c422e2f7d879d37f61be09b4bf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Thu, 04 Feb 2021 01:00:27 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 Feb 2021 01:00:27 GMT
ENV LANG=C.UTF-8
# Thu, 04 Feb 2021 01:31:49 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Thu, 04 Feb 2021 01:31:49 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 04 Feb 2021 01:31:49 GMT
ENV PYTHON_VERSION=3.8.7
# Thu, 04 Feb 2021 01:41:57 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 04 Feb 2021 01:41:59 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 04 Feb 2021 01:42:00 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Thu, 04 Feb 2021 01:42:00 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Thu, 04 Feb 2021 01:42:00 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Thu, 04 Feb 2021 01:42:13 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 04 Feb 2021 01:42:13 GMT
CMD ["python3"]
# Thu, 04 Feb 2021 02:28:43 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Thu, 04 Feb 2021 02:28:44 GMT
LABEL plone=5.2.2 os=alpine os.version=3.12 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 04 Feb 2021 02:28:45 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 04 Feb 2021 02:28:45 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Thu, 04 Feb 2021 02:43:41 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 04 Feb 2021 02:43:43 GMT
VOLUME [/data]
# Thu, 04 Feb 2021 02:43:43 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Thu, 04 Feb 2021 02:43:43 GMT
EXPOSE 8080
# Thu, 04 Feb 2021 02:43:43 GMT
WORKDIR /plone/instance
# Thu, 04 Feb 2021 02:43:44 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 04 Feb 2021 02:43:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 04 Feb 2021 02:43:44 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e807dbff582b104e7a01a4d3233fffb7a34fb609b0c150af584b0ca1db2c2aa`  
		Last Modified: Thu, 04 Feb 2021 02:09:53 GMT  
		Size: 281.2 KB (281203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079acc430bf9db22a2159b57ce704265070f563573f494369721f7753444f923`  
		Last Modified: Thu, 04 Feb 2021 02:09:56 GMT  
		Size: 11.2 MB (11190110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:082445bdccf7c5ad586eec10c25df16de1350b548a5289df87ba948ff59671d1`  
		Last Modified: Thu, 04 Feb 2021 02:09:53 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7192354fc041031115f8a693096f76bdf4f1c815bea373f9bde6d8be621aaba1`  
		Last Modified: Thu, 04 Feb 2021 02:09:54 GMT  
		Size: 2.2 MB (2163739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed987fa5c6bc1e49ebb3f99a64b24783af46c9d1b7f8e1a39c35f9209dbdbea`  
		Last Modified: Thu, 04 Feb 2021 02:44:20 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ba39740e66334335805815fdf462f59125f3a6195b21d517dc52796b2cc6d4`  
		Last Modified: Thu, 04 Feb 2021 02:44:20 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039963f665409499a3f2d19fd2d00b26dcd004c9ad2065cbc7f1c61c6b3bf161`  
		Last Modified: Thu, 04 Feb 2021 02:44:44 GMT  
		Size: 120.8 MB (120771939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5967f6815563f36df0992039d294592afa4cc205d98beedc47b6dde0f8b9d2`  
		Last Modified: Thu, 04 Feb 2021 02:44:20 GMT  
		Size: 2.8 KB (2846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; arm variant v6

```console
$ docker pull plone@sha256:bcce1a03227520edf0885cd1dafcfdd37656358b0a4ad21f6cc59909c4995400
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.2 MB (136199830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1c9c327c357c01757eba29e9542cfdc938e9092799da9fb20589f13983a7747`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Thu, 28 Jan 2021 23:49:59 GMT
ADD file:c197324e4979e2a7b257ad683d20dd9cbdae525a076bd68fe6aa0e0b126875df in / 
# Thu, 28 Jan 2021 23:49:59 GMT
CMD ["/bin/sh"]
# Thu, 04 Feb 2021 01:13:12 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 Feb 2021 01:13:13 GMT
ENV LANG=C.UTF-8
# Thu, 04 Feb 2021 01:45:20 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Thu, 04 Feb 2021 01:45:21 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 04 Feb 2021 01:45:22 GMT
ENV PYTHON_VERSION=3.8.7
# Thu, 04 Feb 2021 01:54:24 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 04 Feb 2021 01:54:28 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 04 Feb 2021 01:54:29 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Thu, 04 Feb 2021 01:54:29 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Thu, 04 Feb 2021 01:54:30 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Thu, 04 Feb 2021 01:54:44 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 04 Feb 2021 01:54:46 GMT
CMD ["python3"]
# Thu, 04 Feb 2021 02:39:54 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Thu, 04 Feb 2021 02:39:55 GMT
LABEL plone=5.2.2 os=alpine os.version=3.12 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 04 Feb 2021 02:39:57 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 04 Feb 2021 02:39:57 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Thu, 04 Feb 2021 03:00:07 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 04 Feb 2021 03:00:11 GMT
VOLUME [/data]
# Thu, 04 Feb 2021 03:00:12 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Thu, 04 Feb 2021 03:00:13 GMT
EXPOSE 8080
# Thu, 04 Feb 2021 03:00:14 GMT
WORKDIR /plone/instance
# Thu, 04 Feb 2021 03:00:15 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 04 Feb 2021 03:00:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 04 Feb 2021 03:00:17 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:a66f440da051140fefcb0a520bdeb69d763b1eb4fd1b2ed46b4c0a168e335108`  
		Last Modified: Thu, 28 Jan 2021 23:50:33 GMT  
		Size: 2.6 MB (2621759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d1ba015d01d7834a4bb30f2679fdb3365d4884d8bd0be8a3729b32a1758874`  
		Last Modified: Thu, 04 Feb 2021 02:22:34 GMT  
		Size: 281.4 KB (281393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8d1e5f06846d3cfb0d1de15baa9ac27068cbb01e3191b8097ac4e53df55be0`  
		Last Modified: Thu, 04 Feb 2021 02:22:37 GMT  
		Size: 10.8 MB (10767422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297899ecc84e40a4fc92dd2a43994c071ab25fc8c6d99e1e66062c07c37d63a0`  
		Last Modified: Thu, 04 Feb 2021 02:22:35 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e807a803ff3d7af6b00c380c34c94ad3f0b8001e2bc5fdb72352d5529541e31d`  
		Last Modified: Thu, 04 Feb 2021 02:22:35 GMT  
		Size: 2.2 MB (2164041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88be0811a584810850a8401105cee1709576f038fe5ac5020c819be760b179a1`  
		Last Modified: Thu, 04 Feb 2021 03:00:43 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca3aaae4d6ba4149a0204ec46e35e25ddf154c59d4725fe29769fb9ef6b750f`  
		Last Modified: Thu, 04 Feb 2021 03:00:43 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9680e2ec3f437ddaddffd4106691cf07db43113a188fcf7e13c8f645af939c51`  
		Last Modified: Thu, 04 Feb 2021 03:01:28 GMT  
		Size: 120.4 MB (120359713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63fa3037cd28f112ad0e6944c5c137ab431dc5ed9e25ba96b13ac0b4e58ab36d`  
		Last Modified: Thu, 04 Feb 2021 03:00:43 GMT  
		Size: 2.8 KB (2847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:a8755d91de67d98871c5f562b3c801153bff05b5d097458738d93e5e9dd2f2d5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.0 MB (137035299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c6a1c73eb294291c79916ee3977f5f96aa2971851b4b0c2f70efd4e93136201`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Thu, 04 Feb 2021 01:24:56 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 Feb 2021 01:24:57 GMT
ENV LANG=C.UTF-8
# Thu, 04 Feb 2021 01:50:46 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Thu, 04 Feb 2021 01:50:47 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 04 Feb 2021 01:50:48 GMT
ENV PYTHON_VERSION=3.8.7
# Thu, 04 Feb 2021 01:58:29 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 04 Feb 2021 01:58:32 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 04 Feb 2021 01:58:33 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Thu, 04 Feb 2021 01:58:34 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Thu, 04 Feb 2021 01:58:35 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Thu, 04 Feb 2021 01:58:49 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 04 Feb 2021 01:58:49 GMT
CMD ["python3"]
# Thu, 04 Feb 2021 02:47:34 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Thu, 04 Feb 2021 02:47:34 GMT
LABEL plone=5.2.2 os=alpine os.version=3.12 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 04 Feb 2021 02:47:37 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 04 Feb 2021 02:47:38 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Thu, 04 Feb 2021 03:08:37 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 04 Feb 2021 03:08:41 GMT
VOLUME [/data]
# Thu, 04 Feb 2021 03:08:42 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Thu, 04 Feb 2021 03:08:43 GMT
EXPOSE 8080
# Thu, 04 Feb 2021 03:08:44 GMT
WORKDIR /plone/instance
# Thu, 04 Feb 2021 03:08:45 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 04 Feb 2021 03:08:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 04 Feb 2021 03:08:48 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9f15009dabcc1acf7e9677cd35f212a401c6d189b9884e39170beddfe52ed9`  
		Last Modified: Thu, 04 Feb 2021 02:26:07 GMT  
		Size: 281.6 KB (281573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e155bf776a3ee4a7dae85ccbe803d100bd5aeb2e9b8c63294bd23b033b4df7`  
		Last Modified: Thu, 04 Feb 2021 02:26:10 GMT  
		Size: 11.3 MB (11256594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d306ba6b29d96a29146f5b9a69c469ef3d1c68ab8bbfbc8af7142c340ffb90`  
		Last Modified: Thu, 04 Feb 2021 02:26:07 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1e00e67c7d6e074dd6a908e03fa769225778367521e7e26cb8d5b5644cfaf6`  
		Last Modified: Thu, 04 Feb 2021 02:26:08 GMT  
		Size: 2.2 MB (2164053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f08eb6613c3c3285a538d408827b65e862a2ebd5f56bcac2d566f90df0f34b2`  
		Last Modified: Thu, 04 Feb 2021 03:09:37 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50af12cd84a7334e3b26a46e55df5459fb7717b550ed0a995dcfb68f5d5ecec0`  
		Last Modified: Thu, 04 Feb 2021 03:09:37 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f1be3d0d00ef445b0737a5d6c4c458afc3e2221e978132115315bc0329a7db`  
		Last Modified: Thu, 04 Feb 2021 03:10:12 GMT  
		Size: 120.6 MB (120616319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637a1dd72c60c2eb70789d8f49d58f9dc39ca2769d267c1e9edd735553132819`  
		Last Modified: Thu, 04 Feb 2021 03:09:37 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; 386

```console
$ docker pull plone@sha256:731ee02a904f562c2f5ec0eca7d4953b9817108ca086afbcd6b1eddcb024486d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137536807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8c67c1bdcf1486a27695f98c3dc711087d29ff890ec0c8c6f78cbd4dfa3bfda`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Thu, 28 Jan 2021 23:38:31 GMT
ADD file:c0e9ea135d66ad6504c77915a7a48b3bead60892d155d3258b746cb4945981c0 in / 
# Thu, 28 Jan 2021 23:38:31 GMT
CMD ["/bin/sh"]
# Thu, 04 Feb 2021 01:38:17 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 Feb 2021 01:38:17 GMT
ENV LANG=C.UTF-8
# Thu, 04 Feb 2021 02:14:27 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Thu, 04 Feb 2021 02:14:27 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 04 Feb 2021 02:14:28 GMT
ENV PYTHON_VERSION=3.8.7
# Thu, 04 Feb 2021 02:22:41 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 04 Feb 2021 02:22:42 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 04 Feb 2021 02:22:42 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Thu, 04 Feb 2021 02:22:42 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Thu, 04 Feb 2021 02:22:43 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Thu, 04 Feb 2021 02:22:50 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 04 Feb 2021 02:22:50 GMT
CMD ["python3"]
# Thu, 04 Feb 2021 03:04:55 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Thu, 04 Feb 2021 03:04:55 GMT
LABEL plone=5.2.2 os=alpine os.version=3.12 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 04 Feb 2021 03:04:56 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 04 Feb 2021 03:04:56 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Thu, 04 Feb 2021 03:19:35 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 04 Feb 2021 03:19:36 GMT
VOLUME [/data]
# Thu, 04 Feb 2021 03:19:37 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Thu, 04 Feb 2021 03:19:37 GMT
EXPOSE 8080
# Thu, 04 Feb 2021 03:19:37 GMT
WORKDIR /plone/instance
# Thu, 04 Feb 2021 03:19:37 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 04 Feb 2021 03:19:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 04 Feb 2021 03:19:38 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:3fea00a81341ce917db671eb3ad24ef5750cb6928b7f760e3ce4dab619eeb1fa`  
		Last Modified: Thu, 28 Jan 2021 23:39:02 GMT  
		Size: 2.8 MB (2817627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3e9f3f5d77bf9b4cea80a4ecb8e9aadefc25c7a537940fa67b58724f195564`  
		Last Modified: Thu, 04 Feb 2021 02:46:26 GMT  
		Size: 281.8 KB (281753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb1a1f3ea530057bc0f145d459fbd24bff49389157cff880c3be801990c3c89`  
		Last Modified: Thu, 04 Feb 2021 02:46:29 GMT  
		Size: 11.4 MB (11370540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904a722302e100e7bbe9f994d787f7ce93d4538e1ab9e69006e567520615bcc3`  
		Last Modified: Thu, 04 Feb 2021 02:46:27 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3661dc17baf7cb50716b8d226974cbe166b536caeaf431f58ada1fe0dc0819`  
		Last Modified: Thu, 04 Feb 2021 02:46:27 GMT  
		Size: 2.2 MB (2163694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b9c311f19d1955f0163597058c1aa051abe55a65f484650d960c207e79bbfb`  
		Last Modified: Thu, 04 Feb 2021 03:20:15 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548b2349649e107f9a0a2c33adf3ff078b8c8edc19a914eb5b74e99573e42bb6`  
		Last Modified: Thu, 04 Feb 2021 03:20:15 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5445bed80057a6cd7e01dfaa030a56556b866003ab6f64a03511a9ee1e620f12`  
		Last Modified: Thu, 04 Feb 2021 03:20:50 GMT  
		Size: 120.9 MB (120897751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f666961a7e8e733988fd5cce351cd58882c5e8a84ee718e05d258a075afec82a`  
		Last Modified: Thu, 04 Feb 2021 03:20:15 GMT  
		Size: 2.8 KB (2846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; ppc64le

```console
$ docker pull plone@sha256:468c1896a4d667c1e5067416b423ebabeb67518e514140a63aa7c35c55da412d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.2 MB (138156849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6467d71de42b2c1566a90ca4d575348e80df551b933464c8e17c3d3fab9dcda`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 09:37:11 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 09:37:14 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 09:56:42 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Thu, 17 Dec 2020 09:56:46 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 22 Dec 2020 18:59:55 GMT
ENV PYTHON_VERSION=3.8.7
# Tue, 22 Dec 2020 19:08:30 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 22 Dec 2020 19:08:50 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Mon, 01 Feb 2021 22:57:28 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Mon, 01 Feb 2021 22:57:32 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Mon, 01 Feb 2021 22:57:38 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Mon, 01 Feb 2021 22:58:25 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 01 Feb 2021 22:58:30 GMT
CMD ["python3"]
# Tue, 02 Feb 2021 01:05:53 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Tue, 02 Feb 2021 01:06:06 GMT
LABEL plone=5.2.2 os=alpine os.version=3.12 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Tue, 02 Feb 2021 01:06:20 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Tue, 02 Feb 2021 01:06:23 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Tue, 02 Feb 2021 01:24:01 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Tue, 02 Feb 2021 01:24:09 GMT
VOLUME [/data]
# Tue, 02 Feb 2021 01:24:13 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Tue, 02 Feb 2021 01:24:17 GMT
EXPOSE 8080
# Tue, 02 Feb 2021 01:24:21 GMT
WORKDIR /plone/instance
# Tue, 02 Feb 2021 01:24:28 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Tue, 02 Feb 2021 01:24:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 02 Feb 2021 01:24:37 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e32daf0112422799b6475c0b476ff0470e857068b39787218b90ee42adb2bb`  
		Last Modified: Thu, 17 Dec 2020 11:03:32 GMT  
		Size: 283.2 KB (283205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5874758b1135c0eafa5689435faf9d472f60237b02b927cb23bcc3999b9b41da`  
		Last Modified: Tue, 22 Dec 2020 19:23:57 GMT  
		Size: 12.1 MB (12077776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838561cab592ea480c5e8a59b2e241fb5f03e55eae5b65214bc55ba6bbe2acbf`  
		Last Modified: Tue, 22 Dec 2020 19:23:54 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac35e84f6baa24740e50396f2ea3782a8d0cbbe746f1aac05063cb8f2b731621`  
		Last Modified: Mon, 01 Feb 2021 23:17:49 GMT  
		Size: 2.2 MB (2164138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b562cb0f88ecc5b65dd2375246cf8b89e0bca897c9aa9cf83d16045daf0716`  
		Last Modified: Tue, 02 Feb 2021 01:42:36 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607331b51779983842864e2fc24e8bc3f82147793fc46c4ebd215c0f321a142d`  
		Last Modified: Tue, 02 Feb 2021 01:42:36 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7758ef11d486ade4b2f29b80910a13952c538fd75f96050954745a5a6ce768`  
		Last Modified: Tue, 02 Feb 2021 01:43:09 GMT  
		Size: 120.8 MB (120821014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2e17f02906f8fd4f0c8c923f7161ec61a052afffa12ef53348b229527b6ca5`  
		Last Modified: Tue, 02 Feb 2021 01:42:36 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; s390x

```console
$ docker pull plone@sha256:a0e12517ddf3759a243b5b7f3298297234286f881e377103bd972284845d3712
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.8 MB (136802196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bae33701493c5ffc38b5eb2085ef9a136aaf809d25d8b0ae8644e19566354f0c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Thu, 28 Jan 2021 23:41:35 GMT
ADD file:d97e6c37df0fb8306b072d9c0a32f68f5aff583ba849303926644deacfa25eb9 in / 
# Thu, 28 Jan 2021 23:41:36 GMT
CMD ["/bin/sh"]
# Thu, 04 Feb 2021 01:26:41 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 Feb 2021 01:26:42 GMT
ENV LANG=C.UTF-8
# Thu, 04 Feb 2021 01:47:36 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Thu, 04 Feb 2021 01:47:36 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 04 Feb 2021 01:47:37 GMT
ENV PYTHON_VERSION=3.8.7
# Thu, 04 Feb 2021 01:52:54 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 04 Feb 2021 01:52:56 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 04 Feb 2021 01:52:56 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Thu, 04 Feb 2021 01:52:57 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Thu, 04 Feb 2021 01:52:57 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Thu, 04 Feb 2021 01:53:04 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 04 Feb 2021 01:53:04 GMT
CMD ["python3"]
# Thu, 04 Feb 2021 02:48:11 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Thu, 04 Feb 2021 02:48:11 GMT
LABEL plone=5.2.2 os=alpine os.version=3.12 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 04 Feb 2021 02:48:12 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 04 Feb 2021 02:48:12 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Thu, 04 Feb 2021 02:58:05 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 04 Feb 2021 02:58:16 GMT
VOLUME [/data]
# Thu, 04 Feb 2021 02:58:17 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Thu, 04 Feb 2021 02:58:17 GMT
EXPOSE 8080
# Thu, 04 Feb 2021 02:58:18 GMT
WORKDIR /plone/instance
# Thu, 04 Feb 2021 02:58:18 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 04 Feb 2021 02:58:19 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 04 Feb 2021 02:58:19 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:43901f1af0ef9db6b0bf30ac6f6dacd78bf1ecfeb47ad0a93aa2370fa8e62407`  
		Last Modified: Thu, 28 Jan 2021 23:42:09 GMT  
		Size: 2.6 MB (2602059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a61a44cad8b926e10a77d45501ae7da819a804a8e15c7c2021574a86564476`  
		Last Modified: Thu, 04 Feb 2021 02:21:45 GMT  
		Size: 281.7 KB (281703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693c4faefc1addb1b9f9e907d24ba6a4db842dcbd32e0f314dba4051015ae0e1`  
		Last Modified: Thu, 04 Feb 2021 02:21:41 GMT  
		Size: 11.2 MB (11172772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e0ce5150c12c10ff8f53f5bb8b9d30ec975447ce7cc0a76604b3d6e7aa0585`  
		Last Modified: Thu, 04 Feb 2021 02:21:45 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc46f313362225721769862c7ab953bc6c8ce3135e8e51740289b7155e704479`  
		Last Modified: Thu, 04 Feb 2021 02:21:45 GMT  
		Size: 2.2 MB (2163819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5948563f043afea5869e89d2e090e1638947d5bc37803b6951488cdb33588a`  
		Last Modified: Thu, 04 Feb 2021 02:59:14 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39cae497d3fff665af3a339f3a3d06dc6360179cfb7e2bd727f8ad9515090a8`  
		Last Modified: Thu, 04 Feb 2021 02:59:14 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df952f0dad838e2e0de3682c989283b4d2d7881b685375dd3e9ed1bd603a0e2c`  
		Last Modified: Thu, 04 Feb 2021 02:59:31 GMT  
		Size: 120.6 MB (120576349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddbc7f1275d33cf7143471c5f94b39285c9adb573b1e5936816b832d886e9ee`  
		Last Modified: Thu, 04 Feb 2021 02:59:14 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
