## `plone:5-alpine`

```console
$ docker pull plone@sha256:79c6497283efddbc5d14a6a02a3642b349637e7d2d4e2b1370116e34b8ba3089
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
$ docker pull plone@sha256:8c22593b3a174a2e11b7227b945ed76068c6304546fd4daf1510ca0e759a8a75
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.1 MB (152113301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b063161698ab0c03a6f7d9bafbba4b84aff6f4a8eb5caa23a602e8fddd00a002`
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
# Wed, 01 Sep 2021 00:30:15 GMT
ENV PYTHON_VERSION=3.8.12
# Wed, 01 Sep 2021 00:36:02 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Wed, 01 Sep 2021 00:36:03 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 01 Sep 2021 00:36:03 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 01 Sep 2021 00:36:04 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Wed, 01 Sep 2021 00:36:04 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Wed, 01 Sep 2021 00:36:10 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 01 Sep 2021 00:36:10 GMT
CMD ["python3"]
# Wed, 01 Sep 2021 10:40:23 GMT
ENV PIP=21.0.1 ZC_BUILDOUT=2.13.4 SETUPTOOLS=51.3.3 WHEEL=0.36.2 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.4 PLONE_VERSION_RELEASE=Plone-5.2.4-UnifiedInstaller-1.0 PLONE_MD5=b682cdf2384e692c033077f448b68afd
# Wed, 01 Sep 2021 10:40:24 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 01 Sep 2021 10:40:24 GMT
COPY file:3ef405a950854449713102e91399f13c5d85d531f4bb6247863ee4357e81ed1c in /plone/instance/ 
# Wed, 01 Sep 2021 10:53:37 GMT
RUN apk add --no-cache --virtual .build-deps     build-base     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     mariadb-dev     openldap-dev     pcre-dev     postgresql-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     git     rsync     libxml2     libxslt     libjpeg-turbo     mariadb-connector-c     postgresql-client && rm -rf /plone/buildout-cache/downloads/*
# Wed, 01 Sep 2021 10:53:40 GMT
VOLUME [/data]
# Wed, 01 Sep 2021 10:53:40 GMT
COPY multi:42ced57fe3a0905e0e2388d9f8e6e5bd32fb0db140cd61d93fb9326734196d09 in / 
# Wed, 01 Sep 2021 10:53:40 GMT
EXPOSE 8080
# Wed, 01 Sep 2021 10:53:40 GMT
WORKDIR /plone/instance
# Wed, 01 Sep 2021 10:53:40 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 01 Sep 2021 10:53:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Sep 2021 10:53:41 GMT
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
	-	`sha256:ea96addd4e5a9065de10c8cc698a1cf86dffd94c88a6cefe314b684aa76c021a`  
		Last Modified: Wed, 01 Sep 2021 00:51:12 GMT  
		Size: 11.3 MB (11302413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968775df8ebc9201256291a162db868cafbe9ca1647d5579df7c6b9e5ac36ba2`  
		Last Modified: Wed, 01 Sep 2021 00:51:10 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad7e7d3e7ccc6c7f88445d8790397b30f3fa43e7b02966fa22c17ed06bb1e9e`  
		Last Modified: Wed, 01 Sep 2021 00:51:10 GMT  
		Size: 2.3 MB (2348852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4392115a182d75ea456bf5a7f50e586667efa16fe3d5861b1b2ebe36191221c6`  
		Last Modified: Wed, 01 Sep 2021 10:54:07 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7b3ef9a8f5f65c4d16471e8446ea3bea1f15118ef06104500c7eadc7406459`  
		Last Modified: Wed, 01 Sep 2021 10:54:07 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484165f58d238e4d4164a39be6649805825f46069fbd6070455ee7b9c9fe4059`  
		Last Modified: Wed, 01 Sep 2021 10:54:30 GMT  
		Size: 135.5 MB (135461865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee57818cdea89754feabb9750a0cdb7449abcad4dcd0f83fd7e8fe356a58228f`  
		Last Modified: Wed, 01 Sep 2021 10:54:07 GMT  
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
$ docker pull plone@sha256:a232b4e2fcf0d701d14248cc19668aca3f5598214d4a45a852a075d832da5492
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.9 MB (153932124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a823b95e2b856fc29e05f5c3feb972ccbd58c23f7819866af2319f42ebe28fe`
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
# Tue, 31 Aug 2021 20:57:23 GMT
ENV PYTHON_VERSION=3.8.12
# Tue, 31 Aug 2021 21:06:08 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Tue, 31 Aug 2021 21:06:20 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Tue, 31 Aug 2021 21:06:22 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Tue, 31 Aug 2021 21:06:27 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Tue, 31 Aug 2021 21:06:32 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Tue, 31 Aug 2021 21:07:00 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 31 Aug 2021 21:07:05 GMT
CMD ["python3"]
# Wed, 01 Sep 2021 05:01:52 GMT
ENV PIP=21.0.1 ZC_BUILDOUT=2.13.4 SETUPTOOLS=51.3.3 WHEEL=0.36.2 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.4 PLONE_VERSION_RELEASE=Plone-5.2.4-UnifiedInstaller-1.0 PLONE_MD5=b682cdf2384e692c033077f448b68afd
# Wed, 01 Sep 2021 05:02:00 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 01 Sep 2021 05:02:02 GMT
COPY file:3ef405a950854449713102e91399f13c5d85d531f4bb6247863ee4357e81ed1c in /plone/instance/ 
# Wed, 01 Sep 2021 05:23:05 GMT
RUN apk add --no-cache --virtual .build-deps     build-base     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     mariadb-dev     openldap-dev     pcre-dev     postgresql-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     git     rsync     libxml2     libxslt     libjpeg-turbo     mariadb-connector-c     postgresql-client && rm -rf /plone/buildout-cache/downloads/*
# Wed, 01 Sep 2021 05:23:13 GMT
VOLUME [/data]
# Wed, 01 Sep 2021 05:23:14 GMT
COPY multi:42ced57fe3a0905e0e2388d9f8e6e5bd32fb0db140cd61d93fb9326734196d09 in / 
# Wed, 01 Sep 2021 05:23:17 GMT
EXPOSE 8080
# Wed, 01 Sep 2021 05:23:21 GMT
WORKDIR /plone/instance
# Wed, 01 Sep 2021 05:23:23 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 01 Sep 2021 05:23:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Sep 2021 05:23:28 GMT
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
	-	`sha256:03111e6e80465281b412893ac14ea6e9a8b32869a86a42619091eb1fb4af7c85`  
		Last Modified: Tue, 31 Aug 2021 21:25:10 GMT  
		Size: 11.5 MB (11539392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13528ec6b56c972fe5234a1ecd40efbf9a45d717a1e28dafabde061f15ab2566`  
		Last Modified: Tue, 31 Aug 2021 21:25:08 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7756602a415ed27acc014aa370804c1653895ebd79fb75426e30585b050821e7`  
		Last Modified: Tue, 31 Aug 2021 21:25:08 GMT  
		Size: 2.3 MB (2348858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6befc9341036096b6dd35d59788ac4f1245bf904c0614d3024245a89ccac681d`  
		Last Modified: Wed, 01 Sep 2021 05:23:52 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f222247d8f56f8eaed85cf53f8346b97b8db3cf5a4d5fd7ab5ab102a9157747`  
		Last Modified: Wed, 01 Sep 2021 05:23:52 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a146644d4e53e75247e700f6313aa3e3d58d8ca73880fe6f978bc5cf138e6ed`  
		Last Modified: Wed, 01 Sep 2021 05:24:19 GMT  
		Size: 136.9 MB (136941277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3075139662ef83fce04b4150db3e0b3150e46b2c1a49ab35fd9cbd0e472623f9`  
		Last Modified: Wed, 01 Sep 2021 05:23:52 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `plone:5-alpine` - linux; s390x

```console
$ docker pull plone@sha256:b47ac491c1cbeb027d6e6d7972c71b41d414c3e8d2360bad5f0b281d2d0fed47
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151909165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9cd263b5c8af3d226b4790aaaf7e54c9868a04c2c568c469544b3f6f1242ae7`
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
# Wed, 01 Sep 2021 00:39:01 GMT
ENV PYTHON_VERSION=3.8.12
# Wed, 01 Sep 2021 00:45:14 GMT
RUN set -ex 	&& apk add --no-cache --virtual .fetch-deps 		gnupg 		tar 		xz 		&& wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz" 	&& wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY" 	&& gpg --batch --verify python.tar.xz.asc python.tar.xz 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" python.tar.xz.asc 	&& mkdir -p /usr/src/python 	&& tar -xJC /usr/src/python --strip-components=1 -f python.tar.xz 	&& rm python.tar.xz 		&& apk add --no-cache --virtual .build-deps  		bluez-dev 		bzip2-dev 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	&& apk del --no-network .fetch-deps 		&& cd /usr/src/python 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-system-expat 		--with-system-ffi 		--without-ensurepip 	&& make -j "$(nproc)" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	&& make install 	&& rm -rf /usr/src/python 		&& find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name '*.a' \) \) 			-o \( -type f -a -name 'wininst-*.exe' \) 		\) -exec rm -rf '{}' + 		&& find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-cache --virtual .python-rundeps 	&& apk del --no-network .build-deps 		&& python3 --version
# Wed, 01 Sep 2021 00:45:16 GMT
RUN cd /usr/local/bin 	&& ln -s idle3 idle 	&& ln -s pydoc3 pydoc 	&& ln -s python3 python 	&& ln -s python3-config python-config
# Wed, 01 Sep 2021 00:45:17 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 01 Sep 2021 00:45:17 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Wed, 01 Sep 2021 00:45:18 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Wed, 01 Sep 2021 00:45:26 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip==$PYTHON_PIP_VERSION" 	; 	pip --version; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 01 Sep 2021 00:45:27 GMT
CMD ["python3"]
# Wed, 01 Sep 2021 12:38:36 GMT
ENV PIP=21.0.1 ZC_BUILDOUT=2.13.4 SETUPTOOLS=51.3.3 WHEEL=0.36.2 PLONE_MAJOR=5.2 PLONE_VERSION=5.2.4 PLONE_VERSION_RELEASE=Plone-5.2.4-UnifiedInstaller-1.0 PLONE_MD5=b682cdf2384e692c033077f448b68afd
# Wed, 01 Sep 2021 12:38:37 GMT
RUN addgroup -g 500 plone  && adduser -S -D -G plone -u 500 plone  && mkdir -p /plone/instance /data/filestorage /data/blobstorage
# Wed, 01 Sep 2021 12:38:37 GMT
COPY file:3ef405a950854449713102e91399f13c5d85d531f4bb6247863ee4357e81ed1c in /plone/instance/ 
# Wed, 01 Sep 2021 12:51:40 GMT
RUN apk add --no-cache --virtual .build-deps     build-base     libc-dev     zlib-dev     libjpeg-turbo-dev     libpng-dev     libxml2-dev     libxslt-dev     mariadb-dev     openldap-dev     pcre-dev     postgresql-dev     libffi-dev && wget -O Plone.tgz https://launchpad.net/plone/$PLONE_MAJOR/$PLONE_VERSION/+download/$PLONE_VERSION_RELEASE.tgz && echo "$PLONE_MD5  Plone.tgz" | md5sum -c - && tar -zxvf Plone.tgz && cp -rv ./$PLONE_VERSION_RELEASE/base_skeleton/* /plone/instance/ && cp -v ./$PLONE_VERSION_RELEASE/buildout_templates/buildout.cfg /plone/instance/buildout-base.cfg && pip install pip==$PIP setuptools==$SETUPTOOLS zc.buildout==$ZC_BUILDOUT wheel==$WHEEL && cd /plone/instance && buildout && ln -s /data/filestorage/ /plone/instance/var/filestorage && ln -s /data/blobstorage /plone/instance//var/blobstorage && find /data  -not -user plone -exec chown plone:plone {} \+ && find /plone -not -user plone -exec chown plone:plone {} \+ && rm -rf /Plone* && apk del .build-deps && apk add --no-cache --virtual .run-deps     su-exec     bash     git     rsync     libxml2     libxslt     libjpeg-turbo     mariadb-connector-c     postgresql-client && rm -rf /plone/buildout-cache/downloads/*
# Wed, 01 Sep 2021 12:52:10 GMT
VOLUME [/data]
# Wed, 01 Sep 2021 12:52:11 GMT
COPY multi:42ced57fe3a0905e0e2388d9f8e6e5bd32fb0db140cd61d93fb9326734196d09 in / 
# Wed, 01 Sep 2021 12:52:11 GMT
EXPOSE 8080
# Wed, 01 Sep 2021 12:52:12 GMT
WORKDIR /plone/instance
# Wed, 01 Sep 2021 12:52:13 GMT
HEALTHCHECK &{["CMD-SHELL" "nc -z -w5 127.0.0.1 8080 || exit 1"] "1m0s" "5s" "1m0s" '\x00'}
# Wed, 01 Sep 2021 12:52:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Sep 2021 12:52:14 GMT
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
	-	`sha256:ac9d7cb30a9a85008d630160359b40b10ceb6c1f34298c9e43b89b54d78c29e9`  
		Last Modified: Wed, 01 Sep 2021 01:01:20 GMT  
		Size: 11.2 MB (11228068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7e5e50920d35ca26df7332a72550284c65c2e618390d3a7b3e7d3d6e17b7fc`  
		Last Modified: Wed, 01 Sep 2021 01:01:18 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b16fd3bc3b465a8e264ee6771858548df7a9f280d469312f4ab90bb98d794d2`  
		Last Modified: Wed, 01 Sep 2021 01:01:18 GMT  
		Size: 2.3 MB (2348777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdaa56f241a685b2d38eca0e8e3ed504f4ffff2b86f731c4524dff4eec1f5dfc`  
		Last Modified: Wed, 01 Sep 2021 12:52:35 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48be30411f313cb6018013c691f26a141eec203a736787fdb6795ada95b0320`  
		Last Modified: Wed, 01 Sep 2021 12:52:35 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281bda2488f8e6765a84af43feac74709f4e147c7a36723c9177f3447427458b`  
		Last Modified: Wed, 01 Sep 2021 12:52:53 GMT  
		Size: 135.4 MB (135440254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4803fe3c91f17407f86991d6f61f226c0cfab96a1dca51ee8c537a0fe1b15a04`  
		Last Modified: Wed, 01 Sep 2021 12:52:35 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
