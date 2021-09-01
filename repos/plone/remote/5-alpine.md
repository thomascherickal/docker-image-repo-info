## `plone:5-alpine`

```console
$ docker pull plone@sha256:a90032d1dcc9bf6e7d3252c926b33ce9abbc9151c8289d8031e90f287044febb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `plone:5-alpine` - linux; amd64

```console
$ docker pull plone@sha256:22fcffa50191253d244edc07b531b7cb5ea07e9c96b3a5471894270d85fe711b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.2 MB (152230151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdaa09fd74549a74df081f0cc8f800b438217158ef77a2c4b4cda12a0dc476f6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:27:41 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Aug 2021 23:31:48 GMT
ENV LANG=C.UTF-8
# Fri, 27 Aug 2021 23:49:40 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Fri, 27 Aug 2021 23:49:40 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 31 Aug 2021 19:50:48 GMT
ENV PYTHON_VERSION=3.8.12
# Tue, 31 Aug 2021 19:58:45 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 31 Aug 2021 19:58:47 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 31 Aug 2021 19:58:48 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 31 Aug 2021 19:58:48 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Tue, 31 Aug 2021 19:58:48 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Tue, 31 Aug 2021 19:58:59 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 31 Aug 2021 19:59:00 GMT
CMD ["python3"]
# Tue, 31 Aug 2021 23:00:45 GMT
ENV PIP=21.0.1 ZC_BUILDOUT=2.13.4 SETUPTOOLS=51.3.3 WHEEL=0.36.2 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.4 PLONE_VERSION_RELEASE=Plone-5.2.4-UnifiedInstaller-1.0 PLONE_MD5=b682cdf2384e692c033077f448b68afd
# Tue, 31 Aug 2021 23:00:46 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Tue, 31 Aug 2021 23:00:46 GMT
COPY file:3ef405a950854449713102e91399f13c5d85d531f4bb6247863ee4357e81ed1c in /plone/instance/ 
# Tue, 31 Aug 2021 23:15:04 GMT
RUN apk add --no-cache --virtual .build-deps     build-base     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     mariadb-dev     openldap-dev     pcre-dev     postgresql-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     git     rsync     libxml2     libxslt     libjpeg-turbo     mariadb-connector-c     postgresql-client && rm -rf /plone/buildout-cache/downloads/*
# Tue, 31 Aug 2021 23:15:06 GMT
VOLUME [/data]
# Tue, 31 Aug 2021 23:15:06 GMT
COPY multi:42ced57fe3a0905e0e2388d9f8e6e5bd32fb0db140cd61d93fb9326734196d09 in / 
# Tue, 31 Aug 2021 23:15:06 GMT
EXPOSE 8080
# Tue, 31 Aug 2021 23:15:06 GMT
WORKDIR /plone/instance
# Tue, 31 Aug 2021 23:15:07 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Tue, 31 Aug 2021 23:15:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 31 Aug 2021 23:15:07 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11246b421beac7bdab2cd3f620a098af2a8bbbf8e608bef7bf056866e710734`  
		Last Modified: Sat, 28 Aug 2021 00:16:58 GMT  
		Size: 281.5 KB (281499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6f9a3065f19547192c18fa1ed3dd5ec163a387fa47d78aec28e960f5c1097c`  
		Last Modified: Tue, 31 Aug 2021 20:13:17 GMT  
		Size: 11.2 MB (11243987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a167f2660c7a9f713d5ccff5a310c5cf7cf2869c3fa195f2296280f9be43d`  
		Last Modified: Tue, 31 Aug 2021 20:13:15 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97dfd359f60b0e2d919eb9e9d3158fc711265d9cb072ccb48d2b0d9c39fed81a`  
		Last Modified: Tue, 31 Aug 2021 20:13:16 GMT  
		Size: 2.3 MB (2348641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45750b12cf620f9f882146b568b6faa208dbcb28bd9d47b2344dddd12bf807b`  
		Last Modified: Tue, 31 Aug 2021 23:16:58 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19be7e6e97f2564e03a929c156f96c822209a3ed23d0d0438c7357d6066dc234`  
		Last Modified: Tue, 31 Aug 2021 23:16:55 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f17019db559429b1546cc10598b759745e6c392fdb9b68d0841c2be503c27ce`  
		Last Modified: Tue, 31 Aug 2021 23:17:22 GMT  
		Size: 135.5 MB (135534915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9964d1e5c5c9de67f4a0c92b35a75905f9ee0d1575e852751aa9513c61a8bf`  
		Last Modified: Tue, 31 Aug 2021 23:16:55 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; arm variant v6

```console
$ docker pull plone@sha256:02f4c88046a43b19052e453204cf3a85961ece233b0105ad7c640790a951e600
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (150988795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffb0876ba411cb6e979baa834594bcddd20ab4d3f5503d2275cd803796f89a64`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 22:42:05 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Aug 2021 22:42:06 GMT
ENV LANG=C.UTF-8
# Fri, 27 Aug 2021 23:08:50 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Fri, 27 Aug 2021 23:08:51 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 31 Aug 2021 21:40:48 GMT
ENV PYTHON_VERSION=3.8.12
# Tue, 31 Aug 2021 21:51:49 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 31 Aug 2021 21:51:51 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 31 Aug 2021 21:51:52 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 31 Aug 2021 21:51:52 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Tue, 31 Aug 2021 21:51:52 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Tue, 31 Aug 2021 21:52:08 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 31 Aug 2021 21:52:08 GMT
CMD ["python3"]
# Wed, 01 Sep 2021 00:51:14 GMT
ENV PIP=21.0.1 ZC_BUILDOUT=2.13.4 SETUPTOOLS=51.3.3 WHEEL=0.36.2 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.4 PLONE_VERSION_RELEASE=Plone-5.2.4-UnifiedInstaller-1.0 PLONE_MD5=b682cdf2384e692c033077f448b68afd
# Wed, 01 Sep 2021 00:51:16 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 01 Sep 2021 00:51:16 GMT
COPY file:3ef405a950854449713102e91399f13c5d85d531f4bb6247863ee4357e81ed1c in /plone/instance/ 
# Wed, 01 Sep 2021 01:16:33 GMT
RUN apk add --no-cache --virtual .build-deps     build-base     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     mariadb-dev     openldap-dev     pcre-dev     postgresql-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     git     rsync     libxml2     libxslt     libjpeg-turbo     mariadb-connector-c     postgresql-client && rm -rf /plone/buildout-cache/downloads/*
# Wed, 01 Sep 2021 01:16:36 GMT
VOLUME [/data]
# Wed, 01 Sep 2021 01:16:37 GMT
COPY multi:42ced57fe3a0905e0e2388d9f8e6e5bd32fb0db140cd61d93fb9326734196d09 in / 
# Wed, 01 Sep 2021 01:16:37 GMT
EXPOSE 8080
# Wed, 01 Sep 2021 01:16:38 GMT
WORKDIR /plone/instance
# Wed, 01 Sep 2021 01:16:38 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 01 Sep 2021 01:16:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Sep 2021 01:16:39 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8e9151897ef0dc047f9ca095a7c3486bf84800e0cf22dcd437dfebbade82d6`  
		Last Modified: Fri, 27 Aug 2021 23:56:29 GMT  
		Size: 281.7 KB (281669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301f8863fef9cfc0749b56e52d4e5e08f8682c60d16837de44dac77d3c668f48`  
		Last Modified: Tue, 31 Aug 2021 22:08:59 GMT  
		Size: 10.8 MB (10834657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fba06605d613f8a3859559f5f2662c24f7de3b834b66af59157df5dda06ffd2`  
		Last Modified: Tue, 31 Aug 2021 22:08:52 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f4c5a6dbf2df548cecb97f190d69204a1cbc8cc3f407e321bad27f3aa11048`  
		Last Modified: Tue, 31 Aug 2021 22:08:54 GMT  
		Size: 2.3 MB (2348883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e760881df794ea1e78d2f5de785cee80bb923611387ad9f95e456d13d4e3d82d`  
		Last Modified: Wed, 01 Sep 2021 01:17:12 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ed427b63b446d668e8fc7d84656ce69dc0d81e7897d20529e14b75ff670350`  
		Last Modified: Wed, 01 Sep 2021 01:17:12 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32bcd70c4d0a09e4321432e174451bde2804c5ef05bbfd85c8ab3d994b0aaafd`  
		Last Modified: Wed, 01 Sep 2021 01:19:01 GMT  
		Size: 134.9 MB (134889473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8988195412370b93d572fc4277f7df5877aadbce4999b93d7582a20cc375d137`  
		Last Modified: Wed, 01 Sep 2021 01:17:12 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; arm64 variant v8

```console
$ docker pull plone@sha256:21ee0a01d231cc7fc3d5258fa22c9c8e19deb50c042d3f798e99eb313a8ec78b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.1 MB (152114943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce5b531709b76f5db56436b04901933a0dd588de7efd53512f09cee9f86a2e43`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:18:09 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Aug 2021 00:00:34 GMT
ENV LANG=C.UTF-8
# Sat, 28 Aug 2021 00:14:42 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Sat, 28 Aug 2021 00:14:42 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 28 Aug 2021 00:14:42 GMT
ENV PYTHON_VERSION=3.8.11
# Sat, 28 Aug 2021 00:20:29 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Sat, 28 Aug 2021 00:20:30 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 28 Aug 2021 00:20:30 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Sat, 28 Aug 2021 00:20:30 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Sat, 28 Aug 2021 00:20:30 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Sat, 28 Aug 2021 00:20:37 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 28 Aug 2021 00:20:37 GMT
CMD ["python3"]
# Sat, 28 Aug 2021 04:52:34 GMT
ENV PIP=21.0.1 ZC_BUILDOUT=2.13.4 SETUPTOOLS=51.3.3 WHEEL=0.36.2 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.4 PLONE_VERSION_RELEASE=Plone-5.2.4-UnifiedInstaller-1.0 PLONE_MD5=b682cdf2384e692c033077f448b68afd
# Sat, 28 Aug 2021 04:52:35 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Sat, 28 Aug 2021 04:52:35 GMT
COPY file:3ef405a950854449713102e91399f13c5d85d531f4bb6247863ee4357e81ed1c in /plone/instance/ 
# Sat, 28 Aug 2021 05:06:35 GMT
RUN apk add --no-cache --virtual .build-deps     build-base     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     mariadb-dev     openldap-dev     pcre-dev     postgresql-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     git     rsync     libxml2     libxslt     libjpeg-turbo     mariadb-connector-c     postgresql-client && rm -rf /plone/buildout-cache/downloads/*
# Sat, 28 Aug 2021 05:06:37 GMT
VOLUME [/data]
# Sat, 28 Aug 2021 05:06:37 GMT
COPY multi:42ced57fe3a0905e0e2388d9f8e6e5bd32fb0db140cd61d93fb9326734196d09 in / 
# Sat, 28 Aug 2021 05:06:37 GMT
EXPOSE 8080
# Sat, 28 Aug 2021 05:06:38 GMT
WORKDIR /plone/instance
# Sat, 28 Aug 2021 05:06:38 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Sat, 28 Aug 2021 05:06:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 28 Aug 2021 05:06:38 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82397dd0b53e51c9238ac3da861e9862f3f01e133f3447bc318b86ede25c8bf1`  
		Last Modified: Sat, 28 Aug 2021 00:42:33 GMT  
		Size: 281.7 KB (281687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40971b39b09e5407ceab6759d4530af2fe42e80bb7b1a0b74cf3a11f6a76113`  
		Last Modified: Sat, 28 Aug 2021 00:42:35 GMT  
		Size: 11.3 MB (11302672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5767b85cc44021cb23496a863930f97b4dbc708c99ac9000b45691253a98b7af`  
		Last Modified: Sat, 28 Aug 2021 00:42:33 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461fa2f93e644eefe4052112db75fbbbfc7376df0e24761f242ba5dd85e3517f`  
		Last Modified: Sat, 28 Aug 2021 00:42:34 GMT  
		Size: 2.3 MB (2348680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d226c0060631f357ba2675c4b661e84bd904215aa5a0166d7eada7805c7739c`  
		Last Modified: Sat, 28 Aug 2021 05:07:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12c3bd1c396e5c078b03bbc1457db73487aa66ecf624594837aca2568a70c57`  
		Last Modified: Sat, 28 Aug 2021 05:07:02 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d45ff74e26fc6b470c9ffe70e75cc2a716260deae543f143a233c97738525a`  
		Last Modified: Sat, 28 Aug 2021 05:07:25 GMT  
		Size: 135.5 MB (135463418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bd853302ae339b401fce837cfdaf68ef9674e43daa0478fa8a3726c4a5b95e`  
		Last Modified: Sat, 28 Aug 2021 05:07:02 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; 386

```console
$ docker pull plone@sha256:06b9977e390af7808867c98fc75db4db37ad68b093bd724f6aa37cd24dc14006
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.4 MB (153445958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2dc0fc2788ce22c44a74d4307e359190b768bc7780f9ba7e41a7197a5ab53f1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 27 Aug 2021 17:38:29 GMT
ADD file:42a7bc5a08b546b47049dd0f89ae4e7a8c86342f87000f39ade3ff52916a6c2e in / 
# Fri, 27 Aug 2021 17:38:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 22:56:18 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Aug 2021 22:56:19 GMT
ENV LANG=C.UTF-8
# Fri, 27 Aug 2021 23:22:52 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Fri, 27 Aug 2021 23:22:53 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Tue, 31 Aug 2021 20:43:27 GMT
ENV PYTHON_VERSION=3.8.12
# Tue, 31 Aug 2021 20:51:14 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 31 Aug 2021 20:51:15 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 31 Aug 2021 20:51:15 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 31 Aug 2021 20:51:16 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Tue, 31 Aug 2021 20:51:16 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Tue, 31 Aug 2021 20:51:25 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 31 Aug 2021 20:51:26 GMT
CMD ["python3"]
# Tue, 31 Aug 2021 21:48:05 GMT
ENV PIP=21.0.1 ZC_BUILDOUT=2.13.4 SETUPTOOLS=51.3.3 WHEEL=0.36.2 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.4 PLONE_VERSION_RELEASE=Plone-5.2.4-UnifiedInstaller-1.0 PLONE_MD5=b682cdf2384e692c033077f448b68afd
# Tue, 31 Aug 2021 21:48:06 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Tue, 31 Aug 2021 21:48:06 GMT
COPY file:3ef405a950854449713102e91399f13c5d85d531f4bb6247863ee4357e81ed1c in /plone/instance/ 
# Tue, 31 Aug 2021 22:03:54 GMT
RUN apk add --no-cache --virtual .build-deps     build-base     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     mariadb-dev     openldap-dev     pcre-dev     postgresql-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     git     rsync     libxml2     libxslt     libjpeg-turbo     mariadb-connector-c     postgresql-client && rm -rf /plone/buildout-cache/downloads/*
# Tue, 31 Aug 2021 22:03:57 GMT
VOLUME [/data]
# Tue, 31 Aug 2021 22:03:57 GMT
COPY multi:42ced57fe3a0905e0e2388d9f8e6e5bd32fb0db140cd61d93fb9326734196d09 in / 
# Tue, 31 Aug 2021 22:03:57 GMT
EXPOSE 8080
# Tue, 31 Aug 2021 22:03:58 GMT
WORKDIR /plone/instance
# Tue, 31 Aug 2021 22:03:58 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Tue, 31 Aug 2021 22:03:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 31 Aug 2021 22:03:58 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:b11ae9fc5d8a106cfed3a6f6c75e5b5b5797c566fac4411622b4055df6541286`  
		Last Modified: Fri, 27 Aug 2021 17:39:18 GMT  
		Size: 2.8 MB (2822857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc387334281d3d644874c7fa4e676cf60daf255166116e3e86f51d42c1fb1c3`  
		Last Modified: Sat, 28 Aug 2021 00:02:33 GMT  
		Size: 282.0 KB (282044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6366d56a862d9afc46f19f490be2aad447ee5bd8a243502a71f6240126dcecaa`  
		Last Modified: Tue, 31 Aug 2021 21:09:12 GMT  
		Size: 11.4 MB (11433452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1927948df88b3052218c6e6063ab72fb1f66e66d1f8bc8af04453ac2ad2a01`  
		Last Modified: Tue, 31 Aug 2021 21:09:09 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a17d5725064e42d756124d8296739e49ce9e919dea69009cb5cd8a7cd886d52`  
		Last Modified: Tue, 31 Aug 2021 21:09:10 GMT  
		Size: 2.3 MB (2348829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de97a13a1d6ec25004eb32327f5e7a19b6c6af4847252c439a04ad62b87d4c9`  
		Last Modified: Tue, 31 Aug 2021 22:04:19 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837f30332771b91a9509573bfc864d79dfcef8b44b31420d1a6ac516b5ab4365`  
		Last Modified: Tue, 31 Aug 2021 22:04:19 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a821177d6aa02d82c5435c3426e7f4df94882f81e8f137a70ffd002fe87d6dd3`  
		Last Modified: Tue, 31 Aug 2021 22:04:51 GMT  
		Size: 136.6 MB (136552111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fff634bf29c6b1412a9f93d53e483aca2d1cfb4777b51f7c4915c12fa78cf96`  
		Last Modified: Tue, 31 Aug 2021 22:04:18 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; ppc64le

```console
$ docker pull plone@sha256:57648a7dfc70da44649cfd14823d8f5bc4eeac64bda732e7405bec2a381fb240
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.9 MB (153932869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7182af6d7903e4c931e6e8227a9fa527e3f1a588f9692bf3575bab3b150fbda8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 01:50:43 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Aug 2021 01:50:49 GMT
ENV LANG=C.UTF-8
# Sat, 28 Aug 2021 02:13:13 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Sat, 28 Aug 2021 02:13:17 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Sat, 28 Aug 2021 02:13:20 GMT
ENV PYTHON_VERSION=3.8.11
# Sat, 28 Aug 2021 02:21:27 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Sat, 28 Aug 2021 02:21:45 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Sat, 28 Aug 2021 02:21:48 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Sat, 28 Aug 2021 02:21:52 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Sat, 28 Aug 2021 02:21:55 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Sat, 28 Aug 2021 02:22:17 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 28 Aug 2021 02:22:21 GMT
CMD ["python3"]
# Sat, 28 Aug 2021 07:16:56 GMT
ENV PIP=21.0.1 ZC_BUILDOUT=2.13.4 SETUPTOOLS=51.3.3 WHEEL=0.36.2 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.4 PLONE_VERSION_RELEASE=Plone-5.2.4-UnifiedInstaller-1.0 PLONE_MD5=b682cdf2384e692c033077f448b68afd
# Sat, 28 Aug 2021 07:17:15 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Sat, 28 Aug 2021 07:17:17 GMT
COPY file:3ef405a950854449713102e91399f13c5d85d531f4bb6247863ee4357e81ed1c in /plone/instance/ 
# Sat, 28 Aug 2021 07:39:06 GMT
RUN apk add --no-cache --virtual .build-deps     build-base     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     mariadb-dev     openldap-dev     pcre-dev     postgresql-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     git     rsync     libxml2     libxslt     libjpeg-turbo     mariadb-connector-c     postgresql-client && rm -rf /plone/buildout-cache/downloads/*
# Sat, 28 Aug 2021 07:39:15 GMT
VOLUME [/data]
# Sat, 28 Aug 2021 07:39:19 GMT
COPY multi:42ced57fe3a0905e0e2388d9f8e6e5bd32fb0db140cd61d93fb9326734196d09 in / 
# Sat, 28 Aug 2021 07:39:21 GMT
EXPOSE 8080
# Sat, 28 Aug 2021 07:39:28 GMT
WORKDIR /plone/instance
# Sat, 28 Aug 2021 07:39:30 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Sat, 28 Aug 2021 07:39:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 28 Aug 2021 07:39:40 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fe2654905aa17b30aba2abaf1ea3d9276357d43f46e9765bf8ee47d4fd2432`  
		Last Modified: Sat, 28 Aug 2021 02:51:08 GMT  
		Size: 283.6 KB (283640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a93813d7dbbf811b7c74b4ca6d33a56238a2b1a9cde6876e33ded3a933d3180`  
		Last Modified: Sat, 28 Aug 2021 02:51:11 GMT  
		Size: 11.5 MB (11539604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4286dab3d0a251cf71f542db0b5161aee17d3d43b9bc018ede7e8e72c675d3`  
		Last Modified: Sat, 28 Aug 2021 02:51:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451d21525d8849a28e62a608c4dc86278b723195cdfa5e8185891733a5e3e5da`  
		Last Modified: Sat, 28 Aug 2021 02:51:09 GMT  
		Size: 2.3 MB (2348866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3a424ea717a4f5c59765f411ae6496556e9f0f7535a8eef814765973cb309f`  
		Last Modified: Sat, 28 Aug 2021 07:40:11 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50582b7f3264b6d9ed33518ae601a42d951aa2237cbbe7f449f2501c4abd809`  
		Last Modified: Sat, 28 Aug 2021 07:40:10 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca641b8a003daaec56bd504614f272f8531672f5fc7edf51e6c91c244f282026`  
		Last Modified: Sat, 28 Aug 2021 07:40:38 GMT  
		Size: 136.9 MB (136941797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d15a9ac92d0136da4505e4e7c4b1165b5f22d1cb392f347ea8aaa894d61ecba`  
		Last Modified: Sat, 28 Aug 2021 07:40:10 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; s390x

```console
$ docker pull plone@sha256:9bf9edc92fa66bb5ba8add38c2027fe182f9dc90b52088c6aa13e6ed7cc5118b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151903283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e481be2fb9c312e482afb10bc6c34e7fbfe3ddfe851b9ffe256ba73d3cf388b3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["start"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:01:52 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Aug 2021 21:01:53 GMT
ENV LANG=C.UTF-8
# Fri, 27 Aug 2021 21:19:34 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 	;
# Fri, 27 Aug 2021 21:19:35 GMT
ENV GPG_KEY=E3FF2839C048B25C084DEBE9B26995E310250568
# Fri, 27 Aug 2021 21:19:35 GMT
ENV PYTHON_VERSION=3.8.11
# Fri, 27 Aug 2021 21:24:53 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Fri, 27 Aug 2021 21:24:56 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Fri, 27 Aug 2021 21:24:57 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Fri, 27 Aug 2021 21:24:57 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Fri, 27 Aug 2021 21:24:58 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Fri, 27 Aug 2021 21:25:05 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Fri, 27 Aug 2021 21:25:06 GMT
CMD ["python3"]
# Sat, 28 Aug 2021 06:31:38 GMT
ENV PIP=21.0.1 ZC_BUILDOUT=2.13.4 SETUPTOOLS=51.3.3 WHEEL=0.36.2 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.4 PLONE_VERSION_RELEASE=Plone-5.2.4-UnifiedInstaller-1.0 PLONE_MD5=b682cdf2384e692c033077f448b68afd
# Sat, 28 Aug 2021 06:31:39 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Sat, 28 Aug 2021 06:31:40 GMT
COPY file:3ef405a950854449713102e91399f13c5d85d531f4bb6247863ee4357e81ed1c in /plone/instance/ 
# Sat, 28 Aug 2021 06:48:23 GMT
RUN apk add --no-cache --virtual .build-deps     build-base     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     mariadb-dev     openldap-dev     pcre-dev     postgresql-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     git     rsync     libxml2     libxslt     libjpeg-turbo     mariadb-connector-c     postgresql-client && rm -rf /plone/buildout-cache/downloads/*
# Sat, 28 Aug 2021 06:48:38 GMT
VOLUME [/data]
# Sat, 28 Aug 2021 06:48:38 GMT
COPY multi:42ced57fe3a0905e0e2388d9f8e6e5bd32fb0db140cd61d93fb9326734196d09 in / 
# Sat, 28 Aug 2021 06:48:38 GMT
EXPOSE 8080
# Sat, 28 Aug 2021 06:48:38 GMT
WORKDIR /plone/instance
# Sat, 28 Aug 2021 06:48:39 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Sat, 28 Aug 2021 06:48:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 28 Aug 2021 06:48:39 GMT
CMD ["start"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad56fe48972d40027df4420737d9917e143ca01da17e3137b85296e421a3bbd8`  
		Last Modified: Sat, 28 Aug 2021 00:39:50 GMT  
		Size: 281.9 KB (281940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1487fc8db6312fea0b2773e02d3afbb7ce7a37b34a947d2f1f992ff98fe57ea0`  
		Last Modified: Sat, 28 Aug 2021 00:39:54 GMT  
		Size: 11.2 MB (11223711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf436e9209b37fca9ada89802b62a2eb106aca4297836a1f71858605f6702a8`  
		Last Modified: Sat, 28 Aug 2021 00:39:50 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59bb9df1e87fdb05d1517730f6c3b55f4f41abec7ea6ea3210a8645c3500c328`  
		Last Modified: Sat, 28 Aug 2021 00:39:50 GMT  
		Size: 2.3 MB (2348756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7c7bce43657c935570289d140ffc8486908c952771ab5a0ae4be2c907ff37f`  
		Last Modified: Sat, 28 Aug 2021 06:49:03 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d129e04a6b19d5fc602ac212509c0268ede7b9f624538181da04d38e22be1bc3`  
		Last Modified: Sat, 28 Aug 2021 06:49:03 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0266ddfe5d8c90a57e3998dff08ccdaea495ae4d9b7188247761446d6ed6e3f9`  
		Last Modified: Sat, 28 Aug 2021 06:49:21 GMT  
		Size: 135.4 MB (135438747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835aa974b1ecb1a154d6ac269ff7eaeddc3f6cad526176ec979e6a97686f7865`  
		Last Modified: Sat, 28 Aug 2021 06:49:03 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
