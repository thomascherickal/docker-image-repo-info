## `plone:alpine`

```console
$ docker pull plone@sha256:9af17ad4b6daa7867edf16b6b0b0d6d31a3e70fc6d0391f55fc9bc053da97297
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `plone:alpine` - linux; amd64

```console
$ docker pull plone@sha256:50bc876fcdc5702d16712a5fbac1883c843222da2db430fc947c5c6ea95546e9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.7 MB (132692282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d479afc1db048042bc46d0c50ce6a92d100ecdbe97895cdab3727398c8083f1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:48:49 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Jun 2020 19:36:53 GMT
ENV LANG=C.UTF-8
# Wed, 03 Jun 2020 19:36:54 GMT
RUN apk add --no-cache ca-certificates
# Wed, 03 Jun 2020 19:36:54 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 24 Sep 2020 21:55:48 GMT
ENV PYTHON_VERSION=3.8.6
# Thu, 24 Sep 2020 22:02:59 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 24 Sep 2020 22:03:00 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 24 Sep 2020 22:03:00 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 24 Sep 2020 22:03:00 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 24 Sep 2020 22:03:01 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 24 Sep 2020 22:03:07 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 24 Sep 2020 22:03:07 GMT
CMD ["python3"]
# Thu, 24 Sep 2020 22:37:46 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Thu, 24 Sep 2020 22:37:47 GMT
LABEL plone=5.2.2 os=alpine os.version=3.12 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 24 Sep 2020 22:37:49 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 24 Sep 2020 22:37:50 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Thu, 24 Sep 2020 22:46:45 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 24 Sep 2020 22:46:46 GMT
VOLUME [/data]
# Thu, 24 Sep 2020 22:46:47 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Thu, 24 Sep 2020 22:46:47 GMT
EXPOSE 8080
# Thu, 24 Sep 2020 22:46:47 GMT
WORKDIR /plone/instance
# Thu, 24 Sep 2020 22:46:47 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 24 Sep 2020 22:46:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 24 Sep 2020 22:46:47 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b3adc4ff6ffb76ae233f0a92177205845aaf3e9a39e0f96405dabd1423edc9`  
		Last Modified: Wed, 03 Jun 2020 20:14:46 GMT  
		Size: 280.8 KB (280840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaf559fa1affb10216b7bf21b1c9c3e45d3cc3edfa399c99047d99e924a99c9`  
		Last Modified: Thu, 24 Sep 2020 22:13:24 GMT  
		Size: 11.7 MB (11670470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff42851d39f6c873f1d5c89d37afcf1cf4fa33d7f390023af678fd71b50a3fec`  
		Last Modified: Thu, 24 Sep 2020 22:13:22 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba142e34a430954db0696c31922450c0292b4a39458fc3d248fadec7c403f5b`  
		Last Modified: Thu, 24 Sep 2020 22:13:23 GMT  
		Size: 2.1 MB (2119277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2cb761a03c5cbf985822663c93bbb6436ba4ffaf1053c86716a0c0bb6b0339`  
		Last Modified: Thu, 24 Sep 2020 22:47:46 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb88742582db79bedb401bb0008a6fbdc64fd729328e42fb7601d439027fbc5`  
		Last Modified: Thu, 24 Sep 2020 22:47:46 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190f2d91ba97af1b653414b124097c52b160d6b253fedeff4890be584710c1d8`  
		Last Modified: Thu, 24 Sep 2020 22:48:07 GMT  
		Size: 115.8 MB (115818732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da86067a9ac8e62a7a0ee133a46c3dfa11d055c56170c34cbca6362515340b9`  
		Last Modified: Thu, 24 Sep 2020 22:47:46 GMT  
		Size: 2.8 KB (2846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:alpine` - linux; arm variant v6

```console
$ docker pull plone@sha256:f6596e2be39e386aee68db3c440c76dfd42c3b504b4b1180d96368143f04c366
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131712979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:715770b6e7ae6f0f5306afae1f0001897f6b7f7fd4e38958808f7c1c5a17a0ad`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Wed, 03 Jun 2020 18:59:55 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Jun 2020 18:59:56 GMT
ENV LANG=C.UTF-8
# Wed, 03 Jun 2020 18:59:59 GMT
RUN apk add --no-cache ca-certificates
# Wed, 03 Jun 2020 19:00:01 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 24 Sep 2020 20:59:20 GMT
ENV PYTHON_VERSION=3.8.6
# Thu, 24 Sep 2020 21:08:36 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 24 Sep 2020 21:08:39 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 24 Sep 2020 21:08:40 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 24 Sep 2020 21:08:40 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 24 Sep 2020 21:08:41 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 24 Sep 2020 21:08:54 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 24 Sep 2020 21:08:55 GMT
CMD ["python3"]
# Thu, 24 Sep 2020 21:38:36 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Thu, 24 Sep 2020 21:38:37 GMT
LABEL plone=5.2.2 os=alpine os.version=3.12 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 24 Sep 2020 21:38:39 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 24 Sep 2020 21:38:40 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Thu, 24 Sep 2020 21:54:54 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 24 Sep 2020 21:55:01 GMT
VOLUME [/data]
# Thu, 24 Sep 2020 21:55:01 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Thu, 24 Sep 2020 21:55:02 GMT
EXPOSE 8080
# Thu, 24 Sep 2020 21:55:03 GMT
WORKDIR /plone/instance
# Thu, 24 Sep 2020 21:55:04 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 24 Sep 2020 21:55:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 24 Sep 2020 21:55:05 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba84132d8cf30d261b7b1e4e503e67af8ea432e7f530a830161cc1b1bd53e82`  
		Last Modified: Wed, 03 Jun 2020 19:55:42 GMT  
		Size: 281.0 KB (281040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2deb0917d132ba0e13e1c3cde5ab4c000f3894a50af54cbbe6c8a31519df6a8c`  
		Last Modified: Thu, 24 Sep 2020 21:19:45 GMT  
		Size: 11.3 MB (11290061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504f63b12f177e21eebbe698e64d4f5f7cf7593de608cdc9dbfe67cd072cb374`  
		Last Modified: Thu, 24 Sep 2020 21:19:41 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89425b3314bfe14ca12de183ce8c4c74e2728ef2bb87a2949af4a2c8823e16b1`  
		Last Modified: Thu, 24 Sep 2020 21:19:42 GMT  
		Size: 2.1 MB (2119514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9a4f8c79f4ac8a59fff013c2d385836b1d35f7735fc5356ced7ba2332470a6`  
		Last Modified: Thu, 24 Sep 2020 21:55:17 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6782f92759c9bcca2a98e9d6bd1700398140b74b657382eb9eb4467c5aa87c`  
		Last Modified: Thu, 24 Sep 2020 21:55:17 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6364f1a45f915106ad3790b30078e37b671c2b5f19fb2b95515313546ea7da0e`  
		Last Modified: Thu, 24 Sep 2020 21:56:00 GMT  
		Size: 115.4 MB (115413588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f213bf3915be9837a0acd9094fab8a29c15a2dc1e75905ec3e78d557eaec53`  
		Last Modified: Thu, 24 Sep 2020 21:55:16 GMT  
		Size: 2.8 KB (2847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:alpine` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:05e6558a41d289fd213e4c76ec27717e725e075b702c7ecbd45ce05d4a1efa3f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132549108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1be372dc7a46b75835803fa0f13b69e41ae1f974fbf199c8006e96c9305908a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 02:35:35 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Jun 2020 18:57:57 GMT
ENV LANG=C.UTF-8
# Wed, 03 Jun 2020 18:58:00 GMT
RUN apk add --no-cache ca-certificates
# Wed, 03 Jun 2020 18:58:01 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 24 Sep 2020 21:02:11 GMT
ENV PYTHON_VERSION=3.8.6
# Thu, 24 Sep 2020 21:09:22 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 24 Sep 2020 21:09:25 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 24 Sep 2020 21:09:26 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 24 Sep 2020 21:09:26 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 24 Sep 2020 21:09:27 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 24 Sep 2020 21:09:38 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 24 Sep 2020 21:09:39 GMT
CMD ["python3"]
# Thu, 24 Sep 2020 21:51:30 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Thu, 24 Sep 2020 21:51:31 GMT
LABEL plone=5.2.2 os=alpine os.version=3.12 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 24 Sep 2020 21:51:34 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 24 Sep 2020 21:51:35 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Thu, 24 Sep 2020 22:08:50 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 24 Sep 2020 22:08:56 GMT
VOLUME [/data]
# Thu, 24 Sep 2020 22:08:57 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Thu, 24 Sep 2020 22:08:58 GMT
EXPOSE 8080
# Thu, 24 Sep 2020 22:09:00 GMT
WORKDIR /plone/instance
# Thu, 24 Sep 2020 22:09:01 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 24 Sep 2020 22:09:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 24 Sep 2020 22:09:04 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d489d24c26399308b276dfa175c049e531d2686fb99e250ad3ede210fd01e9e`  
		Last Modified: Wed, 03 Jun 2020 19:46:54 GMT  
		Size: 281.3 KB (281267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b06c34864ddca6d4776f796a0df3a318c4892e2e24f042cf214472856ee7168`  
		Last Modified: Thu, 24 Sep 2020 21:21:02 GMT  
		Size: 11.8 MB (11765524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:202e94f46b2eefc6a19231b9f3d9b6582a0114cbcb2960cce78767ef32a1a636`  
		Last Modified: Thu, 24 Sep 2020 21:20:59 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d63eaed07be50465852bff4621f5923339a3db74b7c11dc1ae6a4d54243120`  
		Last Modified: Thu, 24 Sep 2020 21:21:00 GMT  
		Size: 2.1 MB (2119504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f90426b031b4b73236e20bc4061f39606b3ec60f52b72979ac23520b7fb7726`  
		Last Modified: Thu, 24 Sep 2020 22:10:40 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c84921072f2d00ac8ed24e681e8fe067ab9f43aa6e5fd3c7841ca9e46ed03f`  
		Last Modified: Thu, 24 Sep 2020 22:10:41 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94855cb3b9793f15cf3bb80a76f29ab4ba723fd7fa971f647d4ccdff0d4aca1`  
		Last Modified: Thu, 24 Sep 2020 22:11:16 GMT  
		Size: 115.7 MB (115669362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16fda5a85fd445fa5317b1a6267d6991dfa2792d5b11b82183f0f94f2eeb882`  
		Last Modified: Thu, 24 Sep 2020 22:10:41 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:alpine` - linux; 386

```console
$ docker pull plone@sha256:07f7d63c6a80c0363e50a521c911b1426a3d7dd7cc35934d78c2fa9682a8bf1f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.0 MB (133035977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c112b0241ec5037947201ae1377e04a4c612b782cf8185c11669671284a6357`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Wed, 03 Jun 2020 18:45:48 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Jun 2020 18:45:48 GMT
ENV LANG=C.UTF-8
# Wed, 03 Jun 2020 18:45:49 GMT
RUN apk add --no-cache ca-certificates
# Wed, 03 Jun 2020 18:45:49 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 24 Sep 2020 21:13:25 GMT
ENV PYTHON_VERSION=3.8.6
# Thu, 24 Sep 2020 21:20:48 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 24 Sep 2020 21:20:49 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 24 Sep 2020 21:20:49 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 24 Sep 2020 21:20:49 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 24 Sep 2020 21:20:49 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 24 Sep 2020 21:20:57 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 24 Sep 2020 21:20:57 GMT
CMD ["python3"]
# Thu, 24 Sep 2020 22:00:40 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Thu, 24 Sep 2020 22:00:40 GMT
LABEL plone=5.2.2 os=alpine os.version=3.12 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 24 Sep 2020 22:00:41 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 24 Sep 2020 22:00:41 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Thu, 24 Sep 2020 22:14:39 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 24 Sep 2020 22:14:40 GMT
VOLUME [/data]
# Thu, 24 Sep 2020 22:14:40 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Thu, 24 Sep 2020 22:14:41 GMT
EXPOSE 8080
# Thu, 24 Sep 2020 22:14:41 GMT
WORKDIR /plone/instance
# Thu, 24 Sep 2020 22:14:41 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 24 Sep 2020 22:14:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 24 Sep 2020 22:14:41 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded523869d7b2121c2a5838365e9f75504b850ecae6661c940242d3456bd53d7`  
		Last Modified: Wed, 03 Jun 2020 19:28:31 GMT  
		Size: 281.4 KB (281373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c0413464c07a774067b12d8966058a68e4a628914aa8870f83cdf0bb06c5ee`  
		Last Modified: Thu, 24 Sep 2020 21:34:06 GMT  
		Size: 11.9 MB (11857864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0cd193bb15f9b6f88e2fe65154ba3082bf04e1f3487bd4525b5a3fc05f0b0d`  
		Last Modified: Thu, 24 Sep 2020 21:33:58 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a85caeef3edab250950c1ca44d680b81093600d8fd606389517609d55e48194`  
		Last Modified: Thu, 24 Sep 2020 21:34:01 GMT  
		Size: 2.1 MB (2119285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577c5dc28de714965c57f4b60f24c8d7dc75c68b4779ce5f440a9cc2e0262c69`  
		Last Modified: Thu, 24 Sep 2020 22:15:53 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e642e5630c6653307b75c0223940a28270be21aa6128dbdccbbc35be767ce9`  
		Last Modified: Thu, 24 Sep 2020 22:15:53 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3751a1e0c085cd11c5f6a807b486e85f871d8d7817330851fea1ff5b8b1d8f3c`  
		Last Modified: Thu, 24 Sep 2020 22:16:22 GMT  
		Size: 116.0 MB (115979733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469cc47614e7fc709ec40903cce0df2c10335bb6c4c954baeede680037c8b024`  
		Last Modified: Thu, 24 Sep 2020 22:15:52 GMT  
		Size: 2.8 KB (2846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:alpine` - linux; ppc64le

```console
$ docker pull plone@sha256:63d7933b61db941e90799b92ad5801735f9a0b19272aa09a1df57e347cc4caf8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133911014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa768e305613f3c49d7f1a1f363b5534fe8d929010e49458aa1800aacf12ec3b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Wed, 03 Jun 2020 19:35:54 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Jun 2020 19:35:58 GMT
ENV LANG=C.UTF-8
# Wed, 03 Jun 2020 19:36:09 GMT
RUN apk add --no-cache ca-certificates
# Wed, 03 Jun 2020 19:36:12 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 24 Sep 2020 22:34:26 GMT
ENV PYTHON_VERSION=3.8.6
# Thu, 24 Sep 2020 22:42:30 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 24 Sep 2020 22:42:39 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 24 Sep 2020 22:42:42 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 24 Sep 2020 22:42:47 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 24 Sep 2020 22:42:50 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 24 Sep 2020 22:43:09 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 24 Sep 2020 22:43:12 GMT
CMD ["python3"]
# Fri, 25 Sep 2020 00:16:36 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Fri, 25 Sep 2020 00:16:41 GMT
LABEL plone=5.2.2 os=alpine os.version=3.12 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Fri, 25 Sep 2020 00:16:55 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Fri, 25 Sep 2020 00:16:57 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Fri, 25 Sep 2020 00:33:12 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Fri, 25 Sep 2020 00:33:20 GMT
VOLUME [/data]
# Fri, 25 Sep 2020 00:33:24 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Fri, 25 Sep 2020 00:33:30 GMT
EXPOSE 8080
# Fri, 25 Sep 2020 00:33:36 GMT
WORKDIR /plone/instance
# Fri, 25 Sep 2020 00:33:40 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Fri, 25 Sep 2020 00:33:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 25 Sep 2020 00:33:49 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c9759563702d3bc987f9dad6559da6de6fa68093dc6b51fb097c1c4abc1876`  
		Last Modified: Wed, 03 Jun 2020 20:26:29 GMT  
		Size: 285.0 KB (285014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17b2fb5e259ccbc7ee8a5c3dc16ec7d98b9d9f8dddf2c87e7587c718e345716`  
		Last Modified: Thu, 24 Sep 2020 22:56:18 GMT  
		Size: 12.4 MB (12418345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8af143f354ce29ccbd0d56a72dceeed09ad870f8b70bc8781c3a61c09a8465`  
		Last Modified: Thu, 24 Sep 2020 22:56:15 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43a55068ee12179bdf7f209ce74cbbc96c34f57db77189c1c06b8014591eb70`  
		Last Modified: Thu, 24 Sep 2020 22:56:16 GMT  
		Size: 2.1 MB (2119541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0c28f940f7fae93b0b62d458fbd11b416324ef7b73d9c07bd820652feeb29a`  
		Last Modified: Fri, 25 Sep 2020 00:38:48 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbb1030af12bc2e18cd1fcd67d55d5fa9d7aa08dde2f37bc7c9e3492780913e`  
		Last Modified: Fri, 25 Sep 2020 00:38:48 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0466312756c36c87cdbe8b04c1558c68c15b7decbca97611a7949bd55def65`  
		Last Modified: Fri, 25 Sep 2020 00:39:16 GMT  
		Size: 116.3 MB (116277427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db058faa2fdc8d7c38b909ad3a05d012d69f908dd46fa913aaeca237b5cde1d`  
		Last Modified: Fri, 25 Sep 2020 00:38:48 GMT  
		Size: 2.8 KB (2846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:alpine` - linux; s390x

```console
$ docker pull plone@sha256:f77cce5cb151713e4df6d729189f760ddd3f0ecb6f862209e9ee1593b29390d2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.2 MB (132175373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ead12696532bf450d7f6befec55e3ed1863b13625d98472849db1e7a4e5aee2b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Wed, 03 Jun 2020 19:13:11 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Jun 2020 19:13:11 GMT
ENV LANG=C.UTF-8
# Wed, 03 Jun 2020 19:13:14 GMT
RUN apk add --no-cache ca-certificates
# Wed, 03 Jun 2020 19:13:14 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Thu, 24 Sep 2020 21:07:35 GMT
ENV PYTHON_VERSION=3.8.6
# Thu, 24 Sep 2020 21:11:39 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Thu, 24 Sep 2020 21:11:40 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Thu, 24 Sep 2020 21:11:40 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Thu, 24 Sep 2020 21:11:40 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Thu, 24 Sep 2020 21:11:40 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Thu, 24 Sep 2020 21:11:45 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 24 Sep 2020 21:11:45 GMT
CMD ["python3"]
# Thu, 24 Sep 2020 21:39:58 GMT
ENV PIP=20.2.3 ZC_BUILDOUT=2.13.3 SETUPTOOLS=50.3.0 WHEEL=0.35.1 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.2 PLONE_VERSION_RELEASE=Plone-5.2.2-UnifiedInstaller PLONE_MD5=a603eddfd3abb0528f0861472ebac934
# Thu, 24 Sep 2020 21:39:58 GMT
LABEL plone=5.2.2 os=alpine os.version=3.12 name=Plone 5.2 description=Plone image, based on Unified Installer maintainer=Plone Community
# Thu, 24 Sep 2020 21:39:59 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Thu, 24 Sep 2020 21:39:59 GMT
COPY file:e1c551fc370867c153c440542b0f297049c860021da1d914d102da702cd4376a in /plone/instance/ 
# Thu, 24 Sep 2020 21:46:48 GMT
RUN apk add --no-cache --virtual .build-deps     gcc     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     pcre-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     rsync     libxml2     libxslt     libjpeg-turbo && rm -rf /plone/buildout-cache/downloads/*
# Thu, 24 Sep 2020 21:46:56 GMT
VOLUME [/data]
# Thu, 24 Sep 2020 21:46:56 GMT
COPY multi:96b4b1619dec8ba8c0507bd3de7fe85d75d30049c6ebd1a2599a7df4353563e5 in / 
# Thu, 24 Sep 2020 21:46:56 GMT
EXPOSE 8080
# Thu, 24 Sep 2020 21:46:56 GMT
WORKDIR /plone/instance
# Thu, 24 Sep 2020 21:46:57 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Thu, 24 Sep 2020 21:46:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 24 Sep 2020 21:46:57 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b76e1d722a55ff4f330c758d9814944d8ab0c8761b42febad3c13edcbc7d4f`  
		Last Modified: Wed, 03 Jun 2020 22:40:13 GMT  
		Size: 281.4 KB (281387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03da35cdfc7442fd260711b60cdfc1df4029191777d352c972c67f44dee2c7d`  
		Last Modified: Thu, 24 Sep 2020 21:18:04 GMT  
		Size: 11.7 MB (11656923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec31c24c702ea17b5562998fd037ea78f8275a82d79b377e53da6dadb0584857`  
		Last Modified: Thu, 24 Sep 2020 21:18:01 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c52b5203c218f478ca3fdce49e47d50886c0b471c038ba396634f81056d3f6`  
		Last Modified: Thu, 24 Sep 2020 21:18:02 GMT  
		Size: 2.1 MB (2119562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28e66b86cd4507235eadc0f6cdbf1f4c38262b1e3650629c47f5d1bc2fc3709`  
		Last Modified: Thu, 24 Sep 2020 21:47:49 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7efe0593cf792343660d554d8b78b9c0d2efa9cdc9f4f42764cf8cef0c8aea23`  
		Last Modified: Thu, 24 Sep 2020 21:47:49 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab9cd0ce4ff6faba6fdab3bbc9634efbdd782279ebc7677277736133fbc986f`  
		Last Modified: Thu, 24 Sep 2020 21:48:05 GMT  
		Size: 115.5 MB (115545831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7903b3309cdb359c81d222ed91112b573f213ab9138d3bb1e07a8d7c153b685`  
		Last Modified: Thu, 24 Sep 2020 21:47:49 GMT  
		Size: 2.8 KB (2845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
